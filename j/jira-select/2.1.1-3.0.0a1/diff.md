# Comparing `tmp/jira-select-2.1.1.tar.gz` & `tmp/jira-select-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-select-2.1.1.tar", last modified: Sun Mar  5 05:13:48 2023, max compression
+gzip compressed data, was "jira-select-3.0.0a1.tar", last modified: Tue Apr 11 05:39:48 2023, max compression
```

## Comparing `jira-select-2.1.1.tar` & `jira-select-3.0.0a1.tar`

### file list

```diff
@@ -1,72 +1,81 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.275647 jira-select-2.1.1/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3962 2023-03-05 05:13:48.275647 jira-select-2.1.1/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.267647 jira-select-2.1.1/jira_select/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-03-05 04:05:11.000000 jira-select-2.1.1/jira_select/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/__main__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/cache.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4214 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/cmdline.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.267647 jira-select-2.1.1/jira_select/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/build_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/configure.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4234 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/install_user_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/remove_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3922 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/commands/run.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/run_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3932 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/schema.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/setup_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6873 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/shell.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1550 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/show_instances.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/commands/store_password.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/exceptions.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.267647 jira-select-2.1.1/jira_select/formatters/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/formatters/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      902 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/formatters/csv.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/formatters/html.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      666 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/formatters/json.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-2.1.1/jira_select/formatters/table.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.271647 jira-select-2.1.1/jira_select/functions/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/estimate_to_days.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/extract.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/field_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1900 2023-02-28 20:50:06.000000 jira-select-2.1.1/jira_select/functions/flatten_changelog.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/flatten_list.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/get_sprint_by_id.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/get_sprint_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1283 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/functions/json_dumps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/functions/parse_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/parse_datetime.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      590 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/simple_filter.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/simple_filter_any.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/sprint_details.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/functions/sprint_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3247 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/functions/workdays_in_state.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     9468 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/plugin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    18886 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/query.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.271647 jira-select-2.1.1/jira_select/sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-2.1.1/jira_select/sources/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/sources/boards.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3397 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/sources/issues.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/sources/sprints.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1866 2023-03-05 02:42:01.000000 jira-select-2.1.1/jira_select/types.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     8468 2023-03-04 07:50:34.000000 jira-select-2.1.1/jira_select/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.267647 jira-select-2.1.1/jira_select.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3962 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1979 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2061 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-2.1.1/jira_select.egg-info/not-zip-safe
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      375 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-03-05 05:13:48.000000 jira-select-2.1.1/jira_select.egg-info/top_level.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-03-05 05:13:48.275647 jira-select-2.1.1/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5047 2023-03-05 04:05:11.000000 jira-select-2.1.1/setup.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-03-05 05:13:48.275647 jira-select-2.1.1/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-2.1.1/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-2.1.1/tests/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-2.1.1/tests/conftest.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10306 2022-05-20 02:53:24.000000 jira-select-2.1.1/tests/test_functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13214 2023-03-04 07:50:34.000000 jira-select-2.1.1/tests/test_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6865 2022-05-20 02:53:24.000000 jira-select-2.1.1/tests/test_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       25 2023-04-11 05:39:25.000000 jira-select-3.0.0a1/jira_select/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/__main__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/cache.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.0a1/jira_select/cmdline.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/build_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/configure.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/install_user_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/remove_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.0a1/jira_select/commands/run.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/run_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/schema.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/setup_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/commands/shell.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/show_instances.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/store_password.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/exceptions.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/formatters/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/formatters/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/formatters/csv.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/formatters/html.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.0a1/jira_select/formatters/json.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      381 2023-04-11 05:13:38.000000 jira-select-3.0.0a1/jira_select/formatters/raw.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.0a1/jira_select/formatters/table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/formatters/tsv.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/jira_select/functions/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.0a1/jira_select/functions/estimate_to_days.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/extract.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/field_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/functions/flatten_changelog.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/flatten_list.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.0a1/jira_select/functions/get_issue.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3602 2023-04-11 03:48:08.000000 jira-select-3.0.0a1/jira_select/functions/get_issue_snapshot_on_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/get_sprint_by_id.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/get_sprint_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.0a1/jira_select/functions/interval_business_hours.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1125 2023-04-10 23:10:31.000000 jira-select-3.0.0a1/jira_select/functions/interval_matching.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.0a1/jira_select/functions/interval_size.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.0a1/jira_select/functions/json_dumps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/functions/parse_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/parse_datetime.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/functions/simple_filter.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/simple_filter_any.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/sprint_details.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/sprint_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1506 2023-04-10 03:30:19.000000 jira-select-3.0.0a1/jira_select/functions/subquery.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.0a1/jira_select/functions/union.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.0a1/jira_select/functions/workdays_in_state.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     9642 2023-04-10 03:28:45.000000 jira-select-3.0.0a1/jira_select/plugin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20521 2023-04-11 05:00:17.000000 jira-select-3.0.0a1/jira_select/query.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/jira_select/sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/sources/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/sources/boards.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3865 2023-04-10 23:39:17.000000 jira-select-3.0.0a1/jira_select/sources/issues.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/sources/sprints.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2176 2023-04-11 05:19:20.000000 jira-select-3.0.0a1/jira_select/types.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10219 2023-04-11 04:51:08.000000 jira-select-3.0.0a1/jira_select/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2322 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.0a1/jira_select.egg-info/not-zip-safe
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      395 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/top_level.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5718 2023-04-11 05:39:25.000000 jira-select-3.0.0a1/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/conftest.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.0a1/tests/test_functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.0a1/tests/test_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.0a1/tests/test_utils.py
```

### Comparing `jira-select-2.1.1/PKG-INFO` & `jira-select-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 2.1.1
+Version: 3.0.0a1
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
@@ -94,16 +94,16 @@
 ```
 
 Now, you can type out your query -- the below will find issues assigned
 to you:
 
 ```yaml
 select:
-  - key
-  - summary
+ Issue Key: key
+ Issue Summary: summary
 from: issues
 where:
   - assignee = "your-email@somecompany.com"
   - resolution is null
 ```
 
 The editor uses `vi` bindings by default; so once you're ready to submit
```

### Comparing `jira-select-2.1.1/jira_select/cache.py` & `jira-select-3.0.0a1/jira_select/cache.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/cmdline.py` & `jira-select-3.0.0a1/jira_select/cmdline.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import sys
 from typing import Any
 from typing import Dict
 from typing import Iterable
 
 from rich.console import Console
