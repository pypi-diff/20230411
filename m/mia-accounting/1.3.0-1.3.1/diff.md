# Comparing `tmp/mia-accounting-1.3.0.tar.gz` & `tmp/mia-accounting-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.3.0.tar", last modified: Mon Apr 10 16:09:35 2023, max compression
+gzip compressed data, was "mia-accounting-1.3.1.tar", last modified: Tue Apr 11 14:32:42 2023, max compression
```

## Comparing `mia-accounting-1.3.0.tar` & `mia-accounting-1.3.1.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.0/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.0/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     6757 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     5958 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.0/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.0/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.0/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.0/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-10 16:08:23.000000 mia-accounting-1.3.0/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.0/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.0/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.0/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.0/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-10 16:08:23.000000 mia-accounting-1.3.0/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.0/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.0/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.3.0/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.0/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.0/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.0/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.0/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.0/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.0/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.0/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     6757 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11392 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38268 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    15398 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4348 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.3.0/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.0/tests/test_site/locale.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.0/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.3.0/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.3.0/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.3.0/tests/test_site/templates/login.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.0/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.3.0/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.445633 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    28229 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    14493 2023-04-09 03:46:55.000000 mia-accounting-1.3.0/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.0/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.088098 mia-accounting-1.3.1/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.1/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.1/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.1/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.1/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.1/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.1/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.1/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-11 14:30:58.000000 mia-accounting-1.3.1/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.1/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.1/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.1/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.1/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.1/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-11 14:30:59.000000 mia-accounting-1.3.1/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-11 14:32:42.088098 mia-accounting-1.3.1/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.1/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.1/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.3.1/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.1/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.1/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.1/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.1/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.1/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.980100 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.980100 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.996100 mia-accounting-1.3.1/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.1/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.1/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.020099 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.064098 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.064098 mia-accounting-1.3.1/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.068098 mia-accounting-1.3.1/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.068098 mia-accounting-1.3.1/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11392 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38268 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15398 2023-04-11 00:28:47.000000 mia-accounting-1.3.1/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4456 2023-04-11 14:03:11.000000 mia-accounting-1.3.1/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3073 2023-04-11 14:24:08.000000 mia-accounting-1.3.1/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.1/tests/test_site/locale.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.1/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.3.1/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.1/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.1/tests/test_site/templates/login.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.1/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     1837 2023-04-11 14:18:30.000000 mia-accounting-1.3.1/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     1486 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     2369 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     1486 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     2369 2023-04-11 14:27:31.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    28229 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14555 2023-04-11 14:26:58.000000 mia-accounting-1.3.1/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.1/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.3.0/LICENSE` & `mia-accounting-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/MANIFEST.in` & `mia-accounting-1.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/PKG-INFO` & `mia-accounting-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
@@ -23,50 +23,51 @@
 ===============
 
 
 Description
 ===========
 
 *Mia! Accounting* is an accounting module for Flask_ applications.
-It implements `double-entry bookkeeping`_, and generates the following
+It is designed both for mobile and desktop environments.  It
+implements `double-entry bookkeeping`_.  It generates the following
 accounting reports:
 
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
 
+Live Demonstration and Test Site
+================================
+
+There is a `live demonstration`_ for *Mia! Accounting*.  It runs the
+same code as the `test site`_ in the `source distribution`_.  It is
+the simplest website that works with *Mia! Accounting*.  It is also
+used in the automatic tests.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
-You may also download the from the `PyPI project page`_ or the
+You may also download from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application or do not know how to
-start one, you may start with the test site.
-
-
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.  You also
 need at least one user.
 
@@ -207,23 +208,22 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _live demonstration: https://accounting.imacat.idv.tw
 .. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
-.. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
-.. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.3.0/README.rst` & `mia-accounting-1.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,50 +3,51 @@
 ===============
 
 
 Description
 ===========
 
 *Mia! Accounting* is an accounting module for Flask_ applications.
-It implements `double-entry bookkeeping`_, and generates the following
+It is designed both for mobile and desktop environments.  It
+implements `double-entry bookkeeping`_.  It generates the following
 accounting reports:
 
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
 
+Live Demonstration and Test Site
+================================
+
+There is a `live demonstration`_ for *Mia! Accounting*.  It runs the
+same code as the `test site`_ in the `source distribution`_.  It is
+the simplest website that works with *Mia! Accounting*.  It is also
+used in the automatic tests.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
-You may also download the from the `PyPI project page`_ or the
+You may also download from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application or do not know how to
-start one, you may start with the test site.
-
-
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.  You also
 need at least one user.
 
