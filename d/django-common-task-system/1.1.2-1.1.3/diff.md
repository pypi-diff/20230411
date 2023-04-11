# Comparing `tmp/django-common-task-system-1.1.2.tar.gz` & `tmp/django-common-task-system-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.2.tar", last modified: Mon Mar 27 03:00:30 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.3.tar", last modified: Tue Apr 11 06:32:32 2023, max compression
```

## Comparing `django-common-task-system-1.1.2.tar` & `django-common-task-system-1.1.3.tar`

### file list

```diff
@@ -1,50 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.212952 django-common-task-system-1.1.2/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-03-27 03:00:30.212952 django-common-task-system-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.065998 django-common-task-system-1.1.2/django_common_task_system/
--rw-rw-rw-   0        0        0     1569 2023-03-13 07:52:28.000000 django-common-task-system-1.1.2/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     5541 2023-03-22 07:31:00.000000 django-common-task-system-1.1.2/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-02-28 03:54:26.000000 django-common-task-system-1.1.2/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.2/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.2/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.2/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.093116 django-common-task-system-1.1.2/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7466 2023-03-07 07:17:56.000000 django-common-task-system-1.1.2/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.2/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0    22489 2023-03-27 02:49:06.000000 django-common-task-system-1.1.2/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.2/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:29.994432 django-common-task-system-1.1.2/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:29.995858 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.104067 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.130714 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:29.996865 django-common-task-system-1.1.2/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.184952 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.2/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      747 2023-03-17 03:41:25.000000 django-common-task-system-1.1.2/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.210951 django-common-task-system-1.1.2/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.2/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.2/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.2/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.2/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.2/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0     4815 2023-03-27 03:00:01.000000 django-common-task-system-1.1.2/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-03-27 03:00:30.085517 django-common-task-system-1.1.2/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-03-27 03:00:29.000000 django-common-task-system-1.1.2/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-03-27 03:00:29.000000 django-common-task-system-1.1.2/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 03:00:29.000000 django-common-task-system-1.1.2/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-03-27 03:00:29.000000 django-common-task-system-1.1.2/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-03-27 03:00:29.000000 django-common-task-system-1.1.2/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 03:00:30.212952 django-common-task-system-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-03-27 02:49:33.000000 django-common-task-system-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.105694 django-common-task-system-1.1.3/django_common_task_system/
+-rw-rw-rw-   0        0        0     2197 2023-04-07 08:17:44.000000 django-common-task-system-1.1.3/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.3/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.3/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.3/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.3/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.3/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.134439 django-common-task-system-1.1.3/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0    23017 2023-04-07 08:40:33.000000 django-common-task-system-1.1.3/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.3/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.032055 django-common-task-system-1.1.3/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.033052 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.145617 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.173028 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.192031 django-common-task-system-1.1.3/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4824 2023-04-11 06:00:14.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.200622 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.202622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-04-07 08:04:08.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.205622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-04-11 05:57:33.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.213622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1113 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      325 2023-04-06 02:19:24.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.034057 django-common-task-system-1.1.3/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.269538 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.3/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.3/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.288649 django-common-task-system-1.1.3/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.3/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.3/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.3/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.3/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.3/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.3/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.124438 django-common-task-system-1.1.3/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3411 2023-04-11 06:32:32.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-07 09:00:10.000000 django-common-task-system-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.3/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.2/LICENSE` & `django-common-task-system-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/__init__.py` & `django-common-task-system-1.1.3/django_common_task_system/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from django.contrib.auth import get_user_model
-import inspect
-import re
-
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
 
 if not hasattr(settings, 'TASK_MODEL'):
     setattr(settings, 'TASK_MODEL', 'django_common_task_system.Task')
 