-from rich.traceback import install as enable_rich_traceback
+from rich.logging import RichHandler
 from safdie import SafdieRunner
 
 from .constants import COMMAND_ENTRYPOINT
 from .exceptions import UserError
 from .plugin import BaseCommand
 from .utils import get_config
 from .utils import get_default_config_path
@@ -88,45 +88,56 @@
         )
         parser.add_argument(
             "--log-level",
             help=(
                 "Print logging messages of the specified level and above "
                 "to the console."
             ),
+            default="INFO",
         )
         return super().add_arguments(parser)
 
     def handle(
         self,
         args: argparse.Namespace,
         init_args: Iterable[Any],
         init_kwargs: Dict[str, Any],
         handle_args: Iterable[Any],
         handle_kwargs: Dict[str, Any],
     ) -> Any:
-        if args.log_level:
-            logging.basicConfig(level=logging.getLevelName(args.log_level))
+        console = Console()
+        logging.basicConfig(
+            level=logging.getLevelName(args.log_level),
+            format="%(message)s",
+            datefmt="[%X]",
+            handlers=[RichHandler(rich_tracebacks=True, console=Console(stderr=True))],
+        )
 
         if args.debugger:
             import debugpy
 
-            debugpy.listen(("0.0.0.0", 5678))
+            debugger_host = "0.0.0.0"
+            debugger_port = 5678
+
+            debugpy.listen((debugger_host, debugger_port))
+
+            console.print(
+                f"[magenta]Waiting for debugger connection on {debugger_host}:{debugger_port}[/magenta]..."
+            )
 
             # Pause the program until a remote debugger is attached
             debugpy.wait_for_client()
 
         config = get_config(path=args.config)
 
         init_kwargs["config"] = config
         return super().handle(args, init_args, init_kwargs, handle_args, handle_kwargs)
 
 
 def main():
-    enable_rich_traceback()
-
     console = Console()
 
     try:
         Runner(COMMAND_ENTRYPOINT, cmd_class=BaseCommand).run()
     except UserError as e:
         console.print(f"[red]{e}[/red]")
         sys.exit(1)
```

### Comparing `jira-select-2.1.1/jira_select/commands/build_query.py` & `jira-select-3.0.0a1/jira_select/commands/build_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/commands/configure.py` & `jira-select-3.0.0a1/jira_select/commands/configure.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/commands/functions.py` & `jira-select-3.0.0a1/jira_select/commands/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 
 from rich.table import Table
 
 from ..plugin import BaseCommand
 from ..plugin import BaseFunction
 from ..plugin import get_installed_functions
+from ..utils import JiraSelectJsonEncoder
 from ..utils import evaluate_expression
 
 
 class Command(BaseCommand):
     @classmethod
     def get_help(cls) -> str:
         return "Lists all available functions, their signatures, and description."
@@ -72,15 +73,19 @@
                         continue
                 if self.options.having:
                     if not evaluate_expression(self.options.having, row, functions):
                         continue
 
                 function_data.append(row)
             function_data.sort(key=lambda row: row["name"])
-            self.console.print(json.dumps(function_data, sort_keys=True, indent=4))
+            self.console.print(
+                json.dumps(
+                    function_data, cls=JiraSelectJsonEncoder, sort_keys=True, indent=4
+                )
+            )
         else:
             table = Table(title="functions")
             table.add_column(header="name", style="green")
             table.add_column(header="description", style="white")
 
             all_functions = []
             for name, fn in functions.items():
```

### Comparing `jira-select-2.1.1/jira_select/commands/install_user_script.py` & `jira-select-3.0.0a1/jira_select/commands/install_user_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/commands/run.py` & `jira-select-3.0.0a1/jira_select/commands/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,24 +70,32 @@
             "-p",
             dest="parameters",
             action="append",
             type=parameter_tuple,
         )
         parser.add_argument(
             "--no-cache",
-            "-n",
-            default=False,
-            action="store_true",
+            "-c",
+            default=True,
+            action="store_false",
             help="Do not use cached data.",
-            dest="no_cache",
+            dest="cache",
+        )
+        parser.add_argument(
+            "--disable-progressbars",
+            "-b",
+            default=True,
+            action="store_false",
+            help="",
+            dest="progressbar",
         )
 
     @classmethod
     def get_help(cls) -> str:
