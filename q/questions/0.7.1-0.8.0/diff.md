# Comparing `tmp/questions-0.7.1.tar.gz` & `tmp/questions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questions-0.7.1.tar", last modified: Sun Sep 18 06:17:51 2022, max compression
+gzip compressed data, was "questions-0.8.0.tar", last modified: Tue Apr 11 00:04:55 2023, max compression
```

## Comparing `questions-0.7.1.tar` & `questions-0.8.0.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.318757 questions-0.7.1/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      164 2020-09-10 02:51:50.000000 questions-0.7.1/AUTHORS.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3521 2020-09-12 23:58:04.000000 questions-0.7.1/CONTRIBUTING.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1199 2022-09-18 06:13:08.000000 questions-0.7.1/HISTORY.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1079 2020-08-15 18:52:11.000000 questions-0.7.1/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      305 2020-12-10 22:30:21.000000 questions-0.7.1/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8735 2022-09-18 06:17:51.318757 questions-0.7.1/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6673 2022-09-16 19:43:40.000000 questions-0.7.1/README.rst
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.310757 questions-0.7.1/docs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      610 2020-08-15 18:52:11.000000 questions-0.7.1/docs/Makefile
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.306757 questions-0.7.1/docs/_build/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.306757 questions-0.7.1/docs/_build/html/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.314757 questions-0.7.1/docs/_build/html/_sources/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       28 2020-08-15 18:52:11.000000 questions-0.7.1/docs/_build/html/_sources/authors.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       33 2020-08-15 18:52:11.000000 questions-0.7.1/docs/_build/html/_sources/contributing.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       28 2020-08-15 18:52:11.000000 questions-0.7.1/docs/_build/html/_sources/history.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      604 2020-09-24 23:07:47.000000 questions-0.7.1/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4583 2020-09-30 07:41:43.000000 questions-0.7.1/docs/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       64 2020-12-09 11:25:39.000000 questions-0.7.1/docs/_build/html/_sources/modules.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      130 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.cli.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      133 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.form.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      148 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.questions.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      331 2020-12-09 11:25:39.000000 questions-0.7.1/docs/_build/html/_sources/questions.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      145 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.settings.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      148 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.templates.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      151 2020-09-24 23:59:36.000000 questions-0.7.1/docs/_build/html/_sources/questions.validators.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       27 2020-08-15 18:52:11.000000 questions-0.7.1/docs/_build/html/_sources/readme.rst.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14412 2020-12-09 11:25:35.000000 questions-0.7.1/docs/_build/html/_sources/usage.rst.txt
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.314757 questions-0.7.1/docs/_build/html/_static/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2020-09-24 23:09:34.000000 questions-0.7.1/docs/_build/html/_static/README.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      286 2020-09-26 01:10:22.000000 questions-0.7.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       90 2020-09-26 01:10:22.000000 questions-0.7.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       90 2020-09-26 01:10:22.000000 questions-0.7.1/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.314757 questions-0.7.1/docs/_static/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2020-09-24 23:09:34.000000 questions-0.7.1/docs/_static/README.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       28 2020-08-15 18:52:11.000000 questions-0.7.1/docs/authors.rst
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     5270 2020-09-26 06:19:32.000000 questions-0.7.1/docs/conf.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       33 2020-08-15 18:52:11.000000 questions-0.7.1/docs/contributing.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       28 2020-08-15 18:52:11.000000 questions-0.7.1/docs/history.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      604 2020-09-24 23:07:47.000000 questions-0.7.1/docs/index.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4792 2020-12-10 22:43:55.000000 questions-0.7.1/docs/installation.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      771 2020-08-15 18:52:11.000000 questions-0.7.1/docs/make.bat
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       64 2020-12-09 11:25:39.000000 questions-0.7.1/docs/modules.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      130 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.cli.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      133 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.form.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      148 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.questions.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      331 2020-12-09 11:25:39.000000 questions-0.7.1/docs/questions.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      145 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.settings.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      148 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.templates.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      151 2020-09-24 23:59:36.000000 questions-0.7.1/docs/questions.validators.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       27 2020-08-15 18:52:11.000000 questions-0.7.1/docs/readme.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      149 2022-09-18 06:04:52.000000 questions-0.7.1/docs/requirements.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      223 2020-10-25 06:47:36.000000 questions-0.7.1/docs/spelling_word_list.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14818 2020-12-13 22:03:02.000000 questions-0.7.1/docs/usage.rst
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.314757 questions-0.7.1/questions/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2568 2021-01-26 21:12:16.000000 questions-0.7.1/questions/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5212 2021-01-26 21:12:16.000000 questions-0.7.1/questions/cli.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20031 2020-12-15 17:26:57.000000 questions-0.7.1/questions/form.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    25521 2020-12-13 22:04:53.000000 questions-0.7.1/questions/questions.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14606 2022-09-18 05:39:46.000000 questions-0.7.1/questions/settings.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.318757 questions-0.7.1/questions/templates/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      305 2020-09-28 19:55:48.000000 questions-0.7.1/questions/templates/survey_html.angular.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      355 2020-09-29 04:05:16.000000 questions-0.7.1/questions/templates/survey_html.jquery.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      376 2020-09-28 19:57:51.000000 questions-0.7.1/questions/templates/survey_html.ko.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      372 2020-09-29 04:05:36.000000 questions-0.7.1/questions/templates/survey_html.react.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      426 2020-09-29 04:05:50.000000 questions-0.7.1/questions/templates/survey_html.vue.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2930 2020-10-02 03:33:35.000000 questions-0.7.1/questions/templates/survey_js.angular.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2370 2020-10-02 03:33:40.000000 questions-0.7.1/questions/templates/survey_js.jquery.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2336 2020-10-02 03:33:47.000000 questions-0.7.1/questions/templates/survey_js.ko.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2413 2020-10-02 03:33:54.000000 questions-0.7.1/questions/templates/survey_js.react.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2390 2020-10-02 03:34:01.000000 questions-0.7.1/questions/templates/survey_js.vue.jinja
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4611 2022-09-18 05:39:46.000000 questions-0.7.1/questions/templates.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      386 2020-12-13 21:46:14.000000 questions-0.7.1/questions/utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4903 2020-09-30 06:19:31.000000 questions-0.7.1/questions/validators.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.318757 questions-0.7.1/questions.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8735 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2295 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      160 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/entry_points.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2020-12-15 08:51:46.000000 questions-0.7.1/questions.egg-info/not-zip-safe
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       63 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2022-09-18 06:17:51.000000 questions-0.7.1/questions.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      406 2022-09-18 06:17:51.318757 questions-0.7.1/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1776 2022-09-18 06:07:56.000000 questions-0.7.1/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-09-18 06:17:51.318757 questions-0.7.1/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       39 2020-08-15 18:52:11.000000 questions-0.7.1/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1162 2020-09-29 22:34:48.000000 questions-0.7.1/tests/test_cli.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8670 2020-12-15 17:52:30.000000 questions-0.7.1/tests/test_form.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2607 2022-09-18 05:54:26.000000 questions-0.7.1/tests/test_templates.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2570 2020-09-29 22:36:25.000000 questions-0.7.1/tests/test_validators.py
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.941492 questions-0.8.0/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      164 2023-03-03 03:25:24.000000 questions-0.8.0/AUTHORS.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     3525 2023-03-03 04:16:39.000000 questions-0.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     1511 2023-04-10 23:20:14.000000 questions-0.8.0/HISTORY.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     1079 2023-03-03 03:25:24.000000 questions-0.8.0/LICENSE
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      305 2023-03-03 03:25:24.000000 questions-0.8.0/MANIFEST.in
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     9047 2023-04-11 00:04:55.941492 questions-0.8.0/PKG-INFO
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     6673 2023-03-03 03:25:24.000000 questions-0.8.0/README.rst
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/docs/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      610 2023-03-03 03:25:24.000000 questions-0.8.0/docs/Makefile
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.933492 questions-0.8.0/docs/_build/
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.933492 questions-0.8.0/docs/_build/html/
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/docs/_build/html/_sources/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       28 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/authors.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       33 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/contributing.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       28 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/history.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      604 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     4792 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       64 2023-03-03 05:00:08.000000 questions-0.8.0/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      130 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.cli.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      133 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.form.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      148 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.questions.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      350 2023-03-03 05:00:08.000000 questions-0.8.0/docs/_build/html/_sources/questions.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      145 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.settings.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      148 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.templates.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      133 2023-03-03 04:40:54.000000 questions-0.8.0/docs/_build/html/_sources/questions.utils.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      151 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/questions.validators.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       27 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/readme.rst.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)    15335 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_sources/usage.rst.txt
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/docs/_build/html/_static/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       31 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_build/html/_static/README.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      286 2023-03-03 04:40:07.000000 questions-0.8.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       90 2023-03-03 04:40:07.000000 questions-0.8.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       90 2023-03-03 04:40:07.000000 questions-0.8.0/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/docs/_static/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       31 2023-03-03 03:25:24.000000 questions-0.8.0/docs/_static/README.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       28 2023-03-03 03:25:24.000000 questions-0.8.0/docs/authors.rst
+-rwxrwxr-x   0 cguardia  (1000) cguardia  (1000)     5327 2023-03-03 03:25:24.000000 questions-0.8.0/docs/conf.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       33 2023-03-03 03:25:24.000000 questions-0.8.0/docs/contributing.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       28 2023-03-03 03:25:24.000000 questions-0.8.0/docs/history.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      604 2023-03-03 03:25:24.000000 questions-0.8.0/docs/index.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     4915 2023-04-10 22:49:05.000000 questions-0.8.0/docs/installation.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      771 2023-03-03 03:25:24.000000 questions-0.8.0/docs/make.bat
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       64 2023-03-03 05:00:08.000000 questions-0.8.0/docs/modules.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      130 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.cli.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      133 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.form.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      148 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.questions.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      350 2023-03-03 05:00:08.000000 questions-0.8.0/docs/questions.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      145 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.settings.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      148 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.templates.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      133 2023-03-03 04:40:54.000000 questions-0.8.0/docs/questions.utils.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      151 2023-03-03 03:25:24.000000 questions-0.8.0/docs/questions.validators.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       27 2023-03-03 03:25:24.000000 questions-0.8.0/docs/readme.rst
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      177 2023-04-10 05:24:52.000000 questions-0.8.0/docs/requirements.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      223 2023-03-03 03:25:24.000000 questions-0.8.0/docs/spelling_word_list.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)    15335 2023-03-03 03:25:24.000000 questions-0.8.0/docs/usage.rst
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/questions/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2568 2023-03-03 03:25:24.000000 questions-0.8.0/questions/__init__.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     5234 2023-04-10 05:29:30.000000 questions-0.8.0/questions/cli.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)    20035 2023-04-10 22:42:33.000000 questions-0.8.0/questions/form.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)    25536 2023-03-03 03:25:24.000000 questions-0.8.0/questions/questions.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)    14517 2023-04-10 22:30:27.000000 questions-0.8.0/questions/settings.py
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.941492 questions-0.8.0/questions/templates/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      305 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_html.angular.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      355 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_html.jquery.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      376 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_html.ko.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      372 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_html.react.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      426 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_html.vue.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2930 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_js.angular.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2370 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_js.jquery.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2336 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_js.ko.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2413 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_js.react.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2390 2023-03-03 03:25:24.000000 questions-0.8.0/questions/templates/survey_js.vue.jinja
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     4679 2023-04-10 22:43:15.000000 questions-0.8.0/questions/templates.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      386 2023-03-03 03:25:24.000000 questions-0.8.0/questions/utils.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     4903 2023-03-03 03:25:24.000000 questions-0.8.0/questions/validators.py
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.937492 questions-0.8.0/questions.egg-info/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     9047 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/PKG-INFO
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2370 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/SOURCES.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)        1 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/dependency_links.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      160 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/entry_points.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)        1 2023-03-03 04:27:42.000000 questions-0.8.0/questions.egg-info/not-zip-safe
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       63 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/requires.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       10 2023-04-11 00:04:55.000000 questions-0.8.0/questions.egg-info/top_level.txt
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)      406 2023-04-11 00:04:55.941492 questions-0.8.0/setup.cfg
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     1705 2023-04-10 23:05:29.000000 questions-0.8.0/setup.py
+drwxrwxr-x   0 cguardia  (1000) cguardia  (1000)        0 2023-04-11 00:04:55.941492 questions-0.8.0/tests/
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)       39 2023-03-03 03:25:24.000000 questions-0.8.0/tests/__init__.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     1162 2023-03-03 03:25:24.000000 questions-0.8.0/tests/test_cli.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     8670 2023-03-03 03:25:24.000000 questions-0.8.0/tests/test_form.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2615 2023-04-10 22:53:28.000000 questions-0.8.0/tests/test_templates.py
+-rw-rw-r--   0 cguardia  (1000) cguardia  (1000)     2570 2023-03-03 03:25:24.000000 questions-0.8.0/tests/test_validators.py
```

### Comparing `questions-0.7.1/CONTRIBUTING.rst` & `questions-0.8.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.6, 3.7 and 3.8, and for PyPy. Check
+3. The pull request should work for Python 3.8, 3.9, 3.10, 3.11, and for PyPy. Check
    https://travis-ci.com/cguardia/questions/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `questions-0.7.1/HISTORY.rst` & `questions-0.8.0/HISTORY.rst`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 * Add feature for creating Form subclasses from JSON data.
 
 * Add screencast to README page.
 
 * Update docs.
 
