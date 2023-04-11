# Comparing `tmp/dacy-2.5.0.tar.gz` & `tmp/dacy-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacy-2.5.0.tar", last modified: Tue Apr 11 00:07:56 2023, max compression
+gzip compressed data, was "dacy-2.5.1.tar", last modified: Tue Apr 11 00:26:24 2023, max compression
```

## Comparing `dacy-2.5.0.tar` & `dacy-2.5.1.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/
--rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 00:07:43.000000 dacy-2.5.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 00:07:43.000000 dacy-2.5.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.991460 dacy-2.5.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/mypy.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 00:07:43.000000 dacy-2.5.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 00:07:43.000000 dacy-2.5.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 00:07:43.000000 dacy-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     7737 2023-04-11 00:07:44.000000 dacy-2.5.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 00:07:43.000000 dacy-2.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 00:07:43.000000 dacy-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 00:07:43.000000 dacy-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:07:56.051463 dacy-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6594 2023-04-11 00:07:43.000000 dacy-2.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 00:07:43.000000 dacy-2.5.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.995460 dacy-2.5.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.011461 dacy-2.5.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
--rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/asent_analysis.png
--rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/asent_prediction.png
--rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/dep_parse.png
--rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/dep_robustness.png
--rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_black_text.png
--rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/icon_no_title.png
--rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/ner.png
--rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/ner_robustness.png
--rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/perf.png
--rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/perf_l.png
--rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/pos_robustness.png
--rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_dep.html
--rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_ent.html
--rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_perf.html
--rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/_static/table_pos.html
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/adv_tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.011461 dacy-2.5.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.datasets.rst
--rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.download.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/api/dacy.score.rst
--rw-r--r--   0 root         (0) root         (0)     3830 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/faq.md
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)     4714 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.general.rst
--rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.robustness.rst
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/performance.rst
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.015461 dacy-2.5.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    26285 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/basic.ipynb
--rw-r--r--   0 root         (0) root         (0)     5953 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)    38230 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)    21177 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/sentiment.ipynb
--rw-r--r--   0 root         (0) root         (0)   106814 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials/textdescriptives.ipynb
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 00:07:43.000000 dacy-2.5.0/docs/tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.983460 dacy-2.5.0/papers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.019461 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.023461 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
--rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
--rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
--rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 00:07:43.000000 dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
--rw-r--r--   0 root         (0) root         (0)     4703 2023-04-11 00:07:44.000000 dacy-2.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 00:07:56.051463 dacy-2.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:55.983460 dacy-2.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.023461 dacy-2.5.0/src/dacy/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy/datasets/
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/constants.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/dane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy/datasets/lookup_tables/
--rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/lookup_tables/names.csv
--rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/datasets/names.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/hate_speech/
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/hate_speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/hate_speech/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/ner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/ner/wrapped_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/score/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/input_length.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/score/score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.031462 dacy-2.5.0/src/dacy/sentiment/
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/sentiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/sentiment/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 00:07:43.000000 dacy-2.5.0/src/dacy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.027462 dacy-2.5.0/src/dacy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6144 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      660 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 00:07:55.000000 dacy-2.5.0/src/dacy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 00:07:43.000000 dacy-2.5.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_datasets.py
--rw-r--r--   0 root         (0) root         (0)      342 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_hate_speech.py
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_ner.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_score.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_sentiment.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 00:07:43.000000 dacy-2.5.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/
--rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 00:07:43.000000 dacy-2.5.0/training/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_-l-ctra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_conv_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_electra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/configs/config_medium.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.035462 dacy-2.5.0/training/v0.0.0/img/
--rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/img/perf_training.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.0.0/metrics/
--rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_cased.json
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_conv_small.json
--rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_electra.json
--rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_large.json
--rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/metrics/dane_medium.json
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/orth_variants.json
--rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/project.yml
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.0.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.039462 dacy-2.5.0/training/v0.1.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/configs/config_small.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.043462 dacy-2.5.0/training/v0.1.0/metrics/
--rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.047463 dacy-2.5.0/training/v0.1.1/
--rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.047463 dacy-2.5.0/training/v0.1.1/configs/
--rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/configs/config_small.cfg
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/danish_augmenter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/training/v0.1.1/metrics/
--rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:07:43.000000 dacy-2.5.0/training/v0.1.1/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:07:56.051463 dacy-2.5.0/tutorials/
--rw-r--r--   0 root         (0) root         (0)    16340 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/dacy-basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    38219 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/dacy-robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)     5333 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     9763 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/sentiment-neural.ipynb
--rw-r--r--   0 root         (0) root         (0)     8741 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/sentiment-rule-based.ipynb
--rw-r--r--   0 root         (0) root         (0)   106539 2023-04-11 00:07:43.000000 dacy-2.5.0/tutorials/textdescriptives_integration.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.259168 dacy-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 00:26:13.000000 dacy-2.5.1/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 00:26:13.000000 dacy-2.5.1/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/mypy.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 00:26:13.000000 dacy-2.5.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 00:26:13.000000 dacy-2.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     8098 2023-04-11 00:26:14.000000 dacy-2.5.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 00:26:13.000000 dacy-2.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 00:26:13.000000 dacy-2.5.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 00:26:13.000000 dacy-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:26:24.255169 dacy-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6594 2023-04-11 00:26:13.000000 dacy-2.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 00:26:13.000000 dacy-2.5.1/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
+-rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/asent_analysis.png
+-rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/asent_prediction.png
+-rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/dep_parse.png
+-rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/dep_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_black_text.png
+-rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_no_title.png
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/ner.png
+-rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/ner_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/perf.png
+-rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/perf_l.png
+-rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/pos_robustness.png
+-rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_dep.html
+-rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_ent.html
+-rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_perf.html
+-rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_pos.html
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/adv_tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.download.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.score.rst
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/faq.md
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.general.rst
+-rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.robustness.rst
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.rst
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    26242 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38230 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)    21177 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/sentiment.ipynb
+-rw-r--r--   0 root         (0) root         (0)   106814 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/textdescriptives.ipynb
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.219169 dacy-2.5.1/papers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.239169 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.239169 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
+-rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-04-11 00:26:14.000000 dacy-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 00:26:24.259168 dacy-2.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.219169 dacy-2.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/datasets/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/dane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/datasets/lookup_tables/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/names.csv
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/names.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/hate_speech/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/hate_speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/hate_speech/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/ner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/ner/wrapped_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/score/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/input_length.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/sentiment/
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/sentiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/sentiment/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6144 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      660 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 00:26:13.000000 dacy-2.5.1/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_datasets.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_hate_speech.py
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_score.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/
+-rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 00:26:13.000000 dacy-2.5.1/training/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_-l-ctra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_conv_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_electra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_medium.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/img/
+-rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/img/perf_training.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_cased.json
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_conv_small.json
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_electra.json
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_large.json
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_medium.json
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/orth_variants.json
+-rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_small.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/training/v0.1.1/configs/
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/danish_augmenter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/training/v0.1.1/metrics/
+-rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    16340 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/dacy-basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38219 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/dacy-robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     9763 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/sentiment-neural.ipynb
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/sentiment-rule-based.ipynb
+-rw-r--r--   0 root         (0) root         (0)   106539 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/textdescriptives_integration.ipynb
```

### Comparing `dacy-2.5.0/.cruft.json` & `dacy-2.5.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/ISSUE_TEMPLATE/01_bugs.md` & `dacy-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/ISSUE_TEMPLATE/config.yml` & `dacy-2.5.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/dependabot.yml` & `dacy-2.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/check_for_rej.yml` & `dacy-2.5.1/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/cruft.yml` & `dacy-2.5.1/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/dependabot_automerge.yml` & `dacy-2.5.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/documentation.yml` & `dacy-2.5.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/mypy.yml` & `dacy-2.5.1/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/pre-commit.yml` & `dacy-2.5.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/release.yml` & `dacy-2.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/stalebot.yml` & `dacy-2.5.1/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.github/workflows/tests.yml` & `dacy-2.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.gitignore` & `dacy-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/.pre-commit-config.yaml` & `dacy-2.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/CHANGELOG.md` & `dacy-2.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.5.1 (2023-04-11)
+### Fix
+* Removed *-latest models ([`b2964e2`](https://github.com/centre-for-humanities-computing/DaCy/commit/b2964e28881e92edfebe1bdbbcf12dd09d9d043c))
+
+### Documentation
+* Updated docs to not include *-latest models ([`3b9c798`](https://github.com/centre-for-humanities-computing/DaCy/commit/3b9c798e794e0f42fa9990f8537c1f591c031553))
+
 ## v2.5.0 (2023-04-11)
 ### Feature
 * Moved dacy to use swift template ([`189c891`](https://github.com/centre-for-humanities-computing/DaCy/commit/189c891323f1ff083d1800fc3acd435c456fd1b5))
 
 ### Fix
 * Mypy ([`3b78e18`](https://github.com/centre-for-humanities-computing/DaCy/commit/3b78e18ef93a09fe2d152a5b9790c521ecffeb02))
 * Removed support for old version 0.0.0 versions ([`17649c3`](https://github.com/centre-for-humanities-computing/DaCy/commit/17649c31fb30cd083d1864b1e9b38389bb543cfd))
```

### Comparing `dacy-2.5.0/CODE_OF_CONDUCT.md` & `dacy-2.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/CONTRIBUTING.md` & `dacy-2.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/LICENSE` & `dacy-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/PKG-INFO` & `dacy-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.5.0
+Version: 2.5.1
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dacy-2.5.0/README.md` & `dacy-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/citation.cff` & `dacy-2.5.1/citation.cff`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png` & `dacy-2.5.1/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/asent_analysis.png` & `dacy-2.5.1/docs/_static/asent_analysis.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/asent_prediction.png` & `dacy-2.5.1/docs/_static/asent_prediction.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/dep_parse.png` & `dacy-2.5.1/docs/_static/dep_parse.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/dep_robustness.png` & `dacy-2.5.1/docs/_static/dep_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/favicon.ico` & `dacy-2.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/icon.png` & `dacy-2.5.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/icon_black_text.png` & `dacy-2.5.1/docs/_static/icon_black_text.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/icon_dark.png` & `dacy-2.5.1/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/icon_no_title.png` & `dacy-2.5.1/docs/_static/icon_no_title.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/ner.png` & `dacy-2.5.1/docs/_static/ner.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/ner_robustness.png` & `dacy-2.5.1/docs/_static/ner_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/perf.png` & `dacy-2.5.1/docs/_static/perf.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/perf_l.png` & `dacy-2.5.1/docs/_static/perf_l.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/pos_robustness.png` & `dacy-2.5.1/docs/_static/pos_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/table_dep.html` & `dacy-2.5.1/docs/_static/table_dep.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/table_ent.html` & `dacy-2.5.1/docs/_static/table_ent.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/table_perf.html` & `dacy-2.5.1/docs/_static/table_perf.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/_static/table_pos.html` & `dacy-2.5.1/docs/_static/table_pos.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/conf.py` & `dacy-2.5.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # Do not execute the notebooks when building the docs (turned off by default)
-# nbsphinx_execute = "never" # noqa ERA001
+nb_execution_allow_errors = False
 
 
 # Automatically extract typehints when specified and place them in
 # descriptions of the relevant function/method.
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#configuration
 autodoc_typehints = "description"
```

### Comparing `dacy-2.5.0/docs/faq.md` & `dacy-2.5.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/index.md` & `dacy-2.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/news.rst` & `dacy-2.5.1/docs/news.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/performance.general.rst` & `dacy-2.5.1/docs/performance.general.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/performance.robustness.rst` & `dacy-2.5.1/docs/performance.robustness.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/tutorials/basic.ipynb` & `dacy-2.5.1/docs/tutorials/basic.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999625%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, '# get the latest small model:\\n')], delete: [1, 0]}}}"}*

```diff
@@ -87,16 +87,15 @@
                         "\t- Explicitly set the environment variable TOKENIZERS_PARALLELISM=(true | false)\n",
                         "Collecting da-dacy-small-trf==any\n",
                         "  Using cached https://huggingface.co/chcaa/da_dacy_small_trf/resolve/main/da_dacy_small_trf-any-py3-none-any.whl (57.5 MB)\n"
                     ]
                 }
             ],
             "source": [
-                "nlp = dacy.load(\"da_dacy_small_trf-latest\")\n",
-                "# or equivalently\n",
+                "# get the latest small model:\n",
                 "nlp = dacy.load(\"small\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dacy-2.5.0/docs/tutorials/hate-speech.ipynb` & `dacy-2.5.1/docs/tutorials/hate-speech.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/tutorials/robustness.ipynb` & `dacy-2.5.1/docs/tutorials/robustness.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/tutorials/sentiment.ipynb` & `dacy-2.5.1/docs/tutorials/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/tutorials/textdescriptives.ipynb` & `dacy-2.5.1/docs/tutorials/textdescriptives.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/docs/tutorials.md` & `dacy-2.5.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd` & `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/pyproject.toml` & `dacy-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dacy"
-version = "2.5.0"
+version = "2.5.1"
 description = "A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish"
 authors = [
   {name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}, 
   {name = "Lasse Hansen"},
   {name = "Emil Jessen"}
 ]
```

### Comparing `dacy-2.5.0/src/dacy/datasets/dane.py` & `dacy-2.5.1/src/dacy/datasets/dane.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/datasets/lookup_tables/README.md` & `dacy-2.5.1/src/dacy/datasets/lookup_tables/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/datasets/lookup_tables/names.csv` & `dacy-2.5.1/src/dacy/datasets/lookup_tables/names.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/datasets/names.py` & `dacy-2.5.1/src/dacy/datasets/names.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/download.py` & `dacy-2.5.1/src/dacy/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functions for downloading DaCy models."""
 import os
 from importlib.metadata import version
 from pathlib import Path
 
+from spacy.util import get_installed_models
 from tqdm import tqdm
 
 DACY_DEFAULT_PATH = Path.home() / ".dacy"
 
 DEFAULT_CACHE_DIR = os.getenv(
     "DACY_CACHE_DIR",
     DACY_DEFAULT_PATH,
@@ -75,24 +76,22 @@
         a string of the model location
 
     Example:
         >>> download_model(model="da_dacy_medium_trf-0.1.0")
     """
     if model in {"small", "medium", "large"}:
         model = f"da_dacy_{model}_trf-0.1.0"
+    mdl_version = model.split("-")[-1]
 
     if model not in models_url:
         raise ValueError(
             "The model is not available in DaCy. Please use dacy.models() to see a"
             + " list of all models",
         )
 
-    mdl_version = model.split("-")[-1]
-    from spacy.util import get_installed_models
-
     mdl = model.split("-")[0]
     if mdl in get_installed_models() and not force:
         if version(mdl) == mdl_version:
             return mdl
     else:
         install(models_url[model])
     return mdl
```

### Comparing `dacy-2.5.0/src/dacy/hate_speech/wrapped_models.py` & `dacy-2.5.1/src/dacy/hate_speech/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/load.py` & `dacy-2.5.1/src/dacy/load.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/ner/wrapped_models.py` & `dacy-2.5.1/src/dacy/ner/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/score/input_length.py` & `dacy-2.5.1/src/dacy/score/input_length.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/score/score.py` & `dacy-2.5.1/src/dacy/score/score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/sentiment/wrapped_models.py` & `dacy-2.5.1/src/dacy/sentiment/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy/utils.py` & `dacy-2.5.1/src/dacy/utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy.egg-info/PKG-INFO` & `dacy-2.5.1/src/dacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.5.0
+Version: 2.5.1
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dacy-2.5.0/src/dacy.egg-info/SOURCES.txt` & `dacy-2.5.1/src/dacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/src/dacy.egg-info/requires.txt` & `dacy-2.5.1/src/dacy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tasks.py` & `dacy-2.5.1/tasks.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tests/test_datasets.py` & `dacy-2.5.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tests/test_hate_speech.py` & `dacy-2.5.1/tests/test_hate_speech.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tests/test_score.py` & `dacy-2.5.1/tests/test_score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tests/test_sentiment.py` & `dacy-2.5.1/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/readme.md` & `dacy-2.5.1/training/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/configs/config_-l-ctra_small.cfg` & `dacy-2.5.1/training/v0.0.0/configs/config_-l-ctra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/configs/config_conv_small.cfg` & `dacy-2.5.1/training/v0.0.0/configs/config_conv_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/configs/config_electra_small.cfg` & `dacy-2.5.1/training/v0.0.0/configs/config_electra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/configs/config_large.cfg` & `dacy-2.5.1/training/v0.0.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/configs/config_medium.cfg` & `dacy-2.5.1/training/v0.0.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/img/perf_training.png` & `dacy-2.5.1/training/v0.0.0/img/perf_training.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_cased.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_cased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_-l-ctra_uncased.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_uncased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_conv_small.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_conv_small.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_electra.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_electra.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_large.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_large.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/metrics/dane_medium.json` & `dacy-2.5.1/training/v0.0.0/metrics/dane_medium.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/orth_variants.json` & `dacy-2.5.1/training/v0.0.0/orth_variants.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.0.0/project.yml` & `dacy-2.5.1/training/v0.0.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/augment.py` & `dacy-2.5.1/training/v0.1.0/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/configs/config_large.cfg` & `dacy-2.5.1/training/v0.1.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/configs/config_medium.cfg` & `dacy-2.5.1/training/v0.1.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/configs/config_small.cfg` & `dacy-2.5.1/training/v0.1.0/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/project.yml` & `dacy-2.5.1/training/v0.1.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.0/update_meta_json.py` & `dacy-2.5.1/training/v0.1.0/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/augment.py` & `dacy-2.5.1/training/v0.1.1/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/configs/config_large.cfg` & `dacy-2.5.1/training/v0.1.1/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/configs/config_medium.cfg` & `dacy-2.5.1/training/v0.1.1/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/configs/config_small.cfg` & `dacy-2.5.1/training/v0.1.1/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/danish_augmenter.py` & `dacy-2.5.1/training/v0.1.1/danish_augmenter.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/project.yml` & `dacy-2.5.1/training/v0.1.1/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/training/v0.1.1/update_meta_json.py` & `dacy-2.5.1/training/v0.1.1/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/dacy-basic.ipynb` & `dacy-2.5.1/tutorials/dacy-basic.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/dacy-robustness.ipynb` & `dacy-2.5.1/tutorials/dacy-robustness.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/hate-speech.ipynb` & `dacy-2.5.1/tutorials/hate-speech.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/sentiment-neural.ipynb` & `dacy-2.5.1/tutorials/sentiment-neural.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/sentiment-rule-based.ipynb` & `dacy-2.5.1/tutorials/sentiment-rule-based.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.5.0/tutorials/textdescriptives_integration.ipynb` & `dacy-2.5.1/tutorials/textdescriptives_integration.ipynb`

 * *Files identical despite different names*

