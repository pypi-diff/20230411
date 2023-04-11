# Comparing `tmp/hdx-python-utilities-3.5.7.tar.gz` & `tmp/hdx-python-utilities-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-utilities-3.5.7.tar", last modified: Mon Mar 27 21:48:06 2023, max compression
+gzip compressed data, was "hdx-python-utilities-3.5.8.tar", last modified: Tue Apr 11 03:19:41 2023, max compression
```

## Comparing `hdx-python-utilities-3.5.7.tar` & `hdx-python-utilities-3.5.8.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.806544 hdx-python-utilities-3.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.778541 hdx-python-utilities-3.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.782542 hdx-python-utilities-3.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-27 21:48:06.806544 hdx-python-utilities-3.5.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.782542 hdx-python-utilities-3.5.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    35300 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-03-27 21:48:06.806544 hdx-python-utilities-3.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.778541 hdx-python-utilities-3.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.778541 hdx-python-utilities-3.5.7/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.786542 hdx-python-utilities-3.5.7/src/hdx/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35023 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15738 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61756 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8054 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2203 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17574 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/saver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7647 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13872 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/typehint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6838 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/src/hdx/utilities/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.786542 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 21:48:06.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:48:05.000000 hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.778541 hdx-python-utilities-3.5.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.786542 hdx-python-utilities-3.5.7/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.786542 hdx-python-utilities-3.5.7/tests/fixtures/compare/
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/compare/test_csv_processing2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.790542 hdx-python-utilities-3.5.7/tests/fixtures/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/empty.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/hdx_email_configuration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/json_csv.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/logging_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      123 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/smtp_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/config/user_agent_config_wrong.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.794543 hdx-python-utilities-3.5.7/tests/fixtures/downloader/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/basicauth.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/extra_params.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/extra_params_tree.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.794543 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data1.csv/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_xlsx_processing.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.794543 hdx-python-utilities-3.5.7/tests/fixtures/html/
--rwxr-xr-x   0 runner    (1001) docker     (123)  1622046 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/html/response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.798543 hdx-python-utilities-3.5.7/tests/fixtures/loader/
--rwxr-xr-x   0 runner    (1001) docker     (123)        2 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/loader/empty.json
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/loader/empty.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.798543 hdx-python-utilities-3.5.7/tests/fixtures/retriever/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.798543 hdx-python-utilities-3.5.7/tests/fixtures/retriever/fallbacks/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/fallbacks/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/test.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/retriever/test_hxl.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.802543 hdx-python-utilities-3.5.7/tests/fixtures/saver/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out.csv
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out2.json
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out5.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out6.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out7.json
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out8.csv
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/out8.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.802543 hdx-python-utilities-3.5.7/tests/fixtures/state/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/fixtures/test_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.802543 hdx-python-utilities-3.5.7/tests/hdx/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:48:06.802543 hdx-python-utilities-3.5.7/tests/hdx/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9698 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13565 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47752 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5656 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5363 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15246 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20894 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14379 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-27 21:47:43.000000 hdx-python-utilities-3.5.7/tests/hdx/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.github/workflows/run-python-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.764089 hdx-python-utilities-3.5.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    35300 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/doc/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.764089 hdx-python-utilities-3.5.8/src/hdx/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35023 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15753 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61799 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8054 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2203 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17574 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/saver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7647 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13872 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6838 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:19:40.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/compare/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/compare/test_csv_processing2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/empty.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_email_configuration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/json_csv.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/project_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      123 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/smtp_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config2.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config3.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config_wrong.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/downloader/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/basicauth.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params_tree.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data1.csv/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xlsx_processing.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/html/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1622046 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/html/response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/loader/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        2 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/loader/empty.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/retriever/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test_hxl.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/saver/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out7.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/state/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/test_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/tests/hdx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/tests/hdx/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9698 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13565 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47752 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5656 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5363 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15246 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20894 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14379 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/utils.py
```

### Comparing `hdx-python-utilities-3.5.7/.github/workflows/publish.yml` & `hdx-python-utilities-3.5.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/.github/workflows/run-python-tests.yml` & `hdx-python-utilities-3.5.8/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/.gitignore` & `hdx-python-utilities-3.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/LICENSE` & `hdx-python-utilities-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/PKG-INFO` & `hdx-python-utilities-3.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-utilities
-Version: 3.5.7
+Version: 3.5.8
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Home-page: https://github.com/OCHA-DAP/hdx-python-utilities
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,utilities,library,streaming,tabular data,datetime,date,time,timezone,dict,list,json,yaml
 Platform: any
