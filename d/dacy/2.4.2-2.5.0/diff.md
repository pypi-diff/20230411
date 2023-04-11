# Comparing `tmp/dacy-2.4.2.tar.gz` & `tmp/dacy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacy-2.4.2.tar", last modified: Wed Mar 15 08:34:53 2023, max compression
+gzip compressed data, was "dacy-2.5.0.tar", last modified: Tue Apr 11 00:07:56 2023, max compression
```

## Comparing `dacy-2.4.2.tar` & `dacy-2.5.0.tar`

### file list

```diff
@@ -1,206 +1,205 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.209430 dacy-2.4.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      713 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      651 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      578 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      816 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      869 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     3141 2023-03-15 08:34:40.000000 dacy-2.4.2/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2186 2023-03-15 08:34:40.000000 dacy-2.4.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      830 2023-03-15 08:34:40.000000 dacy-2.4.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     6374 2023-03-15 08:34:41.000000 dacy-2.4.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-15 08:34:40.000000 dacy-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    21563 2023-03-15 08:34:53.209430 dacy-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7202 2023-03-15 08:34:40.000000 dacy-2.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)      548 2023-03-15 08:34:40.000000 dacy-2.4.2/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/dev/model_comparison/
--rw-r--r--   0 root         (0) root         (0)     3396 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/model_comparison/model_comparison.Rmd
--rw-r--r--   0 root         (0) root         (0)      205 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/model_comparison/model_comparison.Rproj
--rw-r--r--   0 root         (0) root         (0)     2194 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/model_comparison/utility.R
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.169430 dacy-2.4.2/dev/new_projects/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.173430 dacy-2.4.2/dev/new_projects/token_aug/
--rw-r--r--   0 root         (0) root         (0)   748506 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/new_projects/token_aug/ddo-synonyms.csv
--rw-r--r--   0 root         (0) root         (0)   427255 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/new_projects/token_aug/ddo_misspellings_2020-08-26.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.177430 dacy-2.4.2/dev/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34838 2023-03-15 08:34:40.000000 dacy-2.4.2/dev/utilities/twitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.177430 dacy-2.4.2/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.185430 dacy-2.4.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)  1426134 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
--rw-r--r--   0 root         (0) root         (0)    52158 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/asent_analysis.png
--rw-r--r--   0 root         (0) root         (0)    15586 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/asent_prediction.png
--rw-r--r--   0 root         (0) root         (0)    63171 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/dep_parse.png
--rw-r--r--   0 root         (0) root         (0)    61244 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/dep_robustness.png
--rw-r--r--   0 root         (0) root         (0)    15406 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   185775 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   185775 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/icon_black_text.png
--rw-r--r--   0 root         (0) root         (0)   189414 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   154866 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/icon_no_title.png
--rw-r--r--   0 root         (0) root         (0)    12272 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/ner.png
--rw-r--r--   0 root         (0) root         (0)   103739 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/ner_robustness.png
--rw-r--r--   0 root         (0) root         (0)    77390 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/perf.png
--rw-r--r--   0 root         (0) root         (0)    65393 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/perf_l.png
--rw-r--r--   0 root         (0) root         (0)    69095 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/pos_robustness.png
--rw-r--r--   0 root         (0) root         (0)   661625 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/table_dep.html
--rw-r--r--   0 root         (0) root         (0)   666232 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/table_ent.html
--rw-r--r--   0 root         (0) root         (0)   664139 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/table_perf.html
--rw-r--r--   0 root         (0) root         (0)   662541 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/_static/table_pos.html
--rw-r--r--   0 root         (0) root         (0)     3884 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/dacy.datasets.rst
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/dacy.download.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/dacy.score.rst
--rw-r--r--   0 root         (0) root         (0)     2948 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2862 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     4714 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     4201 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/performance.general.rst
--rw-r--r--   0 root         (0) root         (0)     6139 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/performance.robustness.rst
--rw-r--r--   0 root         (0) root         (0)      223 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/performance.rst
--rw-r--r--   0 root         (0) root         (0)      993 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/using_dacy.augmentation.rst
--rw-r--r--   0 root         (0) root         (0)     4937 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/using_dacy.getting_started.rst
--rw-r--r--   0 root         (0) root         (0)     4303 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/using_dacy.hate_speech.rst
--rw-r--r--   0 root         (0) root         (0)     1826 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/using_dacy.rst
--rw-r--r--   0 root         (0) root         (0)    13569 2023-03-15 08:34:40.000000 dacy-2.4.2/docs/using_dacy.sentiment.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.169430 dacy-2.4.2/papers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.189430 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.189430 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
--rw-r--r--   0 root         (0) root         (0)     2395 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
--rw-r--r--   0 root         (0) root         (0)  2323089 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
--rw-r--r--   0 root         (0) root         (0)     4893 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
--rw-r--r--   0 root         (0) root         (0)     2848 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
--rw-r--r--   0 root         (0) root         (0)    12383 2023-03-15 08:34:40.000000 dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
--rw-r--r--   0 root         (0) root         (0)     3582 2023-03-15 08:34:41.000000 dacy-2.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 08:34:53.209430 dacy-2.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.169430 dacy-2.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.189430 dacy-2.4.2/src/dacy/
--rw-r--r--   0 root         (0) root         (0)      295 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/datasets/
--rw-r--r--   0 root         (0) root         (0)      227 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/constants.py
--rw-r--r--   0 root         (0) root         (0)     3496 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/dane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/datasets/lookup_tables/
--rw-r--r--   0 root         (0) root         (0)      578 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/lookup_tables/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/lookup_tables/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126210 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/lookup_tables/names.csv
--rw-r--r--   0 root         (0) root         (0)     4530 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/datasets/names.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/hate_speech/
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/hate_speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/hate_speech/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/ner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/ner/wrapped_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/score/
--rw-r--r--   0 root         (0) root         (0)       81 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/score/input_length.py
--rw-r--r--   0 root         (0) root         (0)     5986 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/score/score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy/sentiment/
--rw-r--r--   0 root         (0) root         (0)       61 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/sentiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5380 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/sentiment/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-03-15 08:34:40.000000 dacy-2.4.2/src/dacy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.193430 dacy-2.4.2/src/dacy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21563 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6176 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      597 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-15 08:34:53.000000 dacy-2.4.2/src/dacy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      843 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_datasets.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_hate_speech.py
--rw-r--r--   0 root         (0) root         (0)      373 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_ner.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_score.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_sentiment.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-03-15 08:34:40.000000 dacy-2.4.2/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/training/
--rw-r--r--   0 root         (0) root         (0)     3495 2023-03-15 08:34:40.000000 dacy-2.4.2/training/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/training/v0.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/training/v0.0.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4458 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/configs/config_-l-ctra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4449 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/configs/config_conv_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4467 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/configs/config_electra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4432 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4440 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/configs/config_medium.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/training/v0.0.0/img/
--rw-r--r--   0 root         (0) root         (0)    40449 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/img/perf_training.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.197430 dacy-2.4.2/training/v0.0.0/metrics/
--rw-r--r--   0 root         (0) root         (0)     3582 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_-l-ctra_cased.json
--rw-r--r--   0 root         (0) root         (0)     3594 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
--rw-r--r--   0 root         (0) root         (0)     3591 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_conv_small.json
--rw-r--r--   0 root         (0) root         (0)     3638 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_electra.json
--rw-r--r--   0 root         (0) root         (0)     4728 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_large.json
--rw-r--r--   0 root         (0) root         (0)     4741 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/metrics/dane_medium.json
--rw-r--r--   0 root         (0) root         (0)     1100 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/orth_variants.json
--rw-r--r--   0 root         (0) root         (0)     9596 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/project.yml
--rw-r--r--   0 root         (0) root         (0)       87 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      439 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.0.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.201430 dacy-2.4.2/training/v0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6617 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.201430 dacy-2.4.2/training/v0.1.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4633 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4640 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4635 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/configs/config_small.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.201430 dacy-2.4.2/training/v0.1.0/metrics/
--rw-r--r--   0 root         (0) root         (0)   237018 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236140 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   237616 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5506 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5502 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5595 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5454 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5557 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5629 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15843 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.205430 dacy-2.4.2/training/v0.1.1/
--rw-r--r--   0 root         (0) root         (0)     7458 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.205430 dacy-2.4.2/training/v0.1.1/configs/
--rw-r--r--   0 root         (0) root         (0)     4619 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4626 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4621 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/configs/config_small.cfg
--rw-r--r--   0 root         (0) root         (0)     1992 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/danish_augmenter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.205430 dacy-2.4.2/training/v0.1.1/metrics/
--rw-r--r--   0 root         (0) root         (0)   236308 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236675 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   238715 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5488 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5522 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5592 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5473 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5485 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5601 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15923 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-03-15 08:34:40.000000 dacy-2.4.2/training/v0.1.1/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:34:53.209430 dacy-2.4.2/tutorials/
--rw-r--r--   0 root         (0) root         (0)    16340 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/dacy-basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    38219 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/dacy-robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)     5333 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     9763 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/sentiment-neural.ipynb
--rw-r--r--   0 root         (0) root         (0)     8741 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/sentiment-rule-based.ipynb
--rw-r--r--   0 root         (0) root         (0)   106539 2023-03-15 08:34:40.000000 dacy-2.4.2/tutorials/textdescriptives_integration.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 00:07:43.000000 dacy-2.5.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 00:07:43.000000 dacy-2.5.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/mypy.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 00:07:43.000000 dacy-2.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 00:07:43.000000 dacy-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     7737 2023-04-11 00:07:44.000000 dacy-2.5.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 00:07:43.000000 dacy-2.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 00:07:43.000000 dacy-2.5.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 00:07:43.000000 dacy-2.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:07:56.051463 dacy-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6594 2023-04-11 00:07:43.000000 dacy-2.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 00:07:43.000000 dacy-2.5.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.995460 dacy-2.5.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.011461 dacy-2.5.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
+-rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/asent_analysis.png
+-rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/asent_prediction.png
+-rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/dep_parse.png
+-rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/dep_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_black_text.png
+-rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_no_title.png
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/ner.png
+-rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/ner_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/perf.png
+-rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/perf_l.png
+-rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/pos_robustness.png
+-rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_dep.html
+-rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_ent.html
+-rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_perf.html
+-rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_pos.html
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/adv_tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.011461 dacy-2.5.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.download.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.score.rst
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/faq.md
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.general.rst
+-rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.robustness.rst
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.rst
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.015461 dacy-2.5.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    26285 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38230 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)    21177 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/sentiment.ipynb
+-rw-r--r--   0 root         (0) root         (0)   106814 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/textdescriptives.ipynb
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.983460 dacy-2.5.0/papers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.019461 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.023461 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
+-rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-04-11 00:07:44.000000 dacy-2.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 00:07:56.051463 dacy-2.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.983460 dacy-2.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.023461 dacy-2.5.0/src/dacy/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy/datasets/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/dane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy/datasets/lookup_tables/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/names.csv
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/names.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/hate_speech/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/hate_speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/hate_speech/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/ner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/ner/wrapped_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/score/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/input_length.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/sentiment/
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/sentiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/sentiment/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6144 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      660 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 00:07:43.000000 dacy-2.5.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_datasets.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_hate_speech.py
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_score.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/
+-rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 00:07:43.000000 dacy-2.5.0/training/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_-l-ctra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_conv_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_electra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_medium.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/img/
+-rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/img/perf_training.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.0.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_cased.json
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_conv_small.json
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_electra.json
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_large.json
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_medium.json
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/orth_variants.json
+-rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.1.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_small.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.043462 dacy-2.5.0/training/v0.1.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.047463 dacy-2.5.0/training/v0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.047463 dacy-2.5.0/training/v0.1.1/configs/
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/danish_augmenter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/training/v0.1.1/metrics/
+-rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    16340 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/dacy-basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38219 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/dacy-robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     9763 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/sentiment-neural.ipynb
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/sentiment-rule-based.ipynb
+-rw-r--r--   0 root         (0) root         (0)   106539 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/textdescriptives_integration.ipynb
```

### Comparing `dacy-2.4.2/.github/ISSUE_TEMPLATE/01_bugs.md` & `dacy-2.5.0/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/.github/ISSUE_TEMPLATE/config.yml` & `dacy-2.5.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/.github/workflows/documentation.yml` & `dacy-2.5.0/.github/workflows/documentation.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+# creates the documentation on pushes it to the gh-pages branch
 name: Documentation
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     concurrency: documentation
-
     steps:
       - name: Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
 
       - name: Install dependencies
         shell: bash
         run: |
           python -m pip install --upgrade pip
