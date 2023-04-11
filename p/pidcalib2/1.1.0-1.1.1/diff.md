# Comparing `tmp/pidcalib2-1.1.0.tar.gz` & `tmp/pidcalib2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-lh1elmhy/pidcalib2-1.1.0.tar", last modified: Fri Dec 16 22:19:21 2022, max compression
+gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-mevam7bq/pidcalib2-1.1.1.tar", last modified: Tue Apr 11 12:06:01 2023, max compression
```

## Comparing `pidcalib2-1.1.0.tar` & `pidcalib2-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)       69 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)       30 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.flake8
--rw-r--r--   0 root         (0) root         (0)     2267 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2364 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      690 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)    35391 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/.sourcery.yaml
--rw-r--r--   0 root         (0) root         (0)    35065 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15419 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14808 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/notebooks/
--rw-r--r--   0 root         (0) root         (0)    15142 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/notebooks/plots.ipynb
--rw-r--r--   0 root         (0) root         (0)      654 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      371 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      796 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1304 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      894 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2/
--rw-r--r--   0 root         (0) root         (0)      577 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1173 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5212 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/aliases.py
--rw-r--r--   0 root         (0) root         (0)     2709 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/argparse_tools.py
--rw-r--r--   0 root         (0) root         (0)     9884 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2/data/
--rw-r--r--   0 root         (0) root         (0)   819948 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/data/samples.json
--rw-r--r--   0 root         (0) root         (0)     8179 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/make_eff_hists.py
--rw-r--r--   0 root         (0) root         (0)     3996 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/markdown_table.py
--rw-r--r--   0 root         (0) root         (0)     3496 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/merge_trees.py
--rw-r--r--   0 root         (0) root         (0)    16282 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/pid_data.py
--rw-r--r--   0 root         (0) root         (0)     6754 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)    13556 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     9937 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     2593 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/samples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2/tests/
--rw-r--r--   0 root         (0) root         (0)       57 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2320 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/
--rw-r--r--   0 root         (0) root         (0)     9898 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/cal_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     5653 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/cal_test_data.pkl
--rw-r--r--   0 root         (0) root         (0)      103 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/custom_binning.json
--rw-r--r--   0 root         (0) root         (0)     2556 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
--rw-r--r--   0 root         (0) root         (0)     2507 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
--rw-r--r--   0 root         (0) root         (0)    36807 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
--rw-r--r--   0 root         (0) root         (0)     2556 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
--rw-r--r--   0 root         (0) root         (0)      865 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
--rw-r--r--   0 root         (0) root         (0)    20907 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_PID_eff.root
--rw-r--r--   0 root         (0) root         (0)     8045 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     9244 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data.root
--rw-r--r--   0 root         (0) root         (0)     9817 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
--rw-r--r--   0 root         (0) root         (0)      127 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/test_file_list
--rw-r--r--   0 root         (0) root         (0)      206 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_data/test_samples.json
--rw-r--r--   0 root         (0) root         (0)     9950 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_make_eff_hist.py
--rw-r--r--   0 root         (0) root         (0)     4109 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_merge_trees.py
--rw-r--r--   0 root         (0) root         (0)     8095 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_pid_data.py
--rw-r--r--   0 root         (0) root         (0)     2549 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)     4297 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     4097 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     4597 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    25827 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/src/pidcalib2/utils.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15419 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2059 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      305 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/src/pidcalib2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 22:19:21.000000 pidcalib2-1.1.0/typings/
--rw-r--r--   0 root         (0) root         (0)       53 2022-12-16 22:19:08.000000 pidcalib2-1.1.0/typings/ROOT.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.flake8
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.sourcery.yaml
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14817 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    15142 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/notebooks/plots.ipynb
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      796 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5212 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/aliases.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/argparse_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/data/
+-rw-r--r--   0 root         (0) root         (0)   819948 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/data/samples.json
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/make_eff_hists.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/markdown_table.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)    16282 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/tests/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/
+-rw-r--r--   0 root         (0) root         (0)     9898 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5653 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.pkl
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/custom_binning.json
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    36807 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    20907 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_PID_eff.root
+-rw-r--r--   0 root         (0) root         (0)     8045 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     9244 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.root
+-rw-r--r--   0 root         (0) root         (0)     9817 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/test_file_list
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/test_samples.json
+-rw-r--r--   0 root         (0) root         (0)     9950 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_make_eff_hist.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    25950 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/utils.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/typings/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/typings/ROOT.pyi
```

### Comparing `pidcalib2-1.1.0/.gitignore` & `pidcalib2-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/.gitlab-ci.yml` & `pidcalib2-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/.pre-commit-config.yaml` & `pidcalib2-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/.pylintrc` & `pidcalib2-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/LICENSE` & `pidcalib2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/PKG-INFO` & `pidcalib2-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -84,15 +84,15 @@
 ```
 All aliases can be listed by running
 ```sh
 pidcalib2.make_eff_hists --list aliases
 ```
 Note that there are many more variables than there are aliases. If you want to find a variable for which no alias exists, you can check one of the calibration files yourself. The paths to the calibration files are printed when the `--verbose` option is specified. Alternatively, you can simply guess the name - if it doesn't exist, PIDCalib2 will let you know and might provide a list of similar names that do exist.
 
-A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, a two-bin binning for particle `Pi`, variable `P` can be defined as
+A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, two-bin binnings for particle `Pi`, variables `P` and `PT` can be defined as
 ```json
 {"Pi": {"P": [10000, 15000, 30000], "PT": [6000, 10000, 20000]}}
 ```
 An arbitrary number of binnings can be defined in a single file.
 
 Complex cut expressions can be created by chaining simpler expressions using `&` (logical and) and `|` (logical or). One can also use standard mathematical symbols, like `*`, `/`, `+`, `-`, `(`, `)`. Whitespace does not matter.
```

