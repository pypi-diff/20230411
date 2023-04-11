# Comparing `tmp/django_rq_scheduler-2023.5.0b2.tar.gz` & `tmp/django_rq_scheduler-2023.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.5.0b2.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.5.0b3.tar", max compression
```

## Comparing `django_rq_scheduler-2023.5.0b2.tar` & `django_rq_scheduler-2023.5.0b3.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0     1096 2023-04-10 22:08:15.141312 django_rq_scheduler-2023.5.0b2/LICENSE
--rw-r--r--   0        0        0     1711 2023-04-10 22:08:15.141312 django_rq_scheduler-2023.5.0b2/README.md
--rw-r--r--   0        0        0     1741 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/pyproject.toml
--rw-r--r--   0        0        0      134 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5461 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/job.py
--rw-r--r--   0        0        0     1646 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      481 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/apps.py
--rw-r--r--   0        0        0     1147 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1189 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1908 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3602 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     2902 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0     1051 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1279 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      662 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     6512 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/queue.py
--rw-r--r--   0        0        0    15395 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/py.typed
--rw-r--r--   0        0        0     5452 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/queues.py
--rw-r--r--   0        0        0     2963 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/rq_classes.py
--rw-r--r--   0        0        0      822 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/settings.py
--rw-r--r--   0        0        0     2628 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1559 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     1282 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/delete_job.html
--rw-r--r--   0        0        0     7124 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     6331 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0     1055 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     4120 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3062 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1835 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0      541 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      535 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5483 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2777 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    26904 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2184 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    14315 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_views.py
--rw-r--r--   0        0        0      517 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3323 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     3273 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tools.py
--rw-r--r--   0        0        0     1735 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/urls.py
--rw-r--r--   0        0        0    15878 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/views.py
--rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-04-11 19:00:13.252306 django_rq_scheduler-2023.5.0b3/LICENSE
+-rw-r--r--   0        0        0     1704 2023-04-11 19:00:13.252306 django_rq_scheduler-2023.5.0b3/README.md
+-rw-r--r--   0        0        0     1741 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5668 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1646 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      481 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/apps.py
+-rw-r--r--   0        0        0     1147 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1189 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1908 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3417 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3602 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     2962 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     7162 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0     1051 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/queue.py
+-rw-r--r--   0        0        0    15168 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/py.typed
+-rw-r--r--   0        0        0     5406 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/queues.py
+-rw-r--r--   0        0        0     5151 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/rq_classes.py
+-rw-r--r--   0        0        0      822 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1559 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     1282 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/delete_job.html
+-rw-r--r--   0        0        0     7124 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2574 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6285 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0     1055 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     4120 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1875 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0      628 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     4304 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27451 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2204 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    15014 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1183 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3323 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     3399 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/tools.py
+-rw-r--r--   0        0        0     1736 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/urls.py
+-rw-r--r--   0        0        0    16289 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/views.py
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b3/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.5.0b2/LICENSE` & `django_rq_scheduler-2023.5.0b3/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022- Daniel Moran, 2016 iStrategyLabs, LLC
+Copyright (c) 2022- Daniel Moran, (Before 2016 - iStrategyLabs, LLC)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django_rq_scheduler-2023.5.0b2/README.md` & `django_rq_scheduler-2023.5.0b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Django RQ Scheduler
 ===================
 [![Django CI](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml/badge.svg)](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml)
 ![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cunla/b756396efb895f0e34558c980f1ca0c7/raw/django-rq-scheduler-4.json)
-
 [![badge](https://img.shields.io/pypi/dm/django-rq-scheduler)](https://pypi.org/project/django-rq-scheduler/)
 [![Open Source Helpers](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler/badges/users.svg)](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler)
 
 Documentation can be found in https://django-rq-scheduler.readthedocs.io/en/latest/
 
-> Notice:
-> 
-> In v2023.3.0, django-rq-scheduler was refactored significantly to support
+>  **Warning**: In v2023.3.0, django-rq-scheduler was refactored significantly to support
 > calculation of parameters in runtime.
-> 
 > You can now add a callable param to your scheduled job, and it will be
 > calculated when the job is performed.
 > 
 > 1. It is highly recommended you save your existing database before upgrading!
 > 2. Once you upgraded, recreate your jobs.
 
-> Notice:
-> 
-> Starting v2023.1, requirement for rq_scheduler was removed and instead
+> **Note** Starting v2023.1, requirement for rq_scheduler was removed and instead
 > one of the django-rq workers should run with `--with-scheduler` parameter
 > as mentioned [here](https://github.com/rq/django-rq#support-for-scheduled-jobs).
 
 
 # Sponsor
 
 django-rq-scheduler is developed for free.
```

### Comparing `django_rq_scheduler-2023.5.0b2/pyproject.toml` & `django_rq_scheduler-2023.5.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.5.0b2"
+version = "2023.5.0b3"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
 ]
 maintainers = [
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/admin/job.py` & `django_rq_scheduler-2023.5.0b3/scheduler/admin/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import redis
 from django.contrib import admin, messages
 from django.contrib.contenttypes.admin import GenericStackedInline
 from django.utils.translation import gettext_lazy as _
 
 from scheduler import tools
 from scheduler.models import CronJob, JobArg, JobKwarg, RepeatableJob, ScheduledJob
+from scheduler.queues import logger
 from scheduler.settings import SCHEDULER
 from scheduler.tools import get_job_executions
 
 
 class HiddenMixin(object):
     class Media:
         js = ['admin/js/jquery.init.js', ]
@@ -51,15 +53,19 @@
             'fields': ('queue', 'job_id',),
         }),
     )
 
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra = extra_context or {}
         obj = self.get_object(request, object_id)
