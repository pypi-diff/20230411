# Comparing `tmp/dacy-2.5.1.tar.gz` & `tmp/dacy-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacy-2.5.1.tar", last modified: Tue Apr 11 00:26:24 2023, max compression
+gzip compressed data, was "dacy-2.5.2.tar", last modified: Tue Apr 11 01:22:18 2023, max compression
```

## Comparing `dacy-2.5.1.tar` & `dacy-2.5.2.tar`

### file list

```diff
@@ -1,205 +1,197 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.259168 dacy-2.5.1/
--rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 00:26:13.000000 dacy-2.5.1/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 00:26:13.000000 dacy-2.5.1/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/mypy.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 00:26:13.000000 dacy-2.5.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 00:26:13.000000 dacy-2.5.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 00:26:13.000000 dacy-2.5.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     8098 2023-04-11 00:26:14.000000 dacy-2.5.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 00:26:13.000000 dacy-2.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 00:26:13.000000 dacy-2.5.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 00:26:13.000000 dacy-2.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:26:24.255169 dacy-2.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6594 2023-04-11 00:26:13.000000 dacy-2.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 00:26:13.000000 dacy-2.5.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.227169 dacy-2.5.1/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
--rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/asent_analysis.png
--rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/asent_prediction.png
--rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/dep_parse.png
--rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/dep_robustness.png
--rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_black_text.png
--rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/icon_no_title.png
--rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/ner.png
--rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/ner_robustness.png
--rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/perf.png
--rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/perf_l.png
--rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/pos_robustness.png
--rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_dep.html
--rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_ent.html
--rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_perf.html
--rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/_static/table_pos.html
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/adv_tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/api/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.datasets.rst
--rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.download.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/api/dacy.score.rst
--rw-r--r--   0 root         (0) root         (0)     3821 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/faq.md
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)     4714 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.general.rst
--rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.robustness.rst
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/performance.rst
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.235169 dacy-2.5.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    26242 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/basic.ipynb
--rw-r--r--   0 root         (0) root         (0)     5953 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)    38230 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)    21177 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/sentiment.ipynb
--rw-r--r--   0 root         (0) root         (0)   106814 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials/textdescriptives.ipynb
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 00:26:13.000000 dacy-2.5.1/docs/tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.219169 dacy-2.5.1/papers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.239169 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.239169 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
--rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
--rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
--rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 00:26:13.000000 dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
--rw-r--r--   0 root         (0) root         (0)     4703 2023-04-11 00:26:14.000000 dacy-2.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 00:26:24.259168 dacy-2.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.219169 dacy-2.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/datasets/
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/constants.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/dane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/datasets/lookup_tables/
--rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/lookup_tables/names.csv
--rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/datasets/names.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/hate_speech/
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/hate_speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/hate_speech/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/ner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/ner/wrapped_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/score/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/input_length.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/score/score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy/sentiment/
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/sentiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/sentiment/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 00:26:13.000000 dacy-2.5.1/src/dacy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.243169 dacy-2.5.1/src/dacy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20891 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6144 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      660 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 00:26:24.000000 dacy-2.5.1/src/dacy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 00:26:13.000000 dacy-2.5.1/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_datasets.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_hate_speech.py
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_ner.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_score.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_sentiment.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 00:26:13.000000 dacy-2.5.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/
--rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 00:26:13.000000 dacy-2.5.1/training/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_-l-ctra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_conv_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_electra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/configs/config_medium.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/img/
--rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/img/perf_training.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.247169 dacy-2.5.1/training/v0.0.0/metrics/
--rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_cased.json
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_conv_small.json
--rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_electra.json
--rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_large.json
--rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/metrics/dane_medium.json
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/orth_variants.json
--rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/project.yml
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.0.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/configs/config_small.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.0/metrics/
--rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.251169 dacy-2.5.1/training/v0.1.1/
--rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/training/v0.1.1/configs/
--rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/configs/config_small.cfg
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/danish_augmenter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/training/v0.1.1/metrics/
--rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 00:26:13.000000 dacy-2.5.1/training/v0.1.1/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 00:26:24.255169 dacy-2.5.1/tutorials/
--rw-r--r--   0 root         (0) root         (0)    16340 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/dacy-basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    38219 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/dacy-robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)     5333 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     9763 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/sentiment-neural.ipynb
--rw-r--r--   0 root         (0) root         (0)     8741 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/sentiment-rule-based.ipynb
--rw-r--r--   0 root         (0) root         (0)   106539 2023-04-11 00:26:13.000000 dacy-2.5.1/tutorials/textdescriptives_integration.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.617076 dacy-2.5.2/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 01:22:07.000000 dacy-2.5.2/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 01:22:07.000000 dacy-2.5.2/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.577075 dacy-2.5.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.577075 dacy-2.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.577075 dacy-2.5.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/mypy.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 01:22:07.000000 dacy-2.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 01:22:07.000000 dacy-2.5.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 01:22:07.000000 dacy-2.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-04-11 01:22:08.000000 dacy-2.5.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 01:22:07.000000 dacy-2.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 01:22:07.000000 dacy-2.5.2/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 01:22:07.000000 dacy-2.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20903 2023-04-11 01:22:18.617076 dacy-2.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6606 2023-04-11 01:22:07.000000 dacy-2.5.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 01:22:07.000000 dacy-2.5.2/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.581075 dacy-2.5.2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.589075 dacy-2.5.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
+-rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/asent_analysis.png
+-rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/asent_prediction.png
+-rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/dep_parse.png
+-rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/dep_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/icon_black_text.png
+-rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/icon_no_title.png
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/ner.png
+-rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/ner_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/perf.png
+-rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/perf_l.png
+-rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/pos_robustness.png
+-rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/table_dep.html
+-rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/table_ent.html
+-rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/table_perf.html
+-rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/_static/table_pos.html
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/adv_tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.593075 dacy-2.5.2/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/api/dacy.datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/api/dacy.download.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/api/dacy.score.rst
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/faq.md
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)     4834 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/performance.general.rst
+-rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/performance.robustness.rst
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/performance.rst
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.593075 dacy-2.5.2/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    26266 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials/basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38507 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials/robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)    21450 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials/sentiment.ipynb
+-rw-r--r--   0 root         (0) root         (0)   108704 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials/textdescriptives.ipynb
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 01:22:07.000000 dacy-2.5.2/docs/tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.569075 dacy-2.5.2/papers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.597075 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.597075 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
+-rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 01:22:07.000000 dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-04-11 01:22:08.000000 dacy-2.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 01:22:18.617076 dacy-2.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.573075 dacy-2.5.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.597075 dacy-2.5.2/src/dacy/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/datasets/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/dane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/datasets/lookup_tables/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/lookup_tables/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/lookup_tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/lookup_tables/names.csv
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/datasets/names.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/hate_speech/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/hate_speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/hate_speech/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/ner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/ner/wrapped_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/score/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/score/input_length.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/score/score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy/sentiment/
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/sentiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/sentiment/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 01:22:07.000000 dacy-2.5.2/src/dacy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.601075 dacy-2.5.2/src/dacy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20903 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5915 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 01:22:18.000000 dacy-2.5.2/src/dacy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 01:22:07.000000 dacy-2.5.2/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.605075 dacy-2.5.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_datasets.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_hate_speech.py
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_score.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 01:22:07.000000 dacy-2.5.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.605075 dacy-2.5.2/training/
+-rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 01:22:07.000000 dacy-2.5.2/training/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.605075 dacy-2.5.2/training/v0.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.605075 dacy-2.5.2/training/v0.0.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/configs/config_-l-ctra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/configs/config_conv_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/configs/config_electra_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/configs/config_medium.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.605075 dacy-2.5.2/training/v0.0.0/img/
+-rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/img/perf_training.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.609075 dacy-2.5.2/training/v0.0.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_-l-ctra_cased.json
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_conv_small.json
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_electra.json
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_large.json
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/metrics/dane_medium.json
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/orth_variants.json
+-rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.0.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.609075 dacy-2.5.2/training/v0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.609075 dacy-2.5.2/training/v0.1.0/configs/
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/configs/config_small.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.613075 dacy-2.5.2/training/v0.1.0/metrics/
+-rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.0/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.613075 dacy-2.5.2/training/v0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.613075 dacy-2.5.2/training/v0.1.1/configs/
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/configs/config_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/danish_augmenter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 01:22:18.617076 dacy-2.5.2/training/v0.1.1/metrics/
+-rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/project.yml
+-rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 01:22:07.000000 dacy-2.5.2/training/v0.1.1/utils.py
```

### Comparing `dacy-2.5.1/.cruft.json` & `dacy-2.5.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `dacy-2.5.2/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/ISSUE_TEMPLATE/config.yml` & `dacy-2.5.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/dependabot.yml` & `dacy-2.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/check_for_rej.yml` & `dacy-2.5.2/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/cruft.yml` & `dacy-2.5.2/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/dependabot_automerge.yml` & `dacy-2.5.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/documentation.yml` & `dacy-2.5.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/mypy.yml` & `dacy-2.5.2/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/pre-commit.yml` & `dacy-2.5.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/release.yml` & `dacy-2.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/stalebot.yml` & `dacy-2.5.2/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.github/workflows/tests.yml` & `dacy-2.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.gitignore` & `dacy-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/.pre-commit-config.yaml` & `dacy-2.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/CHANGELOG.md` & `dacy-2.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.5.2 (2023-04-11)
+### Fix
+* Update dependencies to allow for the latest version ([`86f1d2b`](https://github.com/centre-for-humanities-computing/DaCy/commit/86f1d2b7a99ffea03b2ca6d3506b475207c0fc81))
+
+### Documentation
+* Updated news and changelog ([`b41dc5c`](https://github.com/centre-for-humanities-computing/DaCy/commit/b41dc5c53e2f84a8db516fcb8fa79cd72e814469))
+* Reran tutorials to update the onces in the folder ([`b50701d`](https://github.com/centre-for-humanities-computing/DaCy/commit/b50701dd8dfaa874c9a7ac0a5c56e203a5d6ca44))
+* Hide download outputs from docs ([`493c78f`](https://github.com/centre-for-humanities-computing/DaCy/commit/493c78f4674a7f14989aab8d5d9683b72f281c2e))
+* Updated badges in readme ([`5141760`](https://github.com/centre-for-humanities-computing/DaCy/commit/51417605601e00daf7cadf91a52292758d991494))
+
 ## v2.5.1 (2023-04-11)
 ### Fix
 * Removed *-latest models ([`b2964e2`](https://github.com/centre-for-humanities-computing/DaCy/commit/b2964e28881e92edfebe1bdbbcf12dd09d9d043c))
 
 ### Documentation
 * Updated docs to not include *-latest models ([`3b9c798`](https://github.com/centre-for-humanities-computing/DaCy/commit/3b9c798e794e0f42fa9990f8537c1f591c031553))
 
 ## v2.5.0 (2023-04-11)
-### Feature
-* Moved dacy to use swift template ([`189c891`](https://github.com/centre-for-humanities-computing/DaCy/commit/189c891323f1ff083d1800fc3acd435c456fd1b5))
 
 ### Fix
 * Mypy ([`3b78e18`](https://github.com/centre-for-humanities-computing/DaCy/commit/3b78e18ef93a09fe2d152a5b9790c521ecffeb02))
 * Removed support for old version 0.0.0 versions ([`17649c3`](https://github.com/centre-for-humanities-computing/DaCy/commit/17649c31fb30cd083d1864b1e9b38389bb543cfd))
 * Fixed mypy error ([`38b788a`](https://github.com/centre-for-humanities-computing/DaCy/commit/38b788a16ce9e9d4cf5033984c8331bdfbdc7f46))
 * Dane now download correctly ([`455ac20`](https://github.com/centre-for-humanities-computing/DaCy/commit/455ac201dadd7047b044cd76a98944244fdf9dd9))
 * Fix mypy ([`4dc0df0`](https://github.com/centre-for-humanities-computing/DaCy/commit/4dc0df0158679ffc66ea9dbae6fcf54576340d88))
@@ -56,15 +64,14 @@
 ### Documentation
 * Fixed markdown link in .rst file ([`fe424be`](https://github.com/centre-for-humanities-computing/DaCy/commit/fe424bebdb5b92c1b9af8f9c99a5ed4e4a00f68c))
 * Added news ([`d648ac1`](https://github.com/centre-for-humanities-computing/DaCy/commit/d648ac10d139ff20fa4fe32a98acc65ec6c88ec5))
 
 ## v2.3.0 (2023-01-05)
 ### Feature
 * Added scandi-ner model to dacy ([`dc2a514`](https://github.com/centre-for-humanities-computing/DaCy/commit/dc2a51491eba86c480c000c6707e6a4c572feae5))
-* Added scandi-ner model to dacy ([`a2bec3b`](https://github.com/centre-for-humanities-computing/DaCy/commit/a2bec3bc43296aeb4b7f9059e9123ed48b18e5c2))
 
 ### Documentation
 * Added news ([`f5b64da`](https://github.com/centre-for-humanities-computing/DaCy/commit/f5b64dae0925bd8d7709c29238d860f9297bf761))
 * Added news ([`ed991b8`](https://github.com/centre-for-humanities-computing/DaCy/commit/ed991b816da732e1c9bbb5aaa55175597b34fcc7))
 * Model was trained by dan nielsen ([`be4471b`](https://github.com/centre-for-humanities-computing/DaCy/commit/be4471bdcaf1ce33f51e0e4e8e4382e53a10f0ea))
 * Remove rubbish from changelog ([`35adc3b`](https://github.com/centre-for-humanities-computing/DaCy/commit/35adc3b347600104d68cd03c05b8677078cda6fc))
 * Fix minor ([`b363a4e`](https://github.com/centre-for-humanities-computing/DaCy/commit/b363a4e8cb4b7dc0b0e172b24fecde0eac675197))
```