```

### Comparing `hdx-python-utilities-3.5.7/README.md` & `hdx-python-utilities-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/doc/main.md` & `hdx-python-utilities-3.5.8/doc/main.md`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/pyproject.toml` & `hdx-python-utilities-3.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/setup.cfg` & `hdx-python-utilities-3.5.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,11 @@
 [options.extras_require]
 html = beautifulsoup4; html5lib
 email = email_validator
 
 [options.packages.find]
 where = src
 
-[bdist_wheel]
-universal = 1
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/base_downloader.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/compare.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/dateparse.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/dictandlist.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/dictandlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Dict and List utilities."""
 
 import itertools
 from collections import UserDict
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from .frictionless_wrapper import get_frictionless_resource
+from .frictionless_wrapper import get_frictionless_tableresource
 from .typehint import ListDict, ListTuple, ListTupleDict
 
 
 def merge_two_dictionaries(
     a: Dict, b: Dict, merge_lists: bool = False
 ) -> Dict:
     """Merges b into a and returns merged result.
@@ -385,15 +385,15 @@
         **kwargs: Other arguments to pass to Tabulator Stream
 
     Returns:
         List[ListDict]: List of rows in dict or list form
     """
     if dict_form and headers is None:
         raise ValueError("If dict_form is True, headers must not be None!")
-    resource = get_frictionless_resource(url, headers=headers, **kwargs)
+    resource = get_frictionless_tableresource(url, headers=headers, **kwargs)
     result = []
     if not dict_form:
         result.append(resource.header)
     for inrow in resource.row_stream:
         if dict_form:
             row = inrow.to_dict()
         else:
@@ -452,15 +452,15 @@
                 newrows = []
                 for row in rows:
                     newrow = []
                     for column in columns:
                         newrow.append(row[column - 1])
                     newrows.append(newrow)
                 rows = newrows
-        resource = get_frictionless_resource(
+        resource = get_frictionless_tableresource(
             data=rows,
             has_header=has_header,
             headers=headers,
             encoding=encoding,
         )
         resource.write(filepath, format="csv", encoding=encoding)
         resource.close()
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/downloader.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from copy import deepcopy
 from os import remove
 from os.path import exists, isfile, join, split, splitext
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 from urllib.parse import parse_qsl, urlencode, urlsplit, urlunsplit
 
-import frictionless
 import requests
 from frictionless import FrictionlessException
+from frictionless.resources import TableResource
 from ratelimit import RateLimitDecorator, sleep_and_retry
 from requests import Request
 from ruamel.yaml import YAML
 
 from .base_downloader import BaseDownload, DownloadError
-from .frictionless_wrapper import get_frictionless_resource
+from .frictionless_wrapper import get_frictionless_tableresource
 from .path import get_filename_from_url, get_temp_dir
 from .session import get_session
 from .typehint import ListDict, ListTuple
 
 logger = logging.getLogger(__name__)
 
 
@@ -556,22 +556,22 @@
 
         Returns:
             str: JSON content of download
         """
         self.download(url, **kwargs)
         return self.get_json()
 
-    def get_frictionless_resource(
+    def get_frictionless_tableresource(
         self,
         url: str,
         ignore_blank_rows: bool = True,
         infer_types: bool = False,
         **kwargs: Any,
-    ) -> frictionless.Resource:
-        """Get Frictionless Resource.
+    ) -> TableResource:
+        """Get Frictionless TableResource.
 
         Args:
             url (str): URL or path to download
             ignore_blank_rows (bool): Whether to ignore blank rows. Defaults to True.
             infer_types (bool): Whether to infer types. Defaults to False (strings).
             **kwargs:
             has_header (bool): Whether data has a header. Defaults to True.
@@ -592,19 +592,19 @@
             null_values (List[Any]): Values that will return None. Defaults to [""].
             dialect (Dialect): This can be set to override the above. See Frictionless docs.
             detector (Detector): This can be set to override the above. See Frictionless docs.
             layout (Layout): This can be set to override the above. See Frictionless docs.
             schema (Schema): This can be set to override the above. See Frictionless docs.
 
         Returns:
-            frictionless.Resource: frictionless Resource object
+            TableResource: frictionless TableResource object
         """
         self.close_response()
         try:
-            self.response = get_frictionless_resource(
+            self.response = get_frictionless_tableresource(
                 url, ignore_blank_rows, infer_types, self.session, **kwargs
             )
         except FrictionlessException as e:
             raise DownloadError(str(e)) from e
         return self.response
 
     def _get_tabular_rows(
@@ -666,15 +666,15 @@
             schema (Schema): This can be set to override the above. See Frictionless docs.
 
         Returns:
             Tuple[List[str],Iterator[ListDict]]: Tuple (headers, iterator where each row is a list or dictionary)
         """
         if headers is None:
             raise DownloadError("Argument headers cannot be None!")
-        resource = self.get_frictionless_resource(
+        resource = self.get_frictionless_tableresource(
             url,
             ignore_blank_rows=ignore_blank_rows,
             infer_types=infer_types,
             headers=headers,
             **kwargs,
         )
         origheaders = resource.header
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/easy_logging.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/easy_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,17 +51,22 @@
 
             # Find caller from where originated the logged message.
             frame, depth = sys._getframe(6), 6
             while frame and frame.f_code.co_filename == logging.__file__:
                 frame = frame.f_back
                 depth += 1
 
-            msg = record.getMessage().replace("<locals>", "\\<locals>")
-            logger.opt(
-                colors=True, depth=depth, exception=record.exc_info
-            ).log(level, msg)
+            msg = record.getMessage()
+            try:
+                logger.opt(
+                    colors=True, depth=depth, exception=record.exc_info
+                ).log(level, msg)
+            except ValueError:
+                logger.opt(
+                    colors=False, depth=depth, exception=record.exc_info
+                ).log(level, msg)
 
     root_logger = logging.getLogger()
     while root_logger.hasHandlers():
         root_logger.removeHandler(root_logger.handlers[0])
     root_logger.setLevel(logging.NOTSET)
     logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/email.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/email.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/encoding.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/errors_onexit.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/frictionless_wrapper.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/frictionless_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import requests
 from frictionless import (
     Control,
     Detector,
     Dialect,
     FrictionlessException,
-    Resource,
     system,
 )
 from frictionless.errors import ResourceError
 from frictionless.formats import CsvControl, ExcelControl, JsonControl
 from frictionless.resources import TableResource
 
 
@@ -116,23 +115,23 @@
     columns = kwargs.pop("columns", None)
     if columns:
         dialect.pick_fields = columns
     dialect.skip_blank_rows = ignore_blank_rows
     return dialect, kwargs
 
 
-def get_frictionless_resource(
+def get_frictionless_tableresource(
     url: Optional[str] = None,
     ignore_blank_rows: bool = True,
     infer_types: bool = False,
     session: Optional[requests.Session] = None,
     data: Optional[Any] = None,
     **kwargs: Any,
-) -> Resource:
-    """Get Frictionless Resource. Either url or data must be supplied.
+) -> TableResource:
+    """Get Frictionless TableResource. Either url or data must be supplied.
 
     Args:
         url (Optional[str]): URL or path to download. Defaults to None.
         ignore_blank_rows (bool): Whether to ignore blank rows. Defaults to True.
         infer_types (bool): Whether to infer types. Defaults to False (strings).
         session (Optional[requests.Session]): Session to use. Defaults to not setting a session.
         data (Optional[Any]): Data to parse. Defaults to None.
@@ -157,15 +156,15 @@
         null_values (List[Any]): Values that will return None. Defaults to [""].
         control (Control): This can be set to override the above. See Frictionless docs.
         detector (Detector): This can be set to override the above. See Frictionless docs.
         dialect (Dialect): This can be set to override the above. See Frictionless docs.
         schema (Schema): This can be set to override the above. See Frictionless docs.
 
     Returns:
-        Resource: frictionless Resource object
+        TableResource: frictionless TableResource object
     """
     if not url and not data:
         error = ResourceError(note="Neither url or data supplied!")
         raise FrictionlessException(error=error)
     control, kwargs = get_frictionless_control(**kwargs)
     detector, kwargs = get_frictionless_detector(infer_types, **kwargs)
     dialect, kwargs = get_frictionless_dialect(ignore_blank_rows, **kwargs)
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/html.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/html.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/loader.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/path.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/retriever.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/saver.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/session.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/session.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/state.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/state.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/text.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/useragent.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/useragent.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx/utilities/uuid.py` & `hdx-python-utilities-3.5.8/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/PKG-INFO` & `hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-utilities
-Version: 3.5.7
+Version: 3.5.8
 Summary: HDX Python Utilities for streaming tabular data, date and time handling and other helpful functions
 Home-page: https://github.com/OCHA-DAP/hdx-python-utilities
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,utilities,library,streaming,tabular data,datetime,date,time,timezone,dict,list,json,yaml
 Platform: any
```

### Comparing `hdx-python-utilities-3.5.7/src/hdx_python_utilities.egg-info/SOURCES.txt` & `hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/config/json_csv.yml` & `hdx-python-utilities-3.5.8/tests/fixtures/config/json_csv.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/config/logging_config.json` & `hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/config/logging_config.yml` & `hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_data.xlsx` & `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_xls_processing.xls` & `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/html/response.html` & `hdx-python-utilities-3.5.8/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/fixtures/test_data.csv` & `hdx-python-utilities-3.5.8/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/conftest.py` & `hdx-python-utilities-3.5.8/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_compare.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_dateparse.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_dictandlist.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_downloader.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_easy_logging.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_email.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_email.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_encoding.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_errors_onexit.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_html.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_loader.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_loader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_path.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_retriever.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_saver.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_saver.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_state.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_state.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_text.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/test_useragent.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_useragent.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.7/tests/hdx/utilities/utils.py` & `hdx-python-utilities-3.5.8/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