-        return "Interactively generates a query definition (in yaml format)."
+        return "Runs a query definition specified in yaml format."
 
     def handle(self) -> None:
         if self.options.view and self.options.output is sys.stdout:
             raise UserError("Must specify --output to use --view.")
 
         viewer: Optional[str] = self.config.inline_viewers.get(
             self.options.format, DEFAULT_INLINE_VIEWERS.get(self.options.format)
@@ -97,17 +105,19 @@
 
         query_definition: QueryDefinition
         query_definition = QueryDefinition.parse_obj(safe_load(self.options.query_file))
 
         query = Executor(
             self.jira,
             query_definition,
-            progress_bar=self.options.output is not sys.stdout,
+            progress_bar=(self.options.output is not sys.stdout.buffer)
+            if self.options.progressbar
+            else False,
             parameters=dict(self.options.parameters or []),
-            enable_cache=not self.options.no_cache,
+            enable_cache=self.options.cache,
         )
         with formatter_cls(query, self.options.output) as formatter:
             for row in query:
                 formatter.writerow(row)
                 self.options.output.flush()
 
         if self.options.view and self.options.launch_default_viewer:
```

### Comparing `jira-select-2.1.1/jira_select/commands/run_script.py` & `jira-select-3.0.0a1/jira_select/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/commands/schema.py` & `jira-select-3.0.0a1/jira_select/commands/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from rich.table import Table
 
 from ..exceptions import JiraSelectError
 from ..plugin import BaseCommand
 from ..plugin import get_installed_functions
 from ..plugin import get_installed_sources
+from ..utils import JiraSelectJsonEncoder
 from ..utils import evaluate_expression
 
 
 class Command(BaseCommand):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.functions: Dict[str, Callable] = get_installed_functions(self.jira)
@@ -84,15 +85,17 @@
                 fields.append(
                     {
                         "id": row.id,
                         "type": row.type,
                         "description": row.description,
                     }
                 )
-            self.console.print(json.dumps(fields, sort_keys=True, indent=4))
+            self.console.print(
+                json.dumps(fields, cls=JiraSelectJsonEncoder, sort_keys=True, indent=4)
+            )
         else:
             table = Table(title=self.options.source)
             table.add_column(header="id", style="green")
             table.add_column(header="type", style="cyan")
             table.add_column(header="description", style="bright_cyan")
 
             for row in source.get_schema(self.jira):
```

### Comparing `jira-select-2.1.1/jira_select/commands/setup_instance.py` & `jira-select-3.0.0a1/jira_select/commands/setup_instance.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/commands/shell.py` & `jira-select-3.0.0a1/jira_select/commands/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             "--editor-mode",
             "-m",
             choices=["emacs", "vi"],
             default=None,
         )
         parser.add_argument(
             "--disable-progressbars",
+            "-b",
             action="store_false",
             default=True,
             dest="enable_progressbars",
         )
         parser.add_argument(
             "--output",
             "-o",
```

### Comparing `jira-select-2.1.1/jira_select/commands/show_instances.py` & `jira-select-3.0.0a1/jira_select/commands/show_instances.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import json
 
 from rich.table import Table
 
 from ..plugin import BaseCommand
+from ..utils import JiraSelectJsonEncoder
 
 
 class Command(BaseCommand):
     @classmethod
     def get_help(cls) -> str:
         return (
             "Displays Jira instances that you have configured jira-select "
@@ -31,15 +32,19 @@
                 instances.append(
                     {
                         "name": instance_name,
                         "username": instance_data.username,
                         "url": instance_data.url,
                     }
                 )
-            self.console.print(json.dumps(instances, sort_keys=True, indent=4))
+            self.console.print(
+                json.dumps(
+                    instances, cls=JiraSelectJsonEncoder, sort_keys=True, indent=4
+                )
+            )
         else:
             table = Table(title="Configured Instances")
             table.add_column("name", style="green")
             table.add_column("username", style="cyan")
             table.add_column("url", style="bright_cyan")
 
             for instance_name, instance_data in self.config.instances.items():
```

### Comparing `jira-select-2.1.1/jira_select/commands/store_password.py` & `jira-select-3.0.0a1/jira_select/commands/store_password.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/formatters/csv.py` & `jira-select-3.0.0a1/jira_select/formatters/csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Dict
 from typing import List
 
 from ..plugin import BaseFormatter
 
 
 class Formatter(BaseFormatter):
+    delimiter = ","
+
     @classmethod
     def get_file_extension(cls) -> str:
         return "csv"
 
     def _generate_fieldnames(self) -> List[str]:
         fields = []
 
@@ -22,15 +24,17 @@
 
     def open(self):
         super().open()
         self._wrapped_stream = TextIOWrapper(
             self.stream, encoding="utf-8", write_through=True, newline=""
         )
         self.out = csv.DictWriter(
-            self._wrapped_stream, fieldnames=self._generate_fieldnames()
+            self._wrapped_stream,
+            fieldnames=self._generate_fieldnames(),
+            delimiter=self.delimiter,
         )
         self.out.writeheader()
 
     def close(self):
         self._wrapped_stream.detach()
 
     def writerow(self, row: Dict[str, Any]):
```

### Comparing `jira-select-2.1.1/jira_select/formatters/html.py` & `jira-select-3.0.0a1/jira_select/formatters/html.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/formatters/json.py` & `jira-select-3.0.0a1/jira_select/formatters/json.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from io import TextIOWrapper
 from typing import Any
 from typing import Dict
 from typing import List
 
 from ..plugin import BaseFormatter
+from ..utils import JiraSelectJsonEncoder
 
 
 class Formatter(BaseFormatter):
     _rows: List[Dict] = []
 
     @classmethod
     def get_file_extension(cls) -> str:
@@ -16,13 +17,13 @@
 
     def open(self):
         super().open()
         self._rows = []
 
     def close(self):
         wrapped = TextIOWrapper(self.stream, encoding="utf-8", write_through=True)
-        json.dump(self._rows, wrapped, sort_keys=True, indent=4, default=str)
+        json.dump(self._rows, wrapped, cls=JiraSelectJsonEncoder, indent=4)
         wrapped.detach()
         super().close()
 
     def writerow(self, row: Dict[str, Any]):
         self._rows.append(row)
```

### Comparing `jira-select-2.1.1/jira_select/formatters/table.py` & `jira-select-3.0.0a1/jira_select/formatters/table.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/estimate_to_days.py` & `jira-select-3.0.0a1/jira_select/functions/estimate_to_days.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/extract.py` & `jira-select-3.0.0a1/jira_select/functions/extract.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/field_by_name.py` & `jira-select-3.0.0a1/jira_select/functions/field_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/flatten_changelog.py` & `jira-select-3.0.0a1/jira_select/functions/flatten_changelog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 import datetime
 from dataclasses import dataclass
 from typing import Any
+from typing import Iterator
 from typing import List
 from typing import Optional
 
 from dateutil.parser import parse as parse_date
 
 from ..exceptions import UserError
 from ..plugin import BaseFunction
 
 
 @dataclass
 class ChangelogEntry:
     author: str = ""
-    created: Optional[datetime.datetime] = None
+    created: datetime.datetime = datetime.datetime.utcnow()
     id: int = -1
     field: str = ""
     fieldtype: str = ""
     fromValue: Optional[Any] = None
     fromString: Optional[str] = None
     toValue: Optional[Any] = None
     toString: Optional[str] = None
 
 
+def flatten_changelog(changelog: Any) -> Iterator[ChangelogEntry]:
+    for entry in changelog.histories:
+        author = str(entry.author)
+        created = parse_date(entry.created)
+        id = int(entry.id)
+
+        for item in entry.items:
+            yield ChangelogEntry(
+                author=author,
+                created=created,
+                id=id,
+                field=item.field,
+                fieldtype=item.fieldtype,
+                fromValue=getattr(item, "from"),  # noqa
+                fromString=item.fromString,
+                toValue=getattr(item, "to"),  # noqa
+                toString=item.toString,
+            )
+
+
 class Function(BaseFunction):
     """Returns a flattened list of changelog entries.
 
 
     Returns ``jira_select.functions.flatten_changelog.ChangelogEntry``
     entries for every changelog entry.
     """
@@ -34,30 +55,8 @@
     def __call__(self, changelog: Any) -> List[ChangelogEntry]:  # type: ignore[override]
         if changelog is None or not hasattr(changelog, "histories"):
             raise UserError(
                 "No changelog was provided; did you use the ``expand`` "
                 "option of ``changelog`` in your query?"
             )
 
-        flattened: List[ChangelogEntry] = []
-
-        for entry in changelog.histories:
-            author = str(entry.author)
-            created = parse_date(entry.created)
-            id = int(entry.id)
-
-            for item in entry.items:
-                flattened.append(
-                    ChangelogEntry(
-                        author=author,
-                        created=created,
-                        id=id,
-                        field=item.field,
-                        fieldtype=item.fieldtype,
-                        fromValue=getattr(item, "from"),  # noqa
-                        fromString=item.fromString,
-                        toValue=getattr(item, "to"),  # noqa
-                        toString=item.toString,
-                    )
-                )
-
-        return flattened
+        return list(flatten_changelog(changelog))
```

### Comparing `jira-select-2.1.1/jira_select/functions/get_sprint_by_id.py` & `jira-select-3.0.0a1/jira_select/functions/get_sprint_by_id.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/get_sprint_by_name.py` & `jira-select-3.0.0a1/jira_select/functions/get_sprint_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/parse_date.py` & `jira-select-3.0.0a1/jira_select/functions/parse_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/parse_datetime.py` & `jira-select-3.0.0a1/jira_select/functions/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/simple_filter.py` & `jira-select-3.0.0a1/jira_select/functions/simple_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 from typing import Iterable
 
 from QueryableList import QueryableListMixed
 
 from ..plugin import BaseFunction
 
 
+def simple_filter(iterable: Iterable[Any], **query: Dict[str, Any]) -> Iterable[Any]:
+    queryable = QueryableListMixed(iterable)
+
+    return queryable.filter(**query)
+
+
 class Function(BaseFunction):
     """Returns entries in an iterable matching a provided django-style query.
 
     Returned rows are required to match at least all of the provided query
     parameters.
 
     """
 
     def __call__(  # type: ignore[override]
         self, iterable: Iterable[Any], **query: Dict[str, Any]
     ) -> Iterable[Any]:
-        queryable = QueryableListMixed(iterable)
-
-        return queryable.filter(**query)
+        return simple_filter(iterable, **query)
```

### Comparing `jira-select-2.1.1/jira_select/functions/simple_filter_any.py` & `jira-select-3.0.0a1/jira_select/functions/simple_filter_any.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/sprint_details.py` & `jira-select-3.0.0a1/jira_select/functions/sprint_details.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/functions/workdays_in_state.py` & `jira-select-3.0.0a1/jira_select/functions/workdays_in_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import datetime
 from typing import Any
-from typing import List
+from typing import Iterable
 from typing import Optional
+from warnings import warn
 
 from dateutil.tz import tzlocal
 from pytz import UTC
 from pytz import timezone
 
 from jira_select.plugin import BaseFunction
 
-from .flatten_changelog import Function as FlattenChangelog
+from .flatten_changelog import flatten_changelog
 
 
 class Function(BaseFunction):
     """Count the fractional number of work days an issue was in a given state."""
 
     def __call__(  # type: ignore[override]
         self,
         changelog: Any,
         state: str,
         start_hour: Optional[int] = 9,
         end_hour: Optional[int] = 17,
         timezone_name: Optional[str] = None,
-        work_days: List[int] = [1, 2, 3, 4, 5],
+        work_days: Iterable[int] = (1, 2, 3, 4, 5),
         min_date: datetime.date = datetime.date(1, 1, 1),
         max_date: datetime.date = datetime.date(9999, 1, 1),
-    ):
+    ) -> float:
+        warn(
+            "The `workdays_in_state` function is deprecated; see `interval_business_hours` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         tz = timezone(timezone_name) if timezone_name is not None else tzlocal()
 
         flattened_changelog = sorted(
-            FlattenChangelog(self.jira)(changelog),
+            flatten_changelog(changelog),
             key=lambda row: row.created if row.created else datetime.date(1, 1, 1),
         )
 
         total_time = datetime.timedelta()
 
         cursor = min_date
         while cursor < max_date:
```

### Comparing `jira-select-2.1.1/jira_select/plugin.py` & `jira-select-3.0.0a1/jira_select/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,15 +219,17 @@
 
 
 def register_function(fn: Callable):
     """Register a callable to be a function available in queries."""
     REGISTERED_FUNCTIONS[fn.__name__] = fn
 
 
-def get_installed_functions(jira: JIRA = None) -> Dict[str, Callable]:
+def get_installed_functions(
+    jira: JIRA = None, query: Query = None
+) -> Dict[str, Callable]:
     possible_commands: Dict[str, Callable] = copy.copy(BUILTIN_FUNCTIONS)
 
     # Import any modules in the custom functions directory; as a
     # side-effect of this, the functions will become listed within
     # REGISTERED_FUNCTIONS
     function_dir = get_custom_function_dir()
     for dirname, subdirlist, filelist in os.walk(function_dir):
@@ -254,22 +256,27 @@
                     spec.loader.exec_module(user_module)  # type: ignore
                 except Exception as e:
                     logger.error("Could not import user script at %s: %s", full_path, e)
 
     possible_commands.update(REGISTERED_FUNCTIONS)
 
     for fn_name, fn in get_entrypoints(FUNCTION_ENTRYPOINT, BaseFunction).items():
-        possible_commands[fn_name] = fn(jira)
+        possible_commands[fn_name] = fn(jira, query=query)
 
     return possible_commands
 
 
 class BaseFunction(metaclass=ABCMeta):
-    def __init__(self, jira: Optional[JIRA]):
+    def __init__(self, jira: Optional[JIRA], query: Optional[Query]):
         self._jira = jira
+        self._query = query
+
+    @property
+    def query(self) -> Optional[Query]:
+        return self._query
 
     @property
     def jira(self):
         assert self._jira
 
         return self._jira
```

### Comparing `jira-select-2.1.1/jira_select/query.py` & `jira-select-3.0.0a1/jira_select/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Generator
 from typing import Iterable
 from typing import Iterator
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 from typing import cast
 
 from dotmap import DotMap
 from jira import JIRA
-from jira import Issue
 from rich.progress import BarColumn
 from rich.progress import Progress
 from rich.progress import TaskID
 from rich.progress import TimeRemainingColumn
 
 from .cache import MinimumRecencyCache
 from .exceptions import ExpressionParameterMissing
 from .plugin import BaseSource
 from .plugin import get_installed_functions
 from .plugin import get_installed_sources
 from .types import Expression
 from .types import ExpressionList
+from .types import Field
 from .types import JqlList
 from .types import QueryDefinition
 from .types import SelectFieldDefinition
 from .types import WhereParamDict
 from .utils import calculate_result_hash
 from .utils import expression_includes_group_by
 from .utils import find_missing_parameters
@@ -125,17 +126,21 @@
             interpolations=field_name_map,
         )
 
 
 class SingleResult(Result):
     def __init__(self, row: Any):
         self._row = row
+        self._overlay: dict[str, Any] = {}
+
+    def __setitem__(self, name, value):
+        self._overlay[name] = value
 
     def as_dict(self) -> Dict[str, Any]:
-        return get_row_dict(self._row)
+        return get_row_dict(self._row, self._overlay)
 
     def single(self) -> SingleResult:
         return self
 
 
 class GroupedFieldContainer(list):
     def __getattr__(self, name):
@@ -208,31 +213,61 @@
         try:
             source = sources[self.from_]
         except KeyError:
             return []
 
         return source.get_all_fields(self._jira)
 
-    @property
-    def select(self) -> List[SelectFieldDefinition]:
+    def _get_select_calculate_fields(
+        self, field_data: List[Field] | Mapping[str, str | None]
+    ) -> List[SelectFieldDefinition]:
         fields: List[SelectFieldDefinition] = []
 
-        for field in self._definition.select:
+        if isinstance(field_data, str):
+            field = field_data
             if field == "*":
                 fields.extend(self._get_all_fields())
             else:
                 fields.append(parse_select_definition(field))
+        if isinstance(field_data, dict):
+            for column, expression in field_data.items():
+                fields.append(
+                    SelectFieldDefinition(
+                        expression=expression if expression else column, column=column
+                    )
+                )
+        elif isinstance(field_data, list):
+            for field in field_data:
+                if field == "*":
+                    fields.extend(self._get_all_fields())
+                else:
+                    fields.append(parse_select_definition(field))
 
         return fields
 
     @property
+    def select(self) -> List[SelectFieldDefinition]:
+        return self._get_select_calculate_fields(self._definition.select)
+
+    @property
+    def calculate(self) -> List[SelectFieldDefinition]:
+        return self._get_select_calculate_fields(self._definition.calculate)
+
+    @property
     def from_(self) -> str:
         return self._definition.from_
 
     @property
+    def subqueries(self) -> dict[str, "QueryDefinition"]:
+        return {
+            subquery_name: QueryDefinition.parse_obj(subquery_value)
+            for subquery_name, subquery_value in self._definition.subqueries.items()
+        }
+
+    @property
     def where(self) -> Union[JqlList, WhereParamDict]:
         where = self._definition.where
         if isinstance(where, list):
             return self._ensure_str(where)
         return where
 
     @property
@@ -326,26 +361,27 @@
 class Executor:
     def __init__(
         self,
         jira: JIRA,
         definition: QueryDefinition,
         enable_cache: bool = True,
         progress_bar: bool = False,
-        parameters: Optional[Dict[str, str]] = None,
+        parameters: Optional[Dict[str, Any]] = None,
     ):
         self._query: Query = Query(jira, definition)
-        # self._definition: QueryDefinition = clean_query_definition(definition)
         self._jira: JIRA = jira
-        self._functions: Dict[str, Callable] = get_installed_functions(jira)
+        self._functions: Dict[str, Callable] = get_installed_functions(
+            jira, self._query
+        )
         self._progress_bar_enabled = progress_bar
 
         self._cache = MinimumRecencyCache(get_cache_path())
 
         self._enable_cache = enable_cache
-        self._parameters: Dict[str, str] = parameters or {}
+        self._parameters: Dict[str, Any] = parameters or {}
         self._field_name_map: Dict[str, str] = FieldNameMap()
 
     @property
     def jira(self) -> JIRA:
         return self._jira
 
     @property
@@ -357,41 +393,27 @@
         return self._query
 
     @property
     def functions(self) -> Dict[str, Callable]:
         return self._functions
 
     @property
+    def parameters(self) -> Dict[str, Any]:
+        return self._parameters
+
+    @property
     def field_name_map(self) -> Dict[str, Any]:
         if not self._field_name_map:
             for jira_field in self.jira.fields():
                 self._field_name_map[jira_field["name"]] = jira_field["id"]
 
             self._field_name_map["params"] = DotMap(self._parameters)
 
         return self._field_name_map
 
-    def _get_jql(self) -> str:
-        query = " AND ".join(f"({q})" for q in self.query.where)
-
-        if missing := find_missing_parameters(query, list(self._parameters.keys())):
-            raise ExpressionParameterMissing(
-                "Parameter {params.%s} found in expression, but no parameter was specified!"
-                % missing[0]
-            )
-
-        query = query.format(params=DotMap(self._parameters))
-
-        order_by_fields = ", ".join(self.query.order_by)
-
-        if order_by_fields:
-            query = f"{query} ORDER BY {order_by_fields}"
-
-        return query
-
     def _get_cached(self, source: BaseSource) -> Iterator[Result]:
         cache_key = ":".join(
             [
                 str(self.jira.client_info()),
                 str(self.query.from_),
                 str(self.query.where),
                 str(self.query.order_by),
@@ -408,15 +430,15 @@
                 cached_results = self.cache.get(cache_key, min_recency=min_recency)
                 if not cached_results:
                     raise KeyError(cache_key)
 
                 source.update_count(len(cached_results))
                 source.remove_progress()
                 for result in cached_results:
-                    yield SingleResult(Issue({}, None, result))
+                    yield SingleResult(source.rehydrate(result))
                 return
             except KeyError:
                 pass
 
         cache = []
 
         for result in source:
@@ -424,14 +446,34 @@
             yield SingleResult(source.rehydrate(result))
 
         if self.query.cache:
             _, max_store = self.query.cache
             if max_store is not None:
                 self.cache.set(cache_key, cache, expire=max_store)
 
+    def _process_calculate(
+        self,
+        iterator: Iterator[Result],
+        task: TaskID,
+        input_channel: CounterChannel,
+        output_channel: CounterChannel,
+    ) -> Iterator[Result]:
+        for row in iterator:
+            output_channel.set(input_channel.get())
+            self.progress.update(task, total=input_channel.get(), visible=True)
+
+            for definition in self.query.calculate:
+                row[definition.column] = self.evaluate_expression(
+                    row, definition.expression
+                )
+
+            yield row
+
+            self.progress.update(task, advance=1)
+
     def _process_filter(
         self,
         iterator: Iterator[Result],
         task: TaskID,
         input_channel: CounterChannel,
         output_channel: CounterChannel,
     ) -> Iterator[Result]:
@@ -564,14 +606,17 @@
                         CounterChannel,
                     ],
                     Iterator[Result],
                 ],
                 TaskID,
             ]
         ] = []