@@ -187,23 +188,22 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _live demonstration: https://accounting.imacat.idv.tw
 .. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
-.. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
-.. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.3.0/docs/Makefile` & `mia-accounting-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/make.bat` & `mia-accounting-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.account.rst` & `mia-accounting-1.3.1/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.base_account.rst` & `mia-accounting-1.3.1/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.currency.rst` & `mia-accounting-1.3.1/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.3.1/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.3.1/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.3.1/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.option.rst` & `mia-accounting-1.3.1/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.report.period.rst` & `mia-accounting-1.3.1/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.report.reports.rst` & `mia-accounting-1.3.1/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.report.rst` & `mia-accounting-1.3.1/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.report.utils.rst` & `mia-accounting-1.3.1/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.rst` & `mia-accounting-1.3.1/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.unmatched_offset.rst` & `mia-accounting-1.3.1/docs/source/accounting.unmatched_offset.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/accounting.utils.rst` & `mia-accounting-1.3.1/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/conf.py` & `mia-accounting-1.3.1/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.3.0'
+release = '1.3.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.3.0/docs/source/examples.rst` & `mia-accounting-1.3.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/history.rst` & `mia-accounting-1.3.1/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/docs/source/intro.rst` & `mia-accounting-1.3.1/docs/source/intro.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Introduction
 ============
 
 *Mia! Accounting* is an accounting module for Flask_ applications.
-It implements `double-entry bookkeeping`_, and generates the following
+It is designed both for mobile and desktop environments.  It
+implements `double-entry bookkeeping`_.  It generates the following
 accounting reports:
 
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
 
+Live Demonstration and Test Site
+--------------------------------
+
+There is a `live demonstration`_ for *Mia! Accounting*.  It runs the
+same code as the `test site`_ in the `source distribution`_.  It is
+the simplest website that works with *Mia! Accounting*.  It is also
+used in the automatic tests.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Installation
 ------------
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
-You may also download the from the `PyPI project page`_ or the
+You may also download from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
-Test Site and Live Demonstration
---------------------------------
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application or do not know how to
-start one, you may start with the test site.
-
-
 Prerequisites
 -------------
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.  You also
 need at least one user.
 
@@ -106,21 +107,20 @@
 -------------
 
 Refer to the `documentation on Read the Docs`_.
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _live demonstration: https://accounting.imacat.idv.tw
 .. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
