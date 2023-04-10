# Comparing `tmp/django_rq_scheduler-2023.5.0b1.tar.gz` & `tmp/django_rq_scheduler-2023.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.5.0b1.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.5.0b2.tar", max compression
```

## Comparing `django_rq_scheduler-2023.5.0b1.tar` & `django_rq_scheduler-2023.5.0b2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1096 2023-04-06 22:49:33.158637 django_rq_scheduler-2023.5.0b1/LICENSE
--rw-r--r--   0        0        0     1711 2023-04-06 22:49:33.158637 django_rq_scheduler-2023.5.0b1/README.md
--rw-r--r--   0        0        0     1741 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/pyproject.toml
--rw-r--r--   0        0        0      134 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     4914 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/admin/job.py
--rw-r--r--   0        0        0     1646 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      481 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/apps.py
--rw-r--r--   0        0        0     1308 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1908 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3463 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     2902 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1357 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0     1051 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1279 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      662 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     6512 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/models/queue.py
--rw-r--r--   0        0        0    15115 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/py.typed
--rw-r--r--   0        0        0     5437 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/queues.py
--rw-r--r--   0        0        0     2643 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/rq_classes.py
--rw-r--r--   0        0        0      551 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/settings.py
--rw-r--r--   0        0        0     1555 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1559 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     1282 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/delete_job.html
--rw-r--r--   0        0        0     7124 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     6268 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0     1055 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     3847 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3062 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1835 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0      541 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      535 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5483 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2777 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    26904 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2184 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    13384 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_views.py
--rw-r--r--   0        0        0      517 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3323 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     3273 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/tools.py
--rw-r--r--   0        0        0     1735 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/urls.py
--rw-r--r--   0        0        0    15140 2023-04-06 22:49:33.166637 django_rq_scheduler-2023.5.0b1/scheduler/views.py
--rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-10 22:08:15.141312 django_rq_scheduler-2023.5.0b2/LICENSE
+-rw-r--r--   0        0        0     1711 2023-04-10 22:08:15.141312 django_rq_scheduler-2023.5.0b2/README.md
+-rw-r--r--   0        0        0     1741 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5461 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1646 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      481 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/apps.py
+-rw-r--r--   0        0        0     1147 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1189 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1908 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3417 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3602 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     2902 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     7162 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0     1051 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1279 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      662 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     6512 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/queue.py
+-rw-r--r--   0        0        0    15395 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/py.typed
+-rw-r--r--   0        0        0     5452 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/queues.py
+-rw-r--r--   0        0        0     2963 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/rq_classes.py
+-rw-r--r--   0        0        0      822 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/settings.py
+-rw-r--r--   0        0        0     2628 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1559 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     1282 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/delete_job.html
+-rw-r--r--   0        0        0     7124 2023-04-10 22:08:15.149313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     6331 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0     1055 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     4120 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3062 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1835 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0      541 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5483 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2777 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    26904 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2184 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    14315 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0      517 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3323 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     3273 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/tools.py
+-rw-r--r--   0        0        0     1735 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/urls.py
+-rw-r--r--   0        0        0    15878 2023-04-10 22:08:15.153313 django_rq_scheduler-2023.5.0b2/scheduler/views.py
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b2/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.5.0b1/LICENSE` & `django_rq_scheduler-2023.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/README.md` & `django_rq_scheduler-2023.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/pyproject.toml` & `django_rq_scheduler-2023.5.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.5.0b1"
+version = "2023.5.0b2"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
 ]
 maintainers = [
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/admin/job.py` & `django_rq_scheduler-2023.5.0b2/scheduler/admin/job.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib import admin, messages
 from django.contrib.contenttypes.admin import GenericStackedInline
 from django.utils.translation import gettext_lazy as _
 
 from scheduler import tools
 from scheduler.models import CronJob, JobArg, JobKwarg, RepeatableJob, ScheduledJob
+from scheduler.settings import SCHEDULER
 from scheduler.tools import get_job_executions
 
 
 class HiddenMixin(object):
     class Media:
         js = ['admin/js/jquery.init.js', ]
 
@@ -30,14 +31,15 @@
             'fields': (('key',), ('arg_type', 'val',),),
         }),
     )
 
 
 class JobAdmin(admin.ModelAdmin):
     """BaseJob admin class"""