+        if self.query.calculate:
+            calculate_task = self.progress.add_task("calculate", total=0, visible=False)
+            phases.append((self._process_calculate, calculate_task))
         if self.query.filter:
             filter_task = self.progress.add_task("filter", total=0, visible=False)
             phases.append(
                 (
                     self._process_filter,
                     filter_task,
                 ),
```

### Comparing `jira-select-2.1.1/jira_select/sources/boards.py` & `jira-select-3.0.0a1/jira_select/sources/boards.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/sources/issues.py` & `jira-select-3.0.0a1/jira_select/sources/issues.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from typing import List
 
 from dotmap import DotMap
 from jira import JIRA
 from jira.resources import Issue
 from simpleeval import NameNotDefined
 
+from ..exceptions import ExpressionParameterMissing
 from ..exceptions import QueryError
 from ..plugin import BaseSource
 from ..plugin import get_installed_functions
 from ..types import SchemaRow
 from ..utils import evaluate_expression
+from ..utils import find_missing_parameters
 
 
 class Source(BaseSource):
     SCHEMA: List[SchemaRow] = [
         SchemaRow.parse_obj({"id": "key", "type": "str"}),
         SchemaRow.parse_obj({"id": "id", "type": "int"}),
     ]
@@ -61,14 +63,25 @@
             raise QueryError(
                 "Issue queries 'where' should be a list of JQL expression strings."
             )
 
         assert isinstance(self.query.where, list)
 
         query = " AND ".join(f"({q})" for q in self.query.where)
+
+        if missing := find_missing_parameters(
+            query, list(self._executor.parameters.keys())
+        ):
+            raise ExpressionParameterMissing(
+                "Parameter {params.%s} found in expression, but no parameter was specified!"
+                % missing[0]
+            )
+
+        query = query.format(params=DotMap(self._executor.parameters))
+
         order_by_fields = ", ".join(self.query.order_by)
 
         if order_by_fields:
             query = f"{query} ORDER BY {order_by_fields}"
 
         return query
```

### Comparing `jira-select-2.1.1/jira_select/sources/sprints.py` & `jira-select-3.0.0a1/jira_select/sources/sprints.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/jira_select/types.py` & `jira-select-3.0.0a1/jira_select/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 from pydantic import BaseModel
+from pydantic import Extra
 from pydantic import Field as ModelField
 
 JiraFieldName = str
 
 
 class SelectFieldDefinition(BaseModel):
     expression: str
@@ -27,29 +30,35 @@
 
 Expression = str
 
 ExpressionList = List[Expression]
 
 
 class QueryDefinition(BaseModel):
-    select: List[Field]
+    select: Union[List[Field], Dict[str, Optional[str]]]
+    calculate: Dict[str, str] = ModelField(default_factory=dict)
     from_: str = ModelField(alias="from")
+    subqueries: Dict[str, "QueryDefinition"] = ModelField(default_factory=dict)
     where: Union[JqlList, WhereParamDict] = ModelField(default_factory=list)
     order_by: JqlList = ModelField(default_factory=list)
     filter_: ExpressionList = ModelField(alias="filter", default_factory=list)
     having: ExpressionList = ModelField(default_factory=list)
     group_by: ExpressionList = ModelField(default_factory=list)
     sort_by: ExpressionList = ModelField(default_factory=list)
     expand: ExpressionList = ModelField(default_factory=list)
     limit: Optional[int]
     cap: Optional[int]
     cache: Optional[Union[int, Tuple[Optional[int], Optional[int]]]]
 
     class Config:
         allow_population_by_field_name = True
+        extra = Extra.forbid
+
+
+QueryDefinition.update_forward_refs()
 
 
 class SchemaRow(BaseModel):
     id: str
     type: str
     description: Optional[str]
     raw: Optional[Any]
```

### Comparing `jira-select-2.1.1/jira_select/utils.py` & `jira-select-3.0.0a1/jira_select/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import datetime
 import hashlib
+import json
 import logging
 import os
 import re
 import subprocess
 import sys
 from types import ModuleType
 from typing import TYPE_CHECKING
@@ -16,14 +18,16 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import simpleeval
 from appdirs import user_config_dir
 from jira.resources import Resource
+from portion import Interval
+from pytz import UTC
 from simpleeval import EvalWithCompoundTypes
 from yaml import safe_dump
 from yaml import safe_load
 
 from .constants import APP_NAME
 from .exceptions import FieldNameError
 from .exceptions import JiraSelectError
@@ -36,20 +40,57 @@
 
 if TYPE_CHECKING:
     from .query import Result
 
 FIELD_DISPLAY_DEFN_RE = re.compile(r'^(?P<expression>.*) as "(?P<column>.*)"$')
 SORT_BY_DESC_FN = re.compile(r"^(?P<expression>.*) DESC", re.IGNORECASE)
 SORT_BY_ASC_FN = re.compile(r"^(?P<expression>.*) ASC", re.IGNORECASE)
-PARAM_FINDER = re.compile(r"{params\.([^}]+)}")
+PARAM_FINDER = re.compile(r"{params\.([^}.]+)(?:.[^}.]+)?}")
+
+ISO_FORMAT = "%Y-%m-%d %H:%M:%SZ"
 
 
 logger = logging.getLogger(__name__)
 
 
+class JiraSelectJsonEncoder(json.JSONEncoder):
+    def default(self, obj: Any) -> Any:
+        from .functions.flatten_changelog import ChangelogEntry
+
+        if isinstance(obj, datetime.datetime):
+            return UTC.normalize(obj).strftime(ISO_FORMAT)
+        elif isinstance(obj, ChangelogEntry):
+            return {
+                "author": obj.author,
+                "created": UTC.normalize(obj.created).strftime(ISO_FORMAT)
+                if obj.created
+                else None,
+                "field": obj.field,
+                "fieldtype": obj.fieldtype,
+                "fromValue": obj.fromValue,
+                "fromString": obj.fromString,
+                "toValue": obj.toValue,
+                "toString": obj.toString,
+            }
+        elif isinstance(obj, Interval):
+            interval_list = []
+            for interval in list(obj):
+                interval_list.append(
+                    (
+                        interval.lower,
+                        interval.upper,
+                    )
+                )
+            return interval_list
+        try:
+            return super().default(obj)
+        except TypeError:
+            return str(obj)
+
+
 def get_config_dir() -> str:
     root_path = user_config_dir(APP_NAME, "coddingtonbear")
     os.makedirs(root_path, exist_ok=True)
 
     return root_path
 
 
@@ -151,27 +192,29 @@
     params = [
         str(get_field_data(row, group_field, functions)) for group_field in group_fields
     ]
 
     return int(hashlib.sha1(":".join(params).encode("UTF-8")).hexdigest(), 16)
 
 
-def get_row_dict(row: Any) -> Dict[str, Any]:
-    names: Dict[str, Any] = {}
+def get_row_dict(row: Any, overlay: dict[str, Any] | None = None) -> Dict[str, Any]:
+    names: dict[str, Any] = {}
 
     if hasattr(row, "fields"):
         for field_name in dir(row.fields):
             if not field_name.startswith("_"):
                 names[field_name] = getattr(row.fields, field_name)
 
     # Gather any top-level keys, too, to make sure we fetch any expansions
     for key in dir(row):
         if key != "fields" and not key.startswith("_") and not key.upper() == key:
             names[key] = getattr(row, key)
 
+    names.update(overlay if overlay is not None else {})
+
     return names
 
 
 def expression_includes_group_by(
     expression: Expression, group_by: List[Expression]
 ) -> bool:
     for group_by_expression in group_by:
@@ -235,15 +278,19 @@
     if functions is None:
         functions = {}
 
     try:
         return normalize_value(
             evaluate_expression(
                 expression,
-                names={"_": row, **row.as_dict()},
+                names={
+                    "_": row,  # Pre 3.0 queries
+                    "issue": row,  # Post-3.0 queries
+                    **row.as_dict(),
+                },
                 functions=functions,
                 interpolations=interpolations,
             )
         )
     except FieldNameError as e:
         raise QueryError(f"Field {e} does not exist.") from e
     except JiraSelectError:
@@ -253,15 +300,22 @@
     except (
         simpleeval.AttributeDoesNotExist,
         simpleeval.NameNotDefined,
         KeyError,
         IndexError,
         TypeError,
         AttributeError,
-    ):
+    ) as e:
+        logger.warning(
+            "%s while evaluating expression %s for issue(s) %s: %s",
+            e.__class__.__name__,
+            expression,
+            row.key,
+            e,
+        )
         if not error_returns_null:
             raise
         return None
     except Exception as e:
         raise QueryError(f"{e}: {expression}") from e
