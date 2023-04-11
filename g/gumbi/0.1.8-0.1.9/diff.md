# Comparing `tmp/gumbi-0.1.8.tar.gz` & `tmp/gumbi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumbi-0.1.8.tar", last modified: Wed Feb 16 12:45:59 2022, max compression
+gzip compressed data, was "dist/gumbi-0.1.9.tar", last modified: Thu Feb 17 09:23:04 2022, max compression
```

## Comparing `gumbi-0.1.8.tar` & `gumbi-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.744319 gumbi-0.1.8/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    11357 2021-11-24 11:30:58.000000 gumbi-0.1.8/LICENSE
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      219 2022-02-02 21:01:21.000000 gumbi-0.1.8/MANIFEST.in
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3492 2022-02-16 12:45:59.744319 gumbi-0.1.8/PKG-INFO
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2235 2022-02-16 12:38:51.000000 gumbi-0.1.8/README.md
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.374440 gumbi-0.1.8/docs/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      108 2021-11-26 11:54:36.000000 gumbi-0.1.8/docs/requirements.txt
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.388282 gumbi-0.1.8/docs/source/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2800 2022-02-16 12:38:51.000000 gumbi-0.1.8/docs/source/conf.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      620 2021-12-14 22:56:28.000000 gumbi-0.1.8/docs/source/index.rst
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.317155 gumbi-0.1.8/docs/source/notebooks/
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.454410 gumbi-0.1.8/docs/source/notebooks/examples/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   878795 2022-02-16 12:44:59.000000 gumbi-0.1.8/docs/source/notebooks/examples/Cars_Dataset.ipynb
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)  1991553 2022-02-16 11:36:20.000000 gumbi-0.1.8/docs/source/notebooks/examples/Latent_GP.ipynb
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   271385 2021-12-14 22:56:28.000000 gumbi-0.1.8/docs/source/notebooks/examples/Multioutput_Regression.ipynb
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   245300 2021-12-14 22:56:28.000000 gumbi-0.1.8/docs/source/notebooks/examples/Simple_Regression.ipynb
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.465714 gumbi-0.1.8/docs/source/notebooks/getting_started/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    23977 2021-12-14 22:56:28.000000 gumbi-0.1.8/docs/source/notebooks/getting_started/introduction.ipynb
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.514234 gumbi-0.1.8/gumbi/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      372 2022-02-16 12:38:51.000000 gumbi-0.1.8/gumbi/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    32693 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/aggregation.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    55576 2022-02-02 14:25:13.000000 gumbi-0.1.8/gumbi/arrays.py
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.559419 gumbi-0.1.8/gumbi/data/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   552642 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/data/Example_DataSet.pkl
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      134 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/data/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    16357 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/plotting.py
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.574239 gumbi-0.1.8/gumbi/regression/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      126 2022-02-16 12:38:51.000000 gumbi-0.1.8/gumbi/regression/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    49997 2022-02-16 12:44:59.000000 gumbi-0.1.8/gumbi/regression/base.py
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.634624 gumbi-0.1.8/gumbi/style/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      234 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/style/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33983 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/style/breve_presentation.mplstyle
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33955 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/style/futura_presentation.mplstyle
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33944 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/style/presentation.mplstyle
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.679425 gumbi-0.1.8/gumbi/utils/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       74 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/utils/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2029 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/utils/generic_utils.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      433 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/utils/gp_utils.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3138 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/utils/misc.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1408 2021-11-24 11:30:58.000000 gumbi-0.1.8/gumbi/utils/pymc_utils.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      220 2022-02-16 12:38:51.000000 gumbi-0.1.8/gumbi/versions.py
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.537115 gumbi-0.1.8/gumbi.egg-info/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3492 2022-02-16 12:45:58.000000 gumbi-0.1.8/gumbi.egg-info/PKG-INFO
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1131 2022-02-16 12:45:58.000000 gumbi-0.1.8/gumbi.egg-info/SOURCES.txt
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        1 2022-02-16 12:45:58.000000 gumbi-0.1.8/gumbi.egg-info/dependency_links.txt
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       93 2022-02-16 12:45:58.000000 gumbi-0.1.8/gumbi.egg-info/requires.txt
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       12 2022-02-16 12:45:58.000000 gumbi-0.1.8/gumbi.egg-info/top_level.txt
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      269 2022-02-16 12:38:51.000000 gumbi-0.1.8/requirements.txt
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       79 2022-02-16 12:45:59.744319 gumbi-0.1.8/setup.cfg
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1584 2022-02-16 12:38:51.000000 gumbi-0.1.8/setup.py
-drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 12:45:59.735468 gumbi-0.1.8/tests/
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2021-11-24 11:30:58.000000 gumbi-0.1.8/tests/__init__.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      613 2021-11-24 11:30:58.000000 gumbi-0.1.8/tests/conftest.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3879 2021-11-24 11:30:58.000000 gumbi-0.1.8/tests/test_aggregation.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     6803 2021-11-24 11:30:58.000000 gumbi-0.1.8/tests/test_arrays.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3784 2021-11-24 11:30:58.000000 gumbi-0.1.8/tests/test_plots.py
--rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     5943 2022-01-31 16:10:53.000000 gumbi-0.1.8/tests/test_regression.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    11357 2021-11-24 11:30:58.000000 gumbi-0.1.9/LICENSE
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      235 2022-02-16 17:37:27.000000 gumbi-0.1.9/MANIFEST.in
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3492 2022-02-17 09:23:04.000000 gumbi-0.1.9/PKG-INFO
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2235 2022-02-16 12:38:51.000000 gumbi-0.1.9/README.md
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        6 2022-02-16 17:37:46.000000 gumbi-0.1.9/VERSION
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/docs/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      108 2021-11-26 11:54:36.000000 gumbi-0.1.9/docs/requirements.txt
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/docs/source/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2800 2022-02-16 12:38:51.000000 gumbi-0.1.9/docs/source/conf.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      620 2021-12-14 22:56:28.000000 gumbi-0.1.9/docs/source/index.rst
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/docs/source/notebooks/
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/docs/source/notebooks/examples/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   878795 2022-02-16 12:44:59.000000 gumbi-0.1.9/docs/source/notebooks/examples/Cars_Dataset.ipynb
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)  1991553 2022-02-16 11:36:20.000000 gumbi-0.1.9/docs/source/notebooks/examples/Latent_GP.ipynb
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   271385 2021-12-14 22:56:28.000000 gumbi-0.1.9/docs/source/notebooks/examples/Multioutput_Regression.ipynb
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   245300 2021-12-14 22:56:28.000000 gumbi-0.1.9/docs/source/notebooks/examples/Simple_Regression.ipynb
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/docs/source/notebooks/getting_started/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    23977 2021-12-14 22:56:28.000000 gumbi-0.1.9/docs/source/notebooks/getting_started/introduction.ipynb
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:03.000000 gumbi-0.1.9/gumbi/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      372 2022-02-16 12:38:51.000000 gumbi-0.1.9/gumbi/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    32693 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/aggregation.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    55576 2022-02-02 14:25:13.000000 gumbi-0.1.9/gumbi/arrays.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi/data/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)   552642 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/data/Example_DataSet.pkl
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      134 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/data/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    16357 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/plotting.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi/regression/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      126 2022-02-16 12:38:51.000000 gumbi-0.1.9/gumbi/regression/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    49997 2022-02-16 12:44:59.000000 gumbi-0.1.9/gumbi/regression/base.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi/regression/pymc3/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33457 2022-02-17 09:22:06.000000 gumbi-0.1.9/gumbi/regression/pymc3/GP.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-16 18:15:22.000000 gumbi-0.1.9/gumbi/regression/pymc3/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1614 2022-02-16 12:38:51.000000 gumbi-0.1.9/gumbi/regression/pymc3/extras.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi/style/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      234 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/style/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33983 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/style/breve_presentation.mplstyle
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33955 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/style/futura_presentation.mplstyle
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)    33944 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/style/presentation.mplstyle
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi/utils/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       74 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/utils/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     2029 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/utils/generic_utils.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      433 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/utils/gp_utils.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3138 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/utils/misc.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1408 2021-11-24 11:30:58.000000 gumbi-0.1.9/gumbi/utils/pymc_utils.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      220 2022-02-16 12:38:51.000000 gumbi-0.1.9/gumbi/versions.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/gumbi.egg-info/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3492 2022-02-17 09:22:59.000000 gumbi-0.1.9/gumbi.egg-info/PKG-INFO
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1236 2022-02-17 09:23:00.000000 gumbi-0.1.9/gumbi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        1 2022-02-17 09:22:59.000000 gumbi-0.1.9/gumbi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       93 2022-02-17 09:22:59.000000 gumbi-0.1.9/gumbi.egg-info/requires.txt
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       12 2022-02-17 09:22:59.000000 gumbi-0.1.9/gumbi.egg-info/top_level.txt
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      269 2022-02-16 12:38:51.000000 gumbi-0.1.9/requirements.txt
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)       79 2022-02-17 09:23:04.000000 gumbi-0.1.9/setup.cfg
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     1584 2022-02-16 12:38:51.000000 gumbi-0.1.9/setup.py
+drwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2022-02-17 09:23:04.000000 gumbi-0.1.9/tests/
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)        0 2021-11-24 11:30:58.000000 gumbi-0.1.9/tests/__init__.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)      613 2021-11-24 11:30:58.000000 gumbi-0.1.9/tests/conftest.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3879 2021-11-24 11:30:58.000000 gumbi-0.1.9/tests/test_aggregation.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     6803 2021-11-24 11:30:58.000000 gumbi-0.1.9/tests/test_arrays.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     3784 2021-11-24 11:30:58.000000 gumbi-0.1.9/tests/test_plots.py
+-rwxrwxrwx   0 johngoertz  (1000) johngoertz  (1000)     5943 2022-01-31 16:10:53.000000 gumbi-0.1.9/tests/test_regression.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gumbi-0.1.8/LICENSE` & `gumbi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/PKG-INFO` & `gumbi-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Description: # Gumbi: Gaussian Process Model Building Interface
```

### Comparing `gumbi-0.1.8/README.md` & `gumbi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/conf.py` & `gumbi-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/index.rst` & `gumbi-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/notebooks/examples/Cars_Dataset.ipynb` & `gumbi-0.1.9/docs/source/notebooks/examples/Cars_Dataset.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/notebooks/examples/Latent_GP.ipynb` & `gumbi-0.1.9/docs/source/notebooks/examples/Latent_GP.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/notebooks/examples/Multioutput_Regression.ipynb` & `gumbi-0.1.9/docs/source/notebooks/examples/Multioutput_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/notebooks/examples/Simple_Regression.ipynb` & `gumbi-0.1.9/docs/source/notebooks/examples/Simple_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/docs/source/notebooks/getting_started/introduction.ipynb` & `gumbi-0.1.9/docs/source/notebooks/getting_started/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/aggregation.py` & `gumbi-0.1.9/gumbi/aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/arrays.py` & `gumbi-0.1.9/gumbi/arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/data/Example_DataSet.pkl` & `gumbi-0.1.9/gumbi/data/Example_DataSet.pkl`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/plotting.py` & `gumbi-0.1.9/gumbi/plotting.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/regression/base.py` & `gumbi-0.1.9/gumbi/regression/base.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/style/breve_presentation.mplstyle` & `gumbi-0.1.9/gumbi/style/breve_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/style/futura_presentation.mplstyle` & `gumbi-0.1.9/gumbi/style/futura_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/style/presentation.mplstyle` & `gumbi-0.1.9/gumbi/style/presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/utils/generic_utils.py` & `gumbi-0.1.9/gumbi/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/utils/misc.py` & `gumbi-0.1.9/gumbi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi/utils/pymc_utils.py` & `gumbi-0.1.9/gumbi/utils/pymc_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/gumbi.egg-info/PKG-INFO` & `gumbi-0.1.9/gumbi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Description: # Gumbi: Gaussian Process Model Building Interface
```