+    save_on_top = True
     change_form_template = 'admin/scheduler/change_form.html'
     actions = ['disable_selected', 'enable_selected', 'enqueue_job_now', ]
     inlines = [JobArgInline, JobKwargInline, ]
     list_filter = ('enabled',)
     list_display = ('enabled', 'name', 'job_id', 'function_string', 'is_scheduled', 'queue',)
     list_display_links = ('name',)
     readonly_fields = ('job_id',)
@@ -49,15 +51,26 @@
             'fields': ('queue', 'job_id',),
         }),
     )
 
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra = extra_context or {}
         obj = self.get_object(request, object_id)
-        extra['executions'] = get_job_executions(obj.queue, obj)
+        execution_list = get_job_executions(obj.queue, obj)
+        paginator = self.get_paginator(request, execution_list, SCHEDULER['EXECUTIONS_IN_PAGE'])
+        page_number = request.GET.get('p', 1)
+        page_obj = paginator.get_page(page_number)
+        page_range = paginator.get_elided_page_range(page_obj.number)
+
+        extra.update({
+            "pagination_required": paginator.count > SCHEDULER['EXECUTIONS_IN_PAGE'],
+            'executions': page_obj,
+            'page_range': page_range,
+            'page_var': 'p',
+        })
 
         return super(JobAdmin, self).change_view(
             request, object_id, form_url, extra_context=extra)
 
     def delete_queryset(self, request, queryset):
         for job in queryset:
             job.unschedule()
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.5.0b2/scheduler/admin/redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/decorators.py` & `django_rq_scheduler-2023.5.0b2/scheduler/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     """
     The same as rq package's job decorator, but it automatically works out
     the ``connection`` argument from RQ_QUEUES.
 
     And also, it allows simplified ``@job`` syntax to put job into
     default queue.
 
-    If RQ.DEFAULT_RESULT_TTL setting is set, it is used as default
-    for ``result_ttl`` kwarg.
     """
     if callable(func_or_queue):
         func = func_or_queue
         queue = 'default'
     else:
         func = None
         queue = func_or_queue
@@ -26,20 +24,18 @@
         try:
             queue = get_queue(queue)
             if connection is None:
                 connection = queue.connection
         except KeyError:
             pass
 
-    RQ = getattr(settings, 'RQ', {})
-    default_result_ttl = RQ.get('DEFAULT_RESULT_TTL')
-    if default_result_ttl is not None:
-        kwargs.setdefault('result_ttl', default_result_ttl)
-
-    default_timeout = RQ.get('DEFAULT_TIMEOUT')
-    if default_timeout is not None:
-        kwargs.setdefault('timeout', default_timeout)
+    config = getattr(settings, 'SCHEDULER', {})
+    default_result_ttl = config.get('DEFAULT_RESULT_TTL')
+    kwargs.setdefault('result_ttl', default_result_ttl)
+
+    default_timeout = config.get('DEFAULT_TIMEOUT')
+    kwargs.setdefault('timeout', default_timeout)
 
     decorator = _rq_job(queue, connection=connection, *args, **kwargs)
     if func:
         return decorator(func)
     return decorator
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqstats.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from scheduler.views import get_statistics
 
 ANSI_LIGHT_GREEN = "\033[1;32m"
 ANSI_LIGHT_WHITE = "\033[1;37m"
 ANSI_RESET = "\033[0m"
 
+KEYS = ('jobs', 'started_jobs', 'deferred_jobs', 'finished_jobs', 'canceled_jobs', 'workers')
+
 
 class Command(BaseCommand):
     """
     Print statistics
     """
     help = __doc__
 
@@ -42,25 +44,28 @@
     def _print_stats_dashboard(self, statistics, prev_stats=None):
         if self.interval:
             click.clear()
         click.echo()
         click.echo("Django-Scheduler CLI Dashboard")
         click.echo()
         self._print_separator()
