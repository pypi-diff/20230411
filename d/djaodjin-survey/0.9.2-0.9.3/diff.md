# Comparing `tmp/djaodjin-survey-0.9.2.tar.gz` & `tmp/djaodjin-survey-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.2.tar", last modified: Sun Mar 26 19:30:11 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.3.tar", last modified: Mon Apr 10 22:55:14 2023, max compression
```

## Comparing `djaodjin-survey-0.9.2.tar` & `djaodjin-survey-0.9.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.262530 djaodjin-survey-0.9.2/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1946 2023-03-26 19:30:11.262581 djaodjin-survey-0.9.2/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1631 2023-03-22 21:49:03.000000 djaodjin-survey-0.9.2/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.246141 djaodjin-survey-0.9.2/djaodjin_survey.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1946 2023-03-26 19:30:11.000000 djaodjin-survey-0.9.2/djaodjin_survey.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2363 2023-03-26 19:30:11.000000 djaodjin-survey-0.9.2/djaodjin_survey.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-03-26 19:30:11.000000 djaodjin-survey-0.9.2/djaodjin_survey.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-03-26 19:30:11.000000 djaodjin-survey-0.9.2/djaodjin_survey.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       73 2022-10-01 18:58:35.000000 djaodjin-survey-0.9.2/requirements.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-03-26 19:30:11.262758 djaodjin-survey-0.9.2/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     2242 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.249736 djaodjin-survey-0.9.2/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-03-26 19:27:17.000000 djaodjin-survey-0.9.2/survey/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.252712 djaodjin-survey-0.9.2/survey/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.2/survey/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39086 2023-03-22 18:10:54.000000 djaodjin-survey-0.9.2/survey/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.2/survey/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.2/survey/api/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    55816 2023-03-21 20:48:14.000000 djaodjin-survey-0.9.2/survey/api/sample.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23380 2023-03-24 16:15:38.000000 djaodjin-survey-0.9.2/survey/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.2/survey/api/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5408 2022-11-14 00:13:32.000000 djaodjin-survey-0.9.2/survey/api/units.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.2/survey/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    16872 2023-03-21 21:09:54.000000 djaodjin-survey-0.9.2/survey/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5947 2023-03-21 21:08:04.000000 djaodjin-survey-0.9.2/survey/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14465 2023-03-24 16:25:34.000000 djaodjin-survey-0.9.2/survey/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39701 2023-03-22 20:06:54.000000 djaodjin-survey-0.9.2/survey/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-03-08 18:09:27.000000 djaodjin-survey-0.9.2/survey/pagination.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10962 2023-03-22 17:50:12.000000 djaodjin-survey-0.9.2/survey/queries.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.2/survey/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.2/survey/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.244140 djaodjin-survey-0.9.2/survey/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.252930 djaodjin-survey-0.9.2/survey/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/css/matrix-chart.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.254539 djaodjin-survey-0.9.2/survey/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-categorize.js
--rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-matrix.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51247 2023-03-23 18:16:48.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-set.js
--rw-r--r--   0 smirolo    (501) staff       (20)    16018 2023-03-20 16:58:45.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-survey-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/js/djaodjin-survey.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/static/js/matrix-chart.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.244236 djaodjin-survey-0.9.2/survey/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.256253 djaodjin-survey-0.9.2/survey/templates/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/answer_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/campaign_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.256393 djaodjin-survey-0.9.2/survey/templates/survey/campaigns/
--rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/campaigns/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/categorize.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.257059 djaodjin-survey-0.9.2/survey/templates/survey/matrix/
--rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.2/survey/templates/survey/matrix/compare.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/matrix/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/matrix/matrix.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/portfolios.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/question_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/question_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/respondent_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/result.html
--rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.2/survey/templates/survey/result_quizz.html
--rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/sample_create.html
--rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/sample_update.html
--rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templates/survey/send.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.257299 djaodjin-survey-0.9.2/survey/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.2/survey/templatetags/survey_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.257535 djaodjin-survey-0.9.2/survey/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.2/survey/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.259123 djaodjin-survey-0.9.2/survey/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.2/survey/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.2/survey/urls/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.2/survey/urls/api/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1876 2023-03-22 17:59:22.000000 djaodjin-survey-0.9.2/survey/urls/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.2/survey/urls/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.2/survey/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.2/survey/urls/api/portfolios.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.259696 djaodjin-survey-0.9.2/survey/urls/api/sample/
--rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.2/survey/urls/api/sample/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.2/survey/urls/api/sample/reset.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2467 2023-03-08 00:21:37.000000 djaodjin-survey-0.9.2/survey/urls/api/sample/update.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.260814 djaodjin-survey-0.9.2/survey/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.2/survey/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.2/survey/urls/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.2/survey/urls/views/matrices.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.2/survey/urls/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.2/survey/urls/views/samples.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8382 2023-03-21 21:09:19.000000 djaodjin-survey-0.9.2/survey/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-03-26 19:30:11.262268 djaodjin-survey-0.9.2/survey/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.2/survey/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/views/createquestion.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.2/survey/views/edit.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6154 2023-03-22 18:11:02.000000 djaodjin-survey-0.9.2/survey/views/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.2/survey/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.2/survey/views/sample.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.038765 djaodjin-survey-0.9.3/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1615 2023-04-10 22:55:14.038828 djaodjin-survey-0.9.3/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1300 2023-04-10 22:53:07.000000 djaodjin-survey-0.9.3/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.020823 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1615 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2363 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2022-10-01 18:58:35.000000 djaodjin-survey-0.9.3/requirements.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-10 22:55:14.039015 djaodjin-survey-0.9.3/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     2242 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.024642 djaodjin-survey-0.9.3/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-10 22:49:34.000000 djaodjin-survey-0.9.3/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.028705 djaodjin-survey-0.9.3/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.3/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    44934 2023-04-10 22:13:16.000000 djaodjin-survey-0.9.3/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.3/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.3/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.3/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23664 2023-04-07 16:55:31.000000 djaodjin-survey-0.9.3/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.3/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5408 2022-11-14 00:13:32.000000 djaodjin-survey-0.9.3/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.3/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.3/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.3/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14652 2023-04-10 22:07:21.000000 djaodjin-survey-0.9.3/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.3/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.3/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.3/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.3/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.3/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.018942 djaodjin-survey-0.9.3/survey/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.028946 djaodjin-survey-0.9.3/survey/static/css/
+-rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/css/matrix-chart.css
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.030625 djaodjin-survey-0.9.3/survey/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-categorize.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-matrix.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51291 2023-04-10 22:08:00.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-set.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    16018 2023-03-20 16:58:45.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/matrix-chart.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.019037 djaodjin-survey-0.9.3/survey/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.032446 djaodjin-survey-0.9.3/survey/templates/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/answer_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/campaign_form.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.032585 djaodjin-survey-0.9.3/survey/templates/survey/campaigns/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/campaigns/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/categorize.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033106 djaodjin-survey-0.9.3/survey/templates/survey/matrix/
+-rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/compare.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/matrix.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/portfolios.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/question_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/question_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/respondent_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/result.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.3/survey/templates/survey/result_quizz.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/sample_create.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/sample_update.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/send.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033338 djaodjin-survey-0.9.3/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.3/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033559 djaodjin-survey-0.9.3/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.3/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.035160 djaodjin-survey-0.9.3/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.3/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.3/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.3/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.3/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.3/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.3/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.3/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.035795 djaodjin-survey-0.9.3/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.036976 djaodjin-survey-0.9.3/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.3/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.3/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.3/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.3/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.3/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9305 2023-04-05 18:38:45.000000 djaodjin-survey-0.9.3/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.038499 djaodjin-survey-0.9.3/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.3/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.3/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.3/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.3/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.2/LICENSE.txt` & `djaodjin-survey-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/PKG-INFO` & `djaodjin-survey-0.9.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.2
+Version: 0.9.3
 Summary: Survey Django app
 Home-page: https://github.com/djaodjin/djaodjin-survey/