-.. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
-.. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.3.0/pyproject.toml` & `mia-accounting-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.3.0"
+version = "1.3.1"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.3.0/src/accounting/__init__.py` & `mia-accounting-1.3.1/src/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/__init__.py` & `mia-accounting-1.3.1/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/commands.py` & `mia-accounting-1.3.1/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/converters.py` & `mia-accounting-1.3.1/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/forms.py` & `mia-accounting-1.3.1/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/queries.py` & `mia-accounting-1.3.1/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/account/views.py` & `mia-accounting-1.3.1/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/base_account/__init__.py` & `mia-accounting-1.3.1/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/base_account/commands.py` & `mia-accounting-1.3.1/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/base_account/converters.py` & `mia-accounting-1.3.1/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/base_account/queries.py` & `mia-accounting-1.3.1/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/base_account/views.py` & `mia-accounting-1.3.1/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/commands.py` & `mia-accounting-1.3.1/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/__init__.py` & `mia-accounting-1.3.1/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/commands.py` & `mia-accounting-1.3.1/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/converters.py` & `mia-accounting-1.3.1/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/forms.py` & `mia-accounting-1.3.1/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/queries.py` & `mia-accounting-1.3.1/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/currency/views.py` & `mia-accounting-1.3.1/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/data/base_accounts.csv` & `mia-accounting-1.3.1/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/forms.py` & `mia-accounting-1.3.1/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/converters.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/journal_entry/views.py` & `mia-accounting-1.3.1/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/locale.py` & `mia-accounting-1.3.1/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/models.py` & `mia-accounting-1.3.1/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/option/__init__.py` & `mia-accounting-1.3.1/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/option/forms.py` & `mia-accounting-1.3.1/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/option/views.py` & `mia-accounting-1.3.1/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/__init__.py` & `mia-accounting-1.3.1/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/converters.py` & `mia-accounting-1.3.1/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/__init__.py` & `mia-accounting-1.3.1/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/chooser.py` & `mia-accounting-1.3.1/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/description.py` & `mia-accounting-1.3.1/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/month_end.py` & `mia-accounting-1.3.1/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/parser.py` & `mia-accounting-1.3.1/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/period.py` & `mia-accounting-1.3.1/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.3.1/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/period/specification.py` & `mia-accounting-1.3.1/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/__init__.py` & `mia-accounting-1.3.1/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.3.1/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.3.1/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.3.1/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/journal.py` & `mia-accounting-1.3.1/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/ledger.py` & `mia-accounting-1.3.1/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/search.py` & `mia-accounting-1.3.1/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.3.1/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.3.1/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.3.1/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/template_filters.py` & `mia-accounting-1.3.1/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/__init__.py` & `mia-accounting-1.3.1/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.3.1/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/base_report.py` & `mia-accounting-1.3.1/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.3.1/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/option_link.py` & `mia-accounting-1.3.1/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.3.1/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/report_type.py` & `mia-accounting-1.3.1/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.3.1/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/utils/urls.py` & `mia-accounting-1.3.1/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/report/views.py` & `mia-accounting-1.3.1/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/css/style.css` & `mia-accounting-1.3.1/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/account-form.js` & `mia-accounting-1.3.1/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/account-order.js` & `mia-accounting-1.3.1/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/currency-form.js` & `mia-accounting-1.3.1/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/description-editor.js` & `mia-accounting-1.3.1/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.3.1/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.3.1/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/option-form.js` & `mia-accounting-1.3.1/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.3.1/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.3.1/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/template_filters.py` & `mia-accounting-1.3.1/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/template_globals.py` & `mia-accounting-1.3.1/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/base.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/include/nav.html`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,22 @@
       </li>
       <li>
         <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.currency.") %} active {% endif %}" href="{{ url_for("accounting.currency.list") }}">
           <i class="fa-solid fa-money-bill-wave"></i>
           {{ A_("Currencies") }}
         </a>
       </li>
-      <li>
-        <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.unmatched-offset.") %} active {% endif %}" href="{{ url_for("accounting.unmatched-offset.dashboard") }}">
-          <i class="fa-solid fa-link-slash"></i>
-          {{ A_("Unmatched Offsets") }}
-        </a>
-      </li>
+      {% if accounting_can_edit() %}
+        <li>
+          <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.unmatched-offset.") %} active {% endif %}" href="{{ url_for("accounting.unmatched-offset.dashboard") }}">
+            <i class="fa-solid fa-link-slash"></i>
+            {{ A_("Unmatched Offsets") }}
+          </a>
+        </li>
+      {% endif %}
       {% if accounting_can_admin() %}
         <li>
           <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.option.") %} active {% endif %}" href="{{ url_for("accounting.option.detail") }}">
             <i class="fa-solid fa-gear"></i>
             {{ A_("Settings") }}
           </a>
         </li>
```

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/list.html` & `mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/translations/accounting.pot` & `mia-accounting-1.3.1/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.3.1/src/accounting/unmatched_offset/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/unmatched_offset/queries.py` & `mia-accounting-1.3.1/src/accounting/unmatched_offset/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/unmatched_offset/views.py` & `mia-accounting-1.3.1/src/accounting/unmatched_offset/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/__init__.py` & `mia-accounting-1.3.1/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/cast.py` & `mia-accounting-1.3.1/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/current_account.py` & `mia-accounting-1.3.1/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/flash_errors.py` & `mia-accounting-1.3.1/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.3.1/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/next_uri.py` & `mia-accounting-1.3.1/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/offset_alias.py` & `mia-accounting-1.3.1/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/offset_matcher.py` & `mia-accounting-1.3.1/src/accounting/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/options.py` & `mia-accounting-1.3.1/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/pagination.py` & `mia-accounting-1.3.1/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/permission.py` & `mia-accounting-1.3.1/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/query.py` & `mia-accounting-1.3.1/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/random_id.py` & `mia-accounting-1.3.1/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/strip_text.py` & `mia-accounting-1.3.1/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/unapplied.py` & `mia-accounting-1.3.1/src/accounting/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/accounting/utils/user.py` & `mia-accounting-1.3.1/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.3.1/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
@@ -23,50 +23,51 @@
 ===============
 
 
 Description
 ===========
 
 *Mia! Accounting* is an accounting module for Flask_ applications.