+          pip install -r docs/requirements.txt
           pip install ".[docs]"
 
       - name: Build and Commit
         uses: sphinx-notes/pages@2.1
         with:
           documentation_path: docs
 
       - name: Push changes
         if: ${{ github.event_name == 'push' }}
         uses: ad-m/github-push-action@v0.6.0
         with:
-          github_token: ${{ secrets.SPHINX_DOCUMENTATION }}
+          github_token: ${{ secrets.GITHUB_TOKEN }}
           branch: gh-pages
```

### Comparing `dacy-2.4.2/.github/workflows/tests.yml` & `dacy-2.5.0/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,87 @@
+# This workflow will install Python dependencies, run pytests and run notebooks
+# then it will in python 3.9 (ubuntu-latest) create a badge with the coverage
+# and add it to the PR. This badge will be updated if the PR is updated.
+
 name: Tests
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
-  pytest-and-notebooks:
+  pytest:
     runs-on: ${{ matrix.os }}
+    permissions:
+      contents: read
+      issues: read
+      checks: write
+      pull-requests: write
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.9", "3.8"]
+        python-version: ["3.9", "3.10"]
 
     # This allows a subsequently queued workflow run to interrupt previous runs
     concurrency:
-      group: "${{ github.workflow }} - ${{ matrix.python-version}} - ${{ matrix.os }} @ ${{ github.ref }}"
+      group: "${{ github.workflow }}-${{ matrix.python-version}}-${{ matrix.os }} @ ${{ github.ref }}"
       cancel-in-progress: true
 
     steps:
       - uses: actions/checkout@v3
 
+      - name: Cache venv
+        uses: actions/cache@v3.2.6
+        id: cache_venv
+        with:
+          path: |
+            .venv
+          key: ${{ runner.os }}-venv-${{ matrix.python-version }}-${{ hashFiles('**/pyproject.toml') }}
+
       - name: Set up Python
         uses: actions/setup-python@v4
+        id: setup_python
+        if: steps.cache_venv.outputs.cache-hit != 'true'
         with:
           python-version: ${{ matrix.python-version }}
-          cache: "pip"
-          cache-dependency-path: "**/pyproject.toml"
 
       - name: Install dependencies
         shell: bash
         run: |
+          python -m venv .venv
+          if [ "${{ matrix.os }}" == "windows-latest" ]; then
+            source .venv/Scripts/activate
+          else
+            source .venv/bin/activate
+          fi
           python -m pip install --upgrade pip
-          pip install ".[tests]"
+          pip install -e .[tests]
 
       - name: Run and write pytest
         shell: bash
         run: |
