# Comparing `tmp/cobib-3.5.4.tar.gz` & `tmp/cobib-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-3.5.4.tar", last modified: Mon Dec 26 15:56:02 2022, max compression
+gzip compressed data, was "cobib-3.5.5.tar", last modified: Tue Apr 11 19:23:01 2023, max compression
```

## Comparing `cobib-3.5.4.tar` & `cobib-3.5.5.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.173466 cobib-3.5.4/
--rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-3.5.4/.coveragerc
--rw-r--r--   0 max       (1000) max       (1000)      240 2021-09-20 21:31:31.000000 cobib-3.5.4/.gitignore
--rw-r--r--   0 max       (1000) max       (1000)     2717 2022-12-13 20:07:48.000000 cobib-3.5.4/.gitlab-ci.yml
--rw-r--r--   0 max       (1000) max       (1000)       48 2021-09-20 21:31:31.000000 cobib-3.5.4/.pydocstylerc
--rw-r--r--   0 max       (1000) max       (1000)     1281 2022-11-16 20:11:10.000000 cobib-3.5.4/.pylintdict
--rw-r--r--   0 max       (1000) max       (1000)    11204 2022-06-03 21:13:52.000000 cobib-3.5.4/.pylintrc
--rw-r--r--   0 max       (1000) max       (1000)    25531 2022-12-26 15:53:53.000000 cobib-3.5.4/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     2259 2021-12-01 22:02:28.000000 cobib-3.5.4/CONTRIBUTING.md
--rw-r--r--   0 max       (1000) max       (1000)     1063 2022-01-13 20:47:42.000000 cobib-3.5.4/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      115 2021-09-20 21:31:31.000000 cobib-3.5.4/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      187 2021-09-20 21:31:31.000000 cobib-3.5.4/Makefile
--rw-r--r--   0 max       (1000) max       (1000)    34798 2022-12-26 15:56:02.173466 cobib-3.5.4/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     8437 2022-01-13 21:08:20.000000 cobib-3.5.4/README.md
--rw-r--r--   0 max       (1000) max       (1000)      563 2021-09-20 21:31:31.000000 cobib-3.5.4/_cobib
--rw-r--r--   0 max       (1000) max       (1000)    26588 2022-12-26 15:54:03.000000 cobib-3.5.4/cobib.1
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.133466 cobib-3.5.4/html/
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.4/html/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.4/html/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      558 2022-04-25 20:22:51.000000 cobib-3.5.4/html/index.html.jinja2
--rw-r--r--   0 max       (1000) max       (1000)      398 2022-04-25 20:43:18.000000 cobib-3.5.4/html/module.html.jinja2
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.136799 cobib-3.5.4/logo/
--rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_book-squared.png
--rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_book.png
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_byline.png
--rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_byline.svg
--rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_logo.png
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.4/logo/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      552 2021-12-01 20:44:34.000000 cobib-3.5.4/mypy.ini
--rw-r--r--   0 max       (1000) max       (1000)      328 2021-09-20 21:31:31.000000 cobib-3.5.4/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-3.5.4/pytest.ini
--rw-r--r--   0 max       (1000) max       (1000)       78 2021-12-01 20:44:34.000000 cobib-3.5.4/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)     1084 2022-12-26 15:56:02.176799 cobib-3.5.4/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-3.5.4/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.120133 cobib-3.5.4/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.136799 cobib-3.5.4/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2022-12-26 15:53:27.000000 cobib-3.5.4/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5477 2022-05-22 07:42:34.000000 cobib-3.5.4/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.143466 cobib-3.5.4/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)      899 2021-12-01 20:44:34.000000 cobib-3.5.4/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    13875 2022-11-16 20:02:48.000000 cobib-3.5.4/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     5643 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     3511 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7111 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     8061 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     5981 2021-12-01 20:44:34.000000 cobib-3.5.4/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4745 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)    14235 2021-10-04 21:00:16.000000 cobib-3.5.4/src/cobib/commands/list.py
--rw-r--r--   0 max       (1000) max       (1000)    17172 2021-10-12 20:39:32.000000 cobib-3.5.4/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)     8318 2021-12-01 21:10:29.000000 cobib-3.5.4/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     5322 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)     8601 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     3447 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     6053 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/commands/undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.143466 cobib-3.5.4/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-3.5.4/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    20453 2022-06-03 21:13:52.000000 cobib-3.5.4/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    27156 2022-04-25 18:46:40.000000 cobib-3.5.4/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)    11496 2021-12-01 20:52:02.000000 cobib-3.5.4/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.146799 cobib-3.5.4/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     9792 2022-06-03 21:13:52.000000 cobib-3.5.4/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    17270 2022-12-26 15:50:45.000000 cobib-3.5.4/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.146799 cobib-3.5.4/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-3.5.4/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      930 2021-12-01 20:44:34.000000 cobib-3.5.4/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    13035 2022-08-27 17:46:24.000000 cobib-3.5.4/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.150133 cobib-3.5.4/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-3.5.4/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5058 2022-01-13 20:47:42.000000 cobib-3.5.4/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     3078 2022-11-16 20:17:18.000000 cobib-3.5.4/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3272 2022-12-20 16:58:30.000000 cobib-3.5.4/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4590 2022-06-28 20:53:45.000000 cobib-3.5.4/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3554 2021-10-04 20:58:33.000000 cobib-3.5.4/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     2805 2022-04-25 18:48:18.000000 cobib-3.5.4/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.150133 cobib-3.5.4/src/cobib/tui/
--rw-r--r--   0 max       (1000) max       (1000)     1119 2021-11-17 16:26:13.000000 cobib-3.5.4/src/cobib/tui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    14586 2022-12-26 15:50:59.000000 cobib-3.5.4/src/cobib/tui/buffer.py
--rw-r--r--   0 max       (1000) max       (1000)    11317 2022-01-13 20:47:42.000000 cobib-3.5.4/src/cobib/tui/frame.py
--rw-r--r--   0 max       (1000) max       (1000)     3581 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/tui/state.py
--rw-r--r--   0 max       (1000) max       (1000)    29627 2022-01-13 20:47:42.000000 cobib-3.5.4/src/cobib/tui/tui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.153466 cobib-3.5.4/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     7761 2021-12-01 20:44:34.000000 cobib-3.5.4/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-3.5.4/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     5135 2022-04-25 19:41:11.000000 cobib-3.5.4/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-3.5.4/src/cobib/utils/rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)     7802 2021-09-26 19:17:19.000000 cobib-3.5.4/src/cobib/utils/shell_helper.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.140133 cobib-3.5.4/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    34798 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     4000 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       46 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       78 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2022-12-26 15:56:02.000000 cobib-3.5.4/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.153466 cobib-3.5.4/tests/
--rw-r--r--   0 max       (1000) max       (1000)     1508 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      809 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/cmdline_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.160133 cobib-3.5.4/tests/commands/
--rw-r--r--   0 max       (1000) max       (1000)       68 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5952 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/command_test.py
--rw-r--r--   0 max       (1000) max       (1000)      248 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/commands/example_duplicate_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      261 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/commands/example_duplicate_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      134 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/commands/example_multi_file_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      155 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/commands/example_multi_file_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)    21339 2022-11-16 20:31:43.000000 cobib-3.5.4/tests/commands/test_add.py
--rw-r--r--   0 max       (1000) max       (1000)     8332 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7982 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_edit.py
--rw-r--r--   0 max       (1000) max       (1000)    10071 2022-07-12 20:53:48.000000 cobib-3.5.4/tests/commands/test_export.py
--rw-r--r--   0 max       (1000) max       (1000)     2815 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_git_commit_event.py
--rw-r--r--   0 max       (1000) max       (1000)     2808 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_import.py
--rw-r--r--   0 max       (1000) max       (1000)     6024 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_init.py
--rw-r--r--   0 max       (1000) max       (1000)    14719 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_list.py
--rw-r--r--   0 max       (1000) max       (1000)    10799 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_modify.py
--rw-r--r--   0 max       (1000) max       (1000)    14411 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_open.py
--rw-r--r--   0 max       (1000) max       (1000)     9520 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_redo.py
--rw-r--r--   0 max       (1000) max       (1000)     9949 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_search.py
--rw-r--r--   0 max       (1000) max       (1000)     5663 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_show.py
--rw-r--r--   0 max       (1000) max       (1000)     9072 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/commands/test_undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.163466 cobib-3.5.4/tests/config/
--rw-r--r--   0 max       (1000) max       (1000)       28 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      119 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/config/broken_config.py
--rw-r--r--   0 max       (1000) max       (1000)    11310 2022-01-13 20:47:42.000000 cobib-3.5.4/tests/config/test_config.py
--rw-r--r--   0 max       (1000) max       (1000)     2420 2021-12-01 20:44:34.000000 cobib-3.5.4/tests/config/test_event.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.163466 cobib-3.5.4/tests/database/
--rw-r--r--   0 max       (1000) max       (1000)       30 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)       59 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/database/example_entry_umlaut.bib
--rw-r--r--   0 max       (1000) max       (1000)     8170 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/database/test_database.py
--rw-r--r--   0 max       (1000) max       (1000)    13859 2022-12-26 15:50:50.000000 cobib-3.5.4/tests/database/test_entry.py
--rw-r--r--   0 max       (1000) max       (1000)      444 2022-12-20 16:58:30.000000 cobib-3.5.4/tests/debug.py
--rw-r--r--   0 max       (1000) max       (1000)      651 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/example_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      621 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/example_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      723 2022-07-12 20:53:54.000000 cobib-3.5.4/tests/example_literature.bib
--rw-r--r--   0 max       (1000) max       (1000)      636 2022-12-26 15:48:38.000000 cobib-3.5.4/tests/example_literature.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.163466 cobib-3.5.4/tests/importers/
--rw-r--r--   0 max       (1000) max       (1000)       71 2021-12-01 20:44:34.000000 cobib-3.5.4/tests/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      274 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/importers/importer_test.py
--rw-r--r--   0 max       (1000) max       (1000)     4543 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/importers/test_zotero.py
--rw-r--r--   0 max       (1000) max       (1000)     2609 2021-12-01 20:44:34.000000 cobib-3.5.4/tests/importers/zotero_database.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.166799 cobib-3.5.4/tests/parsers/
--rw-r--r--   0 max       (1000) max       (1000)       65 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1395 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/parsers/parser_test.py
--rw-r--r--   0 max       (1000) max       (1000)     5767 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/parsers/test_arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     3224 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/parsers/test_bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     5017 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/parsers/test_doi.py
--rw-r--r--   0 max       (1000) max       (1000)     5566 2022-06-28 20:53:45.000000 cobib-3.5.4/tests/parsers/test_isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     4399 2022-11-16 20:47:00.000000 cobib-3.5.4/tests/parsers/test_url.py
--rw-r--r--   0 max       (1000) max       (1000)     3251 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/parsers/test_yaml.py
--rw-r--r--   0 max       (1000) max       (1000)     4573 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/test_main.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.170133 cobib-3.5.4/tests/tui/
--rw-r--r--   0 max       (1000) max       (1000)      125 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/tui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4444 2021-11-17 16:25:08.000000 cobib-3.5.4/tests/tui/mock_curses.py
--rw-r--r--   0 max       (1000) max       (1000)     1176 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/tui/mock_tui.py
--rw-r--r--   0 max       (1000) max       (1000)     1134 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/tui/scrolling_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)    19852 2022-12-26 15:50:59.000000 cobib-3.5.4/tests/tui/test_buffer.py
--rw-r--r--   0 max       (1000) max       (1000)    22582 2022-12-26 15:46:45.000000 cobib-3.5.4/tests/tui/test_frame.py
--rw-r--r--   0 max       (1000) max       (1000)     2420 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/tui/test_state.py
--rw-r--r--   0 max       (1000) max       (1000)    41277 2022-09-29 20:29:54.000000 cobib-3.5.4/tests/tui/test_tui.py
--rw-r--r--   0 max       (1000) max       (1000)     8505 2021-12-01 20:44:34.000000 cobib-3.5.4/tests/tui/tui_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-12-26 15:56:02.173466 cobib-3.5.4/tests/utils/
--rw-r--r--   0 max       (1000) max       (1000)       29 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      712 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/utils/expected_changelog_printing.txt
--rw-r--r--   0 max       (1000) max       (1000)      172 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/utils/fixed_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)      163 2021-09-25 23:38:02.000000 cobib-3.5.4/tests/utils/linting_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     9133 2022-08-27 18:09:45.000000 cobib-3.5.4/tests/utils/test_file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     3216 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/utils/test_journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     3135 2022-04-25 19:44:59.000000 cobib-3.5.4/tests/utils/test_logging.py
--rw-r--r--   0 max       (1000) max       (1000)      964 2021-09-20 21:31:31.000000 cobib-3.5.4/tests/utils/test_rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)    13561 2022-06-03 21:13:52.000000 cobib-3.5.4/tests/utils/test_shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)     1909 2021-10-12 20:39:32.000000 cobib-3.5.4/tests/utils/unified_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1907 2021-10-12 20:39:32.000000 cobib-3.5.4/tests/utils/unifying_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1565 2022-12-12 22:11:20.000000 cobib-3.5.4/tox.ini
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.059836 cobib-3.5.5/
+-rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-3.5.5/.coveragerc
+-rw-r--r--   0 max       (1000) max       (1000)      240 2021-09-20 21:31:31.000000 cobib-3.5.5/.gitignore
+-rw-r--r--   0 max       (1000) max       (1000)     2717 2022-12-13 20:07:48.000000 cobib-3.5.5/.gitlab-ci.yml
+-rw-r--r--   0 max       (1000) max       (1000)       48 2021-09-20 21:31:31.000000 cobib-3.5.5/.pydocstylerc
+-rw-r--r--   0 max       (1000) max       (1000)     1281 2022-11-16 20:11:10.000000 cobib-3.5.5/.pylintdict
+-rw-r--r--   0 max       (1000) max       (1000)    11213 2023-02-05 08:34:43.000000 cobib-3.5.5/.pylintrc
+-rw-r--r--   0 max       (1000) max       (1000)    25714 2023-04-11 19:21:05.000000 cobib-3.5.5/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     2259 2021-12-01 22:02:28.000000 cobib-3.5.5/CONTRIBUTING.md
+-rw-r--r--   0 max       (1000) max       (1000)     1063 2022-01-13 20:47:42.000000 cobib-3.5.5/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      115 2021-09-20 21:31:31.000000 cobib-3.5.5/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)      187 2021-09-20 21:31:31.000000 cobib-3.5.5/Makefile
+-rw-r--r--   0 max       (1000) max       (1000)    34981 2023-04-11 19:23:01.059836 cobib-3.5.5/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     8437 2022-01-13 21:08:20.000000 cobib-3.5.5/README.md
+-rw-r--r--   0 max       (1000) max       (1000)      563 2021-09-20 21:31:31.000000 cobib-3.5.5/_cobib
+-rw-r--r--   0 max       (1000) max       (1000)    26588 2023-04-11 19:20:32.000000 cobib-3.5.5/cobib.1
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.023169 cobib-3.5.5/html/
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.5/html/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.5/html/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      558 2022-04-25 20:22:51.000000 cobib-3.5.5/html/index.html.jinja2
+-rw-r--r--   0 max       (1000) max       (1000)      398 2022-04-25 20:43:18.000000 cobib-3.5.5/html/module.html.jinja2
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.026502 cobib-3.5.5/logo/
+-rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book-squared.png
+-rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book.png
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_byline.png
+-rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_byline.svg
+-rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_logo.png
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      552 2021-12-01 20:44:34.000000 cobib-3.5.5/mypy.ini
+-rw-r--r--   0 max       (1000) max       (1000)      328 2021-09-20 21:31:31.000000 cobib-3.5.5/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-3.5.5/pytest.ini
+-rw-r--r--   0 max       (1000) max       (1000)       78 2021-12-01 20:44:34.000000 cobib-3.5.5/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1084 2023-04-11 19:23:01.063169 cobib-3.5.5/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-3.5.5/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.016502 cobib-3.5.5/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.026502 cobib-3.5.5/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2023-04-11 19:20:12.000000 cobib-3.5.5/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5477 2022-05-22 07:42:34.000000 cobib-3.5.5/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)      899 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    13875 2022-11-16 20:02:48.000000 cobib-3.5.5/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     5643 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     3511 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     7111 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     8061 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     5981 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4745 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)    14235 2021-10-04 21:00:16.000000 cobib-3.5.5/src/cobib/commands/list.py
+-rw-r--r--   0 max       (1000) max       (1000)    17172 2021-10-12 20:39:32.000000 cobib-3.5.5/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)     8418 2023-04-11 19:15:41.000000 cobib-3.5.5/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     5322 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)     8601 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     3447 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     6053 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    20453 2023-04-06 21:46:11.000000 cobib-3.5.5/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    27156 2022-04-25 18:46:40.000000 cobib-3.5.5/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)    11521 2023-01-30 19:18:43.000000 cobib-3.5.5/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     9792 2022-06-03 21:13:52.000000 cobib-3.5.5/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    17270 2022-12-26 15:50:45.000000 cobib-3.5.5/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      930 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    13035 2022-08-27 17:46:24.000000 cobib-3.5.5/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-3.5.5/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5058 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     3078 2022-11-16 20:17:18.000000 cobib-3.5.5/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3272 2022-12-20 16:58:30.000000 cobib-3.5.5/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4590 2022-06-28 20:53:45.000000 cobib-3.5.5/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3553 2023-02-05 08:34:32.000000 cobib-3.5.5/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     2805 2022-04-25 18:48:18.000000 cobib-3.5.5/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/tui/
+-rw-r--r--   0 max       (1000) max       (1000)     1119 2021-11-17 16:26:13.000000 cobib-3.5.5/src/cobib/tui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    14586 2022-12-26 15:50:59.000000 cobib-3.5.5/src/cobib/tui/buffer.py
+-rw-r--r--   0 max       (1000) max       (1000)    11317 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/tui/frame.py
+-rw-r--r--   0 max       (1000) max       (1000)     3581 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/tui/state.py
+-rw-r--r--   0 max       (1000) max       (1000)    29627 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/tui/tui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.039836 cobib-3.5.5/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     7761 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-3.5.5/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     5135 2022-04-25 19:41:11.000000 cobib-3.5.5/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/utils/rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)     7802 2021-09-26 19:17:19.000000 cobib-3.5.5/src/cobib/utils/shell_helper.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.029836 cobib-3.5.5/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    34981 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     4000 2023-04-11 19:23:01.000000 cobib-3.5.5/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       46 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       78 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.039836 cobib-3.5.5/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     1508 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      809 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/cmdline_test.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.049836 cobib-3.5.5/tests/commands/
+-rw-r--r--   0 max       (1000) max       (1000)       68 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5950 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/command_test.py
+-rw-r--r--   0 max       (1000) max       (1000)      248 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_duplicate_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      261 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_duplicate_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      134 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_multi_file_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      155 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_multi_file_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)    21339 2022-11-16 20:31:43.000000 cobib-3.5.5/tests/commands/test_add.py
+-rw-r--r--   0 max       (1000) max       (1000)     8332 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     7982 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_edit.py
+-rw-r--r--   0 max       (1000) max       (1000)    10071 2022-07-12 20:53:48.000000 cobib-3.5.5/tests/commands/test_export.py
+-rw-r--r--   0 max       (1000) max       (1000)     2815 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_git_commit_event.py
+-rw-r--r--   0 max       (1000) max       (1000)     2806 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_import.py
+-rw-r--r--   0 max       (1000) max       (1000)     6024 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_init.py
+-rw-r--r--   0 max       (1000) max       (1000)    14719 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_list.py
+-rw-r--r--   0 max       (1000) max       (1000)    10799 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    16138 2023-04-11 19:15:46.000000 cobib-3.5.5/tests/commands/test_open.py
+-rw-r--r--   0 max       (1000) max       (1000)     9514 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_redo.py
+-rw-r--r--   0 max       (1000) max       (1000)     9949 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_search.py
+-rw-r--r--   0 max       (1000) max       (1000)     5663 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_show.py
+-rw-r--r--   0 max       (1000) max       (1000)     9066 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.049836 cobib-3.5.5/tests/config/
+-rw-r--r--   0 max       (1000) max       (1000)       28 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      119 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/config/broken_config.py
+-rw-r--r--   0 max       (1000) max       (1000)    11310 2022-01-13 20:47:42.000000 cobib-3.5.5/tests/config/test_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     2420 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/config/test_event.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.053169 cobib-3.5.5/tests/database/
+-rw-r--r--   0 max       (1000) max       (1000)       30 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)       59 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/database/example_entry_umlaut.bib
+-rw-r--r--   0 max       (1000) max       (1000)     8168 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/database/test_database.py
+-rw-r--r--   0 max       (1000) max       (1000)    13859 2022-12-26 15:50:50.000000 cobib-3.5.5/tests/database/test_entry.py
+-rw-r--r--   0 max       (1000) max       (1000)      444 2022-12-20 16:58:30.000000 cobib-3.5.5/tests/debug.py
+-rw-r--r--   0 max       (1000) max       (1000)      651 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/example_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      621 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/example_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      723 2022-07-12 20:53:54.000000 cobib-3.5.5/tests/example_literature.bib
+-rw-r--r--   0 max       (1000) max       (1000)      636 2023-04-06 21:46:08.000000 cobib-3.5.5/tests/example_literature.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.053169 cobib-3.5.5/tests/importers/
+-rw-r--r--   0 max       (1000) max       (1000)       71 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      274 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/importers/importer_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     4541 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/importers/test_zotero.py
+-rw-r--r--   0 max       (1000) max       (1000)     2609 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/importers/zotero_database.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.056502 cobib-3.5.5/tests/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)       65 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1395 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/parser_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     5767 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     3224 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     5017 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     5566 2022-06-28 20:53:45.000000 cobib-3.5.5/tests/parsers/test_isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     4399 2022-11-16 20:47:00.000000 cobib-3.5.5/tests/parsers/test_url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3251 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)     4573 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.056502 cobib-3.5.5/tests/tui/
+-rw-r--r--   0 max       (1000) max       (1000)      125 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4444 2021-11-17 16:25:08.000000 cobib-3.5.5/tests/tui/mock_curses.py
+-rw-r--r--   0 max       (1000) max       (1000)     1176 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/mock_tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     1134 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/scrolling_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)    19852 2022-12-26 15:50:59.000000 cobib-3.5.5/tests/tui/test_buffer.py
+-rw-r--r--   0 max       (1000) max       (1000)    22582 2022-12-26 15:46:45.000000 cobib-3.5.5/tests/tui/test_frame.py
+-rw-r--r--   0 max       (1000) max       (1000)     2420 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/test_state.py
+-rw-r--r--   0 max       (1000) max       (1000)    41277 2022-09-29 20:29:54.000000 cobib-3.5.5/tests/tui/test_tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     8505 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/tui/tui_test.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.059836 cobib-3.5.5/tests/utils/
+-rw-r--r--   0 max       (1000) max       (1000)       29 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      712 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/expected_changelog_printing.txt
+-rw-r--r--   0 max       (1000) max       (1000)      172 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/fixed_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      163 2021-09-25 23:38:02.000000 cobib-3.5.5/tests/utils/linting_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     9133 2022-08-27 18:09:45.000000 cobib-3.5.5/tests/utils/test_file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3216 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/test_journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     3135 2022-04-25 19:44:59.000000 cobib-3.5.5/tests/utils/test_logging.py
+-rw-r--r--   0 max       (1000) max       (1000)      964 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/test_rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)    13561 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/utils/test_shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)     1909 2021-10-12 20:39:32.000000 cobib-3.5.5/tests/utils/unified_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1907 2021-10-12 20:39:32.000000 cobib-3.5.5/tests/utils/unifying_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1567 2023-01-22 12:13:09.000000 cobib-3.5.5/tox.ini
```

### Comparing `cobib-3.5.4/.gitlab-ci.yml` & `cobib-3.5.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/.pylintdict` & `cobib-3.5.5/.pylintdict`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/.pylintrc` & `cobib-3.5.5/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -349,8 +349,8 @@
 analyse-fallback-blocks=no
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `cobib-3.5.4/CHANGELOG.md` & `cobib-3.5.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.5.5] - 2023-04-11
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### Fixed
+- opening of non-list type fields (#100)
+
 
 ## [3.5.4] - 2022-12-26
 
 Pypi: https://pypi.org/project/cobib/3.5.4/
 
 ### Fixed
 - missing files encountered during searching will log warnings gracefully instead of harshly
@@ -639,15 +646,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4...master
+[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
+[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
 [3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
 [3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
```

### Comparing `cobib-3.5.4/CONTRIBUTING.md` & `cobib-3.5.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/LICENSE.txt` & `cobib-3.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/PKG-INFO` & `cobib-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 3.5.4
+Version: 3.5.5
 Summary: Console Bibliography
 Home-page: https://gitlab.com/mrossinek/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/mrossinek/cobib/-/issues
 Project-URL: Documentation, https://mrossinek.gitlab.io/cobib/cobib.html
@@ -294,14 +294,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.5.5] - 2023-04-11
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### Fixed
+- opening of non-list type fields (#100)
+
 
 ## [3.5.4] - 2022-12-26
 
 Pypi: https://pypi.org/project/cobib/3.5.4/
 
 ### Fixed
 - missing files encountered during searching will log warnings gracefully instead of harshly
@@ -931,15 +938,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4...master
+[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
+[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
 [3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
 [3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
```

### Comparing `cobib-3.5.4/README.md` & `cobib-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/_cobib` & `cobib-3.5.5/_cobib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/cobib.1` & `cobib-3.5.5/cobib.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2022-12-26 v3.5.4
+.TH COBIB 1 2023-04-11 v3.5.5
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
```

### Comparing `cobib-3.5.4/html/cobib_book.svg` & `cobib-3.5.5/html/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/html/cobib_logo.svg` & `cobib-3.5.5/html/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/html/index.html.jinja2` & `cobib-3.5.5/html/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_book-squared.png` & `cobib-3.5.5/logo/cobib_book-squared.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_book.png` & `cobib-3.5.5/logo/cobib_book.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_book.svg` & `cobib-3.5.5/logo/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_byline.png` & `cobib-3.5.5/logo/cobib_byline.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_byline.svg` & `cobib-3.5.5/logo/cobib_byline.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_logo.png` & `cobib-3.5.5/logo/cobib_logo.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/logo/cobib_logo.svg` & `cobib-3.5.5/logo/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/mypy.ini` & `cobib-3.5.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/setup.cfg` & `cobib-3.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/__main__.py` & `cobib-3.5.5/src/cobib/__main__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/__init__.py` & `cobib-3.5.5/src/cobib/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/add.py` & `cobib-3.5.5/src/cobib/commands/add.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/base_command.py` & `cobib-3.5.5/src/cobib/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/delete.py` & `cobib-3.5.5/src/cobib/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/edit.py` & `cobib-3.5.5/src/cobib/commands/edit.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/export.py` & `cobib-3.5.5/src/cobib/commands/export.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/import_.py` & `cobib-3.5.5/src/cobib/commands/import_.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/init.py` & `cobib-3.5.5/src/cobib/commands/init.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/list.py` & `cobib-3.5.5/src/cobib/commands/list.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/modify.py` & `cobib-3.5.5/src/cobib/commands/modify.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/open.py` & `cobib-3.5.5/src/cobib/commands/open.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,16 @@
             count = 0
             # first: find all possible things to open
             try:
                 entry = bib[label]
                 for field in config.commands.open.fields:
                     if field in entry.data.keys() and entry.data[field]:
                         value = entry.data[field]
+                        if not isinstance(value, list):
+                            value = [value]
                         for val in value:
                             val = val.strip()
                             LOGGER.debug('Parsing "%s" for URLs.', val)
                             things_to_open[field] += [urlparse(val)]
                             count += 1
             except KeyError:
                 msg = f"No entry with the label '{label}' could be found."
```

### Comparing `cobib-3.5.4/src/cobib/commands/redo.py` & `cobib-3.5.5/src/cobib/commands/redo.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/search.py` & `cobib-3.5.5/src/cobib/commands/search.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/show.py` & `cobib-3.5.5/src/cobib/commands/show.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/commands/undo.py` & `cobib-3.5.5/src/cobib/commands/undo.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/config/__init__.py` & `cobib-3.5.5/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/config/config.py` & `cobib-3.5.5/src/cobib/config/config.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/config/event.py` & `cobib-3.5.5/src/cobib/config/event.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/config/example.py` & `cobib-3.5.5/src/cobib/config/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,17 @@
 # DATABASE.FORMAT
 # You can also specify some aspects about the format of the database.
 
 # You can specify a default label format which will be used for the database entry keys. The format
 # of this option follows the f-string like formatting of modifications (see also the documentation
 # of the [ModifyCommand](https://mrossinek.gitlab.io/cobib/cobib/commands/modify.html)). The default
 # configuration value leaves the label unchanged compared to the metadata provided by the source
-# from which the entry gets added. A more useful example is `"{author.split()[1]}{year}"` which
-# takes the surname of the first author and immediately appends the publication year.
+# from which the entry gets added. A more useful example is
+#     `"{author.split(' and ')[0].split()[-1]}{year}"`
+# which takes the surname of the first author and immediately appends the publication year.
 config.database.format.label_default = "{label}"
 
 # You can specify the suffix format which is used to disambiguate labels if a conflict would occur.
 # This option takes a tuple of length 2, where the first entry is the string separating the proposed
 # label from the enumerator and the second one is one of the enumerators provided in the
 # `config.LabelSuffix` object. The available enumerators are:
 #   - ALPHA: a, b, ...
```

### Comparing `cobib-3.5.4/src/cobib/database/database.py` & `cobib-3.5.5/src/cobib/database/database.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/database/entry.py` & `cobib-3.5.5/src/cobib/database/entry.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/importers/base_importer.py` & `cobib-3.5.5/src/cobib/importers/base_importer.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/importers/zotero.py` & `cobib-3.5.5/src/cobib/importers/zotero.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/__init__.py` & `cobib-3.5.5/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/arxiv.py` & `cobib-3.5.5/src/cobib/parsers/arxiv.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/base_parser.py` & `cobib-3.5.5/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/bibtex.py` & `cobib-3.5.5/src/cobib/parsers/bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/doi.py` & `cobib-3.5.5/src/cobib/parsers/doi.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/isbn.py` & `cobib-3.5.5/src/cobib/parsers/isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/parsers/url.py` & `cobib-3.5.5/src/cobib/parsers/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         # we assume the most common DOI on the page is the one which we are looking for
         most_common_doi = dois.most_common(1)[0]
         LOGGER.debug("Most common DOI is: %s", most_common_doi)
         if most_common_doi[1] > 1:
             entries = DOIParser().parse(most_common_doi[0])
 
         if entries:
-
             Event.PostURLParse.fire(entries)
 
             LOGGER.debug("Successfully extracted metadata from most common DOI")
             return entries
 
         LOGGER.error("Could not extract metadata from URL: %s", string)
         return OrderedDict()
```

### Comparing `cobib-3.5.4/src/cobib/parsers/yaml.py` & `cobib-3.5.5/src/cobib/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/tui/__init__.py` & `cobib-3.5.5/src/cobib/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/tui/buffer.py` & `cobib-3.5.5/src/cobib/tui/buffer.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/tui/frame.py` & `cobib-3.5.5/src/cobib/tui/frame.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/tui/state.py` & `cobib-3.5.5/src/cobib/tui/state.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/tui/tui.py` & `cobib-3.5.5/src/cobib/tui/tui.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/utils/file_downloader.py` & `cobib-3.5.5/src/cobib/utils/file_downloader.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/utils/journal_abbreviations.py` & `cobib-3.5.5/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/utils/logging.py` & `cobib-3.5.5/src/cobib/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/utils/rel_path.py` & `cobib-3.5.5/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib/utils/shell_helper.py` & `cobib-3.5.5/src/cobib/utils/shell_helper.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/src/cobib.egg-info/PKG-INFO` & `cobib-3.5.5/src/cobib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 3.5.4
+Version: 3.5.5
 Summary: Console Bibliography
 Home-page: https://gitlab.com/mrossinek/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/mrossinek/cobib/-/issues
 Project-URL: Documentation, https://mrossinek.gitlab.io/cobib/cobib.html
@@ -294,14 +294,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.5.5] - 2023-04-11
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### Fixed
+- opening of non-list type fields (#100)
+
 
 ## [3.5.4] - 2022-12-26
 
 Pypi: https://pypi.org/project/cobib/3.5.4/
 
 ### Fixed
 - missing files encountered during searching will log warnings gracefully instead of harshly
@@ -931,15 +938,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4...master
+[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
+[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
 [3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
 [3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
```

### Comparing `cobib-3.5.4/src/cobib.egg-info/SOURCES.txt` & `cobib-3.5.5/src/cobib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/__init__.py` & `cobib-3.5.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/cmdline_test.py` & `cobib-3.5.5/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/command_test.py` & `cobib-3.5.5/tests/commands/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         Args:
             caplog: the built-in pytest fixture.
         """
         command_cls = self.get_command()
         command_cls().execute(["--dummy"])
         name = command_cls.name
         safe_name = self.get_safe_command_name()
-        for (source, level, message) in caplog.record_tuples:
+        for source, level, message in caplog.record_tuples:
             if (f"cobib.commands.{safe_name}", logging.ERROR) == (
                 source,
                 level,
             ) and f"Error: {name}: error:" in message:
                 break
         else:
             pytest.fail("No Error logged from ArgumentParser.")
```

### Comparing `cobib-3.5.4/tests/commands/test_add.py` & `cobib-3.5.5/tests/commands/test_add.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_delete.py` & `cobib-3.5.5/tests/commands/test_delete.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_edit.py` & `cobib-3.5.5/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_export.py` & `cobib-3.5.5/tests/commands/test_export.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_git_commit_event.py` & `cobib-3.5.5/tests/commands/test_git_commit_event.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_import.py` & `cobib-3.5.5/tests/commands/test_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         """Test the TUI access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
         """
 
         def assertion(screen, logs, **kwargs):  # type: ignore
-            for (source, level, message) in logs:
+            for source, level, message in logs:
                 if ("cobib.tui.tui", logging.INFO) == (
                     source,
                     level,
                 ) and "sys.stderr contains:usage: import [-h] [--skip-download]" in message:
                     break
             else:
                 pytest.fail("No help message logged to sys.stderr.")
```

### Comparing `cobib-3.5.4/tests/commands/test_init.py` & `cobib-3.5.5/tests/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_list.py` & `cobib-3.5.5/tests/commands/test_list.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_modify.py` & `cobib-3.5.5/tests/commands/test_modify.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_open.py` & `cobib-3.5.5/tests/commands/test_open.py`

 * *Files 10% similar despite different names*

```diff
@@ -256,14 +256,65 @@
             "  2: [note] " + self.TMP_FILE_B,
             "Entry to open [Type 'help' for more info]: ",
         ]
 
         for line, truth in zip(true_out, expected_out):
             assert line == truth
 
+    def test_open_non_list_field(
+        self,
+        setup: Any,
+        monkeypatch: pytest.MonkeyPatch,
+        caplog: pytest.LogCaptureFixture,
+    ) -> None:
+        """Test opening of non-list type fields.
+
+        This is a regression test against https://gitlab.com/mrossinek/cobib/-/issues/100
+
+        Args:
+            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            monkeypatch: the built-in pytest fixture.
+            caplog: the built-in pytest fixture.
+        """
+        config.commands.open.fields = ["note"]
+
+        with open(
+            get_resource("example_multi_file_entry.yaml", "commands"), "r", encoding="utf-8"
+        ) as multi_file_entry:
+            with open(config.database.file, "a", encoding="utf-8") as database:
+                for line in multi_file_entry.readlines():
+                    if line == "  file:\n":
+                        database.write("  note: /tmp/a.txt\n")
+                        database.write("...\n")
+                        break
+                    database.write(line)
+
+        Database().read()
+
+        monkeypatch.setattr("sys.stdin", MockStdin())
+
+        OpenCommand().execute(["example_multi_file_entry"])
+
+        true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.open"]
+
+        expected_log = [
+            ("cobib.commands.open", 10, "Starting Open command."),
+            (
+                "cobib.commands.open",
+                10,
+                'Parsing "/tmp/a.txt" for URLs.',
+            ),
+            (
+                "cobib.commands.open",
+                10,
+                'Opening "/tmp/a.txt" with cat.',
+            ),
+        ]
+        assert true_log == expected_log
+
     @pytest.mark.parametrize(
         ["post_setup"],
         [
             [{"multi_file": False}],
         ],
         indirect=["post_setup"],
     )
```

### Comparing `cobib-3.5.4/tests/commands/test_redo.py` & `cobib-3.5.5/tests/commands/test_redo.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,28 @@
             expected_exit: whether to expect an early exit.
             caplog: the built-in pytest fixture.
         """
         git = setup.get("git", False)
 
         if not git:
             RedoCommand().execute([])
-            for (source, level, message) in caplog.record_tuples:
+            for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.redo", logging.ERROR) == (
                     source,
                     level,
                 ) and "git-tracking" in message:
                     break
             else:
                 pytest.fail("No Error logged from RedoCommand.")
         elif expected_exit:
             # Regression test against #65
             AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
             with pytest.raises(SystemExit):
                 RedoCommand().execute([])
-            for (source, level, message) in caplog.record_tuples:
+            for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.redo", logging.WARNING) == (
                     source,
                     level,
                 ) and "Could not find a commit to redo." in message:
                     break
             else:
                 pytest.fail("No Error logged from UndoCommand.")
@@ -144,15 +144,15 @@
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         rmtree(self.COBIB_TEST_DIR_GIT)
         RedoCommand().execute([])
-        for (source, level, message) in caplog.record_tuples:
+        for source, level, message in caplog.record_tuples:
             if ("cobib.commands.redo", logging.ERROR) == (
                 source,
                 level,
             ) and "configured, but not initialized" in message:
                 break
         else:
             pytest.fail("No Error logged from RedoCommand.")
```

### Comparing `cobib-3.5.4/tests/commands/test_search.py` & `cobib-3.5.5/tests/commands/test_search.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_show.py` & `cobib-3.5.5/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/commands/test_undo.py` & `cobib-3.5.5/tests/commands/test_undo.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,27 @@
             expected_exit: whether to expect an early exit.
             caplog: the built-in pytest fixture.
         """
         git = setup.get("git", False)
 
         if not git:
             UndoCommand().execute([])
-            for (source, level, message) in caplog.record_tuples:
+            for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.undo", logging.ERROR) == (
                     source,
                     level,
                 ) and "git-tracking" in message:
                     break
             else:
                 pytest.fail("No Error logged from UndoCommand.")
         elif expected_exit:
             # Regression test related to #65
             with pytest.raises(SystemExit):
                 UndoCommand().execute([])
-            for (source, level, message) in caplog.record_tuples:
+            for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.undo", logging.WARNING) == (
                     source,
                     level,
                 ) and "Could not find a commit to undo." in message:
                     break
             else:
                 pytest.fail("No Error logged from UndoCommand.")
@@ -136,15 +136,15 @@
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         rmtree(self.COBIB_TEST_DIR_GIT)
         UndoCommand().execute([])
-        for (source, level, message) in caplog.record_tuples:
+        for source, level, message in caplog.record_tuples:
             if ("cobib.commands.undo", logging.ERROR) == (
                 source,
                 level,
             ) and "configured, but not initialized" in message:
                 break
         else:
             pytest.fail("No Error logged from UndoCommand.")
```

### Comparing `cobib-3.5.4/tests/config/test_config.py` & `cobib-3.5.5/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/config/test_event.py` & `cobib-3.5.5/tests/config/test_event.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/database/test_database.py` & `cobib-3.5.5/tests/database/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     Args:
         caplog: the built-in pytest fixture.
     """
     config.database.file = TMPDIR / "cobib_test_missing_file.yaml"
     try:
         with pytest.raises(SystemExit):
             Database().read()
-        for (source, level, message) in caplog.record_tuples:
+        for source, level, message in caplog.record_tuples:
             if ("cobib.database.database", logging.CRITICAL) == (
                 source,
                 level,
             ) and f"The database file {config.database.file} does not exist!" in message:
                 break
         else:
             pytest.fail("coBib did not exit upon encountering a missing database file!")
```

### Comparing `cobib-3.5.4/tests/database/test_entry.py` & `cobib-3.5.5/tests/database/test_entry.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/example_entry.bib` & `cobib-3.5.5/tests/example_entry.bib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/example_entry.yaml` & `cobib-3.5.5/tests/example_entry.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/example_literature.bib` & `cobib-3.5.5/tests/example_literature.bib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/example_literature.yaml` & `cobib-3.5.5/tests/example_literature.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/importers/test_zotero.py` & `cobib-3.5.5/tests/importers/test_zotero.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test handling of ArgumentError.
 
         Args:
             caplog: the built-in pytest fixture.
         """
         ZoteroImporter().fetch(["--dummy"])
-        for (source, level, message) in caplog.record_tuples:
+        for source, level, message in caplog.record_tuples:
             if ("cobib.importers.zotero", logging.ERROR) == (
                 source,
                 level,
             ) and "Error: zotero: error:" in message:
                 break
         else:
             pytest.fail("No Error logged from ArgumentParser.")
```

### Comparing `cobib-3.5.4/tests/importers/zotero_database.yaml` & `cobib-3.5.5/tests/importers/zotero_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/parser_test.py` & `cobib-3.5.5/tests/parsers/parser_test.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_arxiv.py` & `cobib-3.5.5/tests/parsers/test_arxiv.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_bibtex.py` & `cobib-3.5.5/tests/parsers/test_bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_doi.py` & `cobib-3.5.5/tests/parsers/test_doi.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_isbn.py` & `cobib-3.5.5/tests/parsers/test_isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_url.py` & `cobib-3.5.5/tests/parsers/test_url.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/parsers/test_yaml.py` & `cobib-3.5.5/tests/parsers/test_yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/test_main.py` & `cobib-3.5.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/mock_curses.py` & `cobib-3.5.5/tests/tui/mock_curses.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/mock_tui.py` & `cobib-3.5.5/tests/tui/mock_tui.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/scrolling_database.yaml` & `cobib-3.5.5/tests/tui/scrolling_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/test_buffer.py` & `cobib-3.5.5/tests/tui/test_buffer.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/test_frame.py` & `cobib-3.5.5/tests/tui/test_frame.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/test_state.py` & `cobib-3.5.5/tests/tui/test_state.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/test_tui.py` & `cobib-3.5.5/tests/tui/test_tui.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/tui/tui_test.py` & `cobib-3.5.5/tests/tui/tui_test.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/expected_changelog_printing.txt` & `cobib-3.5.5/tests/utils/expected_changelog_printing.txt`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/test_file_downloader.py` & `cobib-3.5.5/tests/utils/test_file_downloader.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/test_journal_abbreviations.py` & `cobib-3.5.5/tests/utils/test_journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/test_logging.py` & `cobib-3.5.5/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/test_rel_path.py` & `cobib-3.5.5/tests/utils/test_rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/test_shell_helper.py` & `cobib-3.5.5/tests/utils/test_shell_helper.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/unified_database.yaml` & `cobib-3.5.5/tests/utils/unified_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tests/utils/unifying_database.yaml` & `cobib-3.5.5/tests/utils/unifying_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.4/tox.ini` & `cobib-3.5.5/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [testenv:coverage]
 usedevelop = true
 basepython = python3
 changedir = {toxinidir}
 deps =
     {[testenv]deps}
-    coverage
+    coverage<7
     pytest-cov
 commands =
     pytest --cov --cov-config={toxinidir}/.coveragerc tests/
     coverage xml
     coverage html
 
 [testenv:lint]
```