-It implements `double-entry bookkeeping`_, and generates the following
+It is designed both for mobile and desktop environments.  It
+implements `double-entry bookkeeping`_.  It generates the following
 accounting reports:
 
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
 
+Live Demonstration and Test Site
+================================
+
+There is a `live demonstration`_ for *Mia! Accounting*.  It runs the
+same code as the `test site`_ in the `source distribution`_.  It is
+the simplest website that works with *Mia! Accounting*.  It is also
+used in the automatic tests.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
-You may also download the from the `PyPI project page`_ or the
+You may also download from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application or do not know how to
-start one, you may start with the test site.
-
-
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.  You also
 need at least one user.
 
@@ -207,23 +208,22 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _live demonstration: https://accounting.imacat.idv.tw
 .. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
-.. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
-.. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.3.0/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.3.1/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/babel-utils-test-site.py` & `mia-accounting-1.3.1/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/babel-utils.py` & `mia-accounting-1.3.1/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_account.py` & `mia-accounting-1.3.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_base_account.py` & `mia-accounting-1.3.1/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_commands.py` & `mia-accounting-1.3.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_currency.py` & `mia-accounting-1.3.1/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_description_editor.py` & `mia-accounting-1.3.1/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_journal_entry.py` & `mia-accounting-1.3.1/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_offset.py` & `mia-accounting-1.3.1/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_option.py` & `mia-accounting-1.3.1/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_report.py` & `mia-accounting-1.3.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_site/__init__.py` & `mia-accounting-1.3.1/tests/test_site/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 """
 import os
 import typing as t
 from secrets import token_urlsafe
 
 from click.testing import Result
-from flask import Flask, Blueprint, render_template, redirect, Response
+from flask import Flask, Blueprint, render_template, redirect, Response, \
+    url_for
 from flask.testing import FlaskCliRunner
 from flask_babel_js import BabelJS
 from flask_sqlalchemy import SQLAlchemy
 from flask_wtf import CSRFProtect
 from sqlalchemy import Column
 
 bp: Blueprint = Blueprint("home", __name__)
@@ -82,15 +83,16 @@
                 and auth.current_user().username in ["editor", "admin"]
 
         def can_admin(self) -> bool:
             return auth.current_user() is not None \
                 and auth.current_user().username == "admin"
 
         def unauthorized(self) -> Response:
-            return redirect("/login")
+            from accounting.utils.next_uri import append_next
+            return redirect(append_next(url_for("auth.login-form")))
 
         @property
         def cls(self) -> t.Type[auth.User]:
             return auth.User
 
         @property
         def pk_column(self) -> Column:
```

### Comparing `mia-accounting-1.3.0/tests/test_site/auth.py` & `mia-accounting-1.3.1/tests/test_site/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The authentication for the Mia! Accounting demonstration website.
 
 """
 from flask import Blueprint, render_template, Flask, redirect, url_for, \
-    session, request, g
+    session, request, g, Response
 
 from . import db
 
 bp: Blueprint = Blueprint("auth", __name__, url_prefix="/")
 
 
 class User(db.Model):
@@ -40,33 +40,36 @@
 
         :return: The string representation of the user.
         """
         return self.username
 
 
 @bp.get("login", endpoint="login-form")
-def show_login_form() -> str:
+def show_login_form() -> str | Response:
     """Shows the login form.
 
     :return: The login form.
     """
+    if "user" in session:
+        return redirect(url_for("accounting-report.default"))
     return render_template("login.html")
 
 
 @bp.post("login", endpoint="login")
 def login() -> redirect:
     """Logs in the user.
 
     :return: The redirection to the home page.
     """
+    from accounting.utils.next_uri import inherit_next, or_next
     if request.form.get("username") not in {"viewer", "editor", "admin",
                                             "nobody"}:
-        return redirect(url_for("auth.login"))
+        return redirect(inherit_next(url_for("auth.login")))
     session["user"] = request.form.get("username")
-    return redirect(url_for("home.home"))
+    return redirect(or_next(url_for("accounting-report.default")))
 
 
 @bp.post("logout", endpoint="logout")
 def logout() -> redirect:
     """Logs out the user.
 
     :return: The redirection to the home page.