-          set -o pipefail
-          pytest --cov=dacy --cov-report term-missing | tee pytest-coverage.txt
-
-      - name: Install dependencies for notebooks
-        if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' }}
-        # to save time and also to avoid dependency conflicts of NERDA==1.0.0
-        shell: bash
-        run: |
-          pip install ".[tutorials]"
-          pip install -r ./tutorials/requirements.txt
-
-      - name: Convert and run notebooks
-        if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' }}
-        # to save time and also to avoid dependency conflicts of NERDA==1.0.0
-        shell: bash
-        run: |
-          jupyter nbconvert --to python ./tutorials/*.ipynb
-          for f in tutorials/*.py; do python "$f"; done
+          if [ "${{ matrix.os }}" == "windows-latest" ]; then
+            source .venv/Scripts/activate
+          else
+            source .venv/bin/activate
+          fi
+          pytest --durations=0 -n 2 -x --junitxml=pytest.xml --cov-report=term-missing --cov=src/ tests/
+
+      - name: Test report on failures
+        uses: EnricoMi/publish-unit-test-result-action@v2
+        id: test_report_with_annotations
+        if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' && github.actor != 'dependabot[bot]' && github.event_name == 'pull_request' && (success() || failure()) }} # Do not run for dependabot, run whether tests failed or succeeded
+        with:
+          comment_mode: "failures"
+          files: |
+            pytest.xml
 
-      # if it is run on ubuntu-latest, python 3.9, then create the badge
       - name: Pytest coverage comment
-        if:
-          ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' }}
-          # to save time and also to avoid dependency conflicts of NERDA==1.0.0
         id: coverage-comment
-        uses: MishaKav/pytest-coverage-comment@v1.1.43
-        with:
-          pytest-coverage-path: ./pytest-coverage.txt
-
-      - name: Check the output coverage
-        if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' }}
-        shell: bash
-        run: |
-          echo "Coverage Report - ${{ steps.coverage-comment.outputs.coverage }}"
-          echo "Coverage Color - ${{ steps.coverage-comment.outputs.color }}"
-
-      # and if it is a push to main then create the badge
-      - name: Create the Badge
-        if: ${{ github.event_name == 'push' && matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' }}
-        uses: schneegans/dynamic-badges-action@v1.6.0
+        uses: MishaKav/pytest-coverage-comment@main
+        if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.9' &&  github.actor != 'dependabot[bot]' && github.event_name == 'pull_request' && (success() || failure()) }}
         with:
-          auth: ${{ secrets.PYTEST_COVERAGE_COMMENT }}
-          gistID: af8637d94475ea8bcb6b6a03c4fbcd3e
-          filename: badge-dacy-pytest-coverage.json
-          label: Coverage
-          message: ${{ steps.coverage-comment.outputs.coverage }}
-          color: ${{ steps.coverage-comment.outputs.color }}
-          namedLogo: python
+          create-new-comment: false
+          report-only-changed-files: true
+          pytest-coverage-path: pytest-coverage.txt
+          junitxml-path: ./pytest.xml
```

### Comparing `dacy-2.4.2/.gitignore` & `dacy-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/CHANGELOG.md` & `dacy-2.5.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.5.0 (2023-04-11)
+### Feature
+* Moved dacy to use swift template ([`189c891`](https://github.com/centre-for-humanities-computing/DaCy/commit/189c891323f1ff083d1800fc3acd435c456fd1b5))
+
+### Fix
+* Mypy ([`3b78e18`](https://github.com/centre-for-humanities-computing/DaCy/commit/3b78e18ef93a09fe2d152a5b9790c521ecffeb02))
+* Removed support for old version 0.0.0 versions ([`17649c3`](https://github.com/centre-for-humanities-computing/DaCy/commit/17649c31fb30cd083d1864b1e9b38389bb543cfd))
+* Fixed mypy error ([`38b788a`](https://github.com/centre-for-humanities-computing/DaCy/commit/38b788a16ce9e9d4cf5033984c8331bdfbdc7f46))
+* Dane now download correctly ([`455ac20`](https://github.com/centre-for-humanities-computing/DaCy/commit/455ac201dadd7047b044cd76a98944244fdf9dd9))
+* Fix mypy ([`4dc0df0`](https://github.com/centre-for-humanities-computing/DaCy/commit/4dc0df0158679ffc66ea9dbae6fcf54576340d88))
+
+### Documentation
+* Updated cff ([`06b1878`](https://github.com/centre-for-humanities-computing/DaCy/commit/06b187864a5da1f4646645f8da92625c4cf4300c))
+* Added github stars to index ([`4229f9e`](https://github.com/centre-for-humanities-computing/DaCy/commit/4229f9eb5eff5b2e5d2e8aaa5747b5dc94ca5134))
+* Updated docs to swift template ([`966c953`](https://github.com/centre-for-humanities-computing/DaCy/commit/966c95367ea281f3c89bbad9691da51bc0413de8))
+
 ## v2.4.2 (2023-03-15)
 ### Fix
 * Checking to find the latest model ([`50d3d5c`](https://github.com/centre-for-humanities-computing/DaCy/commit/50d3d5c420861af3746b42a80f6a2054c8840cdd))
 
 ## v2.4.1 (2023-03-14)
 ### Fix
 * Formatting erro in model urls ([`0478965`](https://github.com/centre-for-humanities-computing/DaCy/commit/04789655654dedae3f6e61a884fa084fe546f429))
```

### Comparing `dacy-2.4.2/LICENSE` & `dacy-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/PKG-INFO` & `dacy-2.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.4.2
+Version: 2.5.0
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
-Author: Lasse Hansen
-Author-email: Kenneth Enevoldsen <kennethcenevolsen@gmail.com>
+Author: Lasse Hansen, Emil Jessen
+Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -216,57 +216,54 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: style
+Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
-Provides-Extra: tutorials
 License-File: LICENSE
 
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
-# DaCy: An efficient NLP Pipeline for Danish
+# DaCy: An efficient and unified framework for danish NLP
 
-[![PyPI version](https://badge.fury.io/py/dacy.svg)](https://pypi.org/project/dacy/)
+[![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
-[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/DaCy)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
-[![github actions pytest](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/tests.yml/badge.svg)](https://github.com/centre-for-humanities-computing/Dacy/actions)
-[![github actions docs](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/documentation.yml/badge.svg)](https://centre-for-humanities-computing.github.io/DaCy/)
-<!-- 
-![github coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/KennethEnevoldsen/af8637d94475ea8bcb6b6a03c4fbcd3e/raw/badge-dacy-pytest-coverage.json)
--->
+[![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
+
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
+[pypi status]: https://pypi.org/project/dacy/
+[documentation]: https://centre-for-humanities-computing.github.io/dacy/
+[tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
+[black]: https://github.com/psf/black
 
 
+<!-- start short-description -->
 DaCy is a Danish natural language preprocessing framework made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance on Named entity recognition, part-of-speech tagging and dependency parsing for Danish. Feel free to try out the [demo](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.). This repository contains material for using DaCy, reproducing the results and guides on usage of the package. Furthermore, it also contains behavioural tests for biases and robustness of Danish NLP pipelines.
+<!-- end short-description -->
 
-<!--
-EASTER EGG:
-https://www.youtube.com/watch?v=E7WQ1tdxSqI
--->
+## 🔧 Installation
 
+You can install `dacy` via [pip] from [PyPI]:
 
-# 🔧 Installation
-To get started using DaCy simply install it using pip by running the following line in your terminal:
 ```bash
 pip install dacy
 ```
 
-
-# 👩‍💻 Usage
+## 👩‍💻 Usage
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
@@ -288,21 +285,17 @@
 To download the model to a specific directory:
 ```python
 dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
 nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
 ```
 
 
-# 📖 Documentation
-
-DaCy includes detailed documentation as well as a series of Jupyter notebook tutorials.
-If you do not have Jupyter Notebook installed, instructions for installing and running
-it can be found [here]( http://jupyter.org/install). All the tutorials are located in
-the `tutorials` folder.
+To see more examples, see the [documentation].
 
+# 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
 | 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
@@ -325,35 +318,33 @@
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
 the folder `training` contains a SpaCy project which will allow for reproduction of the results. This folder also includes the evaluation metrics on DaNE and scripts for downloading the required data. For more information, please see the training [readme](training/readme.md).
 
-Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.kennethenevoldsen.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
+Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
 
-## 💬 Where to ask questions
+# 💬 Where to ask questions
 To ask report issues or request features, please use the [GitHub Issue Tracker](https://github.com/centre-for-humanities-computing/DaCy/issues).
 Questions related to SpaCy are kindly referred to the SpaCy GitHub or forum. Otherwise, please use the discussion Forums.
 
 | Type                           |                        |
 | ------------------------------ | ---------------------- |
+| 📚 **FAQ**                      | [FAQ]                  |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker] |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker] |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]   |
 | 🗯 **General Discussion**       | [GitHub Discussions]   |
 
-[github issue tracker]: https://github.com/centre-for-humanities-computing/DaCy/issues
-[github discussions]: https://github.com/centre-for-humanities-computing/DaCy/discussions
-
-
-
-
-
-
-## Acknowledgements
-DaCy is a result of great open-source software and contributors. It wouldn't have been possible without the work by the SpaCy team which developed and integrated the software. Huggingface for developing Transformers and making model sharing convenient. Multiple parties including Certainly.io and [Malte Hojmark-Bertelsen](https://github.com/MalteHB) for making their models publicly available. Alexandra Institute for developing and maintaining DaNLP which has made it easy to get access to Danish resources and even supplied some of the tagged data themselves.
+[Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
+[Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
+[Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
+[API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
+[FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
+[github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
+[github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
```

### Comparing `dacy-2.4.2/README.md` & `dacy-2.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
-# DaCy: An efficient NLP Pipeline for Danish
+# DaCy: An efficient and unified framework for danish NLP
 
-[![PyPI version](https://badge.fury.io/py/dacy.svg)](https://pypi.org/project/dacy/)
+[![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
-[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/DaCy)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
-[![github actions pytest](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/tests.yml/badge.svg)](https://github.com/centre-for-humanities-computing/Dacy/actions)
-[![github actions docs](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/documentation.yml/badge.svg)](https://centre-for-humanities-computing.github.io/DaCy/)
-<!-- 
-![github coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/KennethEnevoldsen/af8637d94475ea8bcb6b6a03c4fbcd3e/raw/badge-dacy-pytest-coverage.json)
--->
+[![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
+
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
+[pypi status]: https://pypi.org/project/dacy/
+[documentation]: https://centre-for-humanities-computing.github.io/dacy/
+[tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
+[black]: https://github.com/psf/black
 
 
+<!-- start short-description -->
 DaCy is a Danish natural language preprocessing framework made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance on Named entity recognition, part-of-speech tagging and dependency parsing for Danish. Feel free to try out the [demo](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.). This repository contains material for using DaCy, reproducing the results and guides on usage of the package. Furthermore, it also contains behavioural tests for biases and robustness of Danish NLP pipelines.
+<!-- end short-description -->
 
-<!--
-EASTER EGG:
-https://www.youtube.com/watch?v=E7WQ1tdxSqI
--->
+## 🔧 Installation
 
+You can install `dacy` via [pip] from [PyPI]:
 
-# 🔧 Installation
-To get started using DaCy simply install it using pip by running the following line in your terminal:
 ```bash
 pip install dacy
 ```
 
-
-# 👩‍💻 Usage
+## 👩‍💻 Usage
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
@@ -55,21 +54,17 @@
 To download the model to a specific directory:
 ```python
 dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
 nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
 ```
 
 
-# 📖 Documentation
-
-DaCy includes detailed documentation as well as a series of Jupyter notebook tutorials.
-If you do not have Jupyter Notebook installed, instructions for installing and running
-it can be found [here]( http://jupyter.org/install). All the tutorials are located in
-the `tutorials` folder.
+To see more examples, see the [documentation].
 
+# 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
 | 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
@@ -92,35 +87,33 @@
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
 the folder `training` contains a SpaCy project which will allow for reproduction of the results. This folder also includes the evaluation metrics on DaNE and scripts for downloading the required data. For more information, please see the training [readme](training/readme.md).
 
-Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.kennethenevoldsen.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
+Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
 
-## 💬 Where to ask questions
+# 💬 Where to ask questions
 To ask report issues or request features, please use the [GitHub Issue Tracker](https://github.com/centre-for-humanities-computing/DaCy/issues).
 Questions related to SpaCy are kindly referred to the SpaCy GitHub or forum. Otherwise, please use the discussion Forums.
 
 | Type                           |                        |
 | ------------------------------ | ---------------------- |
+| 📚 **FAQ**                      | [FAQ]                  |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker] |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker] |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]   |
 | 🗯 **General Discussion**       | [GitHub Discussions]   |
 
-[github issue tracker]: https://github.com/centre-for-humanities-computing/DaCy/issues
-[github discussions]: https://github.com/centre-for-humanities-computing/DaCy/discussions
-
-
-
-
-
-
-## Acknowledgements
-DaCy is a result of great open-source software and contributors. It wouldn't have been possible without the work by the SpaCy team which developed and integrated the software. Huggingface for developing Transformers and making model sharing convenient. Multiple parties including Certainly.io and [Malte Hojmark-Bertelsen](https://github.com/MalteHB) for making their models publicly available. Alexandra Institute for developing and maintaining DaNLP which has made it easy to get access to Danish resources and even supplied some of the tagged data themselves.
+[Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
+[Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
+[Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
+[API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
+[FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
+[github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
+[github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
```

#### html2text {}

```diff
@@ -1,51 +1,46 @@
 [https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/
-icon_black_text.png] # DaCy: An efficient NLP Pipeline for Danish [![PyPI
-version](https://badge.fury.io/py/dacy.svg)](https://pypi.org/project/dacy/) [!
-[pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/
-project/dacy/) [![python version](https://img.shields.io/badge/Python-%3E=3.8-
-blue)](https://github.com/centre-for-humanities-computing/DaCy) [![Code style:
-black](https://img.shields.io/badge/Code%20Style-Black-black)](https://
-black.readthedocs.io/en/stable/the_black_code_style/current_style.html) [!
-[github actions pytest](https://github.com/centre-for-humanities-computing/
-DaCy/actions/workflows/tests.yml/badge.svg)](https://github.com/centre-for-
-humanities-computing/Dacy/actions) [![github actions docs](https://github.com/
-centre-for-humanities-computing/DaCy/actions/workflows/documentation.yml/
-badge.svg)](https://centre-for-humanities-computing.github.io/DaCy/)  [![Demo]
-(https://img.shields.io/badge/Try%20the-Demo-important)](https://
-huggingface.co/chcaa/
+icon_black_text.png] # DaCy: An efficient and unified framework for danish NLP
+[![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status] [![pip
+downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/
+dacy/) [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi
+status] [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+[black] [![documentation](https://github.com/centre-for-humanities-computing/
+dacy/workflows/documentation/badge.svg)][documentation] [![Tests](https://
+github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/
+badge.svg)][tests] [![Demo](https://img.shields.io/badge/Try%20the-Demo-
+important)](https://huggingface.co/chcaa/
 da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
-DaCy is a Danish natural language preprocessing framework made with SpaCy. Its
-largest pipeline has achieved State-of-the-Art performance on Named entity
-recognition, part-of-speech tagging and dependency parsing for Danish. Feel
-free to try out the [demo](https://huggingface.co/chcaa/
+[pypi status]: https://pypi.org/project/dacy/ [documentation]: https://centre-
+for-humanities-computing.github.io/dacy/ [tests]: https://github.com/centre-
+for-humanities-computing/dacy/actions?workflow=Tests [black]: https://
+github.com/psf/black  DaCy is a Danish natural language preprocessing framework
+made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance
+on Named entity recognition, part-of-speech tagging and dependency parsing for
+Danish. Feel free to try out the [demo](https://huggingface.co/chcaa/
 da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.).
 This repository contains material for using DaCy, reproducing the results and
 guides on usage of the package. Furthermore, it also contains behavioural tests
-for biases and robustness of Danish NLP pipelines.  # ð§ Installation To get
-started using DaCy simply install it using pip by running the following line in
-your terminal: ```bash pip install dacy ``` # ð©âð» Usage To use the
-model you first have to download either the small, medium, or large model. To
-see a list of all available models: ```python import dacy for model in
-dacy.models(): print(model) # ... # da_dacy_small_trf-0.1.0 #
+for biases and robustness of Danish NLP pipelines.  ## ð§ Installation You
+can install `dacy` via [pip] from [PyPI]: ```bash pip install dacy ``` ##
+ð©âð» Usage To use the model you first have to download either the small,
+medium, or large model. To see a list of all available models: ```python import
+dacy for model in dacy.models(): print(model) # ... # da_dacy_small_trf-0.1.0 #
 da_dacy_medium_trf-0.1.0 # da_dacy_large_trf-0.1.0 ``` To download and load a
 model simply execute: ```python nlp = dacy.load("da_dacy_medium_tfrf-0.1.0") #
 or equivalently nlp = dacy.load("medium") ``` Which will download the model to
 the `.dacy` directory in your home directory. To download the model to a
 specific directory: ```python dacy.download_model("da_dacy_medium_trf-0.1.0",
 your_save_path) nlp = dacy.load_model("da_dacy_medium_trf-0.1.0",
-your_save_path) ``` # ð Documentation DaCy includes detailed documentation
-as well as a series of Jupyter notebook tutorials. If you do not have Jupyter
-Notebook installed, instructions for installing and running it can be found
-[here]( http://jupyter.org/install). All the tutorials are located in the
-`tutorials` folder. | Documentation | | | -------------------------- | --------
--------------------------------------------------------------------------------
----- | | ð **[Getting started]** | Guides and instructions on how to use
-DaCy and its features. | | ð¦¾ **[Performance]** | A detailed description of
-the performance of DaCy and comparison with similar Danish models | | ð **
+your_save_path) ``` To see more examples, see the [documentation]. # ð
+Documentation | Documentation | | | -------------------------- | --------------
+----------------------------------------------------------------------------- |
+| ð **[Getting started]** | Guides and instructions on how to use DaCy and
+its features. | | ð¦¾ **[Performance]** | A detailed description of the
+performance of DaCy and comparison with similar Danish models | | ð **
 [Demo]** | A simple Streamlit demo to try out the augmenters. | | ð° **[News
 and changelog]** | New additions, changes and version history. | | ð **[API
 References]** | The detailed reference for DaCy's API. Including function
 documentation | | ð **[FAQ]** | Frequently asked questions | [Installation]:
 https://centre-for-humanities-computing.github.io/DaCy/installation.html
 [Getting started]: https://centre-for-humanities-computing.github.io/DaCy/
 using_dacy.html [api references]: https://centre-for-humanities-
@@ -56,27 +51,25 @@
 faq.html [Performance]: https://centre-for-humanities-computing.github.io/DaCy/
 performance.html
   Training and reproduction  the folder `training` contains a SpaCy project
 which will allow for reproduction of the results. This folder also includes the
 evaluation metrics on DaNE and scripts for downloading the required data. For
 more information, please see the training [readme](training/readme.md). Want to
 learn more about how DaCy initially came to be, check out this [blog post]
-(https://www.kennethenevoldsen.com/post/new-fast-and-efficient-state-of-the-
-art-in-danish-nlp/).
-## ð¬ Where to ask questions To ask report issues or request features, please
+(https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-
+state-of-the-art-in-danish-nlp/).
+# ð¬ Where to ask questions To ask report issues or request features, please
 use the [GitHub Issue Tracker](https://github.com/centre-for-humanities-
 computing/DaCy/issues). Questions related to SpaCy are kindly referred to the
 SpaCy GitHub or forum. Otherwise, please use the discussion Forums. | Type | |
-| ------------------------------ | ---------------------- | | ð¨ **Bug
-Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas** |
-[GitHub Issue Tracker] | | ð©âð» **Usage Questions** | [GitHub
-Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] | [github
-issue tracker]: https://github.com/centre-for-humanities-computing/DaCy/issues
-[github discussions]: https://github.com/centre-for-humanities-computing/DaCy/
-discussions ## Acknowledgements DaCy is a result of great open-source software
-and contributors. It wouldn't have been possible without the work by the SpaCy
-team which developed and integrated the software. Huggingface for developing
-Transformers and making model sharing convenient. Multiple parties including
-Certainly.io and [Malte Hojmark-Bertelsen](https://github.com/MalteHB) for
-making their models publicly available. Alexandra Institute for developing and
-maintaining DaNLP which has made it easy to get access to Danish resources and
-even supplied some of the tagged data themselves.
+| ------------------------------ | ---------------------- | | ð **FAQ** |
+[FAQ] | | ð¨ **Bug Reports** | [GitHub Issue Tracker] | | ð **Feature
+Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð» **Usage Questions**
+| [GitHub Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] |
+[Documentation]: https://centre-for-humanities-computing.github.io/dacy/
+index.html [Installation]: https://centre-for-humanities-computing.github.io/
+dacy/installation.html [Tutorials]: https://centre-for-humanities-
+computing.github.io/dacy/tutorials.html [API Reference]: https://centre-for-
+humanities-computing.github.io/dacy/references.html [FAQ]: https://centre-for-
+humanities-computing.github.io/dacy/faq.html [github issue tracker]: https://
+github.com/centre-for-humanities-computing/dacy/issues [github discussions]:
+https://github.com/centre-for-humanities-computing/dacy/discussions
```

### Comparing `dacy-2.4.2/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png` & `dacy-2.5.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/asent_analysis.png` & `dacy-2.5.0/docs/_static/asent_analysis.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/asent_prediction.png` & `dacy-2.5.0/docs/_static/asent_prediction.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/dep_parse.png` & `dacy-2.5.0/docs/_static/dep_parse.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/dep_robustness.png` & `dacy-2.5.0/docs/_static/dep_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/favicon.ico` & `dacy-2.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/icon.png` & `dacy-2.5.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/icon_black_text.png` & `dacy-2.5.0/docs/_static/icon_black_text.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/icon_dark.png` & `dacy-2.5.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/icon_no_title.png` & `dacy-2.5.0/docs/_static/icon_no_title.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/ner.png` & `dacy-2.5.0/docs/_static/ner.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/ner_robustness.png` & `dacy-2.5.0/docs/_static/ner_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/perf.png` & `dacy-2.5.0/docs/_static/perf.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/perf_l.png` & `dacy-2.5.0/docs/_static/perf_l.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/pos_robustness.png` & `dacy-2.5.0/docs/_static/pos_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/table_dep.html` & `dacy-2.5.0/docs/_static/table_dep.html`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/table_ent.html` & `dacy-2.5.0/docs/_static/table_ent.html`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/table_perf.html` & `dacy-2.5.0/docs/_static/table_perf.html`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/_static/table_pos.html` & `dacy-2.5.0/docs/_static/table_pos.html`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/conf.py` & `dacy-2.5.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,96 @@
 # Configuration file for the Sphinx documentation builder.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
+from datetime import datetime
 
 from dacy.about import __version__
 
 # -- Project information -----------------------------------------------------
 
-project = "DaCy"
+project = """DaCy"""
+
 author = "Kenneth Enevoldsen"
-repo_url = "https://github.com/centre-for-humanities-computing/DaCy"
 github_user = "centre-for-humanities-computing"
+repo_url = f"https://github.com/{github_user}/{project.lower()}"
 
-# The full version, including alpha/beta/rc tags
+copyright = f"{datetime.now().year}, {author}"  # noqa: A001
 release = __version__
 
-
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "sphinx.ext.napoleon",
-    "sphinx.ext.viewcode",
     "sphinxext.opengraph",
     "sphinx_copybutton",
     "sphinx.ext.githubpages",
+    "sphinx.ext.napoleon",
+    "myst_nb",
     "sphinx_design",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
 ]
 
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
+# Do not execute the notebooks when building the docs (turned off by default)
+# nbsphinx_execute = "never" # noqa ERA001
+
+
+# Automatically extract typehints when specified and place them in
+# descriptions of the relevant function/method.
+# https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#configuration
+autodoc_typehints = "description"
+
+# Don't show class signature with the class' name.
+autodoc_class_signature = "separated"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-#
-html_theme = "furo"  # "press", "sphinx_rtd_theme", "furo"
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
+html_title = "DaCy"
+html_theme = "furo"
 html_static_path = ["_static"]
 html_favicon = "_static/favicon.ico"
 
+html_show_sourcelink = True
 
 html_context = {
-    "display_github": True,
+    "display_github": True,  # Add 'Edit on Github' link instead of 'View page source'
     "github_user": github_user,
     "github_repo": project.lower(),
     "github_version": "main",
     "conf_py_path": "/docs/",
-    "slug": project.lower(),
     "current_version": "latest",
 }
 
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".md": "myst-nb",
+    ".ipynb": "myst-nb",
+}
+
 
 html_theme_options = {
+    # adds github footer icon with link to repo
     "footer_icons": [
         {
             "name": "GitHub",
             "url": repo_url,
             "html": """
                 <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 16 16">
                     <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
                 </svg>
-            """,  # noqa: E501
+            """,
             "class": "",
         },
     ],
     "source_repository": repo_url,
     "source_branch": "main",
     "source_directory": "docs/",
     "light_logo": "icon.png",
@@ -94,10 +99,13 @@
         "color-brand-primary": "#ff5454",
         "color-brand-content": "#ff7575",
     },
     "dark_css_variables": {
         "color-brand-primary": "#ff8f8f",
         "color-brand-content": "#ff8f8f",
     },
-    "sidebar_hide_name": True,
+    "sidebar_hide_name": False,
     "navigation_with_keys": True,
 }
+
+pygments_style = "monokai"
+pygments_dark_style = "monokai"
```

### Comparing `dacy-2.4.2/docs/news.rst` & `dacy-2.5.0/docs/news.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/performance.general.rst` & `dacy-2.5.0/docs/performance.general.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/docs/performance.robustness.rst` & `dacy-2.5.0/docs/performance.robustness.rst`

 * *Files 0% similar despite different names*

```diff
@@ -131,9 +131,9 @@
 
 
 
 .. seealso:: 
 
    Want to do the analysis yourself? Well DaCy includes functions for evaluating the
    robustness of its own and others pipelines as well as a
-   `guide <https://colab.research.google.com/github/centre-for-humanities-computing/DaCy/blob/main/tutorials/dacy-robustness.ipynb>`__
+   `guide <https://colab.research.google.com/github/centre-for-humanities-computing/DaCy/blob/main/docs/tutorials/robustness.ipynb>`__
    on how to use these.
```

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd` & `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/src/dacy/datasets/dane.py` & `dacy-2.5.0/src/dacy/datasets/dane.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """This includes the DaNE dataset wrapped and read in as a SpaCy corpus."""
 
-import os
 import shutil
+import subprocess
+import sys
+from os import PathLike
 from pathlib import Path
 from typing import List, Optional, Union
 
 from spacy.training import Corpus
 
 from ..download import DEFAULT_CACHE_DIR, download_url
 from .constants import DATASETS
 
 
-def dane(
-    save_path: Optional[str] = None,
-    splits: List[str] = ["train", "dev", "test"],
+def dane(  # noqa
+    save_path: Optional[PathLike] = None,
+    splits: List[str] = ["train", "dev", "test"],  # noqa
     redownload: bool = False,
     n_sents: int = 1,
     open_unverified_connection: bool = False,
-    **kwargs,
+    **kwargs,  # noqa
 ) -> Union[List[Corpus], Corpus]:
     """Reads the DaNE dataset as a spacy Corpus.
 
     Args:
         save_path (str, optional): Path to the DaNE dataset If it does not contain the
             dataset it is downloaded to the folder. Defaults to None corresponding to
             dacy.where_is_my_dacy() in the datasets subfolder.
@@ -46,60 +48,67 @@
     """
     if open_unverified_connection:
         import ssl
 
         ssl._create_default_https_context = ssl._create_unverified_context
 
     if save_path is None:
-        save_path_ = os.path.join(DEFAULT_CACHE_DIR, "datasets")
+        save_path_ = Path(DEFAULT_CACHE_DIR) / "datasets"
     else:
-        save_path_ = save_path
-    save_path = os.path.join(save_path_, "dane")
+        save_path_ = Path(save_path)
+    save_path = save_path_ / "dane"
 
-    if (
-        (not os.path.isdir(save_path))
-        or ("dane" not in os.listdir(save_path_))
-        or (redownload is True)
-    ):
-        Path(save_path).mkdir(parents=True, exist_ok=True)
-
-        dl_path = os.path.join(save_path, "dane.zip")
-        download_url(DATASETS["dane"], dl_path)
+    if redownload is True or (not save_path.exists()):
+        save_path.mkdir(parents=True, exist_ok=True)
+        dl_path = save_path / "dane.zip"
+        download_url(DATASETS["dane"], str(dl_path))
         shutil.unpack_archive(dl_path, save_path)
-        os.remove(dl_path)
+        dl_path.unlink()
 
     wpaths = [
         "dane_train.conllu",
         "dane_dev.conllu",
         "dane_test.conllu",
         "dane.conllu",
     ]
 
-    for wpath in wpaths:
-        wpath = os.path.join(save_path, wpath)
-        cpath = wpath[:-7] + f"_{n_sents}"
-        if os.path.isfile(cpath + ".spacy"):
+    for _wpath in wpaths:
+        wpath = save_path / _wpath
+        cpath = save_path / (wpath.stem + f"_{n_sents}")
+
+        if cpath.with_suffix(".spacy").is_file():
             continue
-        cpath += ".conllu"
+        cpath = cpath.with_suffix(".conllu")
         shutil.copyfile(wpath, cpath)
         # convert to spacy
-        os.system(
-            f"python -m spacy convert {cpath} {save_path} --converter conllu "
-            + f"--merge-subtokens -n {n_sents}",
+        subprocess.run(
+            [
+                sys.executable,
+                "-m",
+                "spacy",
+                "convert",
+                cpath,
+                save_path,  # type: ignore
+                "--converter",
+                "conllu",
+                "--merge-subtokens",
+                "-n",
+                str(n_sents),
+            ],
+            check=True,
         )
-        os.remove(cpath)
-
-    if isinstance(splits, str):
-        splits = [splits]
+        cpath.unlink()
+    if isinstance(splits, str):  # type: ignore
+        splits = [splits]  # type: ignore
     corpora = []
     paths = {
         "all": f"dane_{n_sents}.spacy",
         "test": f"dane_test_{n_sents}.spacy",
         "dev": f"dane_dev_{n_sents}.spacy",
         "train": f"dane_train_{n_sents}.spacy",
     }
 
     for split in splits:
-        corpora.append(Corpus(os.path.join(save_path, paths[split])))
+        corpora.append(Corpus(save_path / paths[split]))  # type: ignore
     if len(corpora) == 1:
         return corpora[0]
     return corpora
```

### Comparing `dacy-2.4.2/src/dacy/datasets/lookup_tables/README.md` & `dacy-2.5.0/src/dacy/datasets/lookup_tables/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/src/dacy/datasets/lookup_tables/names.csv` & `dacy-2.5.0/src/dacy/datasets/lookup_tables/names.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/src/dacy/datasets/names.py` & `dacy-2.5.0/src/dacy/datasets/names.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
             proportion of people with the given name of that gender. Only used when
             gender is set. Defaults to 0.
 
     Returns:
         Dict[str, List[str]]: A dictionary of Muslim names containing the keys
             "first_name" and "last_name".
     """
-    path = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)),
+    path = os.path.join(  # noqa
+        os.path.dirname(os.path.abspath(__file__)),  # noqa
         "lookup_tables",
         "names.csv",
     )
     names = pd.read_csv(path)
 
     if min_count:
         names = names.loc[names["count"] >= min_count]
```

### Comparing `dacy-2.4.2/src/dacy/hate_speech/wrapped_models.py` & `dacy-2.5.0/src/dacy/hate_speech/wrapped_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         assign_to_cats=True,
     )
 
     # overwrite extension such that it return not offensive if the document is not
     # offensive
     if Doc.has_extension("is_offensive"):
 
-        def label_getter(doc) -> Optional[str]:
+        def label_getter(doc) -> Optional[str]:  # noqa
             if doc._.is_offensive == "offensive":
                 prob = getattr(doc._, f"{doc_extension_prediction}_prob")
                 if prob["prob"] is not None:
                     return labels[int(prob["prob"].argmax())]
             return doc._.is_offensive
 
         Doc.set_extension(doc_extension_prediction, getter=label_getter, force=True)
```

### Comparing `dacy-2.4.2/src/dacy/load.py` & `dacy-2.5.0/src/dacy/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 """Functionality for loading and locating DaCy models."""
-from typing import Optional
+from pathlib import Path
+from typing import Any, Union
 
+import spacy
 from spacy.language import Language
 from wasabi import msg
 
 from .download import DEFAULT_CACHE_DIR, download_model, models_url
 
 
 def load(
     model: str,
-    path: Optional[str] = None,
-    force_download: bool = False,
-    **kwargs,
+    force: bool = False,
+    **kwargs: Any,
 ) -> Language:
     """Load a DaCy model as a SpaCy text processing pipeline. If the model is
     not downloaded it will also download the model.
 
     Args:
-        model (str): the model you wish to load. To see available model see
+        model: the model you wish to load. To see available model see
             dacy.models()
-        path (str, optional): The path to the downloaded model. Defaults to None which
-            corresponds to the path optained using dacy.where_is_my_dacy().
-        force_redownload (bool, optional): Should the model be redownloaded even if
+        force: Should the model be redownloaded even if
             already downloaded? Default to False.
         kwargs: additional arguments passed to spacy.load()
 
     Returns:
-        Language: a SpaCy text-preprocessing pipeline
+        A SpaCy text-preprocessing pipeline
 
     Example:
         >>> import dacy
         >>> dacy.load("da_dacy_medium_trf-0.1.0")
         >>> # or equivalently
         >>> dacy.load("medium")
     """
-    import spacy
 
-    if path is None:
-        path = DEFAULT_CACHE_DIR
-
-    path = download_model(model, path, force=force_download)
+    path = download_model(model, force=force)
     return spacy.load(path, **kwargs)
 
 
-def where_is_my_dacy(verbose: bool = True) -> str:
+def where_is_my_dacy(verbose: bool = True) -> Union[str, Path]:
     """Returns a path to where DaCy models are located. The default the model
     location can be configured with the environmental variable
     `DACY_CACHE_DIR`.
 
     Args:
         verbose (bool, optional): Toggles the verbosity of the function. Defaults to
             True.
```

### Comparing `dacy-2.4.2/src/dacy/ner/wrapped_models.py` & `dacy-2.5.0/src/dacy/ner/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/src/dacy/score/input_length.py` & `dacy-2.5.0/src/dacy/score/input_length.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 def n_sents_score(
     n_sents: Union[int, List[int]],
     apply_fn: Callable,
     dataset: str = "dane",
     split: str = "test",
-    score_fn: List[Union[str, Callable]] = ["token", "pos", "ents", "dep"],
+    score_fn: List[Union[str, Callable]] = ["token", "pos", "ents", "dep"],  # noqa
     verbose: bool = True,
-    **kwargs,
+    **kwargs,  # noqa
 ) -> pd.DataFrame:
     """scores the performance of a given model on examples of a given number of
     sentences.
 
     Args:
         n_sents (Union[int, List[int]]): Number of sentences which the performance
             should be applied to.
@@ -48,11 +48,11 @@
     dataset_fn = {"dane": dane}
     if isinstance(n_sents, int):
         n_sents = [n_sents]
 
     for i, n in enumerate(n_sents):
         if verbose is True:
             msg.info(f"Calculating score using {n} sentences")
-        corpus = dataset_fn[dataset](splits=split, n_sents=n, **kwargs)
-        scores_ = score(corpus, apply_fn=apply_fn, score_fn=score_fn, **kwargs)
-        scores = pd.concat([scores, scores_]) if i != 0 else scores_  # noqa
+        corpus = dataset_fn[dataset](splits=split, n_sents=n, **kwargs)  # type: ignore
+        scores_ = score(corpus, apply_fn=apply_fn, score_fn=score_fn, **kwargs)  # type: ignore
+        scores = pd.concat([scores, scores_]) if i != 0 else scores_  # type: ignore # noqa
     return scores
```

### Comparing `dacy-2.4.2/src/dacy/score/score.py` & `dacy-2.5.0/src/dacy/score/score.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,33 +28,33 @@
     spans = getattr(doc, attr)
     for span in spans:
         if span.label_ == "MISC":
             continue
         yield span
 
 
-def dep_getter(token, attr):
+def dep_getter(token, attr):  # noqa
     dep = getattr(token, attr)
     dep = token.vocab.strings.as_string(dep).lower()
     return dep
 
 
 def score(  # noqa
     corpus: Corpus,
-    apply_fn: Callable[[Iterable[Example], list[Example]]] | Language,
-    score_fn: list[Callable[[Iterable[Example]], dict] | str] = [
+    apply_fn: Callable[[Iterable[Example], list[Example]]] | Language,  # type: ignore
+    score_fn: list[Callable[[Iterable[Example]], dict] | str] = [  # noqa
         "token",
         "pos",
         "ents",
         "dep",
     ],
-    augmenters: list[Callable[[Language, Example], Iterable[Example]]] = [],
+    augmenters: list[Callable[[Language, Example], Iterable[Example]]] = [],  # noqa
     k: int = 1,
     nlp: Language | None = None,
-    **kwargs,
+    **kwargs,  # noqa
 ) -> pd.DataFrame:
     """scores a models performance on a given corpus with potentially
     augmentations applied to it.
 
     Args:
         corpus (Corpus): A spacy Corpus
         apply_fn (Union[Callable, Language]): A wrapper function for the model you wish
@@ -91,15 +91,15 @@
         >>>                apply_fn = nlp)
     """
     if callable(augmenters):
         augmenters = [augmenters]
     if len(augmenters) == 0:
         augmenters = [dont_augment]
 
-    def __apply_nlp(examples):
+    def __apply_nlp(examples):  # noqa: ANN001
         examples = ((e.x.text, e.y) for e in examples)
         doc_tuples = nlp_.pipe(examples, as_tuples=True)
         return [Example(x, y) for x, y in doc_tuples]
 
     if isinstance(apply_fn, Language):
         nlp_ = apply_fn
         apply_fn = __apply_nlp
@@ -107,27 +107,27 @@
     if nlp is None:
         from spacy.lang.da import Danish
 
         nlp = Danish()
 
     scorer = Scorer(nlp)
 
-    def ents_scorer(examples):
+    def ents_scorer(examples):  # noqa: ANN001
         scores = Scorer.score_spans(examples, attr="ents")
         scores_no_misc = Scorer.score_spans(
             examples,
             attr="ents",
             getter=no_misc_getter,
         )
         scores["ents_excl_MISC"] = {
             k: scores_no_misc[k] for k in ["ents_p", "ents_r", "ents_f"]
         }
         return scores
 
-    def pos_scorer(examples):
+    def pos_scorer(examples):  # noqa: ANN001
         scores = Scorer.score_token_attr(examples, attr="pos")
         scores_ = Scorer.score_token_attr(examples, attr="tag")
         for k in scores_:
             scores[k] = scores_[k]
         return scores
 
     def_scorers = {
@@ -139,35 +139,35 @@
             Scorer.score_deps,
             attr="dep",
             getter=dep_getter,
             ignore_labels=("p", "punct"),
         ),
     }
 
-    def __score(augmenter):
+    def __score(augmenter):  # noqa: ANN001
         corpus_ = copy(corpus)
         corpus_.augmenter = augmenter
         scores_ls = []
-        for i in range(k):
+        for _i in range(k):
             s = time()
             examples = apply_fn(corpus_(nlp))
             speed = time() - s
             scores = {"wall_time": speed}
             for fn in score_fn:
                 if isinstance(fn, str):
-                    fn = def_scorers[fn]
+                    fn = def_scorers[fn]  # noqa
                 scores.update(fn(examples))
             scores = flatten_dict(scores)
             scores_ls.append(scores)
 
         # and collapse list to dict
-        for key in scores.keys():
+        for key in scores:
             scores[key] = [s[key] if key in s else None for s in scores_ls]
 
         scores["k"] = list(range(k))
 
         return pd.DataFrame(scores)
 
     for i, aug in enumerate(augmenters):
         scores_ = __score(aug)
-        scores = pd.concat([scores, scores_]) if i != 0 else scores_  # noqa
+        scores = pd.concat([scores, scores_]) if i != 0 else scores_  # type: ignore  # noqa
     return scores
```

### Comparing `dacy-2.4.2/src/dacy/sentiment/wrapped_models.py` & `dacy-2.5.0/src/dacy/sentiment/wrapped_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 mixed_precision = false
 grad_scaler_config = {}
 
 [emotion.model.get_spans]
 @span_getters = "spacy-transformers.strided_spans.v1"
 window = 128
 stride = 96
-"""  # noqa: E501
+"""
 
 DEFAULT_CONFIG = Config().from_str(DEFAULT_CONFIG_STR)
 
 
 Danish.factory(
     "dacy/subjectivity",
     default_config=DEFAULT_CONFIG["subjectivity"],
@@ -159,15 +159,15 @@
         assign_to_cats=True,
     )
 
     # overwrite extension such that it return no emotion if the document does not have
     # an emotion
     if Doc.has_extension("dacy/emotionally_laden"):
 
-        def label_getter(doc) -> Optional[str]:
+        def label_getter(doc) -> Optional[str]:  # noqa: ANN001
             if doc._.emotionally_laden == "emotional":
                 prob = getattr(doc._, f"{doc_extension_prediction}_prob")
                 if prob["prob"] is not None:
                     return labels[int(prob["prob"].argmax())]
             return doc._.emotionally_laden
 
         Doc.set_extension(doc_extension_prediction, getter=label_getter, force=True)
```

### Comparing `dacy-2.4.2/src/dacy/utils.py` & `dacy-2.5.0/src/dacy/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         dict: the flattened dict.
 
     Example:
         >>> flatten({'a': 1, 'c': {'a': 2, 'b': {'x': 5, 'y' : 10}}, 'd': [1, 2, 3]})
         {'a': 1, 'c_a': 2, 'c_b_x': 5, 'd': [1, 2, 3], 'c_b_y': 10}
     """
 
-    def __inner_flatten(d, parent_key, sep):
+    def __inner_flatten(d, parent_key, sep):  # noqa: ANN001
         items = []
         for k, v in d.items():
             new_key = parent_key + sep + k if parent_key else k
             if isinstance(v, MutableMapping):
                 items.extend(__inner_flatten(v, new_key, sep=sep).items())
             else:
                 items.append((new_key, v))
```

### Comparing `dacy-2.4.2/src/dacy.egg-info/PKG-INFO` & `dacy-2.5.0/src/dacy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.4.2
+Version: 2.5.0
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
-Author: Lasse Hansen
-Author-email: Kenneth Enevoldsen <kennethcenevolsen@gmail.com>
+Author: Lasse Hansen, Emil Jessen
+Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -216,57 +216,54 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: style
+Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
-Provides-Extra: tutorials
 License-File: LICENSE
 
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
-# DaCy: An efficient NLP Pipeline for Danish
+# DaCy: An efficient and unified framework for danish NLP
 
-[![PyPI version](https://badge.fury.io/py/dacy.svg)](https://pypi.org/project/dacy/)
+[![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
-[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/DaCy)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
-[![github actions pytest](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/tests.yml/badge.svg)](https://github.com/centre-for-humanities-computing/Dacy/actions)
-[![github actions docs](https://github.com/centre-for-humanities-computing/DaCy/actions/workflows/documentation.yml/badge.svg)](https://centre-for-humanities-computing.github.io/DaCy/)
-<!-- 
-![github coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/KennethEnevoldsen/af8637d94475ea8bcb6b6a03c4fbcd3e/raw/badge-dacy-pytest-coverage.json)
--->
+[![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
+
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
+[pypi status]: https://pypi.org/project/dacy/
+[documentation]: https://centre-for-humanities-computing.github.io/dacy/
+[tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
+[black]: https://github.com/psf/black
 
 
+<!-- start short-description -->
 DaCy is a Danish natural language preprocessing framework made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance on Named entity recognition, part-of-speech tagging and dependency parsing for Danish. Feel free to try out the [demo](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.). This repository contains material for using DaCy, reproducing the results and guides on usage of the package. Furthermore, it also contains behavioural tests for biases and robustness of Danish NLP pipelines.
+<!-- end short-description -->
 
-<!--
-EASTER EGG:
-https://www.youtube.com/watch?v=E7WQ1tdxSqI
--->
+## 🔧 Installation
 
+You can install `dacy` via [pip] from [PyPI]:
 
-# 🔧 Installation
-To get started using DaCy simply install it using pip by running the following line in your terminal:
 ```bash
 pip install dacy
 ```
 
-
-# 👩‍💻 Usage
+## 👩‍💻 Usage
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
@@ -288,21 +285,17 @@
 To download the model to a specific directory:
 ```python
 dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
 nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
 ```
 
 
-# 📖 Documentation
-
-DaCy includes detailed documentation as well as a series of Jupyter notebook tutorials.
-If you do not have Jupyter Notebook installed, instructions for installing and running
-it can be found [here]( http://jupyter.org/install). All the tutorials are located in
-the `tutorials` folder.
+To see more examples, see the [documentation].
 
+# 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
 | 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
@@ -325,35 +318,33 @@
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
 the folder `training` contains a SpaCy project which will allow for reproduction of the results. This folder also includes the evaluation metrics on DaNE and scripts for downloading the required data. For more information, please see the training [readme](training/readme.md).
 
-Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.kennethenevoldsen.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
+Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
 
-## 💬 Where to ask questions
+# 💬 Where to ask questions
 To ask report issues or request features, please use the [GitHub Issue Tracker](https://github.com/centre-for-humanities-computing/DaCy/issues).
 Questions related to SpaCy are kindly referred to the SpaCy GitHub or forum. Otherwise, please use the discussion Forums.
 
 | Type                           |                        |
 | ------------------------------ | ---------------------- |
+| 📚 **FAQ**                      | [FAQ]                  |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker] |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker] |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]   |
 | 🗯 **General Discussion**       | [GitHub Discussions]   |
 
-[github issue tracker]: https://github.com/centre-for-humanities-computing/DaCy/issues
-[github discussions]: https://github.com/centre-for-humanities-computing/DaCy/discussions
-
-
-
-
-
-
-## Acknowledgements
-DaCy is a result of great open-source software and contributors. It wouldn't have been possible without the work by the SpaCy team which developed and integrated the software. Huggingface for developing Transformers and making model sharing convenient. Multiple parties including Certainly.io and [Malte Hojmark-Bertelsen](https://github.com/MalteHB) for making their models publicly available. Alexandra Institute for developing and maintaining DaNLP which has made it easy to get access to Danish resources and even supplied some of the tagged data themselves.
+[Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
+[Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
+[Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
+[API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
+[FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
+[github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
+[github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
```

### Comparing `dacy-2.4.2/src/dacy.egg-info/SOURCES.txt` & `dacy-2.5.0/src/dacy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,44 @@
+.cookiecutter.json
+.cruft.json
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 citation.cff
 pyproject.toml
+tasks.py
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/01_bugs.md
 .github/ISSUE_TEMPLATE/02_docs.md
 .github/ISSUE_TEMPLATE/03_feature-request.md
 .github/ISSUE_TEMPLATE/config.yml
+.github/workflows/check_for_rej.yml
+.github/workflows/cruft.yml
 .github/workflows/dependabot_automerge.yml
 .github/workflows/documentation.yml
+.github/workflows/mypy.yml
+.github/workflows/pre-commit.yml
 .github/workflows/release.yml
-.github/workflows/stale.yml
+.github/workflows/stalebot.yml
 .github/workflows/tests.yml
-dev/__init__.py
-dev/model_comparison/model_comparison.Rmd
-dev/model_comparison/model_comparison.Rproj
-dev/model_comparison/utility.R
-dev/new_projects/token_aug/ddo-synonyms.csv
-dev/new_projects/token_aug/ddo_misspellings_2020-08-26.csv
-dev/utilities/__init__.py
-dev/utilities/twitter.py
-docs/Makefile
+docs/adv_tutorials.md
 docs/conf.py
-docs/dacy.datasets.rst
-docs/dacy.download.rst
-docs/dacy.score.rst
-docs/faq.rst
-docs/index.rst
-docs/installation.rst
-docs/make.bat
+docs/faq.md
+docs/index.md
+docs/installation.md
 docs/news.rst
 docs/performance.general.rst
 docs/performance.robustness.rst
 docs/performance.rst
-docs/using_dacy.augmentation.rst
-docs/using_dacy.getting_started.rst
-docs/using_dacy.hate_speech.rst
-docs/using_dacy.rst
-docs/using_dacy.sentiment.rst
+docs/requirements.txt
+docs/tutorials.md
 docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
 docs/_static/asent_analysis.png
 docs/_static/asent_prediction.png
 docs/_static/dep_parse.png
 docs/_static/dep_robustness.png
 docs/_static/favicon.ico
 docs/_static/icon.png
@@ -56,14 +50,22 @@
 docs/_static/perf.png
 docs/_static/perf_l.png
 docs/_static/pos_robustness.png
 docs/_static/table_dep.html
 docs/_static/table_ent.html
 docs/_static/table_perf.html
 docs/_static/table_pos.html
+docs/api/dacy.datasets.rst
+docs/api/dacy.download.rst
+docs/api/dacy.score.rst
+docs/tutorials/basic.ipynb
+docs/tutorials/hate-speech.ipynb
+docs/tutorials/robustness.ipynb
+docs/tutorials/sentiment.ipynb
+docs/tutorials/textdescriptives.ipynb
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
 papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
```

### Comparing `dacy-2.4.2/src/dacy.egg-info/requires.txt` & `dacy-2.5.0/src/dacy.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 spacy-wrap<1.5.0,>=1.4.1
 spacy<3.6.0,>=3.2.0
 pandas<2.0.0,>=1.0.0
 wasabi<0.11.0,>=0.8.2
 tqdm<4.65.0,>=4.42.1
 sentencepiece<0.2.0,>=0.1.96
 
-[docs]
-Sphinx<5.1.0,>=4.5.0
-furo<2022.6.30,>=2022.6.21
-sphinxext-opengraph<0.7.0,>=0.6.3
-sphinx-copybutton<0.6.0,>=0.5.0
-myst-parser<0.19.0,>=0.18.0
-ipykernel<6.16.0,>=6.15.0
-sphinx_design<0.3.0,>=0.2.0
-
-[style]
-black<22.4.0,>=22.3.0
-ruff<0.0.195,>=0.0.194
-pre-commit<2.20.0,>=2.19.0
-
-[tests]
-pytest<7.2.0,>=7.1.2
-pytest-cov<3.0.1,>=3.0.0
+[dev]
+cruft
+mypy
+pre-commit<2.21.0,==2.20.0
+ruff==0.0.254
+black[jupyter]==22.8.0
 
-[tutorials]
-jupyter
+[docs]
+sphinx<5.4.0,>=5.3.0
+furo<2022.12.8,>=2022.12.7
+sphinx-copybutton<0.5.2,>=0.5.1
+sphinxext-opengraph<0.7.4,>=0.7.3
+sphinx_design<0.3.1,>=0.3.0
+sphinx_togglebutton<0.4.0,>=0.2.3
+myst-nb<1.17.0,>=0.6.0
+jupyter<1.1.0,>=1.0.0
 asent<0.8.0,>=0.4.2
 augmenty<1.4.0,>=1.0.2
 textdescriptives<3.0.0,>=2.1.0
 seaborn<0.13.0,>=0.11.2
+
+[tests]
+pytest<7.3.0,>=7.1.2
+pytest-cov<3.1.0,>=3.0.0
+pytest-xdist<3.2.0,>=3.0.0
+pytest-instafail<0.5.0,>=0.4.2
```

### Comparing `dacy-2.4.2/tests/test_datasets.py` & `dacy-2.5.0/tests/test_datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from spacy.lang.da import Danish
-from spacy.training import Corpus, Example
-
 import dacy
 from dacy.datasets import dane, female_names, male_names, muslim_names
-
-test = dane(splits=["test"])
+from spacy.lang.da import Danish
+from spacy.training import Corpus, Example
 
 
 def test_dane():
     train, dev, test = dane(open_unverified_connection=True)
     all_ = dacy.datasets.dane(splits=["all"])
     for d in [train, dev, test, all_]:
         assert isinstance(d, Corpus)
```

### Comparing `dacy-2.4.2/tests/test_hate_speech.py` & `dacy-2.5.0/tests/test_hate_speech.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import spacy
-
 import dacy  # noqa
+import spacy
 
 
 def test_add_hate_speech_detection():
     nlp = spacy.blank("da")
     nlp.add_pipe("dacy/hatespeech_detection")
     texts = ["senile gamle idiot", "hej har du haft en god dag"]
     actual = ["offensive", "not offensive"]
```

### Comparing `dacy-2.4.2/tests/test_score.py` & `dacy-2.5.0/tests/test_score.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import pandas as pd
-from spacy.lang.da import Danish
-from spacy.training.augment import create_lower_casing_augmenter
-
 from dacy.datasets import dane
 from dacy.score import n_sents_score, score
+from spacy.lang.da import Danish
+from spacy.training.augment import create_lower_casing_augmenter
 
 
 def test_score():
     nlp = Danish()
 
-    def apply_model(examples):
+    def apply_model(examples):  # noqa: ANN001
         e = []
         for example in examples:
             example.predicted = nlp(example.predicted.text)
             e.append(example)
         return e
 
     test = dane(splits=["test"])
@@ -39,15 +38,15 @@
     for s in scores_:
         assert s in scores.columns
 
 
 def test_n_sents_score():
     nlp = Danish()
 
-    def apply_model(examples):
+    def apply_model(examples):  # noqa: ANN001
         e = []
         for example in examples:
             example.predicted = nlp(example.predicted.text)
             e.append(example)
         return e
 
     scores = n_sents_score(
```

### Comparing `dacy-2.4.2/tests/test_sentiment.py` & `dacy-2.5.0/tests/test_sentiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import spacy
-
 import dacy  # noqa
+import spacy
 
 
 def test_add_subjectivity():
     nlp = spacy.blank("da")
     nlp.add_pipe("dacy/subjectivity")
     texts = [
         "Analysen viser, at økonomien bliver forfærdelig dårlig",
```

### Comparing `dacy-2.4.2/training/readme.md` & `dacy-2.5.0/training/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/configs/config_-l-ctra_small.cfg` & `dacy-2.5.0/training/v0.0.0/configs/config_-l-ctra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/configs/config_conv_small.cfg` & `dacy-2.5.0/training/v0.0.0/configs/config_conv_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/configs/config_electra_small.cfg` & `dacy-2.5.0/training/v0.0.0/configs/config_electra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/configs/config_large.cfg` & `dacy-2.5.0/training/v0.0.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/configs/config_medium.cfg` & `dacy-2.5.0/training/v0.0.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/img/perf_training.png` & `dacy-2.5.0/training/v0.0.0/img/perf_training.png`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_-l-ctra_cased.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_cased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_-l-ctra_uncased.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_uncased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_conv_small.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_conv_small.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_electra.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_electra.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_large.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_large.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/metrics/dane_medium.json` & `dacy-2.5.0/training/v0.0.0/metrics/dane_medium.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/orth_variants.json` & `dacy-2.5.0/training/v0.0.0/orth_variants.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.0.0/project.yml` & `dacy-2.5.0/training/v0.0.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/augment.py` & `dacy-2.5.0/training/v0.1.0/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/configs/config_large.cfg` & `dacy-2.5.0/training/v0.1.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/configs/config_medium.cfg` & `dacy-2.5.0/training/v0.1.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/configs/config_small.cfg` & `dacy-2.5.0/training/v0.1.0/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/project.yml` & `dacy-2.5.0/training/v0.1.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.0/update_meta_json.py` & `dacy-2.5.0/training/v0.1.0/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/augment.py` & `dacy-2.5.0/training/v0.1.1/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/configs/config_large.cfg` & `dacy-2.5.0/training/v0.1.1/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/configs/config_medium.cfg` & `dacy-2.5.0/training/v0.1.1/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/configs/config_small.cfg` & `dacy-2.5.0/training/v0.1.1/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/danish_augmenter.py` & `dacy-2.5.0/training/v0.1.1/danish_augmenter.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/project.yml` & `dacy-2.5.0/training/v0.1.1/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/training/v0.1.1/update_meta_json.py` & `dacy-2.5.0/training/v0.1.1/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/dacy-basic.ipynb` & `dacy-2.5.0/tutorials/dacy-basic.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/dacy-robustness.ipynb` & `dacy-2.5.0/tutorials/dacy-robustness.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/hate-speech.ipynb` & `dacy-2.5.0/tutorials/hate-speech.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/sentiment-neural.ipynb` & `dacy-2.5.0/tutorials/sentiment-neural.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/sentiment-rule-based.ipynb` & `dacy-2.5.0/tutorials/sentiment-rule-based.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.4.2/tutorials/textdescriptives_integration.ipynb` & `dacy-2.5.0/tutorials/textdescriptives_integration.ipynb`

 * *Files identical despite different names*