-        click.echo(f'| {"Name":<16} |    Queued |    Active |  Deferred |  Finished |   Workers |')
+        click.echo(f'| {"Name":<16} |    Queued |    Active |  Deferred |'
+                   f'  Finished |'
+                   f'  Canceled |'
+                   f'   Workers |')
         self._print_separator()
 
         for ind, queue in enumerate(statistics["queues"]):
+            vals = (queue[k] for k in KEYS)
             vals = (queue["jobs"], queue["started_jobs"], queue["deferred_jobs"],
-                    queue["finished_jobs"], queue["workers"])
+                    queue["finished_jobs"], queue['canceled_jobs'], queue["workers"])
             # Deal with colors
             if prev_stats and len(prev_stats['queues']) > ind:
                 prev = prev_stats["queues"][ind]
-                prev_vals = (prev["jobs"], prev["started_jobs"], prev["deferred_jobs"],
-                             prev["finished_jobs"], prev["workers"])
+                prev_vals = (prev[k] for k in KEYS)
                 colors = [ANSI_LIGHT_GREEN
                           if vals[i] != prev_vals[i] else ANSI_LIGHT_WHITE
                           for i in range(len(prev_vals))
                           ]
             else:
                 colors = [ANSI_LIGHT_WHITE for _ in range(len(vals))]
             to_print = ' | '.join([f'{colors[i]}{vals[i]:9}{ANSI_RESET}' for i in range(len(vals))])
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.5.0b2/scheduler/management/commands/run_job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import click
 from django.core.management.base import BaseCommand
 
 from scheduler.queues import get_queue
 
 
 class Command(BaseCommand):
     """
@@ -17,20 +18,20 @@
             help='Specify the queue [default]')
         parser.add_argument(
             '--timeout', '-t', type=int, dest='timeout',
             help='A timeout in seconds')
         parser.add_argument(
             '--result-ttl', '-r', type=int, dest='result_ttl',
             help='Time to store job results in seconds')
-        parser.add_argument('callable', help='Method to call',)
+        parser.add_argument('callable', help='Method to call', )
         parser.add_argument('args', nargs='*', help='Args for callable')
 
     def handle(self, **options):
         verbosity = int(options.get('verbosity', 1))
         timeout = options.get('timeout')
         result_ttl = options.get('result_ttl')
         queue = get_queue(options.get('queue'))
         func = options.get('callable')
         args = options.get('args')
         job = queue.enqueue_call(func, args=args, timeout=timeout, result_ttl=result_ttl)
         if verbosity:
-            print('Job %s created' % job.id)
+            click.echo(f'Job {job.id} created')
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/models/args.py` & `django_rq_scheduler-2023.5.0b2/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.5.0b2/scheduler/models/scheduled_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         scheduled_job.unschedule()
         scheduled_job.schedule()
 
 
 class BaseJob(TimeStampedModel):
     QUEUES = [(key, key) for key in settings.RQ_QUEUES.keys()]
     JOB_TYPE = 'BaseJob'
-    name = models.CharField(_('name'), max_length=128, unique=True)
+    name = models.CharField(
+        _('name'), max_length=128, unique=True,
+        help_text='Name of the job.', )
     callable = models.CharField(_('callable'), max_length=2048)
     callable_args = GenericRelation(JobArg, related_query_name='args')
     callable_kwargs = GenericRelation(JobKwarg, related_query_name='kwargs')
     enabled = models.BooleanField(
         _('enabled'), default=True,
         help_text=_('Should job be scheduled? This field is useful to keep '
                     'past jobs that should no longer be scheduled'),
@@ -106,15 +108,16 @@
     def parse_kwargs(self):
         """Parse kwargs for running job"""
         kwargs = self.callable_kwargs.all()
         return dict([kwarg.value() for kwarg in kwargs])
 
     def _next_job_id(self):
         addition = uuid.uuid4().hex[-10:]
-        return f'{self.queue}:{self.name}:{addition}'
+        name = self.name.replace('/', '.')
+        return f'{self.queue}:{name}:{addition}'
 
     def _enqueue_args(self) -> Dict:
         """args for DjangoQueue.enqueue.
         Set all arguments for DjangoQueue.enqueue/enqueue_at.
         Particularly:
         - set job timeout and ttl
         - ensure a callback to reschedule job next iteration.