### Comparing `dacy-2.5.1/CODE_OF_CONDUCT.md` & `dacy-2.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/CONTRIBUTING.md` & `dacy-2.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/LICENSE` & `dacy-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/PKG-INFO` & `dacy-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.5.1
+Version: 2.5.2
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -232,15 +232,15 @@
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
 # DaCy: An efficient and unified framework for danish NLP
 
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
```

### Comparing `dacy-2.5.1/README.md` & `dacy-2.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
 # DaCy: An efficient and unified framework for danish NLP
 
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 [https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/
 icon_black_text.png] # DaCy: An efficient and unified framework for danish NLP
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status] [![pip
 downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/
 dacy/) [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi
 status] [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 [black] [![documentation](https://github.com/centre-for-humanities-computing/
-dacy/workflows/documentation/badge.svg)][documentation] [![Tests](https://
-github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/
-badge.svg)][tests] [![Demo](https://img.shields.io/badge/Try%20the-Demo-
-important)](https://huggingface.co/chcaa/
+dacy/actions/workflows/documentation.yml/badge.svg)][documentation] [![Tests]
+(https://github.com/centre-for-humanities-computing/dacy/actions/workflows/
+tests.yml/badge.svg)][tests] [![Demo](https://img.shields.io/badge/Try%20the-
+Demo-important)](https://huggingface.co/chcaa/
 da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 [pypi status]: https://pypi.org/project/dacy/ [documentation]: https://centre-
 for-humanities-computing.github.io/dacy/ [tests]: https://github.com/centre-
 for-humanities-computing/dacy/actions?workflow=Tests [black]: https://
 github.com/psf/black  DaCy is a Danish natural language preprocessing framework
 made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance
 on Named entity recognition, part-of-speech tagging and dependency parsing for
```

### Comparing `dacy-2.5.1/citation.cff` & `dacy-2.5.2/citation.cff`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png` & `dacy-2.5.2/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/asent_analysis.png` & `dacy-2.5.2/docs/_static/asent_analysis.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/asent_prediction.png` & `dacy-2.5.2/docs/_static/asent_prediction.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/dep_parse.png` & `dacy-2.5.2/docs/_static/dep_parse.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/dep_robustness.png` & `dacy-2.5.2/docs/_static/dep_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/favicon.ico` & `dacy-2.5.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/icon.png` & `dacy-2.5.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/icon_black_text.png` & `dacy-2.5.2/docs/_static/icon_black_text.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/icon_dark.png` & `dacy-2.5.2/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/icon_no_title.png` & `dacy-2.5.2/docs/_static/icon_no_title.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/ner.png` & `dacy-2.5.2/docs/_static/ner.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/ner_robustness.png` & `dacy-2.5.2/docs/_static/ner_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/perf.png` & `dacy-2.5.2/docs/_static/perf.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/perf_l.png` & `dacy-2.5.2/docs/_static/perf_l.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/pos_robustness.png` & `dacy-2.5.2/docs/_static/pos_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/table_dep.html` & `dacy-2.5.2/docs/_static/table_dep.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/table_ent.html` & `dacy-2.5.2/docs/_static/table_ent.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/table_perf.html` & `dacy-2.5.2/docs/_static/table_perf.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/_static/table_pos.html` & `dacy-2.5.2/docs/_static/table_pos.html`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/conf.py` & `dacy-2.5.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # Do not execute the notebooks when building the docs (turned off by default)
-nb_execution_allow_errors = False
+nb_execution_raise_on_error = True
+nb_execution_mode = "cache"
 
 
 # Automatically extract typehints when specified and place them in
 # descriptions of the relevant function/method.
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#configuration
 autodoc_typehints = "description"
```

### Comparing `dacy-2.5.1/docs/faq.md` & `dacy-2.5.2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/index.md` & `dacy-2.5.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/news.rst` & `dacy-2.5.2/docs/news.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 News and Changelog
 ---------------------------------
 
+**2.5.0 (10/04/23)**
+
+- Removed support for `0.0.0` models. To use these models you will now have to use `DaCy=<2.4.3`
+
 **2.3.0 (05/01/23)**
 
 - New tutorial added for using DaCy with `textdescriptives`. You can find it `here <https://centre-for-humanities-computing.github.io/DaCy/using_dacy.html>`__
 
 **2.2.10 (05/01/23)**
 
 - Added support for spaCy 3.4.0
```

### Comparing `dacy-2.5.1/docs/performance.general.rst` & `dacy-2.5.2/docs/performance.general.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/performance.robustness.rst` & `dacy-2.5.2/docs/performance.robustness.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/docs/tutorials/basic.ipynb` & `dacy-2.5.2/docs/tutorials/basic.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994166666666666%*

 * *Differences: {"'cells'": "{3: {'metadata': {replace: OrderedDict([('tags', ['hide-output'])])}}, 11: {'source': "*

 * *            '{insert: [(1, \'nlp = dacy.load("small", exclude=["ner"])\\n\')], delete: [1]}}}'}*

```diff
@@ -64,15 +64,19 @@
                 "\n",
                 "From here we can now download a model using:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "huggingface/tokenizers: The current process just got forked, after parallelism has already been used. Disabling parallelism to avoid deadlocks...\n",
                         "To disable this warning, you can either:\n",
@@ -249,15 +253,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# load the small dacy model excluding the NER component\n",
-                "nlp = dacy.load(\"da_dacy_small_trf-latest\", exclude=[\"ner\"])\n",
+                "nlp = dacy.load(\"small\", exclude=[\"ner\"])\n",
                 "# or use an empty spacy model if you only want to do NER\n",
                 "# nlp = spacy.blank(\"da\")\n",
                 "\n",
                 "# add the ner component from the state-of-the-art model\n",
                 "nlp.add_pipe(\"dacy/ner\")\n",
                 "\n",
                 "doc = nlp(\"Denne NER model er tr\u00e6net af Dan fra Alexandra Instituttet\")\n",
```

### Comparing `dacy-2.5.1/docs/tutorials/hate-speech.ipynb` & `dacy-2.5.2/docs/tutorials/hate-speech.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889880952380953%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-output'])])}, 'outputs': {0: {'output_type': 'execute_result', 'data': "*

 * *            "OrderedDict([('text/plain', "*

 * *            "['<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at "*

 * *            "0x16c8c2860>'])]), 'execution_count': 1, 'metadata': OrderedDict(), delete: ['name', "*

 * *            "'text']}, delete: [0]}}, 4: {'execution_count': 2}}",*

 * * "'metadata'": "{'language_inf […]*

```diff
@@ -56,31 +56,30 @@
                 "### Usage\n",
                 "\n",
                 "To add the emotion models to your pipeline simply run:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
+            "execution_count": 1,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/au561649/Desktop/Github/DaCy/.venv/lib/python3.9/site-packages/torch/autocast_mode.py:162: UserWarning: User provided device_type of 'cuda', but CUDA is not available. Disabling\n",
-                        "  warnings.warn('User provided device_type of \\'cuda\\', but CUDA is not available. Disabling')\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Added components to pipeline.\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at 0x16c8c2860>"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import dacy\n",
                 "import spacy\n",
                 "\n",
                 "nlp = spacy.blank(\"da\") # create an empty pipeline\n",
@@ -101,15 +100,15 @@
                 "probabilites of the models.\n",
                 "\n",
                 "Let's look at an example using the model:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "offensive\n",
@@ -148,15 +147,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8 (main, Oct 13 2022, 09:48:40) [Clang 14.0.0 (clang-1400.0.29.102)]"
+            "version": "3.10.10"
         },
         "orig_nbformat": 2,
         "vscode": {
             "interpreter": {
                 "hash": "b40b3901be4435b5a71cc3915f22553724b83a304e297d25655c4809f01488a8"
             }
         }
```

### Comparing `dacy-2.5.1/docs/tutorials/robustness.ipynb` & `dacy-2.5.2/docs/tutorials/robustness.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904513888888888%*

 * *Differences: {"'cells'": "{3: {'metadata': {replace: OrderedDict([('tags', ['hide-output'])])}, 'source': "*

 * *            '{insert: [(3, \'test = dane(splits=["test"])\')], delete: [10, 9, 8, 7, 6, 2, 1, '*

 * *            "0]}}, 6: {'metadata': {replace: OrderedDict([('tags', ['hide-output'])])}}, 11: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', ['hide-output'])])}}, insert: [(4, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict([('tags', ['hid […]*

```diff
@@ -36,15 +36,19 @@
             "source": [
                 "## Loading models and data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/Users/au561649/Desktop/Github/DaCy/.venv/lib/python3.9/site-packages/spacy/util.py:833: UserWarning: [W095] Model 'da_dacy_medium_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.2.4). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
                         "  warnings.warn(warn_msg)\n",
@@ -52,21 +56,32 @@
                         "  warnings.warn(warn_msg)\n",
                         "/Users/au561649/Desktop/Github/DaCy/.venv/lib/python3.9/site-packages/spacy_transformers/pipeline_component.py:406: UserWarning: Automatically converting a transformer component from spacy-transformers v1.0 to v1.1+. If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spacy-transformers version. For more details and available updates, run: python -m spacy validate\n",
                         "  warnings.warn(warn_msg)\n"
                     ]
                 }
             ],
             "source": [
-                "import spacy\n",
-                "import dacy\n",
-                "\n",
                 "from dacy.datasets import dane\n",
                 "\n",
                 "# load the DaNE test set\n",
-                "test = dane(splits=[\"test\"])\n",
+                "test = dane(splits=[\"test\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "import spacy\n",
+                "import dacy\n",
                 "\n",
                 "# load models\n",
                 "spacy_small = spacy.load(\"da_core_news_sm\")\n",
                 "dacy_small = dacy.load(\"small\")"
             ]
         },
         {
@@ -76,15 +91,19 @@
                 "## Estimating performance\n",
                 "Evaluating models already in the `SpaCy` framework is very straightforward. Simply call the `score` function on your nlp pipeline and choose which metrics you want to calculate performance for. `score` is a wrapper for `SpaCy.scorer.Scorer` that outputs a nicely formatted dataframe. `score` calculates performance for NER, POS, tokenization, and dependency parsing by default, which can be changed with the score_fn argument."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/Users/au561649/Desktop/Github/DaCy/.venv/lib/python3.9/site-packages/torch/autocast_mode.py:162: UserWarning: User provided device_type of 'cuda', but CUDA is not available. Disabling\n",
                         "  warnings.warn('User provided device_type of \\'cuda\\', but CUDA is not available. Disabling')\n",
@@ -338,15 +357,19 @@
                 "from dacy.datasets import female_names\n",
                 "from spacy.training.augment import create_lower_casing_augmenter"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/Users/au561649/Desktop/Github/DaCy/.venv/lib/python3.9/site-packages/torch/autocast_mode.py:162: UserWarning: User provided device_type of 'cuda', but CUDA is not available. Disabling\n",
                         "  warnings.warn('User provided device_type of \\'cuda\\', but CUDA is not available. Disabling')\n",
```

### Comparing `dacy-2.5.1/docs/tutorials/sentiment.ipynb` & `dacy-2.5.2/docs/tutorials/sentiment.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894806565788709%*

 * *Differences: {"'cells'": "{2: {'execution_count': 2, 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-output'])])}, 'outputs': {0: {'data': {'text/plain': "*

 * *            "['<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at "*

 * *            "0x11f895660>']}, 'execution_count': 2}}}, 4: {'execution_count': 3}, 6: "*

 * *            "{'execution_count': 4, 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-output'])])}, 'outputs': {0: {'output_type': 'execute_result', 'data' […]*

```diff
@@ -53,24 +53,28 @@
                 "text is subjective or objective in its phrasing.\n",
                 "\n",
                 "To add the subjectivity model to your pipeline simply run:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {},
+            "execution_count": 2,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at 0x169757520>"
+                            "<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at 0x11f895660>"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import dacy\n",
                 "import spacy\n",
@@ -89,15 +93,15 @@
                 "two extensions to the Doc object,`subjectivity_prob` and `subjectivity`.\n",
                 "These show the probabilities of a document being subjective and whether not a\n",
                 "document is subjective or objective. Let's look at an example using the model:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "objective\n",
@@ -132,45 +136,51 @@
                 "negative or neutral.\n",
                 "\n",
                 "To add the polarity model to your pipeline simply run:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
+            "execution_count": 4,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Added polarity compoenent\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at 0x16afab340>"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "nlp = spacy.blank(\"da\") # an empty spacy pipeline\n",
                 "# could also be a dacy pipeline, e.g. nlp = dacy.load(\"large\")\n",
-                "nlp.add_pipe(\"dacy/polarity\")\n",
-                "print(\"Added polarity compoenent\")"
+                "nlp.add_pipe(\"dacy/polarity\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This will add the `dacy.polarity` component to your pipeline, which adds\n",
                 "two extensions to the Doc object,`polarity_prob` and `polarity`.\n",
                 "These show the probabilities of a document being positive/neutral/negative and\n",
                 "the resulting classification. Let's look at an example using the model:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "negative\n",
@@ -215,40 +225,45 @@
                 "- \"Frygt/Bekymret\" (Fear)\n",
                 "\n",
                 "To add the emotion models to your pipeline simply run:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
-            "metadata": {},
+            "execution_count": 6,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/Users/au561649/Desktop/Github/DaCy/dacy/sentiment/wrapped_models.py:142: UserWarning: The 'emotion' component assumes the 'emotionally_laden' extension is set. To set it you can run  nlp.add_pipe('dacy.emotionally_laden')\n",
+                        "/Users/au561649/Github/DaCy/src/dacy/sentiment/wrapped_models.py:143: UserWarning: The 'emotion' component assumes the 'emotionally_laden' extension is set. To set it you can run  nlp.add_pipe('dacy/emotionally_laden')\n",
                         "  warn(\n"
                     ]
                 },
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Pipeline components added\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<spacy_wrap.pipeline_component_seq_clf.SequenceClassificationTransformer at 0x16afb91e0>"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "nlp = spacy.blank(\"da\") # an empty spacy pipeline\n",
                 "# could also be a dacy pipeline, e.g. nlp = dacy.load(\"large\")\n",
                 "nlp.add_pipe(\"dacy/emotionally_laden\") # for emotianal/non-emotional\n",
-                "nlp.add_pipe(\"dacy/emotion\") # for type of emotion\n",
-                "\n",
-                "print(\"Pipeline components added\")"
+                "nlp.add_pipe(\"dacy/emotion\") # for type of emotion"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This wil set the two extensions to the Doc object, `laden` and `emotion`.\n",
@@ -257,15 +272,15 @@
                 "probabilites of the model.\n",
                 "\n",
                 "Let's look at an example using the model:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "emotional\n",
@@ -314,15 +329,15 @@
                 "```\n",
                 "\n",
                 "first we will need to set up the spaCy pipeline, which only need to include a method for creating sentences. You can use DaCy for this as it performs dependendency parsing, but it is notably faster to use a rule-based sentencizer. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "neg=0.413 neu=0.587 pos=0.0 compound=-0.5448\n"
@@ -356,15 +371,15 @@
             "metadata": {},
             "source": [
                 "Asent also allow us to obtain more information such as the rated valence of a single token, whether a word is a negation or the valence of a words accounting for its context (polarity):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "polarity=0.0 token=jeg span=jeg | Valence: 0.0 | Negation: False\n",
@@ -394,15 +409,15 @@
                 "\n",
                 "If you want to learn more about how asent works check out the excellent [documentation](https://kennethenevoldsen.github.io/asent/introduction.html).\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<span class=\"tex2jax_ignore\"><div class=\"spans\" style=\"line-height: 2.5; direction: ltr\">jeg er \n",
                             "<span style=\"font-weight: bold; display: inline-block; position: relative; height: 60px;\">\n",
@@ -451,21 +466,21 @@
             "source": [
                 "# visualize model prediction\n",
                 "asent.visualize(doc, style=\"prediction\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<span class=\"tex2jax_ignore\"><svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" xml:lang=\"en\" id=\"5fa531fd73854f7180be4d43d25ff9d9-0\" class=\"displacy\" width=\"1100\" height=\"312.0\" direction=\"ltr\" style=\"max-width: none; height: 312.0px; color: #000000; background: #ffffff; font-family: Arial; direction: ltr\">\n",
+                            "<span class=\"tex2jax_ignore\"><svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" xml:lang=\"en\" id=\"56f40990d572425ea5e7124c8859f5da-0\" class=\"displacy\" width=\"1100\" height=\"312.0\" direction=\"ltr\" style=\"max-width: none; height: 312.0px; color: #000000; background: #ffffff; font-family: Arial; direction: ltr\">\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"222.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"50\">jeg</tspan>\n",
                             "    <tspan class=\"displacy-tag\" dy=\"2em\" fill=\"currentColor\" x=\"50\">0.0</tspan>\n",
                             "</text>\n",
                             "\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"222.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"225\">er</tspan>\n",
@@ -489,25 +504,25 @@
                             "\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"222.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"925\">.</tspan>\n",
                             "    <tspan class=\"displacy-tag\" dy=\"2em\" fill=\"currentColor\" x=\"925\">0.0</tspan>\n",
                             "</text>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-5fa531fd73854f7180be4d43d25ff9d9-0-0\" stroke-width=\"2px\" d=\"M595,177.0 C595,89.5 745.0,89.5 745.0,177.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-56f40990d572425ea5e7124c8859f5da-0-0\" stroke-width=\"2px\" d=\"M595,177.0 C595,89.5 745.0,89.5 745.0,177.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-5fa531fd73854f7180be4d43d25ff9d9-0-0\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">intensified by</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-56f40990d572425ea5e7124c8859f5da-0-0\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">intensified by</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M595,179.0 L587,167.0 603,167.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-5fa531fd73854f7180be4d43d25ff9d9-0-1\" stroke-width=\"2px\" d=\"M420,177.0 C420,2.0 750.0,2.0 750.0,177.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-56f40990d572425ea5e7124c8859f5da-0-1\" stroke-width=\"2px\" d=\"M420,177.0 C420,2.0 750.0,2.0 750.0,177.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-5fa531fd73854f7180be4d43d25ff9d9-0-1\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">negated by</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-56f40990d572425ea5e7124c8859f5da-0-1\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">negated by</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M420,179.0 L412,167.0 428,167.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "</svg></span>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
@@ -551,15 +566,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.10.10"
         },
         "orig_nbformat": 2,
         "vscode": {
             "interpreter": {
                 "hash": "41a0a94681c1d0d7a5ae694864ee715c089937d98d908faa5b8f75504686895e"
             }
         }
```

### Comparing `dacy-2.5.1/docs/tutorials/textdescriptives.ipynb` & `dacy-2.5.2/docs/tutorials/textdescriptives.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950285722116443%*

 * *Differences: {"'cells'": "{5: {'metadata': {replace: OrderedDict([('tags', ['hide-output'])])}, 'outputs': {0: "*

 * *            "{'text': {insert: [(0, "*

 * *            '"/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:887: '*

 * *            "UserWarning: [W095] Model 'da_dacy_medium_trf' (0.1.0) was trained with spaCy v3.1 "*

 * *            'and may not be 100% compatible with the current version (3.5.1). If you see errors or '*

 * *            'degraded performance, download a newer compatible model or retra […]*

```diff
@@ -148,50 +148,46 @@
                 "\n",
                 "Because we are using a DaCy model, the `dependency_distance` component will use the dependency parser from DaCy for its calculations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:877: UserWarning: [W095] Model 'da_dacy_medium_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.4.4). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
+                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:887: UserWarning: [W095] Model 'da_dacy_medium_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.5.1). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
                         "  warnings.warn(warn_msg)\n",
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:877: UserWarning: [W095] Model 'da_dacy_small_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.4.4). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
+                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:887: UserWarning: [W095] Model 'da_dacy_small_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.5.1). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
                         "  warnings.warn(warn_msg)\n",
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy_transformers/pipeline_component.py:405: UserWarning: Automatically converting a transformer component from spacy-transformers v1.0 to v1.1+. If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spacy-transformers version. For more details and available updates, run: python -m spacy validate\n",
+                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy_transformers/pipeline_component.py:402: UserWarning: Automatically converting a transformer component from spacy-transformers v1.0 to v1.1+. If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spacy-transformers version. For more details and available updates, run: python -m spacy validate\n",
                         "  warnings.warn(warn_msg)\n"
                     ]
                 },
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[38;5;4m\u2139 'textdescriptives/descriptive_stats' component is required for\n",
-                        "'textdescriptives.readability'. Adding to pipe.\u001b[0m\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<textdescriptives.components.dependency_distance.DependencyDistance at 0x174c99750>"
+                            "<textdescriptives.components.dependency_distance.DependencyDistance at 0x28198aa10>"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import dacy\n",
-                "nlp = dacy.load(\"da_dacy_medium_trf-0.1.0\")\n",
+                "nlp = dacy.load(\"medium\") # load the latest medium model\n",
                 "\n",
                 "nlp.add_pipe(\"textdescriptives/readability\")\n",
                 "nlp.add_pipe(\"textdescriptives/dependency_distance\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -213,15 +209,19 @@
                 "\n",
                 "doc = nlp.pipe(df[\"message\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/pipeline/attributeruler.py:150: UserWarning: [W036] The component 'matcher' does not have any patterns defined.\n",
                         "  matches = self.matcher(doc, allow_missing=True, as_spans=False)\n"
@@ -258,40 +258,40 @@
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>label</th>\n",
                             "      <th>message</th>\n",
+                            "      <th>dependency_distance_mean</th>\n",
+                            "      <th>dependency_distance_std</th>\n",
+                            "      <th>prop_adjacent_dependency_relation_mean</th>\n",
+                            "      <th>prop_adjacent_dependency_relation_std</th>\n",
+                            "      <th>token_length_mean</th>\n",
+                            "      <th>token_length_median</th>\n",
+                            "      <th>token_length_std</th>\n",
+                            "      <th>sentence_length_mean</th>\n",
+                            "      <th>...</th>\n",
+                            "      <th>n_characters</th>\n",
+                            "      <th>n_sentences</th>\n",
                             "      <th>flesch_reading_ease</th>\n",
                             "      <th>flesch_kincaid_grade</th>\n",
                             "      <th>smog</th>\n",
                             "      <th>gunning_fog</th>\n",
                             "      <th>automated_readability_index</th>\n",
                             "      <th>coleman_liau_index</th>\n",
                             "      <th>lix</th>\n",
                             "      <th>rix</th>\n",
-                            "      <th>...</th>\n",
-                            "      <th>sentence_length_median</th>\n",
-                            "      <th>sentence_length_std</th>\n",
-                            "      <th>syllables_per_token_mean</th>\n",
-                            "      <th>syllables_per_token_median</th>\n",
-                            "      <th>syllables_per_token_std</th>\n",
-                            "      <th>n_tokens</th>\n",
-                            "      <th>n_unique_tokens</th>\n",
-                            "      <th>proportion_unique_tokens</th>\n",
-                            "      <th>n_characters</th>\n",
-                            "      <th>n_sentences</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2417</th>\n",
+                            "      <th>4420</th>\n",
                             "      <td>ham</td>\n",
-                            "      <td>Oh... Lk tt den we take e one tt ends at cine ...</td>\n",
+                            "      <td>Still at west coast... Haiz... \u00cc\u00cf'll take fore...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
@@ -305,17 +305,17 @@
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4746</th>\n",
-                            "      <td>ham</td>\n",
-                            "      <td>When you just put in the + sign, choose my num...</td>\n",
+                            "      <th>1204</th>\n",
+                            "      <td>spam</td>\n",
+                            "      <td>WIN a year supply of CDs 4 a store of ur choic...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
@@ -329,41 +329,41 @@
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>72</th>\n",
+                            "      <th>5552</th>\n",
                             "      <td>ham</td>\n",
-                            "      <td>HI BABE IM AT HOME NOW WANNA DO SOMETHING? XX</td>\n",
-                            "      <td>85.096667</td>\n",
-                            "      <td>2.715</td>\n",
-                            "      <td>3.1291</td>\n",
-                            "      <td>2.133333</td>\n",
-                            "      <td>-1.100833</td>\n",
-                            "      <td>0.7</td>\n",
-                            "      <td>17.833333</td>\n",
-                            "      <td>0.666667</td>\n",
+                            "      <td>Have a safe trip to Nigeria. Wish you happines...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>2.054805</td>\n",
-                            "      <td>1.375</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.484123</td>\n",
-                            "      <td>16.0</td>\n",
-                            "      <td>16.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>63.0</td>\n",
-                            "      <td>3.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>5501</th>\n",
-                            "      <td>spam</td>\n",
-                            "      <td>PRIVATE! Your 2003 Account Statement for 07808...</td>\n",
+                            "      <th>4250</th>\n",
+                            "      <td>ham</td>\n",
+                            "      <td>Omg Joanna is freaking me out. She's looked th...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
@@ -377,17 +377,17 @@
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>5313</th>\n",
+                            "      <th>1699</th>\n",
                             "      <td>ham</td>\n",
-                            "      <td>My sister going to earn more than me da.</td>\n",
+                            "      <td>Ok...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
@@ -407,61 +407,68 @@
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>5 rows \u00d7 28 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "     label                                            message  \\\n",
-                            "2417   ham  Oh... Lk tt den we take e one tt ends at cine ...   \n",
-                            "4746   ham  When you just put in the + sign, choose my num...   \n",
-                            "72     ham      HI BABE IM AT HOME NOW WANNA DO SOMETHING? XX   \n",
-                            "5501  spam  PRIVATE! Your 2003 Account Statement for 07808...   \n",
-                            "5313   ham           My sister going to earn more than me da.   \n",
+                            "4420   ham  Still at west coast... Haiz... \u00cc\u00cf'll take fore...   \n",
+                            "1204  spam  WIN a year supply of CDs 4 a store of ur choic...   \n",
+                            "5552   ham  Have a safe trip to Nigeria. Wish you happines...   \n",
+                            "4250   ham  Omg Joanna is freaking me out. She's looked th...   \n",
+                            "1699   ham                                              Ok...   \n",
                             "\n",
-                            "      flesch_reading_ease  flesch_kincaid_grade    smog  gunning_fog  \\\n",
-                            "2417                  NaN                   NaN     NaN          NaN   \n",
-                            "4746                  NaN                   NaN     NaN          NaN   \n",
-                            "72              85.096667                 2.715  3.1291     2.133333   \n",
-                            "5501                  NaN                   NaN     NaN          NaN   \n",
-                            "5313                  NaN                   NaN     NaN          NaN   \n",
+                            "      dependency_distance_mean  dependency_distance_std  \\\n",
+                            "4420                       NaN                      NaN   \n",
+                            "1204                       NaN                      NaN   \n",
+                            "5552                       NaN                      NaN   \n",
+                            "4250                       NaN                      NaN   \n",
+                            "1699                       NaN                      NaN   \n",
                             "\n",
-                            "      automated_readability_index  coleman_liau_index        lix       rix  \\\n",
-                            "2417                          NaN                 NaN        NaN       NaN   \n",
-                            "4746                          NaN                 NaN        NaN       NaN   \n",
-                            "72                      -1.100833                 0.7  17.833333  0.666667   \n",
-                            "5501                          NaN                 NaN        NaN       NaN   \n",
-                            "5313                          NaN                 NaN        NaN       NaN   \n",
+                            "      prop_adjacent_dependency_relation_mean  \\\n",
+                            "4420                                     NaN   \n",
+                            "1204                                     NaN   \n",
+                            "5552                                     NaN   \n",
+                            "4250                                     NaN   \n",
+                            "1699                                     NaN   \n",
                             "\n",
-                            "      ...  sentence_length_median  sentence_length_std  \\\n",
-                            "2417  ...                     NaN                  NaN   \n",
-                            "4746  ...                     NaN                  NaN   \n",
-                            "72    ...                     5.0             2.054805   \n",
-                            "5501  ...                     NaN                  NaN   \n",
-                            "5313  ...                     NaN                  NaN   \n",
+                            "      prop_adjacent_dependency_relation_std  token_length_mean  \\\n",
+                            "4420                                    NaN                NaN   \n",
+                            "1204                                    NaN                NaN   \n",
+                            "5552                                    NaN                NaN   \n",
+                            "4250                                    NaN                NaN   \n",
+                            "1699                                    NaN                NaN   \n",
                             "\n",
-                            "      syllables_per_token_mean  syllables_per_token_median  \\\n",
-                            "2417                       NaN                         NaN   \n",
-                            "4746                       NaN                         NaN   \n",
-                            "72                       1.375                         1.0   \n",
-                            "5501                       NaN                         NaN   \n",
-                            "5313                       NaN                         NaN   \n",
+                            "      token_length_median  token_length_std  sentence_length_mean  ...  \\\n",
+                            "4420                  NaN               NaN                   NaN  ...   \n",
+                            "1204                  NaN               NaN                   NaN  ...   \n",
+                            "5552                  NaN               NaN                   NaN  ...   \n",
+                            "4250                  NaN               NaN                   NaN  ...   \n",
+                            "1699                  NaN               NaN                   NaN  ...   \n",
                             "\n",
-                            "      syllables_per_token_std  n_tokens  n_unique_tokens  \\\n",
-                            "2417                      NaN       NaN              NaN   \n",
-                            "4746                      NaN       NaN              NaN   \n",
-                            "72                   0.484123      16.0             16.0   \n",
-                            "5501                      NaN       NaN              NaN   \n",
-                            "5313                      NaN       NaN              NaN   \n",
+                            "      n_characters  n_sentences  flesch_reading_ease  flesch_kincaid_grade  \\\n",
+                            "4420           NaN          NaN                  NaN                   NaN   \n",
+                            "1204           NaN          NaN                  NaN                   NaN   \n",
+                            "5552           NaN          NaN                  NaN                   NaN   \n",
+                            "4250           NaN          NaN                  NaN                   NaN   \n",
+                            "1699           NaN          NaN                  NaN                   NaN   \n",
                             "\n",
-                            "      proportion_unique_tokens  n_characters  n_sentences  \n",
-                            "2417                       NaN           NaN          NaN  \n",
-                            "4746                       NaN           NaN          NaN  \n",
-                            "72                         1.0          63.0          3.0  \n",
-                            "5501                       NaN           NaN          NaN  \n",
-                            "5313                       NaN           NaN          NaN  \n",
+                            "      smog  gunning_fog  automated_readability_index  coleman_liau_index  lix  \\\n",
+                            "4420   NaN          NaN                          NaN                 NaN  NaN   \n",
+                            "1204   NaN          NaN                          NaN                 NaN  NaN   \n",
+                            "5552   NaN          NaN                          NaN                 NaN  NaN   \n",
+                            "4250   NaN          NaN                          NaN                 NaN  NaN   \n",
+                            "1699   NaN          NaN                          NaN                 NaN  NaN   \n",
+                            "\n",
+                            "      rix  \n",
+                            "4420  NaN  \n",
+                            "1204  NaN  \n",
+                            "5552  NaN  \n",
+                            "4250  NaN  \n",
+                            "1699  NaN  \n",
                             "\n",
                             "[5 rows x 28 columns]"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -486,30 +493,30 @@
             "source": [
                 "## Exploratory Data Analysis\n",
                 "With the metrics extracted, let's do some quick exploratory data analysis to get a sense of the data. Let us start of by taking a look at the distribution of the readability metrics, `lix`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<AxesSubplot: xlabel='label', ylabel='lix'>"
+                            "<Axes: xlabel='label', ylabel='lix'>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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qqqqVFlZqauuukrnnHOOqqqqdOTIEY0YMUJ79uxRc3OzZs+erYULF+rgwYNavHix5syZo7i4OJ111llKS0vTb37zGw0cOFA1NTW688473d4keASHlmCk0aNH6/7779evf/1rjRw5Uk8++aRKS0vdHgvAGQQCAb3yyiv6zne+o2984xtauHChli9frvz8fEnSlClTdMEFF+iKK67QjBkz9L3vfS/y5xbi4uL09NNPq7q6WiNHjtS8efN07733urg18BLLcf7/s28AALhg1qxZOnr0qDZs2OD2KDAQe2QAAICxCBkAAGAsDi0BAABjsUcGAAAYi5ABAADGImQAAICxCBkAAGAsQgYAABiLkAHgqkmTJmnu3LntWnfz5s2yLEtHjx7t1M8cMmSIHnjggU49BwBvIGQAAICxCBkAAGAsQgaAZzzxxBO65JJLlJycrIyMDF1//fU6fPjwF9bbtm2bsrOzZdu2xo0bp7feeivq/q1bt2rChAny+/3KzMzUbbfdpqampp7aDAA9iJAB4BktLS26++679eabb2rDhg06ePCgZs2a9YX1fv7zn2v58uXauXOnBgwYoKlTp6qlpUWS9OGHH+rb3/62CgsLtWfPHj3zzDPaunWr5syZ08NbA6AnxLs9AACcctNNN0Wun3feeSorK9PYsWN1/PhxJSUlRe5bvHixrrzySknS2rVrNXjwYFVUVOgHP/iBSktLdcMNN0ROIL7gggtUVlamiRMnauXKlbJtu0e3CUD3Yo8MAM+orq7W1KlTlZWVpeTkZE2cOFGSVFNTE7VeTk5O5HpqaqqGDRumd999V5L05ptvas2aNUpKSopc8vLy1NraqgMHDvTcxgDoEeyRAeAJTU1NysvLU15enp588kkNGDBANTU1ysvLU3Nzc7uf5/jx47rlllt02223feG+rKysrhwZgAcQMgA84b333tPHH3+sZcuWKTMzU5K0a9euNtfdsWNHJEo++eQTvf/++xoxYoQk6eKLL9Y777yjoUOH9szgAFzFoSUAnpCVlaWEhAQ99NBD+sc//qE//vGPuvvuu9tcd+nSpaqsrNRbb72lWbNm6eyzz9a0adMkSXfccYdee+01zZkzR7t379b+/fv1/PPPc7IvEKMIGQCeMGDAAK1Zs0br16/XhRdeqGXLlum+++5rc91ly5bp9ttv15gxY1RXV6eNGzcqISFBkpSdna0tW7bo/fff14QJE/TNb35TixYt0qBBg3pycwD0EMtxHMftIQAAADqCPTIAAMBYhAwAADAWIQMAAIxFyAAAAGMRMgAAwFiEDAAAMBYhAwAAjEXIAAAAYxEyAADAWIQMAAAwFiEDAACM9X+v59IfPYaYWwAAAABJRU5ErkJggg==",
+                        "image/png": "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C7BHBq6WmZkZ8fj888/X4cOHJUl//etfNWrUKH3ta19TYmKibrzxRh09elSffPJJ+PmdOnXSxRdfHH6cmpqq7t27KyEhIWLZidcE0Dr69++vUaNGqV+/fvrBD36gZcuW6eOPP45Y36lTp/DjrKws1dXVqby8XJK0d+9ejR8/XhdddJH8fr+6d+8uSSorK4v4d07+mZGamipJ6tevX8Qy3u/RhZCBq3Xs2DHiscfjUVNTkw4cOKBrrrlGmZmZevbZZ1VaWqrFixdLUsRx9ea+/lSvCaD1dOjQQa+88oqKi4t16aWX6tFHH1WvXr20f//+0/r60aNH66OPPtKyZcu0bds2bdu2TVLk+12KfM97PJ5ml/F+jy6xpgcAWqK0tFRNTU1auHChYmI+6/Gnn37a8FQAvozH49GQIUM0ZMgQzZkzRxdccIGKiookSW+99ZaOHTum+Ph4SdLWrVuVkJCg9PR0HT16VHv27NGyZcs0bNgwSdKmTZuMbQfchZCBlXr06KHGxkY9+uijGj16tDZv3qzf/e53pscCcArbtm1TSUmJrrrqKp133nnatm2bjhw5oj59+mjXrl1qaGjQ5MmTNXv2bB04cEBz587V1KlTFRMTo3POOUfJycn6/e9/r/PPP19lZWW66667TG8SXIJDS7BS//799dBDD+m+++5T37599cQTT6igoMD0WABOwe/367XXXtP3vvc9XXLJJZo9e7YWLlyo3NxcSdKoUaPUs2dPXXHFFRo3bpy+//3vhz9uISYmRmvWrFFpaan69u2rGTNm6IEHHjC4NXATj+P899o3AAAMmDRpkqqqqvT888+bHgUWYo8MAACwFiEDAACsxaElAABgLfbIAAAAaxEyAADAWoQMAACwFiEDAACsRcgAAABrETIAjBoxYoSmT59+Ws/dsGGDPB6Pqqqqzujf7N69ux5++OEzeg0A7kDIAAAAaxEyAADAWoQMANd4/PHHdfnllysxMVFpaWm64YYbdPjw4S88b/PmzcrMzJTP59PgwYP19ttvR6zftGmThg0bpvj4eKWnp+v2229XfX19W20GgDZEyABwjcbGRt17771666239Pzzz+vAgQOaNGnSF573y1/+UgsXLtT27duVkpKi0aNHq7GxUZL04Ycf6rvf/a7y8vK0a9cuPfXUU9q0aZOmTp3axlsDoC3Emh4AAE64+eabw/cvuugiFRYWauDAgaqrq1NCQkJ43dy5c3XllVdKklatWqVu3bqpqKhIP/zhD1VQUKAJEyaETyDu2bOnCgsLNXz4cC1dulQ+n69NtwlA62KPDADXKC0t1ejRo5WRkaHExEQNHz5cklRWVhbxvKysrPD9pKQk9erVS++9954k6a233tLKlSuVkJAQvuXk5KipqUn79+9vu40B0CbYIwPAFerr65WTk6OcnBw98cQTSklJUVlZmXJyctTQ0HDar1NXV6dbb71Vt99++xfWZWRknM2RAbgAIQPAFd5//30dPXpUCxYsUHp6uiRpx44dzT5369at4Sj5+OOP9cEHH6hPnz6SpMsuu0zvvvuuevTo0TaDAzCKQ0sAXCEjI0NxcXF69NFH9c9//lN/+tOfdO+99zb73Pnz56ukpERvv/22Jk2apHPPPVfXXXedJOnOO+/U66+/rqlTp2rnzp3au3evXnjhBU72BaIUIQPAFVJSUrRy5UqtXbtWl156qRYsWKAHH3yw2ecuWLBAd9xxhwYMGKCKigqtW7dOcXFxkqTMzExt3LhRH3zwgYYNG6ZvfvObmjNnjrp27dqWmwOgjXgcx3FMDwEAANAS7JEBAADWImQAAIC1CBkAAGAtQgYAAFiLkAEAANYiZAAAgLUIGQAAYC1CBgAAWIuQAQAA1iJkAACAtQgZAABgrf8DceeXkhKu5zwAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -530,24 +537,24 @@
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "prop_adjacent_dependency_relation_std    -0.403782\n",
-                            "dependency_distance_mean                  0.364726\n",
-                            "prop_adjacent_dependency_relation_mean    0.280266\n",
-                            "proportion_unique_tokens                 -0.244895\n",
-                            "sentence_length_median                    0.222776\n",
-                            "token_length_median                      -0.197070\n",
-                            "sentence_length_mean                      0.196973\n",
-                            "dependency_distance_std                  -0.178205\n",
-                            "sentence_length_std                      -0.170378\n",
-                            "syllables_per_token_mean                 -0.169208\n",
+                            "smog                                      0.211242\n",
+                            "syllables_per_token_median                0.202707\n",
+                            "prop_adjacent_dependency_relation_std    -0.183331\n",
+                            "token_length_median                       0.181481\n",
+                            "prop_adjacent_dependency_relation_mean    0.162512\n",
+                            "rix                                       0.157532\n",
+                            "proportion_unique_tokens                  0.150327\n",
+                            "lix                                       0.129722\n",
+                            "sentence_length_median                    0.126950\n",
+                            "sentence_length_mean                      0.124367\n",
                             "dtype: float64"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -567,30 +574,30 @@
                 "That's some pretty high correlations! Notably we see that the mean dependency distance is correlated with `ham`. This makes sense, as the dependency distance is a measure of sentence complexity, and spam messages tend to be shorter and simpler.\n",
                 "\n",
                 "Let's try to plot it:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<AxesSubplot: xlabel='dependency_distance_mean', ylabel='Density'>"
+                            "<Axes: xlabel='dependency_distance_mean', ylabel='Density'>"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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gJEjR+I///kPOjo6ug1t3enJa+jOkCFDMGTIEPzpT3/CXXfdhXXr1uHWW2+FXC7vMuAWAM6ePYu6ujqsWLECYWFhAHDBAOieiI+PR1paGhYsWHDBfT39vbCmnlxz3759uOWWW3DvvfcC6AxqOTk5XVqriGwVZ0sRWYlSqcT999+Pv/zlL/jxxx9x6tQpzJ8/H1Jp5z+zIUOG4J577sHcuXPx5ZdforCwEIcPH8by5cuxbds2y/O4urri8ccfx6FDh5Ceno758+dj4sSJlrCzePFivP/++1i2bBlOnz6NrKwsbNy4Ec8991yPa3344YeRm5uLv/zlL8jOzsbHH3+M9evXdznnmWeewf79+7Fw4UJkZmYiNzcXX3/9NRYuXNjj69x1110ICgrC7NmzsW/fPhQUFOCLL77AgQMHLOcMGzYMEydOxDPPPIO77rqrx1O3e/Iafq21tRULFy7Erl27UFxcjH379uHIkSOW0BgZGQmdToe0tDTU1taipaUF4eHhkMvleOONN1BQUIAtW7bghRde6PHrP2/JkiX45JNPsGTJEmRlZeHkyZN46aWXAPT898KaenLN2NhY7Ny5E/v370dWVhYeeughVFVV9Us9RNbGcENkRS+//DKmTJmCm266CbNmzcJVV12FpKQky/3r1q3D3Llz8ec//xlxcXGYPXs2jhw50qWbx8PDA8888wzuvvtuTJ48GUqlEps2bbLcn5KSgq1bt2LHjh0YN24cJk6ciH//+9+IiIjocZ3h4eH44osvsHnzZiQkJGDNmjV48cUXu5wTHx+P3bt3IycnB1OmTMHo0aOxePFihISE9Pg6crkcO3bsQGBgIK6//nqMGjUKK1asuKAr5P7774fRaMR9991n1dfwazKZDHV1dZg7dy6GDBmCO++8E9dddx2WLVsGAJg0aRIefvhhzJkzBwEBAfjXv/6FgIAArF+/Hp999hmGDx+OFStW4JVXXulxjedNnz4dn332GbZs2YLExERcffXVOHz4sOX+nvxeWNvlrvncc89hzJgxSElJwfTp0y0hlcgeSARBEMQugog6rV+/Hk899ZRdb4HQFy+88AI+++wznDhxQuxSiMgBsOWGiESj0+lw6tQpvPnmm3j88cfFLoeIHATDDRGJZuHChUhKSsL06dMv6JJ6+OGHoVQqu709/PDDIlU88K677rqLvg+X6oYjcmbsliIim1RdXY2mpqZu71OpVAgMDBzgisRRVlaG1tbWbu/z9fW96Cw0ImfGcENEREQOhd1SRERE5FAYboiIiMihMNwQERGRQ2G4ISIiIofCcENEREQOheGGiIiIHArDDRERETmU/w9AB5SvDzSjgAAAAABJRU5ErkJggg==",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -605,30 +612,30 @@
             "metadata": {},
             "source": [
                 "We can do a similar thing for the `lix` score, where we see that here isn't a big difference between the two classes:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<AxesSubplot: xlabel='lix', ylabel='Density'>"
+                            "<Axes: xlabel='lix', ylabel='Density'>"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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ZvPmzQZgpKammhWzTSgtLTW6d+9uLFq0yBgzZkx9YdI+bx733XefMXr06CN+3eFwGNHR0cY///nP+vuKi4sNb29v48MPP2yJiG3OOeecY1x77bUN7rvooouMK6+80jAM1+1znZJzcyUlJYSFhdX/OTU1lVNOOQWbzVZ/3/jx48nIyKCoqMiMiK1adXU1q1atYty4cfX3Wa1Wxo0bR2pqqonJ2raSkhKA+n/bq1atoqampsHfQ69evYiPj9ffwwm65ZZbOOeccxrsW9A+by6ff/45Q4YM4dJLL6VDhw4MGjSIN954o/7rmZmZ5OfnN9jvwcHBDB8+XPu9iUaOHElKSgpbtmwBYN26dfz888+cffbZgOv2uekzfcuRbdu2jRdffJFnnnmm/r78/HwSExMbbHdwVvT8/HxCQ0NbNGNrt2/fPurq6ur34UFRUVGkp6eblKptczgc3HnnnYwaNap+hv78/HxsNtshC1pHRUWRn59vQsq2Yc6cOaxevZoVK1Yc8jXt8+axY8cOXn31VaZOncqDDz7IihUruP3227HZbEyePLl+3x7ue472e9Pcf//92O12evXqhYeHB3V1dTzxxBNceeWVAC7b5zrC1ALuv/9+LBbLUW9//HDOycnhrLPO4tJLL+X66683KbmI691yyy2kpaUxZ84cs6O0adnZ2dxxxx28//77DZaFkublcDg46aST+Mc//sGgQYO44YYb6tctlebx8ccf8/777/PBBx+wevVq3nnnHZ555hneeecdl76OjjC1gLvvvpspU6YcdZsuXbrU/z43N5fTTjuNkSNH1i8qfFB0dPQhV7Ec/HN0dLRrArcjEREReHh4HHafan+63q233sqCBQv46aef6NSpU/390dHRVFdXU1xc3OCIh/4emm7VqlXs2bOHk046qf6+uro6fvrpJ1566SW++eYb7fNmEBMTQ58+fRrc17t3bz755BPgf9+nCwoKiImJqd+moKCApKSkFsvZlvz1r3/l/vvv5/LLLwegf//+7Nq1ixkzZjB58mSX7XMdYWoBkZGR9OrV66i3g2OScnJyOPXUUxk8eDBvv/12g4WHAZKTk/npp5+oqampv2/RokX07NlTp+OawGazMXjwYFJSUurvczgcpKSkkJycbGKytsUwDG699VY+/fRTFi9efMhp5cGDB+Pl5dXg7yEjI4OsrCz9PTTR2LFj2bBhA2vXrq2/DRkyhCuvvLL+99rnrjdq1KhDpszYsmULnTt3BiAxMZHo6OgG+91ut7Ns2TLt9yYqLy8/5LPSw8MDh8MBuHCfu2SIurjE7t27jW7duhljx441du/ebeTl5dXfDiouLjaioqKMq666ykhLSzPmzJlj+Pn5aVqBEzBnzhzD29vbmD17trFp0ybjhhtuMEJCQoz8/Hyzo7UZN998sxEcHGz88MMPDf5dl5eX129z0003GfHx8cbixYuNlStXGsnJyUZycrKJqdue318lZxja581h+fLlhqenp/HEE08YW7duNd5//33Dz8/PeO+99+q3efLJJ42QkBDjs88+M9avX29ccMEFmlbgBEyePNno2LFj/bQC8+bNMyIiIox77723fhtX7HMVJjfy9ttvG8Bhb7+3bt06Y/To0Ya3t7fRsWNH48knnzQpcdvx4osvGvHx8YbNZjOGDRtm/Prrr2ZHalOO9O/67bffrt+moqLC+Mtf/mKEhoYafn5+xoUXXtjghwU5cX8sTNrnzeOLL74w+vXrZ3h7exu9evUyXn/99QZfdzgcxsMPP2xERUUZ3t7extixY42MjAyT0rZ+drvduOOOO4z4+HjDx8fH6NKli/G3v/2twfQ7rtjnFsP43VSYIiIiInIIjWESEREROQYVJhEREZFjUGESEREROQYVJhEREZFjUGESEREROQYVJhEREZFjUGESEREROQYVJhEREZFjUGESkXbr1FNP5c477wQgISGB5557ztQ8IuK+PM0OICLiDlasWIG/v7/ZMUTETakwiYgAkZGRZkcQETemU3IiIjQ8JffDDz9gs9lYsmRJ/deffvppOnToQEFBgUkJRcRMKkwiIn9wcGzTVVddRUlJCWvWrOHhhx/m3//+N1FRUWbHExETqDCJiBzG448/TmhoKDfccAN//vOfmTx5Mueff77ZsUTEJBrDJCJyGDabjffff58BAwbQuXNn/vWvf5kdSURMpCNMIiJHsHTpUgAKCwspLCw0OY2ImEmFSUTkMLZv385dd93FG2+8wfDhw5k8eTIOh8PsWCJiEhUmEZE/qKur489//jPjx4/nmmuu4e2332b9+vXMnDnT7GgiYhIVJhGRP3jiiSfYtWsXr732GgAxMTG8/vrrPPTQQ6xbt87kdCJiBothGIbZIURERETcmY4wiYiIiByDCpOIiIjIMagwiYiIiByDCpOIiIjIMagwiYiIiByDCpOIiIjIMagwiYiIiByDCpOIiIjIMagwiYiIiByDCpOIiIjIMagwiYiIiBzD/wNloMW3A2lR4wAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -659,15 +666,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "b40b3901be4435b5a71cc3915f22553724b83a304e297d25655c4809f01488a8"
             }
         }
```

### Comparing `dacy-2.5.1/docs/tutorials.md` & `dacy-2.5.2/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd` & `dacy-2.5.2/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/pyproject.toml` & `dacy-2.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dacy"
-version = "2.5.1"
+version = "2.5.2"
 description = "A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish"
 authors = [
   {name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}, 
   {name = "Lasse Hansen"},
   {name = "Emil Jessen"}
 ]
 
@@ -32,17 +32,17 @@
     "danish",
     "spacy-universe",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "spacy-wrap>=1.4.1,<1.5.0",
     "spacy>=3.2.0,<3.6.0",
-    "pandas>=1.0.0,<2.0.0",
+    "pandas>=1.0.0,<2.1.0",
     "wasabi>=0.8.2,<0.11.0",
-    "tqdm>=4.42.1,<4.65.0",
+    "tqdm>=4.42.1,<4.66.0",
     "sentencepiece>=0.1.96,<0.2.0",
 ]
 
 
 [project.urls]
 homepage = "https://centre-for-humanities-computing.github.io/DaCy/"
 documentation = "https://centre-for-humanities-computing.github.io/DaCy/"
@@ -50,29 +50,29 @@
 [project.license]
 file = "LICENSE"
 name = "Apache License 2.0"
 [project.optional-dependencies]
 dev = [
   "cruft",
   "mypy",  
-  "pre-commit==2.20.0,<2.21.0",
-  "ruff==0.0.254", # important that these match the pre-commit hooks
-  "black[jupyter]==22.8.0", # important that these match the pre-commit hooks
+  "pre-commit==2.20.0,<3.2.2",
+  "ruff==0.0.261", # important that these match the pre-commit hooks
+  "black[jupyter]==23.3.0", # important that these match the pre-commit hooks
 ]
 tests = [
-  "pytest>=7.1.2,<7.3.0",
+  "pytest>=7.1.2,<7.4.0",
   "pytest-cov>=3.0.0,<3.1.0",
-  "pytest-xdist>=3.0.0,<3.2.0",
-  "pytest-instafail>=0.4.2,<0.5.0",
+  "pytest-xdist>=3.0.0,<3.3.0",
+  "pytest-instafail>=0.4.2,<0.6.0",
 ]
 docs = [
     "sphinx>=5.3.0,<5.4.0",
     "furo>=2022.12.7,< 2022.12.8",  # theme
     "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.7.4",
+    "sphinxext-opengraph>=0.7.3,<0.8.2",
     "sphinx_design>=0.3.0,<0.3.1",
     "sphinx_togglebutton>=0.2.3,<0.4.0",
     "myst-nb>=0.6.0,<1.17.0",  # for rendering notebooks
     # for tutorials
     "jupyter>=1.0.0,<1.1.0",
     # sentiment analysis
     "asent>=0.4.2,<0.8.0",
```

### Comparing `dacy-2.5.1/src/dacy/datasets/dane.py` & `dacy-2.5.2/src/dacy/datasets/dane.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/datasets/lookup_tables/README.md` & `dacy-2.5.2/src/dacy/datasets/lookup_tables/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/datasets/lookup_tables/names.csv` & `dacy-2.5.2/src/dacy/datasets/lookup_tables/names.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/datasets/names.py` & `dacy-2.5.2/src/dacy/datasets/names.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/download.py` & `dacy-2.5.2/src/dacy/download.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/hate_speech/wrapped_models.py` & `dacy-2.5.2/src/dacy/hate_speech/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/load.py` & `dacy-2.5.2/src/dacy/load.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/ner/wrapped_models.py` & `dacy-2.5.2/src/dacy/ner/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/score/input_length.py` & `dacy-2.5.2/src/dacy/score/input_length.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/score/score.py` & `dacy-2.5.2/src/dacy/score/score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/sentiment/wrapped_models.py` & `dacy-2.5.2/src/dacy/sentiment/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy/utils.py` & `dacy-2.5.2/src/dacy/utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/src/dacy.egg-info/PKG-INFO` & `dacy-2.5.2/src/dacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.5.1
+Version: 2.5.2
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -232,15 +232,15 @@
 <a href="https://github.com/centre-for-humanities-computing/Dacy"><img src="https://github.com/centre-for-humanities-computing/DaCy/raw/main/docs/_static/icon_black_text.png" width="175" height="175" align="right" /></a>
 # DaCy: An efficient and unified framework for danish NLP
 
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-[![documentation](https://github.com/centre-for-humanities-computing/dacy/workflows/documentation/badge.svg)][documentation]
+[![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
 [![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
 
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
```

### Comparing `dacy-2.5.1/src/dacy.egg-info/SOURCES.txt` & `dacy-2.5.2/src/dacy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -156,15 +156,8 @@
 training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
 training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
 training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
 training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
 training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
 training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
 training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
-training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
-tutorials/dacy-basic.ipynb
-tutorials/dacy-robustness.ipynb
-tutorials/hate-speech.ipynb
-tutorials/requirements.txt
-tutorials/sentiment-neural.ipynb
-tutorials/sentiment-rule-based.ipynb
-tutorials/textdescriptives_integration.ipynb
+training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
```

### Comparing `dacy-2.5.1/src/dacy.egg-info/requires.txt` & `dacy-2.5.2/src/dacy.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 spacy-wrap<1.5.0,>=1.4.1
 spacy<3.6.0,>=3.2.0
-pandas<2.0.0,>=1.0.0
+pandas<2.1.0,>=1.0.0
 wasabi<0.11.0,>=0.8.2
-tqdm<4.65.0,>=4.42.1
+tqdm<4.66.0,>=4.42.1
 sentencepiece<0.2.0,>=0.1.96
 
 [dev]
 cruft
 mypy
-pre-commit<2.21.0,==2.20.0
-ruff==0.0.254
-black[jupyter]==22.8.0
+pre-commit<3.2.2,==2.20.0
+ruff==0.0.261
+black[jupyter]==23.3.0
 
 [docs]
 sphinx<5.4.0,>=5.3.0
 furo<2022.12.8,>=2022.12.7
 sphinx-copybutton<0.5.2,>=0.5.1
-sphinxext-opengraph<0.7.4,>=0.7.3
+sphinxext-opengraph<0.8.2,>=0.7.3
 sphinx_design<0.3.1,>=0.3.0
 sphinx_togglebutton<0.4.0,>=0.2.3
 myst-nb<1.17.0,>=0.6.0
 jupyter<1.1.0,>=1.0.0
 asent<0.8.0,>=0.4.2
 augmenty<1.4.0,>=1.0.2
 textdescriptives<3.0.0,>=2.1.0
 seaborn<0.13.0,>=0.11.2
 
 [tests]
-pytest<7.3.0,>=7.1.2
+pytest<7.4.0,>=7.1.2
 pytest-cov<3.1.0,>=3.0.0
-pytest-xdist<3.2.0,>=3.0.0
-pytest-instafail<0.5.0,>=0.4.2
+pytest-xdist<3.3.0,>=3.0.0
+pytest-instafail<0.6.0,>=0.4.2
```

### Comparing `dacy-2.5.1/tasks.py` & `dacy-2.5.2/tasks.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/tests/test_datasets.py` & `dacy-2.5.2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/tests/test_hate_speech.py` & `dacy-2.5.2/tests/test_hate_speech.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/tests/test_score.py` & `dacy-2.5.2/tests/test_score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/tests/test_sentiment.py` & `dacy-2.5.2/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/readme.md` & `dacy-2.5.2/training/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/configs/config_-l-ctra_small.cfg` & `dacy-2.5.2/training/v0.0.0/configs/config_-l-ctra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/configs/config_conv_small.cfg` & `dacy-2.5.2/training/v0.0.0/configs/config_conv_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/configs/config_electra_small.cfg` & `dacy-2.5.2/training/v0.0.0/configs/config_electra_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/configs/config_large.cfg` & `dacy-2.5.2/training/v0.0.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/configs/config_medium.cfg` & `dacy-2.5.2/training/v0.0.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/img/perf_training.png` & `dacy-2.5.2/training/v0.0.0/img/perf_training.png`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_cased.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_-l-ctra_cased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_-l-ctra_uncased.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_-l-ctra_uncased.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_conv_small.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_conv_small.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_electra.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_electra.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_large.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_large.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/metrics/dane_medium.json` & `dacy-2.5.2/training/v0.0.0/metrics/dane_medium.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/orth_variants.json` & `dacy-2.5.2/training/v0.0.0/orth_variants.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.0.0/project.yml` & `dacy-2.5.2/training/v0.0.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/augment.py` & `dacy-2.5.2/training/v0.1.0/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/configs/config_large.cfg` & `dacy-2.5.2/training/v0.1.0/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/configs/config_medium.cfg` & `dacy-2.5.2/training/v0.1.0/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/configs/config_small.cfg` & `dacy-2.5.2/training/v0.1.0/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/project.yml` & `dacy-2.5.2/training/v0.1.0/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.0/update_meta_json.py` & `dacy-2.5.2/training/v0.1.0/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/augment.py` & `dacy-2.5.2/training/v0.1.1/augment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/configs/config_large.cfg` & `dacy-2.5.2/training/v0.1.1/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/configs/config_medium.cfg` & `dacy-2.5.2/training/v0.1.1/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/configs/config_small.cfg` & `dacy-2.5.2/training/v0.1.1/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/danish_augmenter.py` & `dacy-2.5.2/training/v0.1.1/danish_augmenter.py`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json` & `dacy-2.5.2/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/project.yml` & `dacy-2.5.2/training/v0.1.1/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.5.1/training/v0.1.1/update_meta_json.py` & `dacy-2.5.2/training/v0.1.1/update_meta_json.py`

 * *Files identical despite different names*