```

### Comparing `jira-select-2.1.1/jira_select.egg-info/PKG-INFO` & `jira-select-3.0.0a1/jira_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 2.1.1
+Version: 3.0.0a1
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
@@ -94,16 +94,16 @@
 ```
 
 Now, you can type out your query -- the below will find issues assigned
 to you:
 
 ```yaml
 select:
-  - key
-  - summary
+ Issue Key: key
+ Issue Summary: summary
 from: issues
 where:
   - assignee = "your-email@somecompany.com"
   - resolution is null
 ```
 
 The editor uses `vi` bindings by default; so once you're ready to submit
```

### Comparing `jira-select-2.1.1/jira_select.egg-info/SOURCES.txt` & `jira-select-3.0.0a1/jira_select.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,30 +30,39 @@
 jira_select/commands/shell.py
 jira_select/commands/show_instances.py
 jira_select/commands/store_password.py
 jira_select/formatters/__init__.py
 jira_select/formatters/csv.py
 jira_select/formatters/html.py
 jira_select/formatters/json.py
+jira_select/formatters/raw.py
 jira_select/formatters/table.py
+jira_select/formatters/tsv.py
 jira_select/functions/__init__.py
 jira_select/functions/estimate_to_days.py
 jira_select/functions/extract.py
 jira_select/functions/field_by_name.py
 jira_select/functions/flatten_changelog.py
 jira_select/functions/flatten_list.py