-Download-URL: https://github.com/djaodjin/djaodjin-survey/tarball/0.9.2
+Download-URL: https://github.com/djaodjin/djaodjin-survey/tarball/0.9.3
 Author: The DjaoDjin Team
 Author-email: support@djaodjin.com
 License: BSD
 License-File: LICENSE.txt
 
 DjaoDjin survey
 ================
@@ -40,22 +40,17 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
 - **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
 - **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
 
-0.9.0
+0.9.3
 
-  * adds compare API
-  * adds ACCESSIBLE_ACCOUNTS_CALLABLE
-  * uses comma to separate multiple terms in search
-  * moves update_context_urls from survey.utils to survey.helpers
-  * defines URL_PATH_SEP and DB_PATH_SEP in settings.py instead of mixins
-  * moves get_collected_by from survey.queries to survey.models
-  * replaces queries.get_frozen_answers by Answer.objects.get_frozen_answers
-  * replaces queries.get_completed_assessments_at_by by Sample.objects.get_completed_assessments_at_by
+  * adds benchmarks APIs
+  * lists all samples for an account, filtered by active or is_frozen
+  * prevents import loops between queries.py, models.py and utils.py
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.2/djaodjin_survey.egg-info/PKG-INFO` & `djaodjin-survey-0.9.3/djaodjin_survey.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.2
+Version: 0.9.3
 Summary: Survey Django app
 Home-page: https://github.com/djaodjin/djaodjin-survey/
-Download-URL: https://github.com/djaodjin/djaodjin-survey/tarball/0.9.2
+Download-URL: https://github.com/djaodjin/djaodjin-survey/tarball/0.9.3
 Author: The DjaoDjin Team
 Author-email: support@djaodjin.com
 License: BSD
 License-File: LICENSE.txt
 
 DjaoDjin survey
 ================
@@ -40,22 +40,17 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
 - **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
 - **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
 
-0.9.0
+0.9.3
 
-  * adds compare API
-  * adds ACCESSIBLE_ACCOUNTS_CALLABLE
-  * uses comma to separate multiple terms in search
-  * moves update_context_urls from survey.utils to survey.helpers
-  * defines URL_PATH_SEP and DB_PATH_SEP in settings.py instead of mixins
-  * moves get_collected_by from survey.queries to survey.models
-  * replaces queries.get_frozen_answers by Answer.objects.get_frozen_answers
-  * replaces queries.get_completed_assessments_at_by by Sample.objects.get_completed_assessments_at_by
+  * adds benchmarks APIs
+  * lists all samples for an account, filtered by active or is_frozen
+  * prevents import loops between queries.py, models.py and utils.py
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.2/djaodjin_survey.egg-info/SOURCES.txt` & `djaodjin-survey-0.9.3/djaodjin_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/setup.py` & `djaodjin-survey-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/__init__.py` & `djaodjin-survey-0.9.3/survey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
```

### Comparing `djaodjin-survey-0.9.2/survey/admin.py` & `djaodjin-survey-0.9.3/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/api/campaigns.py` & `djaodjin-survey-0.9.3/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/api/matrix.py` & `djaodjin-survey-0.9.3/survey/api/matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,25 +33,230 @@
 from rest_framework.mixins import CreateModelMixin
 from rest_framework.filters import OrderingFilter, SearchFilter
 from rest_framework.pagination import PageNumberPagination
 
 from .. import settings
 from ..compat import reverse, six
 from ..mixins import (AccountMixin, CampaignMixin, DateRangeContextMixin,
-    MatrixMixin)
+    MatrixMixin, QuestionMixin, SampleMixin)
 from ..models import (Answer, Matrix, EditableFilter,
-    EditableFilterEnumeratedAccounts, Sample, UnitEquivalences)
-from ..utils import (get_accessible_accounts, get_account_model,
+    EditableFilterEnumeratedAccounts, Sample, Unit, UnitEquivalences)
+from ..pagination import MetricsPagination
+from ..utils import (get_accessible_accounts, get_benchmarks_enumerated,
+    get_account_model, get_question_model,
     get_account_serializer, get_question_serializer)
 from .serializers import (AccountsFilterAddSerializer,
-    CompareQuestionSerializer, EditableFilterSerializer, MatrixSerializer)
+    CompareQuestionSerializer, EditableFilterSerializer, MatrixSerializer,
+    SampleBenchmarksSerializer)
 
 
 LOGGER = logging.getLogger(__name__)
 