-        execution_list = get_job_executions(obj.queue, obj)
+        try:
+            execution_list = get_job_executions(obj.queue, obj)
+        except redis.ConnectionError as e:
+            logger.warn(f'Could not get job executions: {e}')
+            execution_list = list()
         paginator = self.get_paginator(request, execution_list, SCHEDULER['EXECUTIONS_IN_PAGE'])
         page_number = request.GET.get('p', 1)
         page_obj = paginator.get_page(page_number)
         page_range = paginator.get_elided_page_range(page_obj.number)
 
         extra.update({
             "pagination_required": paginator.count > SCHEDULER['EXECUTIONS_IN_PAGE'],
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.5.0b3/scheduler/admin/redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/decorators.py` & `django_rq_scheduler-2023.5.0b3/scheduler/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqworker.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,17 @@
                             help='Default worker timeout to be used')
         parser.add_argument('--max-jobs', action='store', default=None, dest='max_jobs', type=int,
                             help='Maximum number of jobs to execute before terminating worker')
         parser.add_argument(
             'queues', nargs='*', type=str,
             help='The queues to work on, separated by space, all queues should be using the same redis')
 
-    def handle(self, *queues, **options):
+    def handle(self, **options):
+        queues = options.get('queues', 'default')
+        click.echo(f'Starting worker for queues {queues}')
         pidfile = options.get('pidfile')
         if pidfile:
             with open(os.path.expanduser(pidfile), "w") as fp:
                 fp.write(str(os.getpid()))
 
         # Verbosity is defined by default in BaseCommand for all commands
         verbosity = options.get('verbosity', 1)
@@ -68,13 +70,12 @@
             # without this, jobs using RQ's get_current_job() will fail
             use_connection(w.connection)
 
             # Close any opened DB connection before any fork
             reset_db_connections()
 
             w.work(burst=options.get('burst', False),
-                   with_scheduler=True,
                    logging_level=verbosity,
                    max_jobs=options['max_jobs'], )
         except ConnectionError as e:
             click.echo(str(e), err=True)
             sys.exit(1)
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # Generated by Django 4.1.7 on 2023-03-12 19:53
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ('scheduler', '0008_rename_str_val_jobarg_val_and_more'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='jobarg',
             name='arg_type',
-            field=models.CharField(choices=[('str', 'string'), ('int', 'int'), ('bool', 'boolean'), ('datetime', 'datetime'), ('callable', 'callable')], default='str', max_length=12, verbose_name='Argument Type'),
+            field=models.CharField(
+                choices=[('str', 'string'), ('int', 'int'), ('bool', 'boolean'), ('datetime', 'datetime'),
+                         ('callable', 'callable')], default='str', max_length=12, verbose_name='Argument Type'),
         ),
         migrations.AlterField(
             model_name='jobarg',
             name='val',
             field=models.CharField(blank=True, max_length=255, verbose_name='Argument Value'),
         ),
         migrations.AlterField(
             model_name='jobkwarg',
             name='arg_type',
-            field=models.CharField(choices=[('str', 'string'), ('int', 'int'), ('bool', 'boolean'), ('datetime', 'datetime'), ('callable', 'callable')], default='str', max_length=12, verbose_name='Argument Type'),
+            field=models.CharField(
+                choices=[('str', 'string'), ('int', 'int'), ('bool', 'boolean'), ('datetime', 'datetime'),
+                         ('callable', 'callable')], default='str', max_length=12, verbose_name='Argument Type'),
         ),
         migrations.AlterField(
             model_name='jobkwarg',
             name='val',
             field=models.CharField(blank=True, max_length=255, verbose_name='Argument Value'),
         ),
     ]
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0010_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.7 on 2023-03-16 20:59
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ('scheduler', '0009_alter_jobarg_arg_type_alter_jobarg_val_and_more'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Queue',
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.7 on 2023-04-03 00:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ('scheduler', '0010_queue'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Worker',
@@ -20,100 +19,131 @@
                 'permissions': [['view', 'Access admin page']],
                 'managed': False,
                 'default_permissions': (),
             },
         ),
         migrations.AlterModelOptions(
             name='queue',
-            options={'default_permissions': (), 'managed': False, 'permissions': [['view', 'Access admin page']], 'verbose_name_plural': ' Queues'},
+            options={'default_permissions': (), 'managed': False, 'permissions': [['view', 'Access admin page']],
+                     'verbose_name_plural': ' Queues'},
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='at_front',
-            field=models.BooleanField(blank=True, default=False, help_text='When queuing the job, add it in the front of the queue', null=True, verbose_name='At front'),
+            field=models.BooleanField(blank=True, default=False,
+                                      help_text='When queuing the job, add it in the front of the queue', null=True,
+                                      verbose_name='At front'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='cron_string',
-            field=models.CharField(help_text='Define the schedule in a crontab like syntax.\n            Times are in UTC. Use <a href="https://crontab.guru/">crontab.guru</a> to create a cron string.', max_length=64, verbose_name='cron string'),
+            field=models.CharField(
+                help_text='Define the schedule in a crontab like syntax.\n            Times are in UTC. Use <a href="https://crontab.guru/">crontab.guru</a> to create a cron string.',
+                max_length=64, verbose_name='cron string'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='enabled',
-            field=models.BooleanField(default=True, help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled', verbose_name='enabled'),
+            field=models.BooleanField(default=True,
+                                      help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled',
+                                      verbose_name='enabled'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='job_id',
-            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128, null=True, verbose_name='job id'),
+            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128,
+                                   null=True, verbose_name='job id'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='queue',
-            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')], help_text='Queue name', max_length=16, verbose_name='queue'),
+            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')],
+                                   help_text='Queue name', max_length=16, verbose_name='queue'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='repeat',
-            field=models.PositiveIntegerField(blank=True, help_text='Number of times to run the job. Leaving this blank means it will run forever.', null=True, verbose_name='repeat'),
+            field=models.PositiveIntegerField(blank=True,
+                                              help_text='Number of times to run the job. Leaving this blank means it will run forever.',
+                                              null=True, verbose_name='repeat'),
         ),
         migrations.AlterField(
             model_name='cronjob',
             name='result_ttl',
-            field=models.IntegerField(blank=True, help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.', null=True, verbose_name='result ttl'),
+            field=models.IntegerField(blank=True,
+                                      help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.',
+                                      null=True, verbose_name='result ttl'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='at_front',
-            field=models.BooleanField(blank=True, default=False, help_text='When queuing the job, add it in the front of the queue', null=True, verbose_name='At front'),
+            field=models.BooleanField(blank=True, default=False,
+                                      help_text='When queuing the job, add it in the front of the queue', null=True,
+                                      verbose_name='At front'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='enabled',
-            field=models.BooleanField(default=True, help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled', verbose_name='enabled'),
+            field=models.BooleanField(default=True,
+                                      help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled',
+                                      verbose_name='enabled'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='job_id',
-            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128, null=True, verbose_name='job id'),
+            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128,
+                                   null=True, verbose_name='job id'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='queue',
-            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')], help_text='Queue name', max_length=16, verbose_name='queue'),
+            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')],
+                                   help_text='Queue name', max_length=16, verbose_name='queue'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='repeat',
-            field=models.PositiveIntegerField(blank=True, help_text='Number of times to run the job. Leaving this blank means it will run forever.', null=True, verbose_name='repeat'),
+            field=models.PositiveIntegerField(blank=True,
+                                              help_text='Number of times to run the job. Leaving this blank means it will run forever.',
+                                              null=True, verbose_name='repeat'),
         ),
         migrations.AlterField(
             model_name='repeatablejob',
             name='result_ttl',
-            field=models.IntegerField(blank=True, help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.', null=True, verbose_name='result ttl'),
+            field=models.IntegerField(blank=True,
+                                      help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.',
+                                      null=True, verbose_name='result ttl'),
         ),
         migrations.AlterField(
             model_name='scheduledjob',
             name='at_front',
-            field=models.BooleanField(blank=True, default=False, help_text='When queuing the job, add it in the front of the queue', null=True, verbose_name='At front'),
+            field=models.BooleanField(blank=True, default=False,
+                                      help_text='When queuing the job, add it in the front of the queue', null=True,
+                                      verbose_name='At front'),
         ),
         migrations.AlterField(
             model_name='scheduledjob',
             name='enabled',
-            field=models.BooleanField(default=True, help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled', verbose_name='enabled'),
+            field=models.BooleanField(default=True,
+                                      help_text='Should job be scheduled? This field is useful to keep past jobs that should no longer be scheduled',
+                                      verbose_name='enabled'),
         ),
         migrations.AlterField(
             model_name='scheduledjob',
             name='job_id',
-            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128, null=True, verbose_name='job id'),
+            field=models.CharField(blank=True, editable=False, help_text='Current job_id on queue', max_length=128,
+                                   null=True, verbose_name='job id'),
         ),
         migrations.AlterField(
             model_name='scheduledjob',
             name='queue',
-            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')], help_text='Queue name', max_length=16, verbose_name='queue'),
+            field=models.CharField(choices=[('default', 'default'), ('low', 'low'), ('high', 'high')],
+                                   help_text='Queue name', max_length=16, verbose_name='queue'),
         ),
         migrations.AlterField(
             model_name='scheduledjob',
             name='result_ttl',
-            field=models.IntegerField(blank=True, help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.', null=True, verbose_name='result ttl'),
+            field=models.IntegerField(blank=True,
+                                      help_text='The TTL value (in seconds) of the job result.<br/>\n               -1: Result never expires, you should delete jobs manually. <br/>\n                0: Result gets deleted immediately. <br/>\n                >0: Result expires after n seconds.',
+                                      null=True, verbose_name='result ttl'),
         ),
     ]
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/models/args.py` & `django_rq_scheduler-2023.5.0b3/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.5.0b3/scheduler/models/scheduled_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,21 +241,14 @@
             self.schedule()
             super(BaseJob, self).save()
 
     def delete(self, **kwargs):
         self.unschedule()
         super(BaseJob, self).delete(**kwargs)
 
-    def clean_name(self):
-        if '/' in self.name:
-            raise ValidationError({
-                'name': ValidationError(
-                    _('Invalid job name, must not contain /'), code='invalid')
-            })
-
     def clean_callable(self):
         try:
             tools.callable_func(self.callable)
         except Exception:
             raise ValidationError({
                 'callable': ValidationError(
                     _('Invalid callable, must be importable'), code='invalid')
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/queues.py` & `django_rq_scheduler-2023.5.0b3/scheduler/queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,17 @@
     queue_params = QUEUES[queue_names[0]]
     connection_params = _filter_connection_params(queue_params)
     queues = [get_queue(queue_names[0], **kwargs)]
 
     # perform consistency checks while building return list
     for name in queue_names[1:]:
         queue = get_queue(name, **kwargs)
-        if type(queue) is not type(QUEUES[0]):  # noqa: E721
-            raise ValueError(
-                'Queues must have the same class.'
-                '"{0}" and "{1}" have '
-                'different classes'.format(name, queue_names[0])
-            )
+        if type(queue) is not type(queues[0]):  # noqa: E721
+            raise ValueError(f'Queues must have the same class. '
+                             f'"{name}" and "{queue_names[0]}" have different classes')
         if connection_params != _filter_connection_params(QUEUES[name]):
             raise ValueError(
                 f'Queues must have the same redis connection. "{name}" and'
                 f' "{queue_names[0]}" have different connections')
         queues.append(queue)
 
     return queues
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/settings.py` & `django_rq_scheduler-2023.5.0b3/scheduler/settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/delete_job.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/delete_job.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs.html`

 * *Files 8% similar despite different names*

```diff
@@ -54,36 +54,37 @@
                                 <div class="text">
                                     <span><input type="checkbox" id="action-toggle"
                                                  style="display: inline-block;"></span>
                                 </div>
                                 <div class="clear"></div>
                             </th>
                             <th>
-                                <div class='text'><span>ID</span></div>
+                                <div class='text'>ID</div>
                             </th>
                             <th>
-                                <div class='text'><span>Created</span></div>
+                                <div class='text'>Created</div>
+                            </th>
+                            <th>
+                                <div class='text'><span>Scheduled</span></div>
                             </th>
-                            {% if job_status == 'Scheduled' %}
-                                <th>
-                                    <div class='text'><span>Scheduled</span></div>
-                                </th>
-                            {% endif %}
                             <th>
                                 <div class='text'><span>Enqueued</span></div>
                             </th>
                             <th>
                                 <div class='text'><span>Ended</span></div>
                             </th>
                             <th>
                                 <div class='text'><span>Status</span></div>
                             </th>
                             <th>
                                 <div class='text'><span>Callable</span></div>
                             </th>
+                            <th>
+                                <div class='text'><span>Worker</span></div>
+                            </th>
                             {% block extra_columns %}
                             {% endblock extra_columns %}
                         </tr>
                         </thead>
                         <tbody>
                         {% for job in jobs %}
                             <tr class="{% cycle 'row1' 'row2' %}">
@@ -96,27 +97,26 @@
                                     <a href="{% url 'job_details' job.id %}">
                                         {{ job.id }}
                                     </a>
                                 </th>
                                 <td>
                                     {{ job.created_at|date:"Y-m-d, H:i:s" }}
                                 </td>
-                                {% if job_status == 'Scheduled' %}
-                                    <td>
-                                        {{ job.scheduled_at|date:"Y-m-d, H:i:s" }}
-                                    </td>
-                                {% endif %}
+                                <td>
+                                    {{ job.scheduled_at|date:"Y-m-d, H:i:s" }}
+                                </td>
                                 <td>
                                     {{ job.enqueued_at|date:"Y-m-d, H:i:s" }}
                                 </td>
                                 <td>
                                     {{ job.ended_at|date:"Y-m-d, H:i:s" }}
                                 </td>
                                 <td>{{ job.get_status }}</td>
                                 <td>{{ job|show_func_name }}</td>
+                                <td>{{ job.worker_name|default:'-' }}</td>
                                 {% block extra_columns_values %}
                                 {% endblock extra_columns_values %}
                             </tr>
                         {% endfor %}
                         </tbody>
                     </table>
                 </div>
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
     * {% endif %}
     * Empty_Queue
 {% csrf_token %}
 {% if job_status == 'Failed' %}
 Requeue
 {% endif %}
   Go
-�ID     Created              Scheduled              Enqueued              Ended              Status         Callable
-  {      {                    {                      {                     {                  {              {
-�{      {                    {                      {                     {                  {              {
-  job.id job.created_at|date: job.scheduled_at|date: job.enqueued_at|date: job.ended_at|date: job.get_status job|show_func_name
-  }}     "Y-m-d, H:i:s" }}    "Y-m-d, H:i:s" }}      "Y-m-d, H:i:s" }}     "Y-m-d, H:i:s" }}  }}             }}
+�ID     Created              Scheduled              Enqueued              Ended              Status         Callable           Worker
+  {      {                    {                      {                     {                  {              {                  {
+�{      {                    {                      {                     {                  {              {                  {
+  job.id job.created_at|date: job.scheduled_at|date: job.enqueued_at|date: job.ended_at|date: job.get_status job|show_func_name job.worker_name|default:
+  }}     "Y-m-d, H:i:s" }}    "Y-m-d, H:i:s" }}      "Y-m-d, H:i:s" }}     "Y-m-d, H:i:s" }}  }}             }}                 '-' }}
 {% for p in page_range %} {% if p == page %} {{ p }} {% elif forloop.last %} {
 {_p_}} {% else %} {{_p_}} {% endif %} {% endfor %} {{ num_jobs }} jobs
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/stats.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 {% extends 'admin/scheduler/scheduler_base.html' %}
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
-        <a href="{% url 'queues_home' %}">Queues</a> &rsaquo;
-        <a href="{% url 'queue_workers' queue.name %}">{{ queue.name }} Workers</a> &rsaquo;
+        <a href="{% url 'workers_home' %}">Workers</a> &rsaquo;
         <a href="{% url 'worker_details' worker.name %}">{{ worker.name }}</a>
     </div>
 {% endblock %}
 
 {% block content_title %}<h1>Worker Info</h1>{% endblock %}
 
 {% block content %}
-
     <div id="content-main">
-
         <fieldset class="module aligned ">
-
             <div class="form-row">
                 <div>
                     <label class="required">Name:</label>
                     <div class="data">{{ worker.name }}</div>
                 </div>
             </div>
 
@@ -81,15 +77,15 @@
                     <div class="data">{{ worker.failed_job_count|default:0 }}</div>
                 </div>
             </div>
 
             <div class="form-row">
                 <div>
                     <label class="required">Total working time (seconds):</label>
-                    <div class="data">{{ total_working_time|default:0.0 }}</div>
+                    <div class="data">{{ total_working_time|default:0.0 }}ms</div>
                 </div>
             </div>
         </fieldset>
-
+        {% include 'admin/scheduler/jobs-list.partial.html' %}
     </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends 'admin/scheduler/scheduler_base.html' %} {% block breadcrumbs %}
-Home › Queues › {{_queue.name_}}_Workers › {{_worker.name_}}
+Home › Workers › {{_worker.name_}}
 {% endblock %} {% block content_title %}
 ****** Worker Info ******
 {% endblock %} {% block content %}
 Name:
 {{ worker.name }}
 State:
 {{ worker.get_state }}
@@ -17,9 +17,10 @@
 {% if job %} {{ job.func_name }} ({{_job.id_}}) {% else %} No current job {%
 endif %}
 Successful job count:
 {{ worker.successful_job_count|default:0 }}
 Failed job count:
 {{ worker.failed_job_count|default:0 }}
 Total working time (seconds):
-{{ total_working_time|default:0.0 }}
+{{ total_working_time|default:0.0 }}ms
+ {% include 'admin/scheduler/jobs-list.partial.html' %}
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load scheduler_tags %}
 {% load l10n %}
 <div class="results">
     <table id="result_list">
         <thead>
         <tr>
             <th>
                 <div class='text'><span>Name</span></div>
@@ -32,24 +33,24 @@
             </th>
         </tr>
         </thead>
         <tbody>
         {% for worker in workers %}
             <tr class="{% cycle 'row1' 'row2' %}">
                 <td>
-                    <a href='{% url 'worker_details' worker.key %}'>
+                    <a href='{% url 'worker_details' worker.name %}'>
                         {{ worker.name }}
                     </a>
                 </td>
                 <td>{{ worker.get_state }}</td>
                 <td>{{ worker.birth_date|date:"Y-m-d, H:i:s" }}</td>
                 <td>{{ worker.hostname }}</td>
                 <td>{{ worker.pid|unlocalize }}</td>
                 <td>{{ worker.total_working_time|default:0|floatformat }}</td>
                 <td>{{ worker.successful_job_count|default:0 }}</td>
                 <td>{{ worker.failed_job_count|default:0 }}</td>
-                <td>{{ worker.scheduler }}</td>
+                <td>{{ worker | worker_scheduler_pid }}</td>
             </tr>
         {% endfor %}
         </tbody>
     </table>
 </div>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% load l10n %}
-Name        State            Birth                   Hostname        PID                   Working time                       Successful jobs                      Failed jobs                      Scheduler
- worker.key {                {                       {               {                     {                                  {                                    {                                {
-%}'> {      {                {                       {               {                     {                                  {                                    {                                {
-{           worker.get_state worker.birth_date|date: worker.hostname worker.pid|unlocalize worker.total_working_time|default: worker.successful_job_count|default: worker.failed_job_count|default: worker.scheduler
-worker.name }}               "Y-m-d, H:i:s" }}       }}              }}                    0|floatformat }}                   0 }}                                 0 }}                             }}
+{% load scheduler_tags %} {% load l10n %}
+Name         State            Birth                   Hostname        PID                   Working time                       Successful jobs                      Failed jobs                      Scheduler
+ worker.name {                {                       {               {                     {                                  {                                    {
+%}'> {       {                {                       {               {                     {                                  {                                    {                                {{ worker |
+{            worker.get_state worker.birth_date|date: worker.hostname worker.pid|unlocalize worker.total_working_time|default: worker.successful_job_count|default: worker.failed_job_count|default: worker_scheduler_pid
+worker.name  }}               "Y-m-d, H:i:s" }}       }}              }}                    0|floatformat }}                   0 }}                                 0 }}                             }}
 }}
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/jobs.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/jobs.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_job_arg_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,25 +16,35 @@
             arg.clean()
 
     def test_clean_one_value_invalid_str_int(self):
         arg = jobarg_factory(self.JobArgClass, arg_type='int', val='not blank', )
         with self.assertRaises(ValidationError):
             arg.clean()
 