@@ -238,18 +241,20 @@
             self.schedule()
             super(BaseJob, self).save()
 
     def delete(self, **kwargs):
         self.unschedule()
         super(BaseJob, self).delete(**kwargs)
 
-    # Job form validation methods
-    def clean(self):
-        self.clean_callable()
-        self.clean_queue()
+    def clean_name(self):
+        if '/' in self.name:
+            raise ValidationError({
+                'name': ValidationError(
+                    _('Invalid job name, must not contain /'), code='invalid')
+            })
 
     def clean_callable(self):
         try:
             tools.callable_func(self.callable)
         except Exception:
             raise ValidationError({
                 'callable': ValidationError(
@@ -261,14 +266,18 @@
         if self.queue not in queue_keys:
             raise ValidationError({
                 'queue': ValidationError(
                     _('Invalid queue, must be one of: {}'.format(
                         ', '.join(queue_keys))), code='invalid')
             })
 
+    def clean(self):
+        self.clean_queue()
+        self.clean_callable()
+
     class Meta:
         abstract = True
 
 
 class ScheduledTimeMixin(models.Model):
     scheduled_time = models.DateTimeField(_('scheduled time'))
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/queues.py` & `django_rq_scheduler-2023.5.0b2/scheduler/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 def get_queue(
         name='default',
         default_timeout=None, is_async=None,
         autocommit=None,
         connection=None,
         **kwargs
-):
+) -> DjangoQueue:
     """Returns an DjangoQueue using parameters defined in ``RQ_QUEUES``
     """
     from .settings import QUEUES
 
     if is_async is None:
         is_async = QUEUES[name].get('ASYNC', True)
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/rq_classes.py` & `django_rq_scheduler-2023.5.0b2/scheduler/rq_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+from redis import Redis
 from rq import Worker
+from rq.command import send_stop_job_command
 from rq.job import Job, JobStatus
 from rq.queue import Queue
 from rq.registry import (
-    DeferredJobRegistry,
-    FailedJobRegistry,
-    FinishedJobRegistry,
-    ScheduledJobRegistry,
-    StartedJobRegistry,
+    DeferredJobRegistry, FailedJobRegistry, FinishedJobRegistry,
+    ScheduledJobRegistry, StartedJobRegistry, CanceledJobRegistry,
 )
 
 ExecutionStatus = JobStatus
 
 
 class JobExecution(Job):
     def __eq__(self, other):
@@ -20,14 +19,17 @@
     def is_scheduled_job(self):
         return self.meta.get('scheduled_job_id', None) is not None
 
     def is_execution_of(self, scheduled_job):
         return (self.meta.get('job_type', None) == scheduled_job.JOB_TYPE
                 and self.meta.get('scheduled_job_id', None) == scheduled_job.id)
 
+    def stop_execution(self, connection: Redis):
+        send_stop_job_command(connection, self.id)
+
     def to_json(self):
         return dict(
             id=self.id,
             status=self.get_status(),
             started_at=self.started_at,
             ended_at=self.ended_at,
             worker_name=self.worker_name,
@@ -81,7 +83,11 @@
     @property
     def failed_job_registry(self):
         return FailedJobRegistry(self.name, self.connection, job_class=JobExecution, )
 
     @property
     def scheduled_job_registry(self):
         return ScheduledJobRegistry(self.name, self.connection, job_class=JobExecution, )
+
+    @property
+    def canceled_job_registry(self):
+        return CanceledJobRegistry(self.name, self.connection, job_class=JobExecution, )
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/delete_job.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/delete_job.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/jobs.html`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             <form id="changelist-form" action="{% url 'queue_confirm_action' queue.name %}" method="post">
                 {% csrf_token %}
                 <div class="actions">
                     <label>Actions:
                         <select name="action">
                             <option value="" selected="selected">---------</option>
                             <option value="delete">Delete</option>
+                            <option value="stop">Stop</option>
                             {% if job_status == 'Failed' %}
                                 <option value="requeue">Requeue</option>
                             {% endif %}
                         </select>
                     </label>
                     <button type="submit" class="button" title="Execute selected action" name="index" value="0">Go
                     </button>
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/stats.html`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                     <th>Queued Jobs</th>
                     <th>Oldest Queued Job</th>
                     <th>Active Jobs</th>
                     <th>Deferred Jobs</th>
                     <th>Finished Jobs</th>
                     <th>Failed Jobs</th>
                     <th>Scheduled Jobs</th>
+                    <th>Canceled Jobs</th>
                     <th>Workers</th>
                     <th>Host</th>
                     <th>Port</th>
                     <th>DB</th>
                     {% if queue.scheduler_pid is not False %}
                         <th>Scheduler PID</th>
                     {% endif %}
@@ -74,14 +75,19 @@
                         </th>
                         <th>
                             <a href="{% url 'queue_failed_jobs' queue.name %}">
                                 {{ queue.failed_jobs }}
                             </a>
                         </th>
                         <th>
+                            <a href="{% url 'queue_failed_jobs' queue.name %}">
+                                {{ queue.canceled_jobs }}
+                            </a>
+                        </th>
+                        <th>
                             <a href="{% url 'queue_scheduled_jobs' queue.name %}">
                                 {{ queue.scheduled_jobs }}
                             </a>
                         </th>
                         <th><a href="{% url 'queue_workers' queue.name %}">
                             {{ queue.workers }}
                         </a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "admin/base_site.html" %} {% block title %}Queues {{ block.super }}
 {% endblock %} {% block extrastyle %} {{ block.super }}
  {% endblock %} {% block content_title %}
 ****** RQ Queues ******
 {% endblock %} {% block breadcrumbs %}
 Home › Queues
 {% endblock %} {% block content %}
-Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs       Workers       Host                         Port                         DB                         Scheduler PID
+Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs      Canceled Jobs        Workers       Host                         Port                         DB                         Scheduler PID
            Jobs
-{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
-{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
-queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.scheduled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db queue.scheduler_pid|default_if_none:
-}}         }}         }}                         }}                 }}                  }}                  }}                }}                   }}            }}                           }}                           }}                         "Inactive" }}
+{          {          {                          {                  {                   {                   {                 {                   {                    {             {                            {                            {                          {
+{          {          {                          {                  {                   {                   {                 {                   {                    {             {                            {                            {                          {
+queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.canceled_jobs queue.scheduled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db queue.scheduler_pid|default_if_none:
+}}         }}         }}                         }}                 }}                  }}                  }}                }}                  }}                   }}            }}                           }}                           }}                         "Inactive" }}
 
 View_as_JSON
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.5.0b2/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/templatetags/scheduler_tags.py` & `django_rq_scheduler-2023.5.0b2/scheduler/templatetags/scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/jobs.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/jobs.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_mgmt_cmds.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_mgmt_cmds.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,20 @@
 from datetime import datetime
 from unittest.mock import patch, PropertyMock
 
 from django.contrib.auth.models import User
 from django.test import TestCase
 from django.test.client import Client
 from django.urls import reverse