-* Update dependencies to lastest versions.
+* Update dependencies to latest versions.
 
 0.5.0a2 (2020-12-09)
 --------------------
 
 * Fix bug with form parameters in from_json conversion.
 
 0.5.0a3 (2020-12-10)
@@ -33,15 +33,15 @@
 
 0.7.0a4 (2020-12-13)
 --------------------
 
 * Update installation docs to mention typing-extensions requirement for
   Python < 3.8.
 
-* Use correct default value for allow_clear in sugnature pad.
+* Use correct default value for allow_clear in signature pad.
 
 * Set type hints to allow localization arrays in visible text properties.
 
 * Fix bug when generating classes from JSON with dynamic panels.
 
 * Add string representation methods to main classes.
 
@@ -49,7 +49,18 @@
   from_json method.
 
 0.7.1 (2022-09-18)
 ------------------
 
 * Bug fix: do not add a default page when other pages are defined.
 * Update js CDN and tests.
+
+0.8.0 (2023-04-10)
+------------------
+
+* Bug fix: fix choices with translatable text (thanks @joan-qida).
+* Bug fix: fix read the docs build.
+* Update SurveyJS version.
+* Use current SurveyJS supported themes.
+* Include newer Python versions in tests.
+* Add documentation for i18n.
+* Various dependency updates.
```

### Comparing `questions-0.7.1/LICENSE` & `questions-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/PKG-INFO` & `questions-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questions
-Version: 0.7.1
+Version: 0.8.0
 Summary: Questions is a form library that uses the power of SurveyJS for the UI.
 Home-page: https://github.com/cguardia/questions
 Author: Carlos de la Guardia
 Author-email: cguardia@yahoo.com
 License: MIT license
 Keywords: questions
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =========
 Questions
 =========
 