+jira_select/functions/get_issue.py
+jira_select/functions/get_issue_snapshot_on_date.py
 jira_select/functions/get_sprint_by_id.py
 jira_select/functions/get_sprint_by_name.py
+jira_select/functions/interval_business_hours.py
+jira_select/functions/interval_matching.py
+jira_select/functions/interval_size.py
 jira_select/functions/json_dumps.py
 jira_select/functions/parse_date.py
 jira_select/functions/parse_datetime.py
 jira_select/functions/simple_filter.py
 jira_select/functions/simple_filter_any.py
 jira_select/functions/sprint_details.py
 jira_select/functions/sprint_name.py
+jira_select/functions/subquery.py
+jira_select/functions/union.py
 jira_select/functions/workdays_in_state.py
 jira_select/sources/__init__.py
 jira_select/sources/boards.py
 jira_select/sources/issues.py
 jira_select/sources/sprints.py
 tests/__init__.py
 tests/base.py
```

### Comparing `jira-select-2.1.1/jira_select.egg-info/entry_points.txt` & `jira-select-3.0.0a1/jira_select.egg-info/entry_points.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,30 +15,39 @@
 show-instances = jira_select.commands.show_instances:Command
 store-password = jira_select.commands.store_password:Command
 
 [jira_select.formatters]
 csv = jira_select.formatters.csv:Formatter
 html = jira_select.formatters.html:Formatter
 json = jira_select.formatters.json:Formatter