-from rq.job import Job, JobStatus
-from rq.registry import (
-    DeferredJobRegistry,
-    FailedJobRegistry,
-    FinishedJobRegistry,
-    ScheduledJobRegistry,
-    StartedJobRegistry,
-)
 
 from scheduler.queues import get_queue
 from scheduler.tools import create_worker
 from . import test_settings  # noqa
 from .jobs import access_self, failing_job
+from ..rq_classes import JobExecution, ExecutionStatus
 
 
 class ViewTest(TestCase):
     def setUp(self):
         self.user = User.objects.create_user('foo', password='pass')
         self.user.is_staff = True
         self.user.is_active = True
@@ -128,15 +121,15 @@
         In addition to deleting job from Redis, the job id also needs to be
         deleted from Queue.
         """
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
         job = queue.enqueue(access_self)
         self.client.post(reverse('queue_delete_job', args=[queue_name, job.id]), {'post': 'yes'})
-        self.assertFalse(Job.exists(job.id, connection=queue.connection))
+        self.assertFalse(JobExecution.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_action_delete_jobs(self):
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         # enqueue some jobs
@@ -146,38 +139,38 @@
             job_ids.append(job.id)
 
         # remove those jobs using view
         self.client.post(reverse('queue_actions', args=[queue_name]), {'action': 'delete', 'job_ids': job_ids})
 
         # check if jobs are removed
         for job_id in job_ids:
-            self.assertFalse(Job.exists(job_id, connection=queue.connection))
+            self.assertFalse(JobExecution.exists(job_id, connection=queue.connection))
             self.assertNotIn(job_id, queue.job_ids)
 
     def test_enqueue_jobs(self):
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         # enqueue some jobs that depends on other
         previous_job = None
         for _ in range(0, 3):
             job = queue.enqueue(access_self, depends_on=previous_job)
             previous_job = job
 
         # This job is deferred
         last_job = job
-        self.assertEqual(last_job.get_status(), JobStatus.DEFERRED)
+        self.assertEqual(last_job.get_status(), ExecutionStatus.DEFERRED)
         self.assertIsNone(last_job.enqueued_at)
 
         # We want to force-enqueue this job
         self.client.post(reverse('queue_enqueue_job', args=[queue_name, last_job.id]))
 
         # Check that job is updated correctly
         last_job = queue.fetch_job(last_job.id)
-        self.assertEqual(last_job.get_status(), JobStatus.QUEUED)
+        self.assertEqual(last_job.get_status(), ExecutionStatus.QUEUED)
         self.assertIsNotNone(last_job.enqueued_at)
 
     def test_action_requeue_jobs(self):
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         # enqueue some jobs that will fail
@@ -199,45 +192,74 @@
         # re-nqueue failed jobs from failed queue
         self.client.post(reverse('queue_actions', args=[queue_name]), {'action': 'requeue', 'job_ids': job_ids})
 
         # check if we requeue all failed jobs
         for job in jobs:
             self.assertFalse(job.is_failed)
 
+    def test_action_stop_jobs(self):
+        queue_name = 'django_rq_test'
+        queue = get_queue(queue_name)
+
+        # Enqueue some jobs
+        job_ids = []
+        worker = create_worker('django_rq_test')
+        for _ in range(3):
+            job = queue.enqueue(access_self)
+            job_ids.append(job.id)
+            worker.prepare_job_execution(job)
+
+        # Check if the jobs are started
+        for job_id in job_ids:
+            job = JobExecution.fetch(job_id, connection=queue.connection)
+            self.assertEqual(job.get_status(), ExecutionStatus.STARTED)
+
+        # Stop those jobs using the view
+        started_job_registry = queue.started_job_registry
+        self.assertEqual(len(started_job_registry), len(job_ids))
+        self.client.post(reverse('queue_actions', args=[queue_name]), {'action': 'stop', 'job_ids': job_ids})
+        self.assertEqual(len(started_job_registry), 0)
+
+        canceled_job_registry = queue.canceled_job_registry
+        self.assertEqual(len(canceled_job_registry), len(job_ids))
+
+        for job_id in job_ids:
+            self.assertIn(job_id, canceled_job_registry)
+
     def test_clear_queue(self):
         """Test that the queue clear actually clears the queue."""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
         job = queue.enqueue(access_self)
         self.client.post(reverse('queue_clear', args=[queue_name]), {'post': 'yes'})
-        self.assertFalse(Job.exists(job.id, connection=queue.connection))
+        self.assertFalse(JobExecution.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_finished_jobs(self):
         """Ensure that finished jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         job = queue.enqueue(access_self)
