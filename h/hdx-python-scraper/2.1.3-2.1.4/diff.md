# Comparing `tmp/hdx-python-scraper-2.1.3.tar.gz` & `tmp/hdx-python-scraper-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-scraper-2.1.3.tar", last modified: Mon Feb 13 02:34:30 2023, max compression
+gzip compressed data, was "hdx-python-scraper-2.1.4.tar", last modified: Tue Apr 11 01:57:18 2023, max compression
```

## Comparing `hdx-python-scraper-2.1.3.tar` & `hdx-python-scraper-2.1.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.489211 hdx-python-scraper-2.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.449211 hdx-python-scraper-2.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-13 02:34:30.489211 hdx-python-scraper-2.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    62092 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-02-13 02:34:30.489211 hdx-python-scraper-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.449211 hdx-python-scraper-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.449211 hdx-python-scraper-2.1.3/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/src/hdx/scraper/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/base_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14976 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/resource_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14572 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/rowparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2197 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/excelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/googlesheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9499 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    46910 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/fallbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/region_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 02:34:30.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 02:34:28.000000 hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.449211 hdx-python-scraper-2.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.453211 hdx-python-scraper-2.1.3/tests/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)    63512 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/config/project_configuration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.485211 hdx-python-scraper-2.1.3/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/additional-json.json
--rw-r--r--   0 runner    (1001) docker     (123)    57147 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cbpf-allocations-and-contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cbpf2-allocations-and-contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cerf-covid-19-allocations.json
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cerf2-covid-19-allocations.json
--rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
--rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   201089 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/covidtests_data-owid-covid-data.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/download-hno-2017-sahel-nutrition.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/education_closures_download-covid-impact-education.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ethiopia-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/fallbacks.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/global-school-closures-covid19.json
--rw-r--r--   0 runner    (1001) docker     (123)    78566 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/idmc-internally-displaced-persons-idps.json
--rw-r--r--   0 runner    (1001) docker     (123)    51259 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/idps_download-displacement-data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
--rw-r--r--   0 runner    (1001) docker     (123)  1371019 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/kenya-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/population.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rw-r--r--   0 runner    (1001) docker     (123)    19982 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/sadd-countries-to-include.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/sahel-humanitarian-needs-overview.json
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/somalia-acute-food-insecurity-country-data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/somalia-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/somalia-internally-displaced-persons-idps.json
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5328 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/test_output.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/test_scraper_all.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/test_scraper_other.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/test_scraper_population.json
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/total-covid-19-tests-performed-by-country.json
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ukraine-border-crossings.json
--rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/ukraine-who-does-what-where-3w.json
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/unocha-office-locations.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/who_national2_who-covid-19-global-data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/who_national_who-covid-19-global-data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/whowhatwhere_afg_3w_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/fixtures/whowhatwhere_notags_3w_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.449211 hdx-python-scraper-2.1.3/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:34:30.489211 hdx-python-scraper-2.1.3/tests/hdx/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/affected_targeted_reached.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/education_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/education_enrolment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7256 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8566 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_regionlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_runner_get_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_appenddata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25503 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_multipleurls.py
--rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_national.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_resource_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_subnational.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-13 02:34:10.000000 hdx-python-scraper-2.1.3/tests/hdx/scraper/unhcr_myanmar_idps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.304261 hdx-python-scraper-2.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/.github/workflows/run-python-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-11 01:57:18.304261 hdx-python-scraper-2.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/doc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62092 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/doc/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-04-11 01:57:18.304261 hdx-python-scraper-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/src/hdx/scraper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/base_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14976 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/resource_downloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14572 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/rowparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2197 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/excelfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/googlesheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9499 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46947 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/fallbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/region_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 01:57:18.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:57:16.000000 hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.268261 hdx-python-scraper-2.1.4/tests/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63512 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/config/project_configuration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.300261 hdx-python-scraper-2.1.4/tests/fixtures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/fixtures/additional-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57147 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-11 01:57:00.000000 hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cbpf-allocations-and-contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cbpf2-allocations-and-contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cerf-covid-19-allocations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cerf2-covid-19-allocations.json
+-rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   201089 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/covidtests_data-owid-covid-data.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/download-hno-2017-sahel-nutrition.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/education_closures_download-covid-impact-education.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ethiopia-drought-related-key-figures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/fallbacks.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/global-school-closures-covid19.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78566 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/idmc-internally-displaced-persons-idps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51259 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/idps_download-displacement-data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1371019 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/kenya-drought-related-key-figures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/population.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    19982 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/sadd-countries-to-include.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/sahel-humanitarian-needs-overview.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/somalia-acute-food-insecurity-country-data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/somalia-drought-related-key-figures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/somalia-internally-displaced-persons-idps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5328 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/test_output.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/test_scraper_all.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/test_scraper_other.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/test_scraper_population.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/total-covid-19-tests-performed-by-country.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ukraine-border-crossings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/ukraine-who-does-what-where-3w.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/unocha-office-locations.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/who_national2_who-covid-19-global-data.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/who_national_who-covid-19-global-data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/whowhatwhere_afg_3w_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/fixtures/whowhatwhere_notags_3w_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.264261 hdx-python-scraper-2.1.4/tests/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:57:18.304261 hdx-python-scraper-2.1.4/tests/hdx/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/affected_targeted_reached.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/education_closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/education_enrolment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7256 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8566 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_regionlookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_runner_get_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_appenddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25503 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_multipleurls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26538 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_resource_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_subnational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-11 01:57:01.000000 hdx-python-scraper-2.1.4/tests/hdx/scraper/unhcr_myanmar_idps.py
```

### Comparing `hdx-python-scraper-2.1.3/.github/workflows/publish.yml` & `hdx-python-scraper-2.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/.github/workflows/run-python-tests.yml` & `hdx-python-scraper-2.1.4/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/.gitignore` & `hdx-python-scraper-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/LICENSE` & `hdx-python-scraper-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/PKG-INFO` & `hdx-python-scraper-2.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-scraper
-Version: 2.1.3
+Version: 2.1.4
 Summary: HDX Python scraper utilities to assemble data from multiple sources
 Home-page: https://github.com/OCHA-DAP/hdx-python-scraper
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,scrapers,data assembly,data transformation,tabular data,library
 Platform: any