+raw = jira_select.formatters.raw:Formatter
 table = jira_select.formatters.table:Formatter
+tsv = jira_select.formatters.tsv:Formatter
 
 [jira_select.functions]
 estimate_to_days = jira_select.functions.estimate_to_days:Function
 extract = jira_select.functions.extract:Function
 field_by_name = jira_select.functions.field_by_name:Function
 flatten_changelog = jira_select.functions.flatten_changelog:Function
 flatten_list = jira_select.functions.flatten_list:Function
+get_issue = jira_select.functions.get_issue:Function
+get_issue_snapshot_on_date = jira_select.functions.get_issue_snapshot_on_date:Function
 get_sprint_by_id = jira_select.functions.get_sprint_by_id:Function
 get_sprint_by_name = jira_select.functions.get_sprint_by_name:Function
+interval_business_hours = jira_select.functions.interval_business_hours:Function
+interval_matching = jira_select.functions.interval_matching:Function
+interval_size = jira_select.functions.interval_size:Function
 json_dumps = jira_select.functions.json_dumps:Function
 parse_date = jira_select.functions.parse_date:Function
 parse_datetime = jira_select.functions.parse_datetime:Function
 simple_filter = jira_select.functions.simple_filter:Function
 simple_filter_any = jira_select.functions.simple_filter_any:Function
 sprint_details = jira_select.functions.sprint_details:Function
 sprint_name = jira_select.functions.sprint_name:Function
