# Comparing `tmp/img2table-0.0.23.tar.gz` & `tmp/img2table-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.0.23.tar", last modified: Sat Apr  8 17:40:15 2023, max compression
+gzip compressed data, was "dist/img2table-0.0.24.tar", last modified: Tue Apr 11 08:05:20 2023, max compression
```

## Comparing `img2table-0.0.23.tar` & `img2table-0.0.24.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-08 17:38:27.000000 img2table-0.0.23/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 17:38:27.000000 img2table-0.0.23/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-08 17:40:15.000000 img2table-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-08 17:38:27.000000 img2table-0.0.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-08 17:38:27.000000 img2table-0.0.23/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 17:38:27.000000 img2table-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 17:38:27.000000 img2table-0.0.23/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-08 17:38:27.000000 img2table-0.0.23/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-08 17:38:27.000000 img2table-0.0.23/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-08 17:40:15.000000 img2table-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-08 17:38:27.000000 img2table-0.0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    35369 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 08:03:24.000000 img2table-0.0.24/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 08:03:24.000000 img2table-0.0.24/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-11 08:05:20.000000 img2table-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-11 08:03:24.000000 img2table-0.0.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 08:03:24.000000 img2table-0.0.24/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 08:03:24.000000 img2table-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 08:03:24.000000 img2table-0.0.24/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-11 08:03:24.000000 img2table-0.0.24/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 08:03:24.000000 img2table-0.0.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-11 08:05:20.000000 img2table-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 08:03:24.000000 img2table-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    35369 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.0.23/LICENSE.txt` & `img2table-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/Makefile` & `img2table-0.0.24/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/PKG-INFO` & `img2table-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.23
+Version: 0.0.24
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.23 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.0.24 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-0.0.23/README.md` & `img2table-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/Basic_usage.ipynb` & `img2table-0.0.24/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/Implicit_rows.ipynb` & `img2table-0.0.24/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/borderless.ipynb` & `img2table-0.0.24/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/borderless_aws.jpg` & `img2table-0.0.24/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/borderless_ocr.jpg` & `img2table-0.0.24/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/implicit.png` & `img2table-0.0.24/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/tables.pdf` & `img2table-0.0.24/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/tables.png` & `img2table-0.0.24/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/examples/data/tables.xlsx` & `img2table-0.0.24/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/setup.cfg` & `img2table-0.0.24/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/__init__.py` & `img2table-0.0.24/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/document/base/__init__.py` & `img2table-0.0.24/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/document/base/rotation.py` & `img2table-0.0.24/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/document/image.py` & `img2table-0.0.24/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/document/pdf.py` & `img2table-0.0.24/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/aws_textract.py` & `img2table-0.0.24/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/azure.py` & `img2table-0.0.24/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/base.py` & `img2table-0.0.24/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/data.py` & `img2table-0.0.24/src/img2table/ocr/data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/google_vision.py` & `img2table-0.0.24/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/paddle.py` & `img2table-0.0.24/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/pdf.py` & `img2table-0.0.24/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/ocr/tesseract.py` & `img2table-0.0.24/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/image.py` & `img2table-0.0.24/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/objects/__init__.py` & `img2table-0.0.24/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/objects/extraction.py` & `img2table-0.0.24/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/objects/line.py` & `img2table-0.0.24/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/objects/row.py` & `img2table-0.0.24/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/objects/table.py` & `img2table-0.0.24/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 
     # Get contours of dark areas
     contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # For each dark area, use binary threshold instead of regular threshold
     for c in contours:
         x, y, w, h = cv2.boundingRect(c)
-        margin = int(ocr_df.char_length) if ocr_df.char_length else 5
+        
+        try:
+            margin = int(ocr_df.char_length)
+        except Exception as e:
+            margin = 5
         if min(w, h) > 2 * margin and w * h / np.prod(img.shape[:2]) < 0.9:
             thresh[y+margin:y+h-margin, x+margin:x+w-margin] = binary_thresh[y+margin:y+h-margin, x+margin:x+w-margin]
 
     return thresh
 
 
 def overlapping_filter(lines: List[Line], max_gap: int = 5) -> List[Line]:
```

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/common.py` & `img2table-0.0.24/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/prepare_image.py` & `img2table-0.0.24/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table/tables/processing/text/titles.py` & `img2table-0.0.24/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/src/img2table.egg-info/PKG-INFO` & `img2table-0.0.24/src/img2table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.23
+Version: 0.0.24
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.23 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.0.24 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-0.0.23/src/img2table.egg-info/SOURCES.txt` & `img2table-0.0.24/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/_mock_data/azure.pkl` & `img2table-0.0.24/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/_mock_data/tesseract_hocr.html` & `img2table-0.0.24/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/_mock_data/textract.json` & `img2table-0.0.24/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/_mock_data/vision.json` & `img2table-0.0.24/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/_mock_data/vision.pkl` & `img2table-0.0.24/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/conftest.py` & `img2table-0.0.24/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/base/test_data/test.png` & `img2table-0.0.24/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/base/test_rotation.py` & `img2table-0.0.24/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/image/test_data/blank.png` & `img2table-0.0.24/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/image/test_data/expected.xlsx` & `img2table-0.0.24/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/image/test_data/test.png` & `img2table-0.0.24/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/image/test_image.py` & `img2table-0.0.24/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/pdf/test_data/test.pdf` & `img2table-0.0.24/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/document/pdf/test_pdf.py` & `img2table-0.0.24/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.0.24/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.0.24/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.0.24/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/azure/test_azure.py` & `img2table-0.0.24/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/azure/test_data/test.png` & `img2table-0.0.24/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/data/test_data/expected_table.json` & `img2table-0.0.24/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/data/test_ocr_data.py` & `img2table-0.0.24/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.0.24/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/google_vision/test_data/test.png` & `img2table-0.0.24/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.0.24/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.0.24/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/paddle/test_data/test.png` & `img2table-0.0.24/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/paddle/test_paddle.py` & `img2table-0.0.24/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/pdf/test_data/content.json` & `img2table-0.0.24/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.0.24/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.0.24/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.0.24/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/tesseract/test_data/test.png` & `img2table-0.0.24/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.0.24/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/image/test_data/expected_tables.json` & `img2table-0.0.24/tests/tables/image/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/image/test_data/ocr.csv` & `img2table-0.0.24/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/image/test_data/test.png` & `img2table-0.0.24/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/image/test_image.py` & `img2table-0.0.24/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_data/expected_tables.json` & `img2table-0.0.24/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_data/ocr.csv` & `img2table-0.0.24/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_data/tables.json` & `img2table-0.0.24/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_extraction.py` & `img2table-0.0.24/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_line.py` & `img2table-0.0.24/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_row.py` & `img2table-0.0.24/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/objects/test_table.py` & `img2table-0.0.24/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv` & `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv` & `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv` & `img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv` & `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/common/test_common.py` & `img2table-0.0.24/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.0.24/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.0.24/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.0.24/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/text/test_data/table.json` & `img2table-0.0.24/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.0.24/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.23/tests/tables/processing/text/test_titles.py` & `img2table-0.0.24/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