@@ -217,15 +217,15 @@
 
 * Add feature for creating Form subclasses from JSON data.
 
 * Add screencast to README page.
 
 * Update docs.
 
-* Update dependencies to lastest versions.
+* Update dependencies to latest versions.
 
 0.5.0a2 (2020-12-09)
 --------------------
 
 * Fix bug with form parameters in from_json conversion.
 
 0.5.0a3 (2020-12-10)
@@ -235,15 +235,15 @@
 
 0.7.0a4 (2020-12-13)
 --------------------
 
 * Update installation docs to mention typing-extensions requirement for
   Python < 3.8.
 
-* Use correct default value for allow_clear in sugnature pad.
+* Use correct default value for allow_clear in signature pad.
 
 * Set type hints to allow localization arrays in visible text properties.
 
 * Fix bug when generating classes from JSON with dynamic panels.
 
 * Add string representation methods to main classes.
 
@@ -251,7 +251,18 @@
   from_json method.
 
 0.7.1 (2022-09-18)
 ------------------
 
 * Bug fix: do not add a default page when other pages are defined.
 * Update js CDN and tests.
+
+0.8.0 (2023-04-10)
+------------------
+
+* Bug fix: fix choices with translatable text (thanks @joan-qida).
+* Bug fix: fix read the docs build.
+* Update SurveyJS version.
+* Use current SurveyJS supported themes.
+* Include newer Python versions in tests.
+* Add documentation for i18n.
+* Various dependency updates.
```

### Comparing `questions-0.7.1/README.rst` & `questions-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/docs/Makefile` & `questions-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/docs/_build/html/_sources/index.rst.txt` & `questions-0.8.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/docs/_build/html/_sources/installation.rst.txt` & `questions-0.8.0/docs/_build/html/_sources/installation.rst.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 .. code-block:: console
 
     $ pip install questions
 
 This is the preferred method to install Questions, as it will always install the most recent stable release.
 
+If you are using Python 3.7 or earlier, you will need to install the typing-extensions
+package too. This is not required from Python 3.8 onwards.
+
+.. code-block:: console
+
+    $ pip install typing-extensions
+
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
```

#### html2text {}

```diff
@@ -1,31 +1,34 @@
 .. highlight:: shell ============ Installation ============ Stable release ----
 ---------- To install Questions, run this command in your terminal: .. code-
 block:: console $ pip install questions This is the preferred method to install
-Questions, as it will always install the most recent stable release. If you
-don't have `pip`_ installed, this `Python installation guide`_ can guide you
-through the process. .. _pip: https://pip.pypa.io .. _Python installation
-guide: http://docs.python-guide.org/en/latest/starting/installation/ From
-sources ------------ The sources for Questions can be downloaded from the
-`Github repo`_. You can either clone the public repository: .. code-block::
-console $ git clone git://github.com/cguardia/questions Or download the
-`tarball`_: .. code-block:: console $ curl -OJL https://github.com/cguardia/
-questions/tarball/master Once you have a copy of the source, you can install it
-with: .. code-block:: console $ python setup.py install .. _Github repo: https:
-//github.com/cguardia/questions .. _tarball: https://github.com/cguardia/
-questions/tarball/master Installing SurveyJS locally --------------------------
-- Questions can be used without installing the SurveyJS Javascript resources,
-because by default it gets all resources from a CDN, but sometimes it's
-necessary to install all resources locally. Questions does its best to make
-that as easy as possible. The easiest way to install SurveyJS is to use npm_.
-This is also the recommended way to go if your project will be using other JS
-modules. Simply add the SurveyJS module corresponding to your platform to the
-dependencies section in your ``package.json`` file: - survey-angular - survey-
-jquery - survey-knockout - survey-react - survey-vue It's also necessary to add
-the SurveyJS custom widgets (`surveyjs-widgets`), since they are included in
+Questions, as it will always install the most recent stable release. If you are
+using Python 3.7 or earlier, you will need to install the typing-extensions
+package too. This is not required from Python 3.8 onwards. .. code-block::
+console $ pip install typing-extensions If you don't have `pip`_ installed,
+this `Python installation guide`_ can guide you through the process. .. _pip:
+https://pip.pypa.io .. _Python installation guide: http://docs.python-
+guide.org/en/latest/starting/installation/ From sources ------------ The
+sources for Questions can be downloaded from the `Github repo`_. You can either
+clone the public repository: .. code-block:: console $ git clone git://
+github.com/cguardia/questions Or download the `tarball`_: .. code-block::
+console $ curl -OJL https://github.com/cguardia/questions/tarball/master Once
+you have a copy of the source, you can install it with: .. code-block:: console
+$ python setup.py install .. _Github repo: https://github.com/cguardia/
+questions .. _tarball: https://github.com/cguardia/questions/tarball/master
+Installing SurveyJS locally --------------------------- Questions can be used
+without installing the SurveyJS Javascript resources, because by default it
+gets all resources from a CDN, but sometimes it's necessary to install all
+resources locally. Questions does its best to make that as easy as possible.
+The easiest way to install SurveyJS is to use npm_. This is also the
+recommended way to go if your project will be using other JS modules. Simply
+add the SurveyJS module corresponding to your platform to the dependencies
+section in your ``package.json`` file: - survey-angular - survey-jquery -
+survey-knockout - survey-react - survey-vue It's also necessary to add the
+SurveyJS custom widgets (`surveyjs-widgets`), since they are included in
 Questions. If you have ``npm`` available, but are not building a JS application
 and only want the SurveyJS resources, create a directory for static resources
 in your Python web application project, and do the following: .. code-block::
 console $ mkdir static $ cd static $ npm install survey-knockout $ npm install
 surveyjs-widgets These commands will download the complete set of resources for
 the selected platform. After they complete successfully, the files will be
 under `./static/node_modules/`. If ``npm`` is not available, or you can't use