+
+class BenchmarkAPIView(QuestionMixin, CampaignMixin, AccountMixin,
+                       DateRangeContextMixin, generics.ListAPIView):
+    """
+    Aggregated benchmark for requested accounts
+
+    **Examples**:
+
+    .. code-block:: http
+
+        GET /api/energy-utility/reporting/sustainability/benchmarks\
+/sustainability HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+
+        {
+          "count": 4,
+          "results": []
+        }
+    """
+    scale = 1
+    default_unit = 'profiles'
+    valid_units = ('percentage',)
+    title = "Benchmarks"
+    serializer_class = SampleBenchmarksSerializer
+    pagination_class = MetricsPagination
+
+    @property
+    def unit(self):
+        #pylint:disable=attribute-defined-outside-init
+        if not hasattr(self, '_unit'):
+            self._unit = self.default_unit
+            param_unit = self.get_query_param('unit')
+            if param_unit is not None and param_unit in self.valid_units:
+                self._unit = param_unit
+        return self._unit
+
+    def get_query_param(self, key):
+        try:
+            return self.request.query_params.get(key, None)
+        except AttributeError:
+            pass
+        return self.request.GET.get(key, None)
+
+    def get_accessible_accounts(self, grantees):
+        return get_accessible_accounts(grantees, campaign=self.campaign)
+
+    def get_questions(self, prefix):
+        """
+        Overrides CampaignContentMixin.get_questions to return a list
+        of questions based on the answers available in the benchmarkd samples.
+        """
+        if not prefix.endswith(settings.DB_PATH_SEP):
+            prefix = prefix + settings.DB_PATH_SEP
+
+        questions_queryset = get_question_model().objects.filter(
+            path__startswith=self.db_path).values(
+            'pk', 'path', 'ui_hint', 'content__title',
+            'default_unit__slug', 'default_unit__title')
+        questions_by_key = {question['pk']: {
+            'path': question['path'],
+            'title': question['content__title'],
+            'ui_hint': question['ui_hint'],
+            'default_unit': Unit(
+                slug=question['default_unit__slug'],
+                title=question['default_unit__title']),
+        } for question in questions_queryset}
+
+        self.attach_results(questions_by_key)
+
+        return list(six.itervalues(questions_by_key))
+
+
+    def attach_results(self, questions_by_key, account=None):
+        if not account:
+            account = self.account
+
+        # samples that will be counted in the benchmark
+        samples = []
+        accessible_accounts = self.get_accessible_accounts([account])
+        if accessible_accounts:
+            # Calling `get_completed_assessments_at_by` with an `accounts`
+            # arguments evaluating to `False` will return all the latest
+            # frozen samples.
+            samples = Sample.objects.get_completed_assessments_at_by(
+                self.campaign,
+                start_at=self.start_at, ends_at=self.ends_at,
+                accounts=accessible_accounts)
+
+        if samples:
+            questions_by_key = get_benchmarks_enumerated(
+                samples, questions_by_key.keys(), questions_by_key)
+            for question in six.itervalues(questions_by_key):
+                if not 'benchmarks' in question:
+                    question['benchmarks'] = []
+                account_benchmark = {
+                    'slug': account.slug,
+                    'printable_name': account.printable_name,
+                    'values': []
+                }
+                for key, val in six.iteritems(question.get('rate', {})):
+                    account_benchmark['values'] += [(key, int(val))]
+                question['benchmarks'] += [account_benchmark]
+
+    def get_serializer_context(self):
+        context = super(BenchmarkAPIView, self).get_serializer_context()
+        context.update({
+            'prefix': self.db_path if self.db_path else settings.DB_PATH_SEP,
+        })
+        return context
+
+    def get_queryset(self):
+        return self.get_questions(self.db_path)
+
+
+class BenchmarkIndexAPIView(BenchmarkAPIView):
+    """
+    Aggregated benchmark for requested accounts
+
+    **Examples**:
+
+    .. code-block:: http
+
+        GET /api/energy-utility/reporting/sustainability/benchmarks HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+
+        {
+          "count": 4,
+          "results": []
+        }
+    """
+
+
+class SampleBenchmarksAPIView(SampleMixin, BenchmarkAPIView):
+    """
+    Benchmark a sub-tree of questions against peers
+
+    **Examples**:
+
+    .. code-block:: http
+
+        GET /api/supplier-1/sample/46f66f70f5ad41b29c4df08f683a9a7a/benchmarks\
+/sustainability HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+
+        {
+          "count": 4,
+          "results": []
+        }
+    """
+    @property
+    def campaign(self):
+        #pylint:disable=attribute-defined-outside-init
+        if not hasattr(self, '_campaign'):
+            self._campaign = self.sample.campaign
+        return self._campaign
+
+    @property
+    def ends_at(self):
+        #pylint:disable=attribute-defined-outside-init
+        if not hasattr(self, '_ends_at'):
+            self._ends_at = self.sample.created_at
+        return self._ends_at
+
+    def get_accessible_accounts(self, grantees):
+        return get_account_model().objects.all()
+
+
+class SampleBenchmarksIndexAPIView(SampleBenchmarksAPIView):
+    """
+    Benchmark against peers
+
+    **Examples**:
+
+    .. code-block:: http
+
+        GET /api/supplier-1/sample/46f66f70f5ad41b29c4df08f683a9a7a/benchmarks\
+ HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+
+        {
+          "count": 4,
+          "results": []
+        }
+    """
+
+
 class CompareAPIView(CampaignMixin, AccountMixin, DateRangeContextMixin,
                      generics.ListAPIView):
     """
     Lists compared samples
 
     **Examples**:
```

### Comparing `djaodjin-survey-0.9.2/survey/api/metrics.py` & `djaodjin-survey-0.9.3/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/api/portfolios.py` & `djaodjin-survey-0.9.3/survey/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/api/sample.py` & `djaodjin-survey-0.9.3/survey/api/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,21 @@
 from rest_framework import response as http
 from rest_framework.exceptions import ValidationError
 from rest_framework.generics import get_object_or_404
 from rest_framework.status import HTTP_200_OK, HTTP_201_CREATED
 
 from ..compat import six, is_authenticated
 from ..docs import OpenAPIResponse, swagger_auto_schema
+from ..filters import DateRangeFilter, OrderingFilter, SampleStateFilter
 from ..mixins import AccountMixin, SampleMixin
 from ..models import Answer, Choice, Sample, Unit, UnitEquivalences
+from ..queries import is_sqlite3
+from ..utils import datetime_or_now, get_question_model, get_user_serializer
 from .serializers import (AnswerSerializer, NoModelSerializer,
     SampleAnswerSerializer, SampleCreateSerializer, SampleSerializer)
-from ..utils import (datetime_or_now, get_question_model, get_user_serializer,
-    is_sqlite3)
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def update_or_create_answer(datapoint, question, sample, created_at,
                             collected_by=None):
@@ -1481,19 +1482,38 @@
                 "campaign": "sustainability",
                 "is_frozen": false,
                 "extra": null
             }
             ]
         }
     """
+    search_fields = (
+        'is_frozen',
+        'campaign',
+    )
+    alternate_fields = {
+        'campaign': 'campaign__slug',
+    }
+    ordering_fields = (
+        ('created_at', 'created_at'),
+        ('campaign__title', 'campaign__title'),
+        ('is_frozen', 'is_frozen'),
+    )
+
+    ordering = ('-created_at',)
+
+    filter_backends = (DateRangeFilter, SampleStateFilter, OrderingFilter)
+
     serializer_class = SampleSerializer
 
     def get_queryset(self):
         return Sample.objects.filter(
-            account=self.account, is_frozen=False).order_by('-created_at')
+            account=self.account,
+            extra__isnull=True         # XXX convinience
+        ).select_related('campaign')
 
     @swagger_auto_schema(request_body=SampleCreateSerializer)
     def post(self, request, *args, **kwargs):
         """
         Creates a new sample
 
         Creates a new sample to record qualitative and/or quantitative data.
@@ -1565,16 +1585,17 @@
     """
     serializer_class = get_user_serializer()
 
     def get_queryset(self):
         kwargs = {}
         if self.path:
             kwargs = {'answer__question__path__startwith': self.path}