```

### Comparing `mia-accounting-1.3.0/tests/test_site/locale.py` & `mia-accounting-1.3.1/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_site/static/favicon.svg` & `mia-accounting-1.3.1/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_site/templates/base.html` & `mia-accounting-1.3.1/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_site/templates/home.html` & `mia-accounting-1.3.1/tests/test_site/templates/home.html`

 * *Files 26% similar despite different names*

```diff
@@ -42,10 +42,37 @@
 00000290: 6d61 6361 742e 6964 762e 7477 2028 696d  macat.idv.tw (im
 000002a0: 6163 6174 290a 4669 7273 7420 7772 6974  acat).First writ
 000002b0: 7465 6e3a 2032 3032 332f 312f 3237 0a23  ten: 2023/1/27.#
 000002c0: 7d0a 7b25 2065 7874 656e 6473 2022 6261  }.{% extends "ba
 000002d0: 7365 2e68 746d 6c22 2025 7d0a 0a7b 2520  se.html" %}..{% 
 000002e0: 626c 6f63 6b20 6865 6164 6572 2025 7d7b  block header %}{
 000002f0: 2520 626c 6f63 6b20 7469 746c 6520 257d  % block title %}
-00000300: 7b7b 205f 2822 486f 6d65 2229 207d 7d7b  {{ _("Home") }}{
-00000310: 2520 656e 6462 6c6f 636b 2025 7d7b 2520  % endblock %}{% 
-00000320: 656e 6462 6c6f 636b 2025 7d0a            endblock %}.
+00000300: 7b7b 205f 2822 4d69 6121 2041 6363 6f75  {{ _("Mia! Accou
+00000310: 6e74 696e 6720 4c69 7665 2044 656d 6f6e  nting Live Demon
+00000320: 7374 7261 7469 6f6e 2229 207d 7d7b 2520  stration") }}{% 
+00000330: 656e 6462 6c6f 636b 2025 7d7b 2520 656e  endblock %}{% en
+00000340: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
+00000350: 6f63 6b20 636f 6e74 656e 7420 257d 0a0a  ock content %}..
+00000360: 3c70 3e7b 7b20 5f28 2254 6869 7320 6973  <p>{{ _("This is
+00000370: 2074 6865 206c 6976 6520 6465 6d6f 6e73   the live demons
+00000380: 7472 6174 696f 6e20 6f66 2074 6865 204d  tration of the M
+00000390: 6961 2120 4163 636f 756e 7469 6e67 2070  ia! Accounting p
+000003a0: 726f 6a65 6374 2e20 2050 6c65 6173 6520  roject.  Please 
+000003b0: 3c61 2068 7265 663d 5c22 2f6c 6f67 696e  <a href=\"/login
+000003c0: 3f6e 6578 743d 2525 3246 6163 636f 756e  ?next=%%2Faccoun
+000003d0: 7469 6e67 5c22 3e6c 6f67 2069 6e3c 2f61  ting\">log in</a
+000003e0: 3e20 746f 2063 6f6e 7469 6e75 652e 2229  > to continue.")
+000003f0: 207d 7d3c 2f70 3e0a 0a3c 703e 7b7b 205f   }}</p>..<p>{{ _
+00000400: 2822 596f 7520 6d61 7920 616c 736f 2077  ("You may also w
+00000410: 616e 7420 746f 2063 6865 636b 2074 6865  ant to check the
+00000420: 203c 6120 6872 6566 3d5c 2268 7474 7073   <a href=\"https
+00000430: 3a2f 2f6d 6961 2d61 6363 6f75 6e74 696e  ://mia-accountin
+00000440: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
+00000450: 5c22 3e66 756c 6c20 646f 6375 6d65 6e74  \">full document
+00000460: 6174 696f 6e3c 2f61 3e20 616e 6420 7468  ation</a> and th
+00000470: 6520 3c61 2068 7265 663d 5c22 6874 7470  e <a href=\"http
+00000480: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00000490: 6d61 6361 742f 6d69 612d 6163 636f 756e  macat/mia-accoun
+000004a0: 7469 6e67 5c22 3e47 6974 6875 6220 7265  ting\">Github re
+000004b0: 706f 7369 746f 7279 3c2f 613e 2e22 2920  pository</a>.") 
+000004c0: 7d7d 3c2f 703e 0a0a 7b25 2065 6e64 626c  }}</p>..{% endbl
+000004d0: 6f63 6b20 257d 0a                        ock %}.
```

### Comparing `mia-accounting-1.3.0/tests/test_site/templates/login.html` & `mia-accounting-1.3.1/tests/test_site/templates/login.html`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
 {% block header %}{% block title %}{{ _("Log In") }}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <form action="{{ url_for("auth.login") }}" method="post">
   <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
+  {% if request.args.next %}
+    <input type="hidden" name="next" value="{{ request.args.next }}">
+  {% endif %}
   <button class="btn btn-primary" type="submit" name="username" value="viewer">{{ _("Viewer") }}</button>
   <button class="btn btn-primary" type="submit" name="username" value="editor">{{ _("Editor") }}</button>
   <button class="btn btn-primary" type="submit" name="username" value="admin">{{ _("Administrator") }}</button>
   <button class="btn btn-primary" type="submit" name="username" value="nobody">{{ _("Nobody") }}</button>
 </form>
 
 {% endblock %}
```

### Comparing `mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.3.1/tests/test_site/translations/messages.pot`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,74 @@
-# Chinese (Traditional) translations for the Mia! Accounting
-# Test website.
-# Copyright (C) 2023 imacat
-# This file is distributed under the same license as the Mia! Accounting
-# project.
-# imacat <imacat@mail.imacat.idv.tw>, 2023.
+# Translations template for PROJECT.
+# Copyright (C) 2023 ORGANIZATION
+# This file is distributed under the same license as the PROJECT project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting-test-site 1.0.0\n"
-"Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
-"PO-Revision-Date: 2023-04-06 02:34+0800\n"
-"Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
-"Language: zh_Hans\n"
-"Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Project-Id-Version: PROJECT VERSION\n"
+"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
+"POT-Creation-Date: 2023-04-11 22:18+0800\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: tests/test_site/templates/base.html:23
 msgid "en"
-msgstr "zh-Hans"
+msgstr ""
 
 #: tests/test_site/templates/base.html:46
-#: tests/test_site/templates/home.html:24
 msgid "Home"
-msgstr "首页"
+msgstr ""
 
 #: tests/test_site/templates/base.html:71
 msgid "Log Out"
-msgstr "注销"
+msgstr ""
 
 #: tests/test_site/templates/base.html:81
 #: tests/test_site/templates/login.html:24
 msgid "Log In"
-msgstr "登录"
+msgstr ""
 
 #: tests/test_site/templates/base.html:122
 msgid "Error:"
-msgstr "错误："
+msgstr ""
 
-#: tests/test_site/templates/login.html:30
+#: tests/test_site/templates/home.html:24
+msgid "Mia! Accounting Live Demonstration"
+msgstr ""
+
+#: tests/test_site/templates/home.html:28
+#, python-format
+msgid ""
+"This is the live demonstration of the Mia! Accounting project.  Please <a"
+" href=\"/login?next=%%2Faccounting\">log in</a> to continue."
+msgstr ""
+
+#: tests/test_site/templates/home.html:30
+msgid ""
+"You may also want to check the <a href=\"https://mia-"
+"accounting.readthedocs.io\">full documentation</a> and the <a "
+"href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
+msgstr ""
+
+#: tests/test_site/templates/login.html:33
 msgid "Viewer"
-msgstr "读报表者"
+msgstr ""
 
-#: tests/test_site/templates/login.html:31
+#: tests/test_site/templates/login.html:34
 msgid "Editor"
-msgstr "记帐者"
+msgstr ""
 
-#: tests/test_site/templates/login.html:32
+#: tests/test_site/templates/login.html:35
 msgid "Administrator"
-msgstr "管理者"
+msgstr ""
 
-#: tests/test_site/templates/login.html:33
+#: tests/test_site/templates/login.html:36
 msgid "Nobody"
-msgstr "没有权限者"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mia-accounting-1.3.0/tests/test_unmatched_offset.py` & `mia-accounting-1.3.1/tests/test_unmatched_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/test_utils.py` & `mia-accounting-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.0/tests/testlib.py` & `mia-accounting-1.3.1/tests/testlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     :return: A tuple of the client and the CSRF token.
     """
     client: httpx.Client = httpx.Client(app=app, base_url=TEST_SERVER)
     client.headers["Referer"] = TEST_SERVER
     csrf_token: str = get_csrf_token(client)
     response: httpx.Response = client.post("/login",
                                            data={"csrf_token": csrf_token,
+                                                 "next": "/",
                                                  "username": username})
     assert response.status_code == 302
     assert response.headers["Location"] == "/"
     return client, csrf_token
 
 
 def set_locale(client: httpx.Client, csrf_token: str,
```

### Comparing `mia-accounting-1.3.0/tests/testlib_journal_entry.py` & `mia-accounting-1.3.1/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