```

### Comparing `questions-0.7.1/docs/_build/html/_sources/usage.rst.txt` & `questions-0.8.0/docs/_build/html/_sources/usage.rst.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,24 @@
             }
         ]
     }
     """
 
     PreferencesForm = Form.from_json(json, "PreferencesForm")
 
+The forms generated using the ``from_json`` class method are dynamic types
+that have no code equivalent. Questions includes a console script that can
+generate actual Python code for these forms::
+
+.. code-block:: console
+
+    $ generate_code {class_name} path/to/file.json
+
+All the script needs is a class name for the generated form class, and the
+path to the JSON file with the SurveyJS form definition.
                   
 Displaying the forms
 ====================
 
 Questions generates a SurveyJS form, which requires a few Javascript and CSS
 resources to work. The simplest way to display a form is to use the SurveyJS
 CDN to serve all these resources, which requires no work and is the default
@@ -401,7 +411,55 @@
             return form.render_html(form_data=form_data)
 
 This example demonstrates a common pattern for responding to form POST
 requests. If the validation is successful, the data is saved, and then we
 return a redirection to the success or thanks page. If validation fails,
 we redisplay the form with the data that was sent, and the errors will be
 highlighted.
+
+Internationalization
+====================
+
+SurveyJS supports many different languages, and ``questions`` makes it easy to
+tale advantage of that. Simply pass in the locale when instantiating a form::
+
+    form = YourFormSubclass(title="Formulaire en français", locale="fr")
+
+The current list of supported locales is below.
+
+- ar
+- bg
+- ca
+- cs
+- da
+- de
+- en
+- es
+- et
+- fa
+- fi
+- fr
+- gr
+- he
+- hu
+- id
+- is
+- it
+- ja
+- ka
+- ko
+- lt
+- lv
+- nl
+- no
+- pl
+- pt
+- ro
+- ru
+- sv
+- sw
+- tg
+- th
+- tr
+- ua
+- zh-cn
+- zh-tw
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `questions-0.7.1/docs/conf.py` & `questions-0.8.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,47 +15,48 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import questions
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode',
-    'sphinx_autodoc_typehints',
-    'sphinxcontrib.spelling',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx_autodoc_typehints",
+    "sphinxcontrib.spelling",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'Questions'
+project = "Questions"
 copyright = "2020, Carlos de la Guardia"
 author = "Carlos de la Guardia"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -70,29 +71,29 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     "page_width": "1200px",
@@ -101,77 +102,77 @@
     "github_banner": "true",
     "github_button": "false",
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'questionsdoc'
+htmlhelp_basename = "questionsdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'questions.tex',
-     'Questions Documentation',
-     'Carlos de la Guardia', 'manual'),
+    (
+        master_doc,
+        "questions.tex",
+        "Questions Documentation",
+        "Carlos de la Guardia",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'questions',
-     'Questions Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "questions", "Questions Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'questions',
-     'Questions Documentation',
-     author,
-     'questions',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "questions",
+        "Questions Documentation",
+        author,
+        "questions",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Options for spell checking ----------------------------------------
 
 # File containing list of words known to be spelled correctly, but not in
 # the dictionary.
-spelling_word_list_filename = 'spelling_word_list.txt'
+spelling_word_list_filename = "spelling_word_list.txt"
```

### Comparing `questions-0.7.1/docs/index.rst` & `questions-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/docs/installation.rst` & `questions-0.8.0/docs/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -184,117 +184,125 @@
 00000b70: 7220 7b70 6c61 7466 6f72 6d7d 207b 7468  r {platform} {th
 00000b80: 656d 657d 0a0a 5468 6520 706c 6174 666f  eme}..The platfo
 00000b90: 726d 7320 6172 653a 0a0a 202d 2061 6e67  rms are:.. - ang
 00000ba0: 756c 6172 0a20 2d20 6a71 7565 7279 0a20  ular. - jquery. 
 00000bb0: 2d20 6b6e 6f63 6b6f 7574 0a20 2d20 7265  - knockout. - re
 00000bc0: 6163 740a 202d 2076 7565 0a0a 5468 6520  act. - vue..The 
 00000bd0: 7468 656d 6573 2061 7265 3a0a 0a20 2d20  themes are:.. - 
-00000be0: 6465 6661 756c 740a 202d 2062 6f6f 7473  default. - boots
-00000bf0: 7472 6170 0a20 2d20 6461 726b 626c 7565  trap. - darkblue
-00000c00: 0a20 2d20 6461 726b 726f 7365 0a20 2d20  . - darkrose. - 
-00000c10: 6d6f 6465 726e 0a20 2d20 6f72 616e 6765  modern. - orange
-00000c20: 0a20 2d20 7374 6f6e 650a 202d 2077 696e  . - stone. - win
-00000c30: 7465 720a 202d 2077 696e 7465 7273 746f  ter. - wintersto
-00000c40: 6e65 0a0a 5468 6973 2063 6f6d 6d61 6e64  ne..This command
-00000c50: 2077 696c 6c20 646f 776e 6c6f 6164 2061   will download a
-00000c60: 6c6c 2074 6865 2072 6571 7569 7265 6420  ll the required 
-00000c70: 7265 736f 7572 6365 7320 746f 2074 6865  resources to the
-00000c80: 2064 6972 6563 746f 7279 2073 7065 6369   directory speci
-00000c90: 6669 6564 2e0a 5468 6973 2069 7320 6279  fied..This is by
-00000ca0: 2066 6172 2074 6865 2073 696d 706c 6573   far the simples
-00000cb0: 7420 7761 7920 746f 2067 6574 2072 756e  t way to get run
-00000cc0: 6e69 6e67 2069 6620 796f 7520 646f 6e27  ning if you don'
-00000cd0: 7420 706c 616e 2074 6f20 646f 2061 6e79  t plan to do any
-00000ce0: 0a6a 6176 6173 6372 6970 7420 6465 7665  .javascript deve
-00000cf0: 6c6f 706d 656e 7420 6173 2070 6172 7420  lopment as part 
-00000d00: 6f66 2079 6f75 7220 6170 706c 6963 6174  of your applicat
-00000d10: 696f 6e2e 0a0a 496e 6465 7065 6e64 656e  ion...Independen
-00000d20: 746c 7920 6f66 2074 6865 206d 6574 686f  tly of the metho
-00000d30: 6420 796f 7520 7573 6520 746f 2064 6f77  d you use to dow
-00000d40: 6e6c 6f61 6420 7468 6520 7265 736f 7572  nload the resour
-00000d50: 6365 732e 2059 6f75 2077 696c 6c20 6e65  ces. You will ne
-00000d60: 6564 2074 6f0a 7365 7420 7570 2079 6f75  ed to.set up you
-00000d70: 7220 6170 706c 6963 6174 696f 6e20 746f  r application to
-00000d80: 2075 7365 2074 6865 2072 6573 756c 7469   use the resulti
-00000d90: 6e67 2072 6573 6f75 7263 6520 6469 7265  ng resource dire
-00000da0: 6374 6f72 792e 2049 6620 616c 6c0a 7265  ctory. If all.re
-00000db0: 736f 7572 6365 7320 6172 6520 7072 6573  sources are pres
-00000dc0: 656e 7420 696e 2074 6865 2073 616d 6520  ent in the same 
-00000dd0: 6469 7265 6374 6f72 792c 2061 6c6c 2074  directory, all t
-00000de0: 6861 7420 6973 206e 6565 6465 6420 6973  hat is needed is
-00000df0: 2074 6f20 7061 7373 2069 6e0a 7468 6520   to pass in.the 
-00000e00: 5552 4c20 666f 7220 7468 6973 2064 6972  URL for this dir
-00000e10: 6563 746f 7279 2077 6865 6e20 6372 6561  ectory when crea
-00000e20: 7469 6e67 2074 6865 2066 6f72 6d2c 206c  ting the form, l
-00000e30: 696b 6520 7468 6973 3a3a 0a0a 2020 2020  ike this::..    
-00000e40: 666f 726d 203d 2046 6f72 6d28 7265 736f  form = Form(reso
-00000e50: 7572 6365 5f75 726c 3d22 2f73 7461 7469  urce_url="/stati
-00000e60: 632f 796f 7572 2f70 6174 6822 290a 0a49  c/your/path")..I
-00000e70: 6620 7468 6520 7265 736f 7572 6365 7320  f the resources 
-00000e80: 6172 6520 7374 6f72 6564 2075 7369 6e67  are stored using
-00000e90: 2060 606e 706d 6060 206f 7220 6120 6469   ``npm`` or a di
-00000ea0: 6666 6572 656e 7420 6469 7265 6374 6f72  fferent director
-00000eb0: 7920 6c61 796f 7574 2c20 6974 0a77 696c  y layout, it.wil
-00000ec0: 6c20 6265 206e 6563 6573 7361 7279 2074  l be necessary t
-00000ed0: 6f20 6164 6420 7468 6520 7265 736f 7572  o add the resour
-00000ee0: 6365 2064 6566 696e 6974 696f 6e73 2074  ce definitions t
-00000ef0: 6f20 7468 6520 4854 4d4c 2074 656d 706c  o the HTML templ
-00000f00: 6174 6573 2062 7920 6861 6e64 2e0a 486f  ates by hand..Ho
-00000f10: 7720 746f 2064 6f20 7468 6973 2076 6172  w to do this var
-00000f20: 6965 7320 6672 6f6d 2066 7261 6d65 776f  ies from framewo
-00000f30: 726b 2074 6f20 6672 616d 6577 6f72 6b2e  rk to framework.
-00000f40: 2049 6e20 466c 6173 6b2c 2074 6865 2066   In Flask, the f
-00000f50: 6f6c 6c6f 7769 6e67 2077 696c 6c0a 776f  ollowing will.wo
-00000f60: 726b 2c20 6173 7375 6d69 6e67 2079 6f75  rk, assuming you
-00000f70: 2061 7265 2075 7369 6e67 2074 6865 2064   are using the d
-00000f80: 6566 6175 6c74 2060 7374 6174 6963 6020  efault `static` 
-00000f90: 6469 7265 6374 6f72 793a 0a0a 2e2e 2063  directory:.... c
-00000fa0: 6f64 652d 626c 6f63 6b3a 3a20 6874 6d6c  ode-block:: html
-00000fb0: 2b6a 696e 6a61 0a0a 2020 2020 3c73 6372  +jinja..    <scr
-00000fc0: 6970 7420 7372 633d 227b 7b20 7572 6c5f  ipt src="{{ url_
-00000fd0: 666f 7228 2773 7461 7469 6327 2c0a 2020  for('static',.  
-00000fe0: 2020 2020 2020 6669 6c65 6e61 6d65 3d27        filename='
-00000ff0: 6e70 6d5f 6d6f 6475 6c65 732f 7375 7276  npm_modules/surv
-00001000: 6579 2d6b 6e6f 636b 6f75 742f 7375 7276  ey-knockout/surv
-00001010: 6579 2e6b 6f2e 6d69 6e2e 6a73 2729 207d  ey.ko.min.js') }
-00001020: 7d22 3e0a 2020 2020 3c2f 7363 7269 7074  }">.    </script
-00001030: 3e0a 0a20 2020 203c 6c69 6e6b 2072 656c  >..    <link rel
-00001040: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-00001050: 6566 3d22 7b7b 2075 726c 5f66 6f72 2827  ef="{{ url_for('
-00001060: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
-00001070: 2066 696c 656e 616d 653d 276e 706d 5f6d   filename='npm_m
-00001080: 6f64 756c 6573 2f73 7572 7665 792d 6b6e  odules/survey-kn
-00001090: 6f63 6b6f 7574 2f73 7572 7665 792e 6373  ockout/survey.cs
-000010a0: 7327 2920 7d7d 2220 2f3e 0a0a 5265 736f  s') }}" />..Reso
-000010b0: 7572 6365 7320 7661 7279 2062 7920 706c  urces vary by pl
-000010c0: 6174 666f 726d 2c20 7468 656d 6520 616e  atform, theme an
-000010d0: 6420 7479 7065 7320 6f66 2071 7565 7374  d types of quest
-000010e0: 696f 6e73 2075 7365 642e 2054 6f20 6d61  ions used. To ma
-000010f0: 6b65 2073 7572 6520 796f 750a 6861 7665  ke sure you.have
-00001100: 2061 6c6c 2074 6865 2072 6571 7569 7265   all the require
-00001110: 6420 7265 736f 7572 6365 7320 666f 7220  d resources for 
-00001120: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-00001130: 2c20 5175 6573 7469 6f6e 7320 696e 636c  , Questions incl
-00001140: 7564 6573 2061 0a73 6372 6970 7420 746f  udes a.script to
-00001150: 206c 6973 7420 7468 656d 3a0a 0a2e 2e20   list them:.... 
-00001160: 636f 6465 2d62 6c6f 636b 3a3a 2063 6f6e  code-block:: con
-00001170: 736f 6c65 0a0a 2020 2020 2420 6c69 7374  sole..    $ list
-00001180: 5f72 6573 6f75 7263 6573 207b 706c 6174  _resources {plat
-00001190: 666f 726d 7d20 7b74 6865 6d65 7d0a 0a54  form} {theme}..T
-000011a0: 6869 7320 7769 6c6c 206c 6973 7420 616c  his will list al
-000011b0: 6c20 7265 7175 6972 6564 2072 6573 6f75  l required resou
-000011c0: 7263 6573 2e20 4e6f 7465 2074 6861 7420  rces. Note that 
-000011d0: 6375 7374 6f6d 2077 6964 6765 7473 2c20  custom widgets, 
-000011e0: 6c69 6b65 2053 656c 6563 7432 2c0a 7265  like Select2,.re
-000011f0: 7175 6972 6520 6578 7472 6120 4a53 2061  quire extra JS a
-00001200: 6e64 2043 5353 2072 6573 6f75 7263 6573  nd CSS resources
-00001210: 2e20 546f 2066 696e 6420 6f75 7420 6966  . To find out if
-00001220: 2074 6865 2071 7565 7374 696f 6e20 7479   the question ty
-00001230: 7065 7320 796f 7520 6172 650a 7573 696e  pes you are.usin
-00001240: 6720 6465 7065 6e64 206f 6e20 6578 7472  g depend on extr
-00001250: 6120 7265 736f 7572 6365 732c 2061 6464  a resources, add
-00001260: 2074 6865 2060 272d 2d69 6e63 6c75 6465   the `'--include
-00001270: 2d77 6964 6765 7473 6060 2066 6c61 6720  -widgets`` flag 
-00001280: 746f 2074 6865 0a63 6f6d 6d61 6e64 2e0a  to the.command..
-00001290: 0a2e 2e20 5f6e 706d 3a20 6874 7470 733a  ... _npm: https:
-000012a0: 2f2f 7777 772e 6e70 6d6a 732e 636f 6d2f  //www.npmjs.com/
-000012b0: 6765 742d 6e70 6d0a                      get-npm.
+00000be0: 6465 6661 756c 7420 286c 6567 6163 7929  default (legacy)
+00000bf0: 0a20 2d20 6465 6661 756c 7456 320a 202d  . - defaultV2. -
+00000c00: 2062 6f6f 7473 7472 6170 2028 6c65 6761   bootstrap (lega
+00000c10: 6379 290a 202d 206d 6f64 6572 6e0a 0a54  cy). - modern..T
+00000c20: 6865 2064 6566 6175 6c74 2074 6865 6d65  he default theme
+00000c30: 2069 7320 6e61 6d65 6420 6060 6465 6661   is named ``defa
+00000c40: 756c 7456 3260 602e 2054 6865 7265 2069  ultV2``. There i
+00000c50: 7320 616e 206f 6c64 6572 2064 6566 6175  s an older defau
+00000c60: 6c74 2074 6865 6d65 2074 6861 7420 6973  lt theme that is
+00000c70: 0a6e 6f77 2063 6f6e 7369 6465 7265 6420  .now considered 
+00000c80: 6c65 6761 6379 2e20 5468 6520 6f6c 6420  legacy. The old 
+00000c90: 626f 6f74 7374 7261 7020 7468 656d 6520  bootstrap theme 
+00000ca0: 6973 2061 6c73 6f20 6c65 6761 6379 2061  is also legacy a
+00000cb0: 6e64 2064 6570 7265 6361 7465 642e 0a54  nd deprecated..T
+00000cc0: 6869 7320 636f 6d6d 616e 6420 7769 6c6c  his command will
+00000cd0: 2064 6f77 6e6c 6f61 6420 616c 6c20 7468   download all th
+00000ce0: 6520 7265 7175 6972 6564 2072 6573 6f75  e required resou
+00000cf0: 7263 6573 2074 6f20 7468 6520 6469 7265  rces to the dire
+00000d00: 6374 6f72 7920 7370 6563 6966 6965 642e  ctory specified.
+00000d10: 0a54 6869 7320 6973 2062 7920 6661 7220  .This is by far 
+00000d20: 7468 6520 7369 6d70 6c65 7374 2077 6179  the simplest way
+00000d30: 2074 6f20 6765 7420 7275 6e6e 696e 6720   to get running 
+00000d40: 6966 2079 6f75 2064 6f6e 2774 2070 6c61  if you don't pla
+00000d50: 6e20 746f 2064 6f20 616e 790a 6a61 7661  n to do any.java
+00000d60: 7363 7269 7074 2064 6576 656c 6f70 6d65  script developme
+00000d70: 6e74 2061 7320 7061 7274 206f 6620 796f  nt as part of yo
+00000d80: 7572 2061 7070 6c69 6361 7469 6f6e 2e0a  ur application..
+00000d90: 0a49 6e64 6570 656e 6465 6e74 6c79 206f  .Independently o
+00000da0: 6620 7468 6520 6d65 7468 6f64 2079 6f75  f the method you
+00000db0: 2075 7365 2074 6f20 646f 776e 6c6f 6164   use to download
+00000dc0: 2074 6865 2072 6573 6f75 7263 6573 2e20   the resources. 
+00000dd0: 596f 7520 7769 6c6c 206e 6565 6420 746f  You will need to
+00000de0: 0a73 6574 2075 7020 796f 7572 2061 7070  .set up your app
+00000df0: 6c69 6361 7469 6f6e 2074 6f20 7573 6520  lication to use 
+00000e00: 7468 6520 7265 7375 6c74 696e 6720 7265  the resulting re
+00000e10: 736f 7572 6365 2064 6972 6563 746f 7279  source directory
+00000e20: 2e20 4966 2061 6c6c 0a72 6573 6f75 7263  . If all.resourc
+00000e30: 6573 2061 7265 2070 7265 7365 6e74 2069  es are present i
+00000e40: 6e20 7468 6520 7361 6d65 2064 6972 6563  n the same direc
+00000e50: 746f 7279 2c20 616c 6c20 7468 6174 2069  tory, all that i
+00000e60: 7320 6e65 6564 6564 2069 7320 746f 2070  s needed is to p
+00000e70: 6173 7320 696e 0a74 6865 2055 524c 2066  ass in.the URL f
+00000e80: 6f72 2074 6869 7320 6469 7265 6374 6f72  or this director
+00000e90: 7920 7768 656e 2063 7265 6174 696e 6720  y when creating 
+00000ea0: 7468 6520 666f 726d 2c20 6c69 6b65 2074  the form, like t
+00000eb0: 6869 733a 3a0a 0a20 2020 2066 6f72 6d20  his::..    form 
+00000ec0: 3d20 466f 726d 2872 6573 6f75 7263 655f  = Form(resource_
+00000ed0: 7572 6c3d 222f 7374 6174 6963 2f79 6f75  url="/static/you
+00000ee0: 722f 7061 7468 2229 0a0a 4966 2074 6865  r/path")..If the
+00000ef0: 2072 6573 6f75 7263 6573 2061 7265 2073   resources are s
+00000f00: 746f 7265 6420 7573 696e 6720 6060 6e70  tored using ``np
+00000f10: 6d60 6020 6f72 2061 2064 6966 6665 7265  m`` or a differe
+00000f20: 6e74 2064 6972 6563 746f 7279 206c 6179  nt directory lay
+00000f30: 6f75 742c 2069 740a 7769 6c6c 2062 6520  out, it.will be 
+00000f40: 6e65 6365 7373 6172 7920 746f 2061 6464  necessary to add
+00000f50: 2074 6865 2072 6573 6f75 7263 6520 6465   the resource de
+00000f60: 6669 6e69 7469 6f6e 7320 746f 2074 6865  finitions to the
+00000f70: 2048 544d 4c20 7465 6d70 6c61 7465 7320   HTML templates 
+00000f80: 6279 2068 616e 642e 0a48 6f77 2074 6f20  by hand..How to 
+00000f90: 646f 2074 6869 7320 7661 7269 6573 2066  do this varies f
+00000fa0: 726f 6d20 6672 616d 6577 6f72 6b20 746f  rom framework to
+00000fb0: 2066 7261 6d65 776f 726b 2e20 496e 2046   framework. In F
+00000fc0: 6c61 736b 2c20 7468 6520 666f 6c6c 6f77  lask, the follow
+00000fd0: 696e 6720 7769 6c6c 0a77 6f72 6b2c 2061  ing will.work, a
+00000fe0: 7373 756d 696e 6720 796f 7520 6172 6520  ssuming you are 
+00000ff0: 7573 696e 6720 7468 6520 6465 6661 756c  using the defaul
+00001000: 7420 6073 7461 7469 6360 2064 6972 6563  t `static` direc
+00001010: 746f 7279 3a0a 0a2e 2e20 636f 6465 2d62  tory:.... code-b
+00001020: 6c6f 636b 3a3a 2068 746d 6c2b 6a69 6e6a  lock:: html+jinj
+00001030: 610a 0a20 2020 203c 7363 7269 7074 2073  a..    <script s
+00001040: 7263 3d22 7b7b 2075 726c 5f66 6f72 2827  rc="{{ url_for('
+00001050: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
+00001060: 2066 696c 656e 616d 653d 276e 706d 5f6d   filename='npm_m
+00001070: 6f64 756c 6573 2f73 7572 7665 792d 6b6e  odules/survey-kn
+00001080: 6f63 6b6f 7574 2f73 7572 7665 792e 6b6f  ockout/survey.ko
+00001090: 2e6d 696e 2e6a 7327 2920 7d7d 223e 0a20  .min.js') }}">. 
+000010a0: 2020 203c 2f73 6372 6970 743e 0a0a 2020     </script>..  
+000010b0: 2020 3c6c 696e 6b20 7265 6c3d 2273 7479    <link rel="sty
+000010c0: 6c65 7368 6565 7422 2068 7265 663d 227b  lesheet" href="{
+000010d0: 7b20 7572 6c5f 666f 7228 2773 7461 7469  { url_for('stati
+000010e0: 6327 2c0a 2020 2020 2020 2020 6669 6c65  c',.        file
+000010f0: 6e61 6d65 3d27 6e70 6d5f 6d6f 6475 6c65  name='npm_module
+00001100: 732f 7375 7276 6579 2d6b 6e6f 636b 6f75  s/survey-knockou
+00001110: 742f 7375 7276 6579 2e63 7373 2729 207d  t/survey.css') }
+00001120: 7d22 202f 3e0a 0a52 6573 6f75 7263 6573  }" />..Resources
+00001130: 2076 6172 7920 6279 2070 6c61 7466 6f72   vary by platfor
+00001140: 6d2c 2074 6865 6d65 2061 6e64 2074 7970  m, theme and typ
+00001150: 6573 206f 6620 7175 6573 7469 6f6e 7320  es of questions 
+00001160: 7573 6564 2e20 546f 206d 616b 6520 7375  used. To make su
+00001170: 7265 2079 6f75 0a68 6176 6520 616c 6c20  re you.have all 
+00001180: 7468 6520 7265 7175 6972 6564 2072 6573  the required res
+00001190: 6f75 7263 6573 2066 6f72 2079 6f75 7220  ources for your 
+000011a0: 6170 706c 6963 6174 696f 6e2c 2051 7565  application, Que
+000011b0: 7374 696f 6e73 2069 6e63 6c75 6465 7320  stions includes 
+000011c0: 610a 7363 7269 7074 2074 6f20 6c69 7374  a.script to list
+000011d0: 2074 6865 6d3a 0a0a 2e2e 2063 6f64 652d   them:.... code-
+000011e0: 626c 6f63 6b3a 3a20 636f 6e73 6f6c 650a  block:: console.
+000011f0: 0a20 2020 2024 206c 6973 745f 7265 736f  .    $ list_reso
+00001200: 7572 6365 7320 7b70 6c61 7466 6f72 6d7d  urces {platform}
+00001210: 207b 7468 656d 657d 0a0a 5468 6973 2077   {theme}..This w
+00001220: 696c 6c20 6c69 7374 2061 6c6c 2072 6571  ill list all req
+00001230: 7569 7265 6420 7265 736f 7572 6365 732e  uired resources.
+00001240: 204e 6f74 6520 7468 6174 2063 7573 746f   Note that custo
+00001250: 6d20 7769 6467 6574 732c 206c 696b 6520  m widgets, like 
+00001260: 5365 6c65 6374 322c 0a72 6571 7569 7265  Select2,.require
+00001270: 2065 7874 7261 204a 5320 616e 6420 4353   extra JS and CS
+00001280: 5320 7265 736f 7572 6365 732e 2054 6f20  S resources. To 
+00001290: 6669 6e64 206f 7574 2069 6620 7468 6520  find out if the 
+000012a0: 7175 6573 7469 6f6e 2074 7970 6573 2079  question types y
+000012b0: 6f75 2061 7265 0a75 7369 6e67 2064 6570  ou are.using dep
+000012c0: 656e 6420 6f6e 2065 7874 7261 2072 6573  end on extra res
+000012d0: 6f75 7263 6573 2c20 6164 6420 7468 6520  ources, add the 
+000012e0: 6027 2d2d 696e 636c 7564 652d 7769 6467  `'--include-widg
+000012f0: 6574 7360 6020 666c 6167 2074 6f20 7468  ets`` flag to th
+00001300: 650a 636f 6d6d 616e 642e 0a0a 2e2e 205f  e.command..... _
+00001310: 6e70 6d3a 2068 7474 7073 3a2f 2f77 7777  npm: https://www
+00001320: 2e6e 706d 6a73 2e63 6f6d 2f67 6574 2d6e  .npmjs.com/get-n
+00001330: 706d 0a                                  pm.
```

### Comparing `questions-0.7.1/docs/make.bat` & `questions-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/docs/usage.rst` & `questions-0.8.0/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -411,7 +411,55 @@
             return form.render_html(form_data=form_data)
 
 This example demonstrates a common pattern for responding to form POST
 requests. If the validation is successful, the data is saved, and then we
 return a redirection to the success or thanks page. If validation fails,
 we redisplay the form with the data that was sent, and the errors will be
 highlighted.
+
+Internationalization
+====================
+
+SurveyJS supports many different languages, and ``questions`` makes it easy to
+tale advantage of that. Simply pass in the locale when instantiating a form::
+
+    form = YourFormSubclass(title="Formulaire en français", locale="fr")
+
+The current list of supported locales is below.
+
+- ar
+- bg
+- ca
+- cs
+- da
+- de
+- en
+- es
+- et
+- fa
+- fi
+- fr
+- gr
+- he
+- hu
+- id
+- is
+- it
+- ja
+- ka
+- ko
+- lt
+- lv
+- nl
+- no
+- pl
+- pt
+- ro
+- ru
+- sv
+- sw
+- tg
+- th
+- tr
+- ua
+- zh-cn
+- zh-tw
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `questions-0.7.1/questions/__init__.py` & `questions-0.8.0/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/cli.py` & `questions-0.8.0/questions/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Download SurveyJS files to specified location.
 
     Supplied path must exist.
 
     Platforms are: angular, jquery, knockout, react, vue.
 
-    Themes are: default, bootstrap, darkblue, darkrose, modern, orange, stone
+    Themes are: default, defaultV2, bootstrap, darkblue, darkrose, modern, orange, stone
                 winter, winterstone.
     """
     click.echo()
     js = get_platform_js_resources(platform=platform, resource_url=SURVEY_JS_CDN)
     css = get_theme_css_resources(theme=theme, resource_url=SURVEY_JS_CDN)
     widgets_js = set()
     widgets_css = set()