### Comparing `gumbi-0.1.8/gumbi.egg-info/SOURCES.txt` & `gumbi-0.1.9/gumbi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+VERSION
 requirements.txt
 setup.cfg
 setup.py
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/notebooks/examples/Cars_Dataset.ipynb
@@ -22,14 +23,17 @@
 gumbi.egg-info/dependency_links.txt
 gumbi.egg-info/requires.txt
 gumbi.egg-info/top_level.txt
 gumbi/data/Example_DataSet.pkl
 gumbi/data/__init__.py
 gumbi/regression/__init__.py
 gumbi/regression/base.py
+gumbi/regression/pymc3/GP.py
+gumbi/regression/pymc3/__init__.py
+gumbi/regression/pymc3/extras.py
 gumbi/style/__init__.py
 gumbi/style/breve_presentation.mplstyle
 gumbi/style/futura_presentation.mplstyle
 gumbi/style/presentation.mplstyle
 gumbi/utils/__init__.py
 gumbi/utils/generic_utils.py
 gumbi/utils/gp_utils.py
```

### Comparing `gumbi-0.1.8/setup.py` & `gumbi-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/tests/conftest.py` & `gumbi-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/tests/test_aggregation.py` & `gumbi-0.1.9/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/tests/test_arrays.py` & `gumbi-0.1.9/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/tests/test_plots.py` & `gumbi-0.1.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.1.8/tests/test_regression.py` & `gumbi-0.1.9/tests/test_regression.py`

 * *Files identical despite different names*