-        return get_user_model().objects.filter(
+        queryset = get_user_model().objects.filter(
             answer__sample=self.sample, **kwargs).distinct()
+        return queryset
 
 
 class SampleRespondentsIndexAPIView(SampleRespondentsAPIView):
     """
     Lists unique respondents
 
     The list returned contains the information about the users who answered
```

### Comparing `djaodjin-survey-0.9.2/survey/api/serializers.py` & `djaodjin-survey-0.9.3/survey/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 class QuestionDetailSerializer(QuestionCreateSerializer):
 
     class Meta:
         model = QuestionCreateSerializer.Meta.model
         fields = QuestionCreateSerializer.Meta.fields + ('path',)
 
 
-class CampaignQuestionSerializer(serializers.ModelSerializer):
+class QuestionSerializer(serializers.ModelSerializer):
     """
     Serializer of ``Question`` when used in a list of answers
     """
     title = serializers.CharField(allow_blank=True,
         help_text=_("Short description"))
     default_unit = UnitSerializer()
     ui_hint = EnumField(choices=get_question_model().UI_HINTS,
@@ -230,99 +230,100 @@
         fields = ('path', 'title', 'default_unit', 'ui_hint')
 
 
 class SampleAnswerSerializer(AnswerSerializer):
     """
     Serializer of ``Answer`` when used in list.
     """
-    question = CampaignQuestionSerializer(
+    question = QuestionSerializer(
         help_text=_("Question the answer refers to"))
     required = serializers.BooleanField(required=False,
         help_text=_("Whether an answer is required or not."))
 
     class Meta(object):
         model = AnswerSerializer.Meta.model
         fields = AnswerSerializer.Meta.fields + ('question', 'required')
         read_only_fields = AnswerSerializer.Meta.read_only_fields + (
             'required',)
 
 
-class SampleCreateSerializer(serializers.ModelSerializer):
-
-    campaign = serializers.SlugRelatedField(slug_field='slug',
-        queryset=Campaign.objects.all(), required=False,
-        help_text=("Campaign this sample is part of."))
-
-    class Meta(object):
-        model = Sample
-        fields = ('campaign',)
-
-
-class SampleSerializer(SampleCreateSerializer):
-
-    campaign = serializers.SlugRelatedField(slug_field='slug',
-        read_only=True, allow_null=True,
-        help_text=("Campaign this sample is part of."))
-    account = serializers.SlugRelatedField(slug_field='slug',
-        read_only=True, required=False,
-        help_text=("Account this sample belongs to."))
-    location = serializers.URLField(read_only=True, allow_null=True,
-        help_text=("URL at which the response is visible."))
-
-    class Meta(object):
-        model = Sample
-        fields = ('campaign', 'slug', 'account', 'created_at',
-            'updated_at', 'is_frozen', 'location')
-        read_only_fields = ('campaign', 'slug', 'account', 'created_at',
-            'updated_at', 'is_frozen', 'location')
-
-    @staticmethod
-    def get_location(obj):
-        return getattr(obj, 'location', None)
-
-
 class CampaignSerializer(serializers.ModelSerializer):
     """
     Short description of the campaign.
     """
 
     account = serializers.SlugRelatedField(
         slug_field=settings.BELONGS_LOOKUP_FIELD,
         queryset=get_belongs_model().objects.all(),
         help_text=("Account this sample belongs to."))
 
     class Meta(object):
         model = Campaign
-        fields = ('slug', 'account', 'title', 'description', 'active',)
+        fields = ('slug', 'account', 'title', 'description', 'created_at',
+            'active')
+        read_only_fields = ('slug', 'account', 'created_at')
+
+
+class CampaignCreateSerializer(serializers.ModelSerializer):
+
+    questions = QuestionCreateSerializer(many=True, required=False)
+
+    class Meta(object):
+        model = Campaign
+        fields = ('slug', 'title', 'description', 'quizz_mode', 'questions')
         read_only_fields = ('slug',)
 
 
 class CampaignDetailSerializer(serializers.ModelSerializer):
 
     account = serializers.SlugRelatedField(
         slug_field=settings.BELONGS_LOOKUP_FIELD,
         queryset=get_belongs_model().objects.all(),
         help_text=("Account this sample belongs to."))
-    questions = CampaignQuestionSerializer(many=True)
+    questions = QuestionSerializer(many=True)
 
     class Meta(object):
         model = Campaign
         fields = ('slug', 'account', 'title', 'description', 'active',
             'quizz_mode', 'questions')
         read_only_fields = ('slug',)
 
 
-class CampaignCreateSerializer(serializers.ModelSerializer):
+class SampleCreateSerializer(serializers.ModelSerializer):
 
-    questions = QuestionCreateSerializer(many=True, required=False)
+    campaign = serializers.SlugRelatedField(slug_field='slug',
+        queryset=Campaign.objects.all(), required=False,
+        help_text=("Campaign this sample is part of."))
 
     class Meta(object):
-        model = Campaign
-        fields = ('slug', 'title', 'description', 'quizz_mode', 'questions')
-        read_only_fields = ('slug',)
+        model = Sample
+        fields = ('campaign',)
+
+
+class SampleSerializer(SampleCreateSerializer):
+
+    campaign = CampaignSerializer(
+        read_only=True, allow_null=True,
+        help_text=("Campaign this sample is part of."))
+    account = serializers.SlugRelatedField(slug_field='slug',
+        read_only=True, required=False,
+        help_text=("Account this sample belongs to."))
+    location = serializers.URLField(read_only=True, allow_null=True,
+        help_text=("URL at which the response is visible."))
+
+    class Meta(object):
+        model = Sample
+        fields = ('campaign', 'slug', 'account', 'created_at',
+            'updated_at', 'is_frozen', 'location')
+        read_only_fields = ('campaign', 'slug', 'account', 'created_at',
+            'updated_at', 'is_frozen', 'location')
+
+    @staticmethod
+    def get_location(obj):
+        return getattr(obj, 'location', None)
 
 
 class DatapointSerializer(AnswerSerializer):
     """
     Serializer of ``Answer`` when used to retrieve data points.
     """
     account = serializers.SerializerMethodField()
@@ -484,36 +485,46 @@
     extra = ExtraField(required=False,
         help_text=_("Extra meta data (can be stringify JSON)"))
     values = serializers.ListField(
         child=KeyValueTuple(),
         help_text="Datapoints in the serie")
 
 
+class SampleBenchmarksSerializer(QuestionSerializer):
+    """
+    Benchmarks for one question when used in a list of `Question`.
+    """
+    benchmarks = serializers.ListField(child=TableSerializer())
+
+    class Meta(QuestionSerializer.Meta):
+        fields = QuestionSerializer.Meta.fields + ('benchmarks',)
+
+
 class MetricsSerializer(NoModelSerializer):
 
     scale = serializers.FloatField(required=False,
         help_text=_("The scale of the number reported in the tables (ex: 1000"\
         " when numbers are reported in thousands)"))
     unit = serializers.SlugRelatedField(required=False, allow_null=True,
         queryset=Unit.objects.all(), slug_field='slug',
         help_text=_("Unit the measured field is in"))
     title = serializers.CharField(
         help_text=_("Title for the table"))
     results = TableSerializer(many=True)
 
 
-class CompareQuestionSerializer(CampaignQuestionSerializer):
+class CompareQuestionSerializer(QuestionSerializer):
     """
     Serializer for a question in the `results` field of a Compare API call.
     """
     values = serializers.ListField(
         child=serializers.ListField(child=AnswerSerializer()), required=False)
 
-    class Meta(CampaignQuestionSerializer.Meta):
-        fields = CampaignQuestionSerializer.Meta.fields + ('values',)
+    class Meta(QuestionSerializer.Meta):
+        fields = QuestionSerializer.Meta.fields + ('values',)
 
 
 
 class InviteeSerializer(NoModelSerializer):
 
     slug = serializers.SlugField()
     full_name = serializers.CharField()
```

### Comparing `djaodjin-survey-0.9.2/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.3/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/api/units.py` & `djaodjin-survey-0.9.3/survey/api/units.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/compat.py` & `djaodjin-survey-0.9.3/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/docs.py` & `djaodjin-survey-0.9.3/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/filters.py` & `djaodjin-survey-0.9.3/survey/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,39 +397,62 @@
                 'schema': {
                     'type': 'string',
                 },
             }]
         return fields
 
 
-class DoubleOptInStateFilter(BaseFilterBackend):
+class StateFilter(BaseFilterBackend):
+
+    state_param = 'state'
+    state_field = 'state'
+    state_candidates = []
 
     def filter_queryset(self, request, queryset, view):
-        state = request.query_params.get('state', '')
+        state = request.query_params.get(self.state_param, '')
         flt = None
         for val in state.split(','):
-            for candidate in PortfolioDoubleOptIn.STATES:
+            for candidate in self.state_candidates:
                 if val == candidate[1]:
                     if flt:
-                        flt |= models.Q(state=candidate[0])
+                        flt |= models.Q(**{self.state_field: candidate[0]})
                     else:
-                        flt = models.Q(state=candidate[0])
+                        flt = models.Q(**{self.state_field: candidate[0]})
                     break
         if flt is not None:
             queryset = queryset.filter(flt)
         return queryset
 
     def get_schema_operation_parameters(self, view):
-        fields = super(DoubleOptInStateFilter,
-            self).get_schema_operation_parameters(view)
+        fields = super(StateFilter, self).get_schema_operation_parameters(view)
         fields += [
             {
-                'name': 'state',
+                'name': self.state_param,
                 'required': False,
                 'in': 'query',
-                'description': force_str("filter by state"),
+                'description': force_str("filter by state (%(choices)s)" % {
+                    'choices': ", ".join([
+                        candidate[1] for candidate in self.state_candidates])
+                }),
                 'schema': {
                     'type': 'string',
                 },
             },
         ]
         return fields
+
+
+class DoubleOptInStateFilter(StateFilter):
+
+    state_param = 'state'
+    state_field = 'state'
+    state_candidates = PortfolioDoubleOptIn.STATES
+
+
+class SampleStateFilter(StateFilter):
+
+    state_param = 'state'
+    state_field = 'is_frozen'
+    state_candidates = [
+        (False, 'active'),
+        (True, 'completed')
+    ]
```

### Comparing `djaodjin-survey-0.9.2/survey/forms.py` & `djaodjin-survey-0.9.3/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/helpers.py` & `djaodjin-survey-0.9.3/survey/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+"""
+This file contains functions useful throughout the whole project which do
+not require to import `django` modules.
 
+See utils.py for functions useful throughout the whole project which depend
+on importing Django models.
+"""
 import datetime, json
 
 from dateutil.relativedelta import relativedelta, SU
 from pytz import timezone, utc, UnknownTimeZoneError
 from pytz.tzinfo import DstTzInfo
 
 from .compat import six
```

### Comparing `djaodjin-survey-0.9.2/survey/mixins.py` & `djaodjin-survey-0.9.3/survey/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,37 +132,44 @@
 
     forced_date_range = True
     default_ends_at = None
 
     @property
     def start_at(self):
         if not hasattr(self, '_start_at'):
-            self._start_at = self.request.GET.get('start_at', None)
+            self._start_at = self.get_query_param('start_at')
             if self._start_at:
                 self._start_at = datetime_or_now(self._start_at.strip('"'))
         return self._start_at
 
     @property
     def ends_at(self):
         if not hasattr(self, '_ends_at'):
-            self._ends_at = self.request.GET.get('ends_at', None)
+            self._ends_at = self.get_query_param('ends_at')
             if self.forced_date_range or self._ends_at:
                 if self._ends_at is not None:
                     self._ends_at = self._ends_at.strip('"')
                 else:
                     self._ends_at = self.default_ends_at
                 self._ends_at = datetime_or_now(self._ends_at)
         return self._ends_at
 
     @property
     def timezone(self):
         if not hasattr(self, '_timezone'):
-            self._timezone = self.request.GET.get('timezone', None)
+            self._timezone = self.get_query_param('timezone')
         return self._timezone
 
+    def get_query_param(self, key):
+        try:
+            return self.request.query_params.get(key, None)
+        except AttributeError:
+            pass
+        return self.request.GET.get(key, None)
+
     def get_context_data(self, **kwargs):
         context = super(DateRangeContextMixin, self).get_context_data(**kwargs)
         if self.start_at:
             context.update({'start_at': self.start_at})
         if self.ends_at:
             context.update({'ends_at': self.ends_at})
         return context
@@ -286,15 +293,15 @@
         if not hasattr(self, '_question'):
             self._question = get_object_or_404(
                 get_question_model().objects.all(),
                 path=self.db_path)
         return self._question
 
 
-class SampleMixin(AccountMixin, QuestionMixin):
+class SampleMixin(QuestionMixin, AccountMixin):
     """
     Returns a ``Sample`` to a ``Campaign``.
     """
 
     # We have to use a special url_kwarg here because 'sample'
     # interfers with the way rest_framework handles **kwargs.
     sample_url_kwarg = 'sample'
```

### Comparing `djaodjin-survey-0.9.2/survey/models.py` & `djaodjin-survey-0.9.3/survey/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,16 @@
 from django.db import models, transaction, IntegrityError
 from django.template.defaultfilters import slugify
 from rest_framework.exceptions import ValidationError
 
 from . import settings
 from .compat import (gettext_lazy as _, import_string,
     python_2_unicode_compatible)
-from .utils import datetime_or_now, get_account_model, get_question_model
-from .queries import (sql_completed_at_by, sql_latest_frozen_by_accounts,
-    sql_frozen_answers)
+from .queries import (datetime_or_now, get_account_model, get_question_model,
+    sql_completed_at_by, sql_latest_frozen_by_accounts, sql_frozen_answers)
 
 
 def get_extra_field_class():
     extra_class = settings.EXTRA_FIELD
     if extra_class is None:
         extra_class = models.TextField
     elif isinstance(extra_class, str):
```

### Comparing `djaodjin-survey-0.9.2/survey/pagination.py` & `djaodjin-survey-0.9.3/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/queries.py` & `djaodjin-survey-0.9.3/survey/queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,81 @@
 # Copyright (c) 2023, DjaoDjin inc.
 # see LICENSE.
 """
 This file contains SQL statements as building blocks for benchmarking
 results in APIs, downloads, etc.
 """
+import datetime
+
+from django.apps import apps as django_apps
+from django.core.exceptions import ImproperlyConfigured
+from django.db import connections
+from django.db.utils import DEFAULT_DB_ALIAS
 from django.db.models.query import QuerySet, RawQuerySet
+from django.utils.dateparse import parse_date, parse_datetime
+from django.utils.timezone import utc
+
+from . import settings
+from .compat import six
+
+
+def as_sql_date_trunc_year(field_name, db_key=None):
+    if is_sqlite3(db_key):
+        return "strftime('%%Y', %s)" % field_name
+    return "date_trunc('year', %s)" % field_name
+
+
+def datetime_or_now(dtime_at=None):
+    as_datetime = dtime_at
+    if isinstance(dtime_at, six.string_types):
+        as_datetime = parse_datetime(dtime_at)
+        if not as_datetime:
+            as_date = parse_date(dtime_at)
+            if as_date:
+                as_datetime = datetime.datetime.combine(
+                    as_date, datetime.time.min)
+    if not as_datetime:
+        as_datetime = datetime.datetime.utcnow().replace(tzinfo=utc)
+    if as_datetime.tzinfo is None:
+        as_datetime = as_datetime.replace(tzinfo=utc)
+    return as_datetime
+
+
+def is_sqlite3(db_key=None):
+    if db_key is None:
+        db_key = DEFAULT_DB_ALIAS
+    return connections.databases[db_key]['ENGINE'].endswith('sqlite3')
 
-#from .models import Campaign
-from .utils import get_account_model, is_sqlite3
+
+def get_account_model():
+    """
+    Returns the ``Account`` model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.ACCOUNT_MODEL)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "ACCOUNT_MODEL must be of the form 'app_label.model_name'")
+    except LookupError:
+        raise ImproperlyConfigured("ACCOUNT_MODEL refers to model '%s'"\
+" that has not been installed" % settings.ACCOUNT_MODEL)
+
+
+def get_question_model():
+    """
+    Returns the ``Question`` model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.QUESTION_MODEL)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "QUESTION_MODEL must be of the form 'app_label.model_name'")
+    except LookupError:
+        raise ImproperlyConfigured("QUESTION_MODEL refers to model '%s'"\
+" that has not been installed" % settings.QUESTION_MODEL)
 
 
 def sql_latest_frozen_by_accounts(campaign=None,
                                   start_at=None, ends_at=None,
                                   tags=None, pks_only=False):
     """
     Returns the most recent frozen sample in an optionally specified