@@ -62,15 +62,15 @@
 )
 def list_resources(platform, theme, include_widgets):
     """
     List required resources for a platform and theme.
 
     Platforms are: angular, jquery, knockout, react, vue.
 
-    Themes are: default, bootstrap, darkblue, darkrose, modern, orange, stone
+    Themes are: default, defaultV2, bootstrap, darkblue, darkrose, modern, orange, stone
                 winter, winterstone.
     """
     click.echo()
     js = get_platform_js_resources(platform=platform, resource_url=SURVEY_JS_CDN)
     css = get_theme_css_resources(theme=theme, resource_url=SURVEY_JS_CDN)
     click.echo("Required Javascript resources:")
     for url in js:
```

### Comparing `questions-0.7.1/questions/form.py` & `questions-0.8.0/questions/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         The name of the form. If empty, the class name is used.
     :param action:
         The URL where the form data will be posted. If empty, the
         same URL for the form is used.
     :param html_id:
         The id for the div element that will be used to render the form.
     :param theme:
-        The name of the base theme for the form. Default value is 'default'.
+        The name of the base theme for the form. Default value is 'defaultV2'.
     :param platform:
         The JS platform to use for generating the form. Default value is 'jquery'.
     :param resource_url:
         The base URL for the theme resources. If provided,
         Questions will expect to find all resources under this URL. If
         empty, the SurveyJS CDN will be used for all resources.
     :param params:
@@ -80,15 +80,15 @@
         cls.questions_resource_url = url
 
     def __init__(
         self,
         name: str = "",
         action: str = "",
         html_id: str = "questions_form",
-        theme: Literal[SURVEY_JS_THEMES] = "default",
+        theme: Literal[SURVEY_JS_THEMES] = "defaultV2",
         platform: Literal[SURVEY_JS_PLATFORMS] = "jquery",
         resource_url: str = None,
         **params,
     ):
         if name == "":
             name = self.__class__.__name__
         self.name = name
```

### Comparing `questions-0.7.1/questions/questions.py` & `questions-0.8.0/questions/questions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     def __repr__(self):
         class_name = self.__class__.__name__
         params = get_params_for_repr(dict(self))
         return f"{class_name}({params}\n    )"
 
     class Config:
-
         fields = {
             "kind": "type",
             "all_rows_required": "isAllRowRequired",
             "expression_format": "format",
             "max_value": "max",
             "min_value": "min",
             "required": "isRequired",
@@ -157,15 +156,15 @@
     Base class for questions that let the user select one or more options
     from a list of choices. The choices can either be set at question
     instantiation time, or come from a JSON web service at run time.
     """
 
     kind: str = ""
     col_count: int = 4
-    choices: List[Union[str, Dict[str, Union[str, HttpUrl]]]] = []
+    choices: List[Union[str, Dict[str, Union[str, HttpUrl, Dict[str, str]]]]] = []
     choices_by_url: Dict[Literal[settings.CHOICES_BY_URL_KEYS], str] = []
     choices_order: Literal[settings.CHOICE_ORDER_VALUES] = "none"
     choices_enable_if: str = ""
     choices_visible_if: str = ""
     hide_if_choices_empty: bool = True
     has_other: bool = False
     other_text: Union[str, Dict[str, str]] = "Other"
```

### Comparing `questions-0.7.1/questions/settings.py` & `questions-0.8.0/questions/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Defines constants to be used throughout the code."""
 
-SURVEY_JS_VERSION = "1.8.2"
+SURVEY_JS_VERSION = "1.9.81"
 
 SURVEY_JS_CDN = "https://unpkg.com"
 
 SURVEY_JS_WIDGETS = "surveyjs-widgets/surveyjs-widgets.min.js"
 
 SURVEY_JS_PLATFORMS = (
     "angular",
@@ -556,22 +556,16 @@
     "default",
     "top",
     "bottom",
     "topBottom",
 )
 
 SURVEY_JS_THEMES = (
-    "default",
+    "defaultV2",
     "bootstrap",
-    "orange",
-    "darkblue",
-    "darkrose",
-    "stone",
-    "winter",
-    "winterstone",
     "modern",
 )
 
 BAR_RATING_THEMES = (
     "fontawesome-stars",
     "css-stars",
     "bars-pill",
```

### Comparing `questions-0.7.1/questions/templates/survey_js.angular.jinja` & `questions-0.8.0/questions/templates/survey_js.angular.jinja`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/templates/survey_js.jquery.jinja` & `questions-0.8.0/questions/templates/survey_js.jquery.jinja`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/templates/survey_js.ko.jinja` & `questions-0.8.0/questions/templates/survey_js.ko.jinja`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/templates/survey_js.react.jinja` & `questions-0.8.0/questions/templates/survey_js.react.jinja`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/templates/survey_js.vue.jinja` & `questions-0.8.0/questions/templates/survey_js.vue.jinja`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions/templates.py` & `questions-0.8.0/questions/templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
 
 from .settings import BOOTSTRAP_URL
 from .settings import SUGGESTED_JS_BY_PLATFORM
 from .settings import SURVEY_JS_CDN
+from .settings import SURVEY_JS_THEMES
 
 
 # Initialize Jinja environment
 env = Environment(
     loader=PackageLoader("questions", "templates"),
     autoescape=select_autoescape(["html", "xml"]),
 )
@@ -54,45 +55,44 @@
             filename = js.split("/")[-1]
             platform_js.append(f"{resource_url}/{filename}")
     platform_js.append(survey_js)
     return platform_js
 
 
 def get_theme_css_resources(
-    theme: str = "default",
+    theme: str = "defaultV2",
     resource_url: str = SURVEY_JS_CDN,
 ):
     """
     Get the list of suggested CSS resources for a theme. if not using the
-    CDN, only the main SurveyJS CSS file is returned.
+    CDN, or using an unsupported theme, only the main SurveyJS CSS file is returned.
 
     :param theme:
         The name of the CSS theme.
     :param resource_url:
         The URL where all SurveyJS resources are located.
 
     :Returns:
         The list of resource URLs.
     """
     if theme == "bootstrap" and resource_url == SURVEY_JS_CDN:
         return [BOOTSTRAP_URL]
     elif theme == "bootstrap":
         return [f"{resource_url}/bootstrap.min.css"]
-    name = "survey"
-    if theme == "modern":
-        name = "modern"
-    return [f"{resource_url}/survey-core/{name}.min.css"]
+    if theme not in SURVEY_JS_THEMES:
+        theme = "survey"
+    return [f"{resource_url}/survey-core/{theme}.min.css"]
 
 
 def get_survey_js(
     form_json: str = "",
     form_data: Dict[str, Any] = None,
     html_id: str = "questions_form",
     action: str = "",
-    theme: str = "default",
+    theme: str = "defaultV2",
     platform: str = "jquery",
 ):
     """
     Get the SurveyJS initialization script and form definition.
 
     :param form_json:
         The JSON generated from the questions form.
```

### Comparing `questions-0.7.1/questions/validators.py` & `questions-0.8.0/questions/validators.py`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/questions.egg-info/PKG-INFO` & `questions-0.8.0/questions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questions
-Version: 0.7.1
+Version: 0.8.0
 Summary: Questions is a form library that uses the power of SurveyJS for the UI.
 Home-page: https://github.com/cguardia/questions
 Author: Carlos de la Guardia
 Author-email: cguardia@yahoo.com
 License: MIT license
 Keywords: questions
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =========
 Questions
 =========
 
@@ -217,15 +217,15 @@
 
 * Add feature for creating Form subclasses from JSON data.
 
 * Add screencast to README page.
 
 * Update docs.
 
-* Update dependencies to lastest versions.
+* Update dependencies to latest versions.
 
 0.5.0a2 (2020-12-09)
 --------------------
 
 * Fix bug with form parameters in from_json conversion.
 
 0.5.0a3 (2020-12-10)
@@ -235,15 +235,15 @@
 
 0.7.0a4 (2020-12-13)
 --------------------
 
 * Update installation docs to mention typing-extensions requirement for
   Python < 3.8.
 
-* Use correct default value for allow_clear in sugnature pad.
+* Use correct default value for allow_clear in signature pad.
 
 * Set type hints to allow localization arrays in visible text properties.
 
 * Fix bug when generating classes from JSON with dynamic panels.
 
 * Add string representation methods to main classes.
 
@@ -251,7 +251,18 @@
   from_json method.
 
 0.7.1 (2022-09-18)
 ------------------
 
 * Bug fix: do not add a default page when other pages are defined.
 * Update js CDN and tests.
+
+0.8.0 (2023-04-10)
+------------------
+
+* Bug fix: fix choices with translatable text (thanks @joan-qida).
+* Bug fix: fix read the docs build.
+* Update SurveyJS version.
+* Use current SurveyJS supported themes.
+* Include newer Python versions in tests.
+* Add documentation for i18n.
+* Various dependency updates.
```

### Comparing `questions-0.7.1/questions.egg-info/SOURCES.txt` & `questions-0.8.0/questions.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/modules.rst
 docs/questions.cli.rst
 docs/questions.form.rst
 docs/questions.questions.rst
 docs/questions.rst
 docs/questions.settings.rst
 docs/questions.templates.rst
+docs/questions.utils.rst
 docs/questions.validators.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_word_list.txt
 docs/usage.rst
 docs/_build/html/_sources/authors.rst.txt
 docs/_build/html/_sources/contributing.rst.txt
@@ -34,14 +35,15 @@
 docs/_build/html/_sources/modules.rst.txt
 docs/_build/html/_sources/questions.cli.rst.txt
 docs/_build/html/_sources/questions.form.rst.txt
 docs/_build/html/_sources/questions.questions.rst.txt
 docs/_build/html/_sources/questions.rst.txt
 docs/_build/html/_sources/questions.settings.rst.txt
 docs/_build/html/_sources/questions.templates.rst.txt
+docs/_build/html/_sources/questions.utils.rst.txt
 docs/_build/html/_sources/questions.validators.rst.txt
 docs/_build/html/_sources/readme.rst.txt
 docs/_build/html/_sources/usage.rst.txt
 docs/_build/html/_static/README.txt
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
```

### Comparing `questions-0.7.1/tests/test_cli.py` & `questions-0.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/tests/test_form.py` & `questions-0.8.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `questions-0.7.1/tests/test_templates.py` & `questions-0.8.0/tests/test_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,35 +29,35 @@
 
 def test_get_survey_js():
     survey_js = templates.get_survey_js(
         form_json="FORM_JSON",
         form_data="FORM_DATA",
         html_id="id",
         action="http://testing",
-        theme="default",
+        theme="defaultV2",
         platform="jquery",
     )
     assert "FORM_JSON" in survey_js
     assert "FORM_DATA" in survey_js
     assert "http://testing" in survey_js
-    assert "default" in survey_js
+    assert "defaultV2" in survey_js
 
 
 def test_get_survey_js_form_data_is_none():
     survey_js = templates.get_survey_js(
         form_json="FORM_JSON",
         form_data=None,
         html_id="id",
         action="http://testing",
-        theme="default",
+        theme="defaultV2",
         platform="jquery",
     )
     assert "FORM_JSON" in survey_js
     assert "http://testing" in survey_js
-    assert "default" in survey_js
+    assert "defaultV2" in survey_js
 
 
 def test_get_form_page():
     html = templates.get_form_page(
         title="Title",
         html_id="id",
         platform="jquery",
```

### Comparing `questions-0.7.1/tests/test_validators.py` & `questions-0.8.0/tests/test_validators.py`

 * *Files identical despite different names*