@@ -26,15 +26,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: pandas
 License-File: LICENSE
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/workflows/build/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions?query=workflow%3Abuild)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 The HDX Python Scraper Library is designed to enable you to easily develop code that 
 assembles data from one or more tabular sources that can be csv, xls, xlsx or JSON. It 
 uses a YAML file that specifies for each source what needs to be read and allows some
```

### Comparing `hdx-python-scraper-2.1.3/README.md` & `hdx-python-scraper-2.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/workflows/build/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions?query=workflow%3Abuild)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 The HDX Python Scraper Library is designed to enable you to easily develop code that 
 assembles data from one or more tabular sources that can be csv, xls, xlsx or JSON. It 
 uses a YAML file that specifies for each source what needs to be read and allows some
```

### Comparing `hdx-python-scraper-2.1.3/doc/main.md` & `hdx-python-scraper-2.1.4/doc/main.md`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/pyproject.toml` & `hdx-python-scraper-2.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/setup.cfg` & `hdx-python-scraper-2.1.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -34,20 +34,20 @@
 zip_safe = True
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
-	hdx-python-api>=5.9.8
+	hdx-python-api>=5.9.9
 	gspread
 	regex
 
 [options.extras_require]
-pandas = pandas>=1.5.3
+pandas = pandas>=2.0.0
 
 [options.packages.find]
 where = src
 
 [bdist_wheel]
 universal = 1
```

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/base_scraper.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/base_scraper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/aggregator.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/aggregator.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/resource_downloader.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/rowparser.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/rowparser.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/scraper.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/scraper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/configurable/timeseries.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/configurable/timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/base.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/base.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/excelfile.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/excelfile.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/googlesheets.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/googlesheets.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/outputs/json.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/outputs/json.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/runner.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from datetime import datetime
+from traceback import format_exc
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from hdx.location.adminlevel import AdminLevel
 from hdx.utilities.dateparse import now_utc
 from hdx.utilities.errors_onexit import ErrorsOnExit
 from hdx.utilities.typehint import ListTuple
 
@@ -581,21 +582,21 @@
             try:
                 scraper.pre_run()
                 scraper.run()
                 scraper.add_sources()
                 scraper.add_source_urls()
                 scraper.add_population()
                 logger.info(f"Processed {scraper.name}")
-            except Exception as ex:
+            except Exception:
                 if not Fallbacks.exist() or scraper.can_fallback is False:
                     raise
                 logger.exception(f"Using fallbacks for {scraper.name}!")
                 if self.errors_on_exit:
                     self.errors_on_exit.add(
-                        f"Using fallbacks for {scraper.name}! Error: {ex}"
+                        f"Using fallbacks for {scraper.name}! Error: {format_exc()}"
                     )
                 for level in scraper.headers.keys():
                     values, sources = Fallbacks.get(
                         level, scraper.headers[level]
                     )
                     scraper.values[level] = values
                     scraper.sources[level] = sources
```

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/__init__.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/fallbacks.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/fallbacks.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/reader.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/region_lookup.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/region_lookup.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/sources.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/sources.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx/scraper/utilities/writer.py` & `hdx-python-scraper-2.1.4/src/hdx/scraper/utilities/writer.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/PKG-INFO` & `hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-scraper
-Version: 2.1.3
+Version: 2.1.4
 Summary: HDX Python scraper utilities to assemble data from multiple sources
 Home-page: https://github.com/OCHA-DAP/hdx-python-scraper
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,scrapers,data assembly,data transformation,tabular data,library
 Platform: any
@@ -26,15 +26,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: pandas
 License-File: LICENSE
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/workflows/build/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions?query=workflow%3Abuild)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 The HDX Python Scraper Library is designed to enable you to easily develop code that 
 assembles data from one or more tabular sources that can be csv, xls, xlsx or JSON. It 
 uses a YAML file that specifies for each source what needs to be read and allows some
```