### Comparing `pidcalib2-1.1.0/README.md` & `pidcalib2-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ```
 All aliases can be listed by running
 ```sh
 pidcalib2.make_eff_hists --list aliases
 ```
 Note that there are many more variables than there are aliases. If you want to find a variable for which no alias exists, you can check one of the calibration files yourself. The paths to the calibration files are printed when the `--verbose` option is specified. Alternatively, you can simply guess the name - if it doesn't exist, PIDCalib2 will let you know and might provide a list of similar names that do exist.
 
-A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, a two-bin binning for particle `Pi`, variable `P` can be defined as
+A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, two-bin binnings for particle `Pi`, variables `P` and `PT` can be defined as
 ```json
 {"Pi": {"P": [10000, 15000, 30000], "PT": [6000, 10000, 20000]}}
 ```
 An arbitrary number of binnings can be defined in a single file.
 
 Complex cut expressions can be created by chaining simpler expressions using `&` (logical and) and `|` (logical or). One can also use standard mathematical symbols, like `*`, `/`, `+`, `-`, `(`, `)`. Whitespace does not matter.
```

### Comparing `pidcalib2-1.1.0/notebooks/plots.ipynb` & `pidcalib2-1.1.1/notebooks/plots.ipynb`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/pyproject.toml` & `pidcalib2-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/requirements-dev.txt` & `pidcalib2-1.1.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/setup.cfg` & `pidcalib2-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/setup.py` & `pidcalib2-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/__init__.py` & `pidcalib2-1.1.1/src/pidcalib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/__main__.py` & `pidcalib2-1.1.1/src/pidcalib2/__main__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/aliases.py` & `pidcalib2-1.1.1/src/pidcalib2/aliases.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/argparse_tools.py` & `pidcalib2-1.1.1/src/pidcalib2/argparse_tools.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/binning.py` & `pidcalib2-1.1.1/src/pidcalib2/binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/data/samples.json` & `pidcalib2-1.1.1/src/pidcalib2/data/samples.json`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/make_eff_hists.py` & `pidcalib2-1.1.1/src/pidcalib2/make_eff_hists.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/markdown_table.py` & `pidcalib2-1.1.1/src/pidcalib2/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/merge_trees.py` & `pidcalib2-1.1.1/src/pidcalib2/merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/pid_data.py` & `pidcalib2-1.1.1/src/pidcalib2/pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/pklhisto2root.py` & `pidcalib2-1.1.1/src/pidcalib2/pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/plot_calib_distributions.py` & `pidcalib2-1.1.1/src/pidcalib2/plot_calib_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     cuts = config["cuts"]
     if "cuts" in calib_sample:
         if cuts is None:
             cuts = []
         cuts += calib_sample["cuts"]
 
     branch_names = pid_data.get_relevant_branch_names([], config["bin_vars"], cuts)
-    log.info(f"Branches to be read: {branch_names}")
+    log.debug(f"Branches to be read: {branch_names}")
     log.info(
         f"{len(calib_sample['files'])} calibration files from EOS will be processed"
     )
     for path in calib_sample["files"]:
         log.debug(f"  {path}")
 
     if config["binning_file"]:
```

### Comparing `pidcalib2-1.1.0/src/pidcalib2/ref_calib.py` & `pidcalib2-1.1.1/src/pidcalib2/ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/samples.py` & `pidcalib2-1.1.1/src/pidcalib2/samples.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_binning.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/cal_test_data.csv` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/cal_test_data.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_PID_eff.root` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_PID_eff.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data.csv` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data.root` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_data/ref_test_data_subdir.root` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_make_eff_hist.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_make_eff_hist.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_merge_trees.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_pid_data.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_pklhisto2root.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_plot_calib_distributions.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_ref_calib.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/tests/test_utils.py` & `pidcalib2-1.1.1/src/pidcalib2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.0/src/pidcalib2/utils.py` & `pidcalib2-1.1.1/src/pidcalib2/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,16 +347,16 @@
             squares of the event weights). Can be ommited for unweighted events.
     """
     if err_pass_sq is None:
         err_pass_sq = num_pass
     if err_tot_sq is None:
         err_tot_sq = num_total
     prob = num_pass / num_total
-    prob_sq = prob ** 2
-    num_total_sq = num_total ** 2
+    prob_sq = prob**2
+    num_total_sq = num_total**2
     return np.sqrt(
         abs(((1 - 2 * prob) * err_pass_sq + err_tot_sq * prob_sq) / num_total_sq)
     )
 
 
 def create_error_histogram(eff_hists: Dict[str, bh.Histogram]) -> bh.Histogram:
     """Create a histogram with the binomial uncertainty of the efficiency.
@@ -504,30 +504,35 @@
             config["particle"],
             config["samples_file"],
             config["max_files"],
         )
     tree_paths = pid_data.get_tree_paths(
         config["particle"],
         config["sample"],
-        calib_sample["tuple_names"] if "tuple_names" in calib_sample else None,
+        calib_sample["tuple_names"][config["particle"]]
+        if (
+            "tuple_names" in calib_sample
+            and config["particle"] in calib_sample["tuple_names"]
+        )
+        else None,
     )
     log.debug(f"Trees to be read: {tree_paths}")
 
     # If there are hard-coded cuts, the variables must be included in the
     # branches to read.
     cuts = config["cuts"]
     if "cuts" in calib_sample:
         if cuts is None:
             cuts = []
         cuts += calib_sample["cuts"]
 
     branch_names = pid_data.get_relevant_branch_names(
         config["pid_cuts"], config["bin_vars"], cuts
     )
-    log.info(f"Branches to be read: {branch_names}")
+    log.debug(f"Branches to be read: {branch_names}")
     log.info(
         f"{len(calib_sample['files'])} calibration files from EOS will be processed"
     )
     for path in calib_sample["files"]:
         log.debug(f"  {path}")
 
     binning_range_cuts = []
```

### Comparing `pidcalib2-1.1.0/src/pidcalib2.egg-info/PKG-INFO` & `pidcalib2-1.1.1/src/pidcalib2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -84,15 +84,15 @@
 ```
 All aliases can be listed by running
 ```sh
 pidcalib2.make_eff_hists --list aliases
 ```
 Note that there are many more variables than there are aliases. If you want to find a variable for which no alias exists, you can check one of the calibration files yourself. The paths to the calibration files are printed when the `--verbose` option is specified. Alternatively, you can simply guess the name - if it doesn't exist, PIDCalib2 will let you know and might provide a list of similar names that do exist.
 
-A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, a two-bin binning for particle `Pi`, variable `P` can be defined as
+A file with alternative binnings can be specified using `--binning-file`. The file must contain valid JSON specifying bin edges. For example, two-bin binnings for particle `Pi`, variables `P` and `PT` can be defined as
 ```json
 {"Pi": {"P": [10000, 15000, 30000], "PT": [6000, 10000, 20000]}}
 ```
 An arbitrary number of binnings can be defined in a single file.
 
 Complex cut expressions can be created by chaining simpler expressions using `&` (logical and) and `|` (logical or). One can also use standard mathematical symbols, like `*`, `/`, `+`, `-`, `(`, `)`. Whitespace does not matter.
```

### Comparing `pidcalib2-1.1.0/src/pidcalib2.egg-info/SOURCES.txt` & `pidcalib2-1.1.1/src/pidcalib2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