-    def test_callable_arg_type__not_clean(self):
+    def test_clean_callable_invalid(self):
         arg = jobarg_factory(self.JobArgClass, arg_type='callable', val='bad_callable', )
         with self.assertRaises(ValidationError):
             arg.clean()
 
-    def test_clean_invalid(self):
+    def test_clean_datetime_invalid(self):
+        arg = jobarg_factory(self.JobArgClass, arg_type='datetime', val='bad datetime', )
+        with self.assertRaises(ValidationError):
+            arg.clean()
+
+    def test_clean_bool_invalid(self):
+        arg = jobarg_factory(self.JobArgClass, arg_type='bool', val='bad bool', )
+        with self.assertRaises(ValidationError):
+            arg.clean()
+
+    def test_clean_int_invalid(self):
         arg = jobarg_factory(self.JobArgClass, arg_type='int', val='str')
         with self.assertRaises(ValidationError):
             arg.clean()
 
-    def test_clean(self):
+    def test_str_clean(self):
         arg = jobarg_factory(self.JobArgClass, val='something')
         self.assertIsNone(arg.clean())
 
 
 class TestJobArg(TestCase):
     JobArgClass = JobArg
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def assert_response_has_msg(response, message):
     messages = [m.message for m in get_messages(response.wsgi_request)]
     assert message in messages, f'expected "{message}" in {messages}'
 
 