-        registry = FinishedJobRegistry(queue.name, queue.connection)
+        registry = queue.finished_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_finished_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_failed_jobs(self):
         """Ensure that failed jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         # Test that page doesn't fail when FailedJobRegistry is empty
         response = self.client.get(reverse('queue_failed_jobs', args=[queue_name]))
         self.assertEqual(response.status_code, 200)
 
         job = queue.enqueue(access_self)
-        registry = FailedJobRegistry(queue.name, queue.connection)
+        registry = queue.failed_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_failed_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_scheduled_jobs(self):
         """Ensure that scheduled jobs page works properly."""
         queue = get_queue('django_rq_test')
@@ -252,15 +274,15 @@
         self.assertEqual(response.context['jobs'], [job])
 
     def test_scheduled_jobs_registry_removal(self):
         """Ensure that non-existing job is being deleted from registry by view"""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
-        registry = ScheduledJobRegistry(queue.name, queue.connection)
+        registry = queue.scheduled_job_registry
         job = queue.enqueue_at(datetime.now(), access_self)
         self.assertEqual(len(registry), 1)
 
         queue.connection.delete(job.key)
         response = self.client.get(reverse('queue_scheduled_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [])
 
@@ -268,26 +290,26 @@
 
     def test_started_jobs(self):
         """Ensure that active jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         job = queue.enqueue(access_self)