### Comparing `hdx-python-scraper-2.1.3/src/hdx_python_scraper.egg-info/SOURCES.txt` & `hdx-python-scraper-2.1.4/src/hdx_python_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/config/project_configuration.yml` & `hdx-python-scraper-2.1.4/tests/config/project_configuration.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cbpf-allocations-and-contributions.json` & `hdx-python-scraper-2.1.4/tests/fixtures/cbpf-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cbpf2-allocations-and-contributions.json` & `hdx-python-scraper-2.1.4/tests/fixtures/cbpf2-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cerf-covid-19-allocations.json` & `hdx-python-scraper-2.1.4/tests/fixtures/cerf-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cerf2-covid-19-allocations.json` & `hdx-python-scraper-2.1.4/tests/fixtures/cerf2-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/covidtests_data-owid-covid-data.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/covidtests_data-owid-covid-data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/download-hno-2017-sahel-nutrition.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/download-hno-2017-sahel-nutrition.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ethiopia-drought-related-key-figures.json` & `hdx-python-scraper-2.1.4/tests/fixtures/ethiopia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json` & `hdx-python-scraper-2.1.4/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/fallbacks.json` & `hdx-python-scraper-2.1.4/tests/fixtures/fallbacks.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/global-school-closures-covid19.json` & `hdx-python-scraper-2.1.4/tests/fixtures/global-school-closures-covid19.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/idmc-internally-displaced-persons-idps.json` & `hdx-python-scraper-2.1.4/tests/fixtures/idmc-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/idps_download-displacement-data.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/idps_download-displacement-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json` & `hdx-python-scraper-2.1.4/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/kenya-drought-related-key-figures.json` & `hdx-python-scraper-2.1.4/tests/fixtures/kenya-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json` & `hdx-python-scraper-2.1.4/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/population.json` & `hdx-python-scraper-2.1.4/tests/fixtures/population.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx-python-scraper-2.1.4/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx-python-scraper-2.1.4/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/sahel-humanitarian-needs-overview.json` & `hdx-python-scraper-2.1.4/tests/fixtures/sahel-humanitarian-needs-overview.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/somalia-acute-food-insecurity-country-data.json` & `hdx-python-scraper-2.1.4/tests/fixtures/somalia-acute-food-insecurity-country-data.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/somalia-drought-related-key-figures.json` & `hdx-python-scraper-2.1.4/tests/fixtures/somalia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/somalia-internally-displaced-persons-idps.json` & `hdx-python-scraper-2.1.4/tests/fixtures/somalia-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json` & `hdx-python-scraper-2.1.4/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/test_output.xlsx` & `hdx-python-scraper-2.1.4/tests/fixtures/test_output.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/total-covid-19-tests-performed-by-country.json` & `hdx-python-scraper-2.1.4/tests/fixtures/total-covid-19-tests-performed-by-country.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ukraine-border-crossings.json` & `hdx-python-scraper-2.1.4/tests/fixtures/ukraine-border-crossings.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/ukraine-who-does-what-where-3w.json` & `hdx-python-scraper-2.1.4/tests/fixtures/ukraine-who-does-what-where-3w.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/unocha-office-locations.json` & `hdx-python-scraper-2.1.4/tests/fixtures/unocha-office-locations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/who_national2_who-covid-19-global-data.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/who_national2_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/who_national_who-covid-19-global-data.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/who_national_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/fixtures/whowhatwhere_afg_3w_data.csv` & `hdx-python-scraper-2.1.4/tests/fixtures/whowhatwhere_afg_3w_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/__init__.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/affected_targeted_reached.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/affected_targeted_reached.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/conftest.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/education_closures.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/education_closures.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/education_enrolment.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/education_enrolment.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_output.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_output.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_readers.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_readers.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_regionlookup.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_regionlookup.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_runner_get_results.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_runner_get_results.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_aggregation.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_aggregation.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_appenddata.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_appenddata.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_custom.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_custom.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_global.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_global.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_multipleurls.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_multipleurls.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_national.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_national.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,17 +533,20 @@
             runner,
             level,
             headers,
             values,
             sources,
             fallbacks_used=True,
         )
-        assert errors_on_exit.errors == [
-            "Using fallbacks for broken_owd_url! Error: [scheme-error] The data source could not be successfully loaded: [Errno 2] No such file or directory: 'tests/fixtures/broken_owd_url_notexist.csv'"
-        ]
+        error = errors_on_exit.errors[0]
+        assert "Using fallbacks for broken_owd_url!" in error
+        assert (
+            "No such file or directory: 'tests/fixtures/broken_owd_url_notexist.csv'"
+            in error
+        )
 
     def test_get_national_afg_mmr_phl(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2021-05-03")
         errors_on_exit = ErrorsOnExit()
         level = "national"
         countries = ("AFG", "MMR", "PHL")
```

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_regionaltoplevel.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_regionaltoplevel.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_resource_downloaders.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_resource_downloaders.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_subnational.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_subnational.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_scrapers_timeseries.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_scrapers_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/test_sources.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/test_sources.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.3/tests/hdx/scraper/unhcr_myanmar_idps.py` & `hdx-python-scraper-2.1.4/tests/hdx/scraper/unhcr_myanmar_idps.py`

 * *Files identical despite different names*