-def has_execution_with_status(django_job, status):
+def has_execution_with_status(django_job, status) -> bool:
     job_list = _get_executions(django_job)
     job_list = [(j.id, j.get_status()) for j in job_list]
     for job in job_list:
         if job[1] == status:
             return True
     print(f'{job_list} does not contain a job with status {status}')
     return False
@@ -286,25 +286,37 @@
             })
             # assert
             self.assertEqual(302, res.status_code)
             job.refresh_from_db()
             queue = get_queue(job.queue)
             self.assertIn(job.job_id, queue.get_job_ids())
 
-        def test_admin_single_view(self):
+        def test_admin_change_view(self):
             # arrange
             self.client.login(username='admin', password='admin')
             job = job_factory(self.JobModelClass, )
             model = job._meta.model.__name__.lower()
             url = reverse(f'admin:scheduler_{model}_change', args=[job.pk, ])
             # act
             res = self.client.get(url)
             # assert
             self.assertEqual(200, res.status_code)
 
+        def test_admin_change_view__bad_redis_connection(self):
+            # arrange
+            self.client.login(username='admin', password='admin')
+            job = job_factory(self.JobModelClass, queue='test2', instance_only=True)
+            job.save(schedule_job=False)
+            model = job._meta.model.__name__.lower()
+            url = reverse(f'admin:scheduler_{model}_change', args=[job.pk, ])
+            # act
+            res = self.client.get(url)
+            # assert
+            self.assertEqual(200, res.status_code)
+
         def test_admin_enqueue_job_now(self):
             # arrange
             self.client.login(username='admin', password='admin')
             job = job_factory(self.JobModelClass, )
             self.assertIsNotNone(job.job_id)
             self.assertTrue(job.is_scheduled())
             data = {
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     },
     'url_with_db': {
         'URL': 'redis://username:password@host:1234/5',
     },
     'url_default_db': {
         'URL': 'redis://username:password@host:1234',
     },