-        registry = StartedJobRegistry(queue.name, queue.connection)
+        registry = queue.started_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_started_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_deferred_jobs(self):
         """Ensure that active jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_name = 'django_rq_test'
 
         job = queue.enqueue(access_self)
-        registry = DeferredJobRegistry(queue.name, queue.connection)
+        registry = queue.deferred_job_registry
         registry.add(job, 2)
         response = self.client.get(reverse('queue_deferred_jobs', args=[queue_name]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_workers_home(self):
         response = self.client.get(reverse('workers_home'))
         prev_workers = response.context['workers']
```

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/tools.py` & `django_rq_scheduler-2023.5.0b2/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/urls.py` & `django_rq_scheduler-2023.5.0b2/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b1/scheduler/views.py` & `django_rq_scheduler-2023.5.0b2/scheduler/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     StartedJobRegistry,
     clean_registries,
 )
 from rq.worker_registration import clean_worker_registry
 
 from .queues import get_all_workers, get_connection, logger, get_queue
 from .rq_classes import JobExecution, ExecutionStatus, DjangoWorker
+from .settings import SCHEDULER
 
 
 # Create your views here.
 @never_cache
 @staff_member_required
 def stats(request):
     context_data = {**admin.site.each_context(request), **get_statistics(run_maintenance_tasks=True)}
@@ -79,25 +80,26 @@
                 scheduler_pid=queue.scheduler_pid,
                 workers=DjangoWorker.count(queue=queue),
                 finished_jobs=len(queue.finished_job_registry),
                 started_jobs=len(queue.started_job_registry),
                 deferred_jobs=len(queue.deferred_job_registry),
                 failed_jobs=len(queue.failed_job_registry),
                 scheduled_jobs=len(queue.scheduled_job_registry),
+                canceled_jobs=len(queue.canceled_job_registry),
             )
             queues.append(queue_data)
         except redis.ConnectionError as e:
             logger.error(f'Could not connect for queue {queue_name}: {e}')
             continue
 
     return {'queues': queues}
 
 
 def _get_registry_job_list(queue, registry, page):
-    items_per_page = 100
+    items_per_page = SCHEDULER['EXECUTIONS_IN_PAGE']
     num_jobs = len(registry)
     job_list = []
 
     if num_jobs == 0:
         return job_list, num_jobs, []
 
     last_page = int(ceil(num_jobs / items_per_page))
@@ -411,14 +413,26 @@
                     queue.connection.lrem(queue.key, 0, job.id)
                     job.delete()
                 messages.info(request, f'You have successfully deleted {len(job_ids)} jobs!')
             elif request.POST['action'] == 'requeue':
                 for job_id in job_ids:
                     requeue_job(job_id, connection=queue.connection)
                 messages.info(request, f'You have successfully re-queued {len(job_ids)}  jobs!')
+            elif request.POST['action'] == 'stop':
+                cancelled_jobs = 0
+                for job_id in job_ids:
+                    try:
+                        job = JobExecution.fetch(job_id, connection=queue.connection)
+                        job.stop_execution(queue.connection)
+                        job.cancel()
+                        cancelled_jobs += 1
+                    except Exception as e:
+                        logger.warning(f'Could not stop job: {e}')
+                        pass
+                messages.info(request, f'You have successfully stopped {cancelled_jobs}  jobs!')
 
     return redirect(next_url)
 
 
 @never_cache
 @staff_member_required
 def enqueue_job(request, queue_name, job_id):
```

### Comparing `django_rq_scheduler-2023.5.0b1/PKG-INFO` & `django_rq_scheduler-2023.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.5.0b1
+Version: 2023.5.0b2
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
```