+if not hasattr(settings, 'TASK_SCHEDULE_MODEL'):
+    setattr(settings, 'TASK_SCHEDULE_MODEL', 'django_common_task_system.TaskSchedule')
+
 if not hasattr(settings, 'TASK_SCHEDULE_LOG_MODEL'):
     setattr(settings, 'TASK_SCHEDULE_LOG_MODEL', 'django_common_task_system.TaskScheduleLog')
 
 
 def get_task_model():
     """
     Return the User model that is active in this project.
@@ -27,22 +26,39 @@
     except LookupError:
         raise ImproperlyConfigured(
             "TASK_MODEL refers to model '%s' that has not been installed"
             % settings.TASK_MODEL
         )
 
 
+def get_task_schedule_model():
+    """
+    Return the User model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.TASK_SCHEDULE_MODEL, require_ready=False)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_MODEL must be of the form 'app_label.model_name'"
+        )
+    except LookupError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_MODEL refers to model '%s' that has not been installed"
+            % settings.TASK_SCHEDULE_MODEL
+        )
+
+
 def get_schedule_log_model():
     """
     Return the User model that is active in this project.
     """
     try:
         return django_apps.get_model(settings.TASK_SCHEDULE_LOG_MODEL, require_ready=False)
     except ValueError:
         raise ImproperlyConfigured(
             "TASK_SCHEDULE_LOG_MODEL must be of the form 'app_label.model_name'"
         )
     except LookupError:
         raise ImproperlyConfigured(
             "TASK_SCHEDULE_LOG_MODEL refers to model '%s' that has not been installed"
             % settings.SCHEDULE_LOG_MODEL
-        )
+        )
```

### Comparing `django-common-task-system-1.1.2/django_common_task_system/choices.py` & `django-common-task-system-1.1.3/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/fields.py` & `django-common-task-system-1.1.3/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/forms.py` & `django-common-task-system-1.1.3/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.3/django_common_task_system/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-# Generated by Django 4.1.7 on 2023-03-07 15:14
+# Generated by Django 4.1.7 on 2023-03-30 03:30
 
-import django_common_objects.fields
-import django_common_objects.models
 import datetime
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
+import django_common_objects.fields
+import django_common_objects.models
 import django_common_task_system.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('django_common_objects', '0001_initial'),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('django_common_objects', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Task',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('name', models.CharField(max_length=100, verbose_name='任务名')),
                 ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
                 ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('Task'), null=True, verbose_name='参数')),
                 ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
                 ('category', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_objects.commoncategory', verbose_name='类别')),
-                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_task_system.task', verbose_name='父任务')),
+                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to=settings.TASK_MODEL, verbose_name='父任务')),
                 ('tags', models.ManyToManyField(blank=True, db_constraint=False, to='django_common_objects.commontag', verbose_name='标签')),
                 ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
             ],
             options={
                 'verbose_name': '任务中心',
                 'verbose_name_plural': '任务中心',
                 'db_table': 'taskhub',
+                'abstract': False,
+                'swappable': 'TASK_MODEL',
                 'unique_together': {('name', 'user', 'parent')},
             },
         ),
         migrations.CreateModel(
             name='TaskSchedule',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
@@ -54,32 +56,18 @@
                 ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
             ],
             options={
                 'verbose_name': '任务计划',
                 'verbose_name_plural': '任务计划',
-                'db_table': 'django_common_task_system',
+                'db_table': 'task_schedule',
                 'ordering': ('-priority', 'next_schedule_time'),
-            },
-        ),
-        migrations.CreateModel(
-            name='TaskScheduleLog',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
-                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
-                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.taskschedule', verbose_name='任务计划')),
-            ],
-            options={
-                'verbose_name': '任务日志',
-                'verbose_name_plural': '任务日志',
-                'db_table': 'django_common_task_system_log',
+                'abstract': False,
+                'swappable': 'TASK_SCHEDULE_MODEL',
             },
         ),
         migrations.CreateModel(
             name='TaskScheduleCallback',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('name', models.CharField(max_length=100, verbose_name='回调')),
@@ -90,27 +78,50 @@
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
                 ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
             ],
             options={
                 'verbose_name': '任务回调',
                 'verbose_name_plural': '任务回调',
-                'db_table': 'django_common_task_system_callback',
+                'db_table': 'task_schedule_callback',
+                'abstract': False,
                 'unique_together': {('name', 'user')},
             },
         ),
+        migrations.CreateModel(
+            name='TaskScheduleLog',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
+                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
+                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_SCHEDULE_MODEL, verbose_name='任务计划')),
+            ],
+            options={
+                'verbose_name': '任务日志',
+                'verbose_name_plural': '任务日志',
+                'db_table': 'task_schedule_log',
+                'abstract': False,
+                'swappable': 'TASK_SCHEDULE_LOG_MODEL',
+            },
+        ),
         migrations.AddField(
             model_name='taskschedule',
             name='callback',
             field=models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.taskschedulecallback', verbose_name='回调'),
         ),
         migrations.AddField(
             model_name='taskschedule',
             name='task',
-            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.task', verbose_name='任务'),
+            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_MODEL, verbose_name='任务'),
         ),
         migrations.AddField(
             model_name='taskschedule',
             name='user',
             field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户'),
         ),
+        migrations.AlterUniqueTogether(
+            name='taskschedule',
+            unique_together={('task', 'user')},
+        ),
     ]