-    'django_rq_test': {
+    'django_rq_scheduler_test': {
         'HOST': 'localhost',
         'PORT': 6379,
         'DB': 0,
     },
     'scheduler_scheduler_active_test': {
         'HOST': 'localhost',
         'PORT': 6379,
@@ -76,15 +76,15 @@
     },
     'worker_scheduler_inactive_test': {
         'HOST': 'localhost',
         'PORT': 6379,
         'DB': 0,
         'ASYNC': False,
     },
-    'django_rq_test2': {
+    'django_rq_scheduler_test2': {
         'HOST': 'localhost',
         'PORT': 6379,
         'DB': 0,
     },
     'test_scheduler': {
         'HOST': 'localhost',
         'PORT': 6379,
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def setUp(self):
         self.user = User.objects.create_user('foo', password='pass')
         self.user.is_staff = True
         self.user.is_active = True
         self.user.save()
         self.client = Client()
         self.client.login(username=self.user.username, password='pass')
-        get_queue('django_rq_test').connection.flushall()
+        get_queue('django_rq_scheduler_test').connection.flushall()
 
     def test_jobs(self):
         """Jobs in queue are displayed properly"""
         queue = get_queue('default')
         job = queue.enqueue(access_self)
         queue_name = 'default'
         response = self.client.get(reverse('queue_jobs', args=[queue_name]))
@@ -117,24 +117,24 @@
         self.assertEqual(len(queue), 1)
 
     def test_delete_job(self):
         """
         In addition to deleting job from Redis, the job id also needs to be
         deleted from Queue.
         """
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
         job = queue.enqueue(access_self)
         self.client.post(reverse('queue_delete_job', args=[queue_name, job.id]), {'post': 'yes'})
         self.assertFalse(JobExecution.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_action_delete_jobs(self):
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         # enqueue some jobs
         job_ids = []
         for _ in range(0, 3):
             job = queue.enqueue(access_self)
             job_ids.append(job.id)
 
@@ -143,16 +143,16 @@
 
         # check if jobs are removed
         for job_id in job_ids:
             self.assertFalse(JobExecution.exists(job_id, connection=queue.connection))
             self.assertNotIn(job_id, queue.job_ids)
 
     def test_enqueue_jobs(self):
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         # enqueue some jobs that depends on other
         previous_job = None
         for _ in range(0, 3):
             job = queue.enqueue(access_self, depends_on=previous_job)
             previous_job = job
 
@@ -166,47 +166,47 @@
 
         # Check that job is updated correctly
         last_job = queue.fetch_job(last_job.id)
         self.assertEqual(last_job.get_status(), ExecutionStatus.QUEUED)
         self.assertIsNotNone(last_job.enqueued_at)
 
     def test_action_requeue_jobs(self):
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         # enqueue some jobs that will fail
         jobs = []
         job_ids = []
         for _ in range(0, 3):
             job = queue.enqueue(failing_job)
             jobs.append(job)
             job_ids.append(job.id)
 
         # do those jobs = fail them
-        worker = create_worker('django_rq_test')
+        worker = create_worker('django_rq_scheduler_test')
         worker.work(burst=True)
 
         # check if all jobs are really failed
         for job in jobs:
             self.assertTrue(job.is_failed)
 
         # re-nqueue failed jobs from failed queue
         self.client.post(reverse('queue_actions', args=[queue_name]), {'action': 'requeue', 'job_ids': job_ids})
 
         # check if we requeue all failed jobs
         for job in jobs:
             self.assertFalse(job.is_failed)
 
     def test_action_stop_jobs(self):
-        queue_name = 'django_rq_test'
+        queue_name = 'django_rq_scheduler_test'
         queue = get_queue(queue_name)
 
         # Enqueue some jobs
         job_ids = []
-        worker = create_worker('django_rq_test')
+        worker = create_worker('django_rq_scheduler_test')
         for _ in range(3):
             job = queue.enqueue(access_self)
             job_ids.append(job.id)
             worker.prepare_job_execution(job)
 
         # Check if the jobs are started
         for job_id in job_ids:
@@ -223,129 +223,139 @@
         self.assertEqual(len(canceled_job_registry), len(job_ids))
 
         for job_id in job_ids:
             self.assertIn(job_id, canceled_job_registry)
 
     def test_clear_queue(self):
         """Test that the queue clear actually clears the queue."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
         job = queue.enqueue(access_self)
         self.client.post(reverse('queue_clear', args=[queue_name]), {'post': 'yes'})
         self.assertFalse(JobExecution.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_finished_jobs(self):
         """Ensure that finished jobs page works properly."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         job = queue.enqueue(access_self)
         registry = queue.finished_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_finished_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_failed_jobs(self):
         """Ensure that failed jobs page works properly."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         # Test that page doesn't fail when FailedJobRegistry is empty
         response = self.client.get(reverse('queue_failed_jobs', args=[queue_name]))
         self.assertEqual(response.status_code, 200)
 
         job = queue.enqueue(access_self)
         registry = queue.failed_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_failed_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_scheduled_jobs(self):
         """Ensure that scheduled jobs page works properly."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         # Test that page doesn't fail when ScheduledJobRegistry is empty
         response = self.client.get(reverse('queue_scheduled_jobs', args=[queue_name]))
         self.assertEqual(response.status_code, 200)
 
         job = queue.enqueue_at(datetime.now(), access_self)
         response = self.client.get(reverse('queue_scheduled_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_scheduled_jobs_registry_removal(self):
         """Ensure that non-existing job is being deleted from registry by view"""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         registry = queue.scheduled_job_registry
         job = queue.enqueue_at(datetime.now(), access_self)
         self.assertEqual(len(registry), 1)
 
         queue.connection.delete(job.key)
         response = self.client.get(reverse('queue_scheduled_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [])
 
         self.assertEqual(len(registry), 0)
 
     def test_started_jobs(self):
         """Ensure that active jobs page works properly."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         job = queue.enqueue(access_self)
         registry = queue.started_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_started_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_deferred_jobs(self):
         """Ensure that active jobs page works properly."""
-        queue = get_queue('django_rq_test')
-        queue_name = 'django_rq_test'
+        queue = get_queue('django_rq_scheduler_test')
+        queue_name = 'django_rq_scheduler_test'
 
         job = queue.enqueue(access_self)
         registry = queue.deferred_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_deferred_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_workers_home(self):
         response = self.client.get(reverse('workers_home'))
         prev_workers = response.context['workers']
-        worker1 = create_worker('django_rq_test')
+        worker1 = create_worker('django_rq_scheduler_test')
         worker1.register_birth()
         worker2 = create_worker('test3')
         worker2.register_birth()
 
         response = self.client.get(reverse('workers_home'))
         self.assertEqual(response.context['workers'], prev_workers + [worker1, worker2])
 
     def test_queue_workers(self):
         """Worker index page should show workers for a specific queue"""
-        queue_name = 'django_rq_test'
+        queue_name = 'django_rq_scheduler_test'
 
-        worker1 = create_worker('django_rq_test')
+        worker1 = create_worker('django_rq_scheduler_test')
         worker1.register_birth()
         worker2 = create_worker('test3')
         worker2.register_birth()
 
         response = self.client.get(reverse('queue_workers', args=[queue_name]))
         self.assertEqual(response.context['workers'], [worker1])
 
     def test_worker_details(self):
         """Worker index page should show workers for a specific queue"""
 
-        worker = create_worker('django_rq_test', name=uuid.uuid4().hex)
+        worker = create_worker('django_rq_scheduler_test', name=uuid.uuid4().hex)
         worker.register_birth()
 
-        response = self.client.get(reverse('worker_details', args=[worker.key]))
+        url = reverse('worker_details', args=[worker.name, ])
+        response = self.client.get(url)
         self.assertEqual(response.context['worker'], worker)
 
+    def test_worker_details__non_existing_worker(self):
+        """Worker index page should show workers for a specific queue"""
+
+        worker = create_worker('django_rq_scheduler_test', name='WORKER')
+        worker.register_birth()
+
+        response = self.client.get(reverse('worker_details', args=['bad-worker-name']))
+        self.assertEqual(404, response.status_code)
+
     def test_statistics_json_view(self):
         """
         Django-RQ's statistic as JSON only viewable by staff or with API_TOKEN
         """
 
         # Override testing RQ_QUEUES
         queues = {
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/tools.py` & `django_rq_scheduler-2023.5.0b3/scheduler/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import importlib
 import os
 
 import croniter
-import redis
 from django.apps import apps
 from django.utils import timezone
 
 from scheduler.decorators import job
 from scheduler.queues import get_queues, logger, get_queue
 from scheduler.rq_classes import DjangoWorker
 
@@ -59,39 +58,44 @@
     logger.debug(f'Running task {str(scheduled_job)}')
     args = scheduled_job.parse_args()
     kwargs = scheduled_job.parse_kwargs()
     res = scheduled_job.callable_func()(*args, **kwargs)
     return res
 
 
+def _calc_worker_name(existing_worker_names):
+    hostname = os.uname()[1]
+    c = 1
+    worker_name = f'{hostname}-worker.{c}'
+    while worker_name in existing_worker_names:
+        c += 1
+        worker_name = f'{hostname}-worker.{c}'
+    return worker_name
+
+
 def create_worker(*queue_names, **kwargs):
     """
     Returns a Django worker for all queues or specified ones.
     """
+
     queues = get_queues(*queue_names)
     existing_workers = DjangoWorker.all(connection=queues[0].connection)
     existing_worker_names = set(map(lambda w: w.name, existing_workers))
-    hostname = os.uname()[1]
-    c = 1
-    worker_name = f'{hostname}-worker:{c}'
-    while worker_name in existing_worker_names:
-        c += 1
-        worker_name = f'{hostname}-worker:{c}'
-    kwargs['name'] = worker_name
+    if kwargs.get('name', None) is None:
+        kwargs['name'] = _calc_worker_name(existing_worker_names)
+
+    kwargs['name'] = kwargs['name'].replace('/', '.')
     worker = DjangoWorker(queues, connection=queues[0].connection, **kwargs)
     return worker
 
 
 def get_job_executions(queue_name, scheduled_job):
     queue = get_queue(queue_name)
     res = list()
-    try:
-        job_list = queue.get_jobs()
-    except redis.ConnectionError:
-        return res
+    job_list = queue.get_all_jobs()
     res.extend(list(filter(lambda j: j.is_execution_of(scheduled_job), job_list)))
     scheduled_job_id_list = queue.scheduled_job_registry.get_job_ids()
 
     res.extend(list(
         map(lambda j: j.to_json(),
             filter(lambda j: j.is_execution_of(scheduled_job),
                    map(queue.fetch_job, scheduled_job_id_list)
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/urls.py` & `django_rq_scheduler-2023.5.0b3/scheduler/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,10 +19,10 @@
     path('queues/<str:queue_name>/actions/', views.actions, name='queue_actions'),
     path('queues/<str:queue_name>/<str:job_id>/requeue/', views.requeue_job_view, name='queue_requeue_job', ),
     path('queues/<str:queue_name>/<str:job_id>/enqueue/', views.enqueue_job, name='queue_enqueue_job'),
 ]
 
 urlpatterns += [
     path('workers/', views.workers, name='workers_home'),
-    path('workers/<str:key>/', views.worker_details, name='worker_details'),
+    path('workers/<str:name>/', views.worker_details, name='worker_details'),
     path('jobs/<str:job_id>/', views.job_detail, name='job_details'),
 ]
```

### Comparing `django_rq_scheduler-2023.5.0b2/scheduler/views.py` & `django_rq_scheduler-2023.5.0b3/scheduler/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from math import ceil
 
 import redis
 from django.contrib import admin, messages
 from django.contrib.admin.views.decorators import staff_member_required
+from django.core.paginator import Paginator
 from django.http import JsonResponse
 from django.http.response import HttpResponseNotFound, Http404
 from django.shortcuts import redirect
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.decorators.cache import never_cache
 from redis.exceptions import ResponseError
@@ -23,14 +24,23 @@
 from rq.worker_registration import clean_worker_registry
 
 from .queues import get_all_workers, get_connection, logger, get_queue
 from .rq_classes import JobExecution, ExecutionStatus, DjangoWorker
 from .settings import SCHEDULER
 
 
+def get_worker_executions(worker):
+    res = list()
+    for queue in worker.queues:
+        curr_jobs = queue.get_all_jobs()
+        curr_jobs = [j for j in curr_jobs if j.worker_name == worker.name]
+        res.extend(curr_jobs)
+    return res
+
+
 # Create your views here.
 @never_cache
 @staff_member_required
 def stats(request):
     context_data = {**admin.site.each_context(request), **get_statistics(run_maintenance_tasks=True)}
     return render(request, 'admin/scheduler/stats.html', context_data)
 
@@ -198,40 +208,39 @@
         'workers': worker_list,
     }
     return render(request, 'admin/scheduler/workers.html', context_data)
 
 
 @never_cache
 @staff_member_required
-def worker_details(request, key):
-    from scheduler.settings import QUEUES
+def worker_details(request, name):
     queue, worker = None, None
-    for queue_name in QUEUES:
-        try:
-            queue = get_queue(queue_name)
-            worker = DjangoWorker.find_by_key(key, connection=queue.connection)
-            if worker is not None:
-                break
-        except redis.ConnectionError:
-            pass
+    workers = get_all_workers()
+    worker = next((w for w in workers if w.name == name), None)
 
     if worker is None:
-        raise Http404(f"Couldn't find worker with this ID: {key}")
+        raise Http404(f"Couldn't find worker with this ID: {name}")
     # Convert microseconds to milliseconds
     worker.total_working_time = worker.total_working_time / 1000
 
-    queue_names = ', '.join(worker.queue_names())
-
+    execution_list = get_worker_executions(worker)
+    paginator = Paginator(execution_list, SCHEDULER['EXECUTIONS_IN_PAGE'])
+    page_number = request.GET.get('p', 1)
+    page_obj = paginator.get_page(page_number)
+    page_range = paginator.get_elided_page_range(page_obj.number)
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'worker': worker,
-        'queue_names': queue_names,
+        'queue_names': ', '.join(worker.queue_names()),
         'job': worker.get_current_job(),
         'total_working_time': worker.total_working_time * 1000,
+        'executions': page_obj,
+        'page_range': page_range,
+        'page_var': 'p',
     }
     return render(request, 'admin/scheduler/worker_details.html', context_data)
 
 
 @never_cache
 @staff_member_required
 def job_detail(request, job_id):
```

### Comparing `django_rq_scheduler-2023.5.0b2/PKG-INFO` & `django_rq_scheduler-2023.5.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.5.0b2
+Version: 2023.5.0b3
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
@@ -39,34 +39,28 @@
 Project-URL: Funding, https://github.com/sponsors/cunla
 Description-Content-Type: text/markdown
 
 Django RQ Scheduler
 ===================
 [![Django CI](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml/badge.svg)](https://github.com/dsoftwareinc/django-rq-scheduler/actions/workflows/test.yml)
 ![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cunla/b756396efb895f0e34558c980f1ca0c7/raw/django-rq-scheduler-4.json)
-
 [![badge](https://img.shields.io/pypi/dm/django-rq-scheduler)](https://pypi.org/project/django-rq-scheduler/)
 [![Open Source Helpers](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler/badges/users.svg)](https://www.codetriage.com/dsoftwareinc/django-rq-scheduler)
 
 Documentation can be found in https://django-rq-scheduler.readthedocs.io/en/latest/
 
-> Notice:
-> 
-> In v2023.3.0, django-rq-scheduler was refactored significantly to support
+>  **Warning**: In v2023.3.0, django-rq-scheduler was refactored significantly to support
 > calculation of parameters in runtime.
-> 
 > You can now add a callable param to your scheduled job, and it will be
 > calculated when the job is performed.
 > 
 > 1. It is highly recommended you save your existing database before upgrading!
 > 2. Once you upgraded, recreate your jobs.
 
-> Notice:
-> 
-> Starting v2023.1, requirement for rq_scheduler was removed and instead
+> **Note** Starting v2023.1, requirement for rq_scheduler was removed and instead
 > one of the django-rq workers should run with `--with-scheduler` parameter
 > as mentioned [here](https://github.com/rq/django-rq#support-for-scheduled-jobs).
 
 
 # Sponsor
 
 django-rq-scheduler is developed for free.
```