```

### Comparing `djaodjin-survey-0.9.2/survey/settings.py` & `djaodjin-survey-0.9.3/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/signals.py` & `djaodjin-survey-0.9.3/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-categorize.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-categorize.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-matrix.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-matrix.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-resources-vue.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-resources-vue.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -187,14 +187,31 @@
                     if (vm.params.hasOwnProperty(key) && vm.params[key]) {
                         if (excludes && key in excludes) continue;
                         params[key] = vm.params[key];
                     }
                 }
                 return params;
             },
+            getQueryString: function(excludes) {
+                var vm = this;
+                var sep = "";
+                var result = "";
+                var params = vm.getParams(excludes);
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        result += sep + key + '=' + encodeURIComponent(
+                            params[key].toString());
+                        sep = "&";
+                    }
+                }
+                if (result) {
+                    result = '?' + result;
+                }
+                return result;
+            },
         },
         computed: {
             _start_at: {
                 get: function() {
                     return this.asDateInputField(this.params.start_at);
                 },
                 set: function(newVal) {
@@ -340,31 +357,14 @@
                 var cleanUrl = cleanParts[0];
                 for (idx = 1; idx < cleanParts.length; ++idx) {
                     cleanUrl += '/' + cleanParts[idx];
                 }
                 return cleanUrl.startsWith('http') ? cleanUrl[0] : '/' + cleanUrl;
             },
 
-            getQueryString: function(excludes) {
-                var vm = this;
-                var sep = "";
-                var result = "";
-                var params = vm.getParams(excludes);
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        result += sep + key + '=' + params[key].toString();
-                        sep = "&";
-                    }
-                }
-                if (result) {
-                    result = '?' + result;
-                }
-                return result;
-            },
-
             /** This method generates a GET HTTP request to `url` with a query
                 string built of a `queryParams` dictionnary.
 
                 It supports the following prototypes:
 
                 - reqGet(url, successCallback)
                 - reqGet(url, queryParams, successCallback)
```

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-set.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-set.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-survey-vue.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/djaodjin-survey.js` & `djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/static/js/matrix-chart.js` & `djaodjin-survey-0.9.3/survey/static/js/matrix-chart.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/answer_form.html` & `djaodjin-survey-0.9.3/survey/templates/survey/answer_form.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/campaigns/index.html` & `djaodjin-survey-0.9.3/survey/templates/survey/campaigns/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/categorize.html` & `djaodjin-survey-0.9.3/survey/templates/survey/categorize.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/matrix/index.html` & `djaodjin-survey-0.9.3/survey/templates/survey/matrix/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/matrix/matrix.html` & `djaodjin-survey-0.9.3/survey/templates/survey/matrix/matrix.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/portfolios.html` & `djaodjin-survey-0.9.3/survey/templates/survey/portfolios.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/question_list.html` & `djaodjin-survey-0.9.3/survey/templates/survey/question_list.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/result.html` & `djaodjin-survey-0.9.3/survey/templates/survey/result.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/result_quizz.html` & `djaodjin-survey-0.9.3/survey/templates/survey/result_quizz.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templates/survey/sample_create.html` & `djaodjin-survey-0.9.3/survey/templates/survey/sample_create.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.3/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/__init__.py` & `djaodjin-survey-0.9.3/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.3/survey/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.3/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/filters.py` & `djaodjin-survey-0.9.3/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.3/survey/urls/api/matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,22 +18,27 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from ...api.matrix import (CompareAPIView, CompareIndexAPIView,
+from ...api.matrix import (BenchmarkAPIView, BenchmarkIndexAPIView,
+    CompareAPIView, CompareIndexAPIView,
     MatrixCreateAPIView, MatrixDetailAPIView)
 from ...compat import path
 
 
 urlpatterns = [
+    path('benchmarks/<path:path>',
+        BenchmarkAPIView.as_view(), name='survey_api_benchmarks'),
+    path('benchmarks',
+        BenchmarkIndexAPIView.as_view(), name='survey_api_benchmarks_index'),
     path('compare/<path:path>',
-        CompareAPIView.as_view(), name='survey_api_compare_samples_path'),
+        CompareAPIView.as_view(), name='survey_api_compare_samples'),
     path('compare',
-        CompareIndexAPIView.as_view(), name='survey_api_compare_samples'),
+        CompareIndexAPIView.as_view(), name='survey_api_compare_samples_index'),
     path('matrix/<path:path>',
         MatrixDetailAPIView.as_view(), name='matrix_api'),
     path('matrix',
         MatrixCreateAPIView.as_view(), name='matrix_api_base'),
 ]
```

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.3/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.3/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.3/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.3/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.3/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.3/survey/urls/api/sample/update.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,27 +21,33 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ....api.sample import (SampleAPIView, SampleAnswersAPIView,
     SampleCandidatesAPIView, SampleFreezeAPIView, SampleRecentCreateAPIView,
     SampleRespondentsAPIView, SampleRespondentsIndexAPIView)
+from ....api.matrix import SampleBenchmarksAPIView, SampleBenchmarksIndexAPIView
 from ....compat import path
 
 urlpatterns = [
     path('sample/<slug:sample>/freeze/<path:path>',
         SampleFreezeAPIView.as_view(), name='survey_api_sample_freeze'),
     path('sample/<slug:sample>/candidates/<path:path>',
         SampleCandidatesAPIView.as_view(), name='survey_api_sample_candidates'),
     path('sample/<slug:sample>/answers/<path:path>',
         SampleAnswersAPIView.as_view(), name='survey_api_sample_answers'),
+    path('sample/<slug:sample>/benchmarks/<path:path>',
+        SampleBenchmarksAPIView.as_view(), name='survey_api_sample_benchmarks'),
+    path('sample/<slug:sample>/benchmarks',
+        SampleBenchmarksIndexAPIView.as_view(),
+        name='survey_api_sample_benchmarks_index'),
     path('sample/<slug:sample>/respondents/<path:path>',
         SampleRespondentsAPIView.as_view(),
         name='survey_api_sample_respondents'),
     path('sample/<slug:sample>/respondents',
         SampleRespondentsIndexAPIView.as_view(),
         name='survey_api_sample_respondents_index'),
     path('sample/<slug:sample>',
         SampleAPIView.as_view(), name='survey_api_sample'),
     path('sample',
-        SampleRecentCreateAPIView.as_view(), name='survey_api_sample_new'),
+        SampleRecentCreateAPIView.as_view(), name='survey_api_sample_list'),
 ]
```

### Comparing `djaodjin-survey-0.9.2/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.3/survey/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.3/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.3/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.3/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/urls/views/samples.py` & `djaodjin-survey-0.9.3/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/utils.py` & `djaodjin-survey-0.9.3/survey/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,70 +17,59 @@
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
+"""
+This file contains functions useful throughout the whole project which depend
+on importing Django models.
+
+See helpers.py for functions useful throughout the whole project which do
+not require to import `django` modules.
+"""
 import datetime, logging
 from importlib import import_module
 
 from django.apps import apps as django_apps
 from django.conf import settings as django_settings
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.core.exceptions import ImproperlyConfigured
-from django.db import connections
-from django.db.utils import DEFAULT_DB_ALIAS
+from django.db.models import Count, F
 from django.http.request import split_domain_port, validate_host
-from django.utils.dateparse import parse_date, parse_datetime
 from django.utils.timezone import utc
 
 from . import settings
-from .compat import import_string, six, urlparse, urlunparse
-
+from .compat import import_string, urlparse, urlunparse
+from .models import Answer, Unit
+#pylint:disable=unused-import
+from .queries import datetime_or_now, get_account_model, get_question_model
 
 LOGGER = logging.getLogger(__name__)
 
 
-def as_sql_date_trunc_year(field_name, db_key=None):
-    if is_sqlite3(db_key):
-        return "strftime('%%Y', %s)" % field_name
-    return "date_trunc('year', %s)" % field_name
-
-
 def as_timestamp(dtime_at=None):
     if not dtime_at:
         dtime_at = datetime_or_now()
     return int((
         dtime_at - datetime.datetime(1970, 1, 1, tzinfo=utc)).total_seconds())
 
 
-def datetime_or_now(dtime_at=None):
-    as_datetime = dtime_at
-    if isinstance(dtime_at, six.string_types):
-        as_datetime = parse_datetime(dtime_at)
-        if not as_datetime:
-            as_date = parse_date(dtime_at)
-            if as_date:
-                as_datetime = datetime.datetime.combine(
-                    as_date, datetime.time.min)
-    if not as_datetime:
-        as_datetime = datetime.datetime.utcnow().replace(tzinfo=utc)
-    if as_datetime.tzinfo is None:
-        as_datetime = as_datetime.replace(tzinfo=utc)
-    return as_datetime
-
-
 def get_accessible_accounts(grantees,
                             campaign=None, start_at=None, ends_at=None):
     """
     All accounts which have elected to share samples with at least one
     account in grantees.
     """
+    try:
+        iter(grantees)
+    except TypeError:
+        grantees = [grantees]
+
     queryset = None
     if (hasattr(settings, 'ACCESSIBLE_ACCOUNTS_CALLABLE') and
         settings.ACCESSIBLE_ACCOUNTS_CALLABLE):
         queryset = import_string(settings.ACCESSIBLE_ACCOUNTS_CALLABLE)(
             grantees, campaign=campaign, start_at=start_at, ends_at=ends_at)
 
     if queryset is None:
@@ -88,31 +77,80 @@
         if start_at:
             filter_params.update({
                 'portfolio_double_optin_accounts__created_at__gte': start_at})
         if campaign:
             filter_params.update({'portfolios__campaign': campaign})
         queryset = get_account_model().objects.filter(
             portfolios__grantee__in=grantees,
-            **filter_params).distinct()
+            **filter_params).annotate(
+                _extra=F('portfolio_double_optin_accounts__extra')).distinct()
 
     return queryset
 
 
-def get_account_model():
-    """
-    Returns the ``Account`` model that is active in this project.
+def get_benchmarks_enumerated(samples, questions, questions_by_key=None):
     """
-    try:
-        return django_apps.get_model(settings.ACCOUNT_MODEL)
-    except ValueError:
-        raise ImproperlyConfigured(
-            "ACCOUNT_MODEL must be of the form 'app_label.model_name'")
-    except LookupError:
-        raise ImproperlyConfigured("ACCOUNT_MODEL refers to model '%s'"\
-" that has not been installed" % settings.ACCOUNT_MODEL)
+    Returns a dictionnary indexed by a question's primary key where
+    each question in `questions` is associated a a dictionnary that contains:
+      - the total number of samples in `samples` with an anwer to the question
+      - a dictionnary of the number of samples in `samples` for each choice
+        available when the question's unit is an enum.
+
+    Example:
+
+    {
+        12: {
+            "path": "/sustainability/governance/formalized-esg-strategy",
+            "nb_respondents": 10,
+            "rate": {
+                "Yes": 5,
+                "No": 5
+            }
+        }
+    }
+    """
+    if not questions_by_key:
+        questions_by_key = {}
+
+    # total number of answers
+    for row in Answer.objects.filter(
+            question__in=questions,
+            unit_id=F('question__default_unit_id'),
+            sample_id__in=samples).values('question__id',
+                'question__path').annotate(Count('sample_id')):
+        question_pk = row['question__id']
+        count = row['sample_id__count']
+        path = row['question__path']
+        value = questions_by_key.get(question_pk, {'path': path})
+        value.update({'nb_respondents': count})
+        if question_pk not in questions_by_key:
+            questions_by_key.update({question_pk: value})
+
+    # per-choice number of answers
+    for row in Answer.objects.filter(
+            question__in=questions,
+            unit_id=F('question__default_unit_id'),
+            sample_id__in=samples,
+            question__default_unit__system=Unit.SYSTEM_ENUMERATED,
+            unit__enums__id=F('measured')).values('question__id',
+                'measured', 'unit__enums__text').annotate(Count('sample_id')):
+        question_pk = row['question__id']
+        count = row['sample_id__count']
+        measured = row['unit__enums__text']
+        value = questions_by_key.get(question_pk)
+        total = value.get('nb_respondents', None)
+        rate = value.get('rate', {})
+        rate.update({
+            measured: (int(count * 100 // total) if total else 0)})
+        if 'rate' not in value:
+            value.update({'rate': rate})
+        if question_pk not in questions_by_key:
+            questions_by_key.update({question_pk: value})
+
+    return questions_by_key
 
 
 def get_account_serializer():
     """
     Returns the ``AccountSerializer`` model that is active in this project.
     """
     path = settings.ACCOUNT_SERIALIZER
@@ -156,28 +194,14 @@
         raise ImproperlyConfigured(
             "CONTENT_MODEL must be of the form 'app_label.model_name'")
     except LookupError:
         raise ImproperlyConfigured("CONTENT_MODEL refers to model '%s'"\
 " that has not been installed" % settings.CONTENT_MODEL)
 
 
-def get_question_model():
-    """
-    Returns the ``Question`` model that is active in this project.
-    """
-    try:
-        return django_apps.get_model(settings.QUESTION_MODEL)
-    except ValueError:
-        raise ImproperlyConfigured(
-            "QUESTION_MODEL must be of the form 'app_label.model_name'")
-    except LookupError:
-        raise ImproperlyConfigured("QUESTION_MODEL refers to model '%s'"\
-" that has not been installed" % settings.QUESTION_MODEL)
-
-
 def get_question_serializer():
     """
     Returns the ``QuestionDetailSerializer`` model that is active
     in this project.
     """
     path = settings.QUESTION_SERIALIZER
     dot_pos = path.rfind('.')
@@ -206,20 +230,14 @@
 def get_user_detail_serializer():
     """
     Returns the user serializer model that is active in this project.
     """
     return import_string(settings.USER_DETAIL_SERIALIZER)
 
 
-def is_sqlite3(db_key=None):
-    if db_key is None:
-        db_key = DEFAULT_DB_ALIAS
-    return connections.databases[db_key]['ENGINE'].endswith('sqlite3')
-
-
 def validate_redirect(request):
     """
     Get the REDIRECT_FIELD_NAME and validates it is a URL on allowed hosts.
     """
     return validate_redirect_url(request.GET.get(REDIRECT_FIELD_NAME, None))
```

### Comparing `djaodjin-survey-0.9.2/survey/views/campaigns.py` & `djaodjin-survey-0.9.3/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/views/createquestion.py` & `djaodjin-survey-0.9.3/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/views/edit.py` & `djaodjin-survey-0.9.3/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/views/matrix.py` & `djaodjin-survey-0.9.3/survey/views/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         context = super(CompareView, self).get_context_data(**kwargs)
         url_kwargs = self.get_url_kwargs()
         if self.path_url_kwarg in self.kwargs:
             url_kwargs.update({
                 self.path_url_kwarg: self.kwargs.get(self.path_url_kwarg)})
             update_context_urls(context, {
                 'survey_api_compare_samples': reverse(
-                    'survey_api_compare_samples_path', kwargs=url_kwargs),
+                    'survey_api_compare_samples', kwargs=url_kwargs),
             })
         else:
             update_context_urls(context, {
                 'survey_api_compare_samples': reverse(
-                    'survey_api_compare_samples', kwargs=url_kwargs),
+                    'survey_api_compare_samples_index', kwargs=url_kwargs),
             })
         return context
 
 
 class MatrixListView(MatrixQuerysetMixin, ListView):
 
     template_name = "survey/matrix/index.html"
```

### Comparing `djaodjin-survey-0.9.2/survey/views/portfolios.py` & `djaodjin-survey-0.9.3/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.2/survey/views/sample.py` & `djaodjin-survey-0.9.3/survey/views/sample.py`

 * *Files identical despite different names*