+subquery = jira_select.functions.subquery:Function
+union = jira_select.functions.union:Function
 workdays_in_state = jira_select.functions.workdays_in_state:Function
 
 [jira_select.sources]
 boards = jira_select.sources.boards:Source
 issues = jira_select.sources.issues:Source
 sprints = jira_select.sources.sprints:Source
```

### Comparing `jira-select-2.1.1/setup.cfg` & `jira-select-3.0.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/setup.py` & `jira-select-3.0.0a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="jira-select",
-    version="2.1.1",
+    version="3.0.0.a1",
     license="MIT",
     description=(
         "Easily run complex SQL-like queries far beyond what "
         "Jira's standard JQL query language can provide."
     ),
     long_description_content_type="text/markdown",
     long_description=read("readme.md"),
@@ -91,17 +91,19 @@
             "show-instances = jira_select.commands.show_instances:Command",
             "setup-instance = jira_select.commands.setup_instance:Command",
             "remove-instance = jira_select.commands.remove_instance:Command",
             "install-user-script = jira_select.commands.install_user_script:Command",
         ],
         "jira_select.formatters": [
             "csv = jira_select.formatters.csv:Formatter",
+            "tsv = jira_select.formatters.tsv:Formatter",
             "html = jira_select.formatters.html:Formatter",
             "json = jira_select.formatters.json:Formatter",
             "table = jira_select.formatters.table:Formatter",
+            "raw = jira_select.formatters.raw:Formatter",
         ],
         "jira_select.functions": [
             "sprint_details = jira_select.functions.sprint_details:Function",
             "sprint_name = jira_select.functions.sprint_name:Function",
             "get_sprint_by_id = jira_select.functions.get_sprint_by_id:Function",
             "get_sprint_by_name = jira_select.functions.get_sprint_by_name:Function",
             "field_by_name = jira_select.functions.field_by_name:Function",
@@ -110,15 +112,22 @@
             "flatten_list = jira_select.functions.flatten_list:Function",
             "flatten_changelog = jira_select.functions.flatten_changelog:Function",
             "simple_filter = jira_select.functions.simple_filter:Function",
             "simple_filter_any = jira_select.functions.simple_filter_any:Function",
             "parse_datetime = jira_select.functions.parse_datetime:Function",
             "parse_date = jira_select.functions.parse_date:Function",
             "json_dumps = jira_select.functions.json_dumps:Function",
+            "get_issue = jira_select.functions.get_issue:Function",
             "workdays_in_state = jira_select.functions.workdays_in_state:Function",
+            "get_issue_snapshot_on_date = jira_select.functions.get_issue_snapshot_on_date:Function",
+            "interval_business_hours = jira_select.functions.interval_business_hours:Function",
+            "interval_matching = jira_select.functions.interval_matching:Function",
+            "interval_size = jira_select.functions.interval_size:Function",
+            "subquery = jira_select.functions.subquery:Function",
+            "union = jira_select.functions.union:Function",
         ],
         "jira_select.sources": [
             "issues = jira_select.sources.issues:Source",
             "boards = jira_select.sources.boards:Source",
             "sprints = jira_select.sources.sprints:Source",
         ],
     },
```

### Comparing `jira-select-2.1.1/tests/base.py` & `jira-select-3.0.0a1/tests/base.py`

 * *Files identical despite different names*

### Comparing `jira-select-2.1.1/tests/test_functions.py` & `jira-select-3.0.0a1/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 from types import SimpleNamespace
 from unittest.mock import Mock
 
 import pytz
 
 from jira_select.functions.flatten_changelog import ChangelogEntry
```

### Comparing `jira-select-2.1.1/tests/test_query.py` & `jira-select-3.0.0a1/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import uuid
 from unittest.mock import Mock
 
 import pytest
 from dotmap import DotMap
 from jira import Issue
 from jira.resources import Resource
@@ -419,55 +421,59 @@
         )
 
         query = Executor(self.mock_jira, query, parameters={"ok": arbitrary_value})
         results = list(query)
 
         assert results[0]["value"] == arbitrary_value
 
-    def test_param_expression_unspecified(self):
+    def test_param_expression_unspecified_select(self):
         query = QueryDefinition.parse_obj(
             {
                 "select": ["'{params.ok}'"],
                 "from": "issues",
                 "cap": 1,
             }
         )
 
         query = Executor(self.mock_jira, query)
 
         with pytest.raises(ExpressionParameterMissing):
             list(query)
 
-    def test_param_jql_specified(self):
-        arbitrary_value = str(uuid.uuid4())
-
+    def test_param_expression_unspecified_where(self):
         query = QueryDefinition.parse_obj(
             {
-                "select": ["'{params.ok}' as \"value\""],
+                "select": ["True"],
                 "from": "issues",
                 "where": [
-                    '"{params.ok}"',
+                    "'{params.ok}'",
                 ],
                 "cap": 1,
             }
         )
 
-        query = Executor(self.mock_jira, query, parameters={"ok": arbitrary_value})
+        query = Executor(self.mock_jira, query)
 
-        assert arbitrary_value in query._get_jql()
+        with pytest.raises(ExpressionParameterMissing):
+            list(query)
+
+    def test_param_jql_specified(self):
+        arbitrary_value = str(uuid.uuid4())
 
-    def test_param_jql_unspecified(self):
         query = QueryDefinition.parse_obj(
             {
                 "select": ["'{params.ok}' as \"value\""],
                 "from": "issues",
                 "where": [
                     '"{params.ok}"',
                 ],
                 "cap": 1,
             }
         )
 
-        query = Executor(self.mock_jira, query)
+        query = list(
+            Executor(self.mock_jira, query, parameters={"ok": arbitrary_value})
+        )
 
-        with pytest.raises(ExpressionParameterMissing):
-            query._get_jql()
+        args, _ = self.mock_jira.search_issues.call_args
+
+        assert arbitrary_value in args[0]
```

### Comparing `jira-select-2.1.1/tests/test_utils.py` & `jira-select-3.0.0a1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 from unittest.mock import ANY
 from unittest.mock import Mock
 from unittest.mock import patch
 
 import simpleeval
```