```

### Comparing `django-common-task-system-1.1.2/django_common_task_system/models.py` & `django-common-task-system-1.1.3/django_common_task_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 class Task(AbstractTask):
 
     class Meta(AbstractTask.Meta):
         swappable = 'TASK_MODEL'
         abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
 
 
-class TaskScheduleCallback(models.Model):
+class AbstractScheduleCallback(models.Model):
     id = models.AutoField(primary_key=True)
     name = models.CharField(max_length=100, verbose_name='回调')
     description = models.TextField(blank=True, null=True, verbose_name='描述')
     trigger_event = common_fields.CharField(default=TaskCallbackEvent.DONE, choices=TaskCallbackEvent.choices,
                                             verbose_name='触发事件')
     status = common_fields.CharField(default=TaskCallbackStatus.ENABLE.value, verbose_name='状态',
                                      choices=TaskCallbackStatus.choices)
@@ -75,22 +75,27 @@
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
     update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
 
     class Meta:
         db_table = 'task_schedule_callback'
         verbose_name = verbose_name_plural = '任务回调'
         unique_together = ('name', 'user')
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+        abstract = True
 
     def __str__(self):
         return self.name
 
     __repr__ = __str__
 
 
+class TaskScheduleCallback(AbstractScheduleCallback):
+    class Meta(AbstractScheduleCallback.Meta):
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
 class ScheduleConfig:
 
     def __init__(self,
                  base_on_now=True,
                  nlp_sentence=None,
                  schedule_type=None,
                  crontab=None,
@@ -202,20 +207,20 @@
                 raise ValidationError("timing_type is invalid")
         else:
             raise ValidationError("type<%s> is invalid" % schedule_type)
         return config
 
     def get_current_time(self, start_time=None):
         if self.base_on_now:
-            now = timezone.now()
+            now = datetime.now()
         else:
             if start_time and start_time != datetime.min:
-                now = start_time
+                now = datetime.fromtimestamp(start_time.timestamp())
             else:
-                now = timezone.now()
+                now = datetime.now()
         now_seconds = now.hour * 3600 + now.minute * 60 + now.second
         schedule_type = self.schedule_type
         type_config = self.config[schedule_type]
         schedule_time = None
         if schedule_type == TaskScheduleType.CONTINUOUS.value:
             schedule_time, period = self.period_schedule
             while schedule_time < now:
@@ -380,15 +385,15 @@
         elif schedule_type == TaskScheduleType.ONCE:
             next_time = datetime.max
         else:
             raise ValidationError("unsupported schedule type: %s" % schedule_type)
         return next_time
 
 
-class TaskSchedule(models.Model):
+class AbstractTaskSchedule(models.Model):
     id = models.AutoField(primary_key=True)
     task = models.ForeignKey(settings.TASK_MODEL, on_delete=models.CASCADE, db_constraint=False, verbose_name='任务')
     priority = models.IntegerField(default=0, verbose_name='优先级')
     next_schedule_time = models.DateTimeField(default=timezone.now, verbose_name='下次运行时间', db_index=True)
     schedule_start_time = models.DateTimeField(default=datetime.min, verbose_name='开始时间')
     schedule_end_time = models.DateTimeField(default=datetime.max, verbose_name='结束时间')
     config = fields.ScheduleConfigField(default=dict, verbose_name='参数')
@@ -413,29 +418,35 @@
         self.save(update_fields=('next_schedule_time', 'status'))
         return self
 
     class Meta:
         db_table = 'task_schedule'
         verbose_name = verbose_name_plural = '任务计划'
         ordering = ('-priority', 'next_schedule_time')
-        unique_together = ('task', 'user')
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+        unique_together = ('task', 'status', 'user')
+        abstract = True
 
     def __str__(self):
         return self.task.name
 
     __repr__ = __str__
 
     def __lt__(self, other):
         return self.priority < other.priority
 
     def __gt__(self, other):
         return self.priority > other.priority
 
 
+class TaskSchedule(AbstractTaskSchedule):
+    class Meta(AbstractTaskSchedule.Meta):
+        swappable = 'TASK_SCHEDULE_MODEL'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
 class AbstractTaskScheduleLog(models.Model):
     id = models.AutoField(primary_key=True)
     schedule = models.ForeignKey(TaskSchedule, db_constraint=False, on_delete=models.CASCADE, verbose_name='任务计划')
     status = common_fields.CharField(verbose_name='运行状态')
     result = common_fields.ConfigField(blank=True, null=True, verbose_name='结果')
     schedule_time = models.DateTimeField(verbose_name='计划时间')
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
@@ -448,11 +459,13 @@
     def __str__(self):
         return "schedule: %s, status: %s" % (self.schedule, self.status)
 
     __repr__ = __str__
 
 
 class TaskScheduleLog(AbstractTaskScheduleLog):
+    schedule = models.ForeignKey(TaskSchedule, db_constraint=False, related_name='logs',
+                                 on_delete=models.CASCADE, verbose_name='任务计划')
 
     class Meta(AbstractTaskScheduleLog.Meta):
         swappable = 'TASK_SCHEDULE_LOG_MODEL'
         abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
```

### Comparing `django-common-task-system-1.1.2/django_common_task_system/serializers.py` & `django-common-task-system-1.1.3/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/urls.py` & `django-common-task-system-1.1.3/django_common_task_system/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,13 +6,15 @@
 router.register(r'schedule-log', views.ScheduleLogViewSet)
 
 
 urlpatterns = [
     path('task/', views.TaskListView.as_view()),
     path('task/<int:pk>/', views.TaskDetailView.as_view()),
     path('schedule/', views.TaskScheduleListView.as_view()),
+    path('schedule/retry/<int:pk>/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
+    path('schedule/queue/<int:pk>/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
     path('schedule/<int:pk>/', views.TaskScheduleDetailView.as_view()),
     path('schedule/queue/get/', views.TaskScheduleQueueAPI.get),
-    path('schedule/queue/', views.TaskScheduleQueueAPI.size),
+    path('schedule/queue/', views.TaskScheduleQueueAPI.status),
     path('schedule/queue/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
     path('schedule/time-parse/', views.ScheduleTimeParseView.as_view()),
 ] + router.urls
```

### Comparing `django-common-task-system-1.1.2/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.3/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.3/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.3/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.2/django_common_task_system/views.py` & `django-common-task-system-1.1.3/django_common_task_system/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from rest_framework import status
 from rest_framework.decorators import api_view
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
-from . import serializers, get_task_model, get_schedule_log_model
+from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model
 from .models import TaskSchedule
 from .choices import TaskScheduleStatus
 from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
 from queue import Queue, Empty
 from datetime import datetime
 from jionlp_time import parse_time
 from .utils.schedule_time import nlp_config_to_schedule_config
 from threading import Lock
 
 
 schedule_queue_lock = Lock()
 TaskModel = get_task_model()
 ScheduleLogModel = get_schedule_log_model()
+ScheduleModel = get_task_schedule_model()
 
 
-status_params_mapping = {
+params_status_mapping = {
     'opening': TaskScheduleStatus.OPENING.value,
     'closed': TaskScheduleStatus.CLOSED.value,
     'test': TaskScheduleStatus.TEST.value,
     'done': TaskScheduleStatus.DONE.value,
     'error': TaskScheduleStatus.ERROR.value,
 }
 
+status_params_mapping = {v: k for k, v in params_status_mapping.items()}
+
+
+def get_schedule_queue(schedule: ScheduleModel):
+    return TaskScheduleQueueAPI.queue_mapping[status_params_mapping[schedule.status]]
+
 
 class QueueMapping(dict):
 
     def __init__(self, keys):
         super().__init__()
         for key in keys:
             self[key] = Queue()
@@ -59,31 +66,31 @@
 
 class ScheduleLogViewSet(ModelViewSet):
     queryset = ScheduleLogModel.objects.all()
     serializer_class = serializers.TaskScheduleLogSerializer
 
 
 class TaskScheduleQueueAPI:
-    queue_mapping = QueueMapping(status_params_mapping)
+    queue_mapping = QueueMapping(params_status_mapping)
 
     @staticmethod
     def query_expiring_schedules(queue, schedule_status):
         now = datetime.now()
         queryset = TaskSchedule.objects.filter(next_schedule_time__lte=now, status=TaskScheduleStatus.OPENING.value)
         for schedule in queryset:
             queue.put(serializers.QueueScheduleSerializer(schedule).data)
-            queue.generate_next_schedule()
+            schedule.generate_next_schedule()
         return queryset
 
     @staticmethod
     @api_view(['GET'])
     def get(request: Request):
         schedule_status = request.query_params.get('status', 'opening')
-        if schedule_status not in status_params_mapping:
-            return Response({'error': 'status must be in {}'.format(list(status_params_mapping.keys()))},
+        if schedule_status not in params_status_mapping:
+            return Response({'error': 'status must be in {}'.format(list(params_status_mapping.keys()))},
                             status=status.HTTP_400_BAD_REQUEST)
         queue = TaskScheduleQueueAPI.queue_mapping[schedule_status]
         try:
             schedule = queue.get(block=False)
         except Empty:
             try:
                 if schedule_queue_lock.locked():
@@ -106,15 +113,44 @@
             schedule = TaskSchedule.objects.get(id=pk)
             return Response(serializers.QueueScheduleSerializer(schedule).data)
         except TaskSchedule.DoesNotExist:
             return Response({'msg': 'schedule not found'}, status=status.HTTP_404_NOT_FOUND)
 
     @staticmethod
     @api_view(['GET'])
-    def size(request):
+    def retry(request, pk):
+        try:
+            # 重试失败的任务, 这里的pk应该是schedule_log的id，schedule是会变的
+            log = ScheduleLogModel.objects.get(id=pk)
+        except ScheduleLogModel.DoesNotExist:
+            return Response({'error': 'schedule_id(%s)不存在, 重试失败' % pk}, status=status.HTTP_404_NOT_FOUND)
+        try:
+            queue = get_schedule_queue(log.schedule)
+            queue.put(serializers.QueueScheduleSerializer(log.schedule).data)
+            return Response({'message': '成功添加到重试队列'})
+        except Exception as e:
+            return Response({'error': '重试失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+
+    @staticmethod
+    @api_view(['GET'])
+    def put(request: Request, pk: int):
+        try:
+            schedule = TaskSchedule.objects.get(id=pk)
+        except TaskSchedule.DoesNotExist:
+            return Response({'error': 'TaskSchedule(%s)不存在, 重试失败' % pk}, status=status.HTTP_404_NOT_FOUND)
+        try:
+            queue = get_schedule_queue(schedule)
+            queue.put(serializers.QueueScheduleSerializer(schedule).data)
+            return Response({'message': '成功添加到队列'})
+        except Exception as e:
+            return Response({'error': '添加到队列失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+
+    @staticmethod
+    @api_view(['GET'])
+    def status(request):
         return Response({x: y.qsize() for x, y in TaskScheduleQueueAPI.queue_mapping.items()})
 
 
 class ScheduleTimeParseView(APIView):
 
     def get(self, request, *args, **kwargs):
         sentence = request.query_params.get('sentence')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-common-task-system-1.1.2/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.3/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,23 +15,49 @@
 django_common_task_system/views.py
 django_common_task_system.egg-info/PKG-INFO
 django_common_task_system.egg-info/SOURCES.txt
 django_common_task_system.egg-info/dependency_links.txt
 django_common_task_system.egg-info/requires.txt
 django_common_task_system.egg-info/top_level.txt
 django_common_task_system/migrations/0001_initial.py
+django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
 django_common_task_system/migrations/__init__.py
 django_common_task_system/static/common_task_system/css/calendar.css
 django_common_task_system/static/common_task_system/css/task_schedule_admin.css
 django_common_task_system/static/common_task_system/js/calendar.js
 django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+django_common_task_system/system_task/__init__.py
+django_common_task_system/system_task/admin.py
+django_common_task_system/system_task/apps.py
+django_common_task_system/system_task/choices.py
+django_common_task_system/system_task/forms.py
+django_common_task_system/system_task/models.py
+django_common_task_system/system_task/process.py
+django_common_task_system/system_task/tests.py
+django_common_task_system/system_task/urls.py
+django_common_task_system/system_task/views.py
+django_common_task_system/system_task/migrations/0001_initial.py
+django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+django_common_task_system/system_task/migrations/__init__.py
+django_common_task_system/system_task_execution/__init__.py
+django_common_task_system/system_task_execution/main.py
+django_common_task_system/system_task_execution/system_task_execution/__init__.py
+django_common_task_system/system_task_execution/system_task_execution/executor.py
+django_common_task_system/system_task_execution/system_task_execution/settings.py
+django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
 django_common_task_system/templates/task_schedule/datetime_range.html
 django_common_task_system/templates/task_schedule/multi_day_select.html
 django_common_task_system/templates/task_schedule/multi_month_day_select.html
 django_common_task_system/templates/task_schedule/nlp_input.html
 django_common_task_system/templates/task_schedule/period.html
 django_common_task_system/templates/task_schedule/period_schedule.html
 django_common_task_system/utils/__init__.py
 django_common_task_system/utils/algorithm.py
 django_common_task_system/utils/cron_utils.py
 django_common_task_system/utils/foreign_key.py
-django_common_task_system/utils/schedule_time.py
+django_common_task_system/utils/schedule_time.py
+tests/__init__.py
```

### Comparing `django-common-task-system-1.1.2/setup.py` & `django-common-task-system-1.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.2',
+    version='1.1.3',
     install_requires=[
-        "django-common-objects>=1.0.4",
+        "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
     ],
     include_package_data=True,
```

