# Comparing `tmp/django-sorcery-0.9.3.tar.gz` & `tmp/django-sorcery-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-sorcery-0.9.3.tar", last modified: Thu Jun 27 02:30:14 2019, max compression
+gzip compressed data, was "dist/django-sorcery-0.9.4.tar", last modified: Sun Jul 14 23:15:47 2019, max compression
```

## Comparing `django-sorcery-0.9.3.tar` & `django-sorcery-0.9.4.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      115 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/AUTHORS.rst
--rw-r--r--   0 serkan    (1000) serkan    (1000)    13647 2019-06-27 02:29:06.000000 django-sorcery-0.9.3/HISTORY.rst
--rw-r--r--   0 serkan    (1000) serkan    (1000)      152 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/MANIFEST.in
--rw-r--r--   0 serkan    (1000) serkan    (1000)    26015 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/PKG-INFO
--rw-r--r--   0 serkan    (1000) serkan    (1000)    19456 2019-04-23 12:29:18.000000 django-sorcery-0.9.3/README.rst
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      190 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      241 2019-06-27 02:29:06.000000 django-sorcery-0.9.3/django_sorcery/__version__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      348 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/compat.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/db/
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5345 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/__init__.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/db/alembic/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      157 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/alembic/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1059 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/alembic/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      495 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/alembic/script.py.mako
--rw-r--r--   0 serkan    (1000) serkan    (1000)      998 2019-04-16 14:52:17.000000 django-sorcery-0.9.3/django_sorcery/db/alembic/signals.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3379 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/composites.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    11997 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/fields.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/db/meta/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      315 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/meta/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      708 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/meta/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    16753 2019-06-02 01:18:46.000000 django-sorcery-0.9.3/django_sorcery/db/meta/column.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4249 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/meta/composite.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    13314 2019-06-24 10:31:18.000000 django-sorcery-0.9.3/django_sorcery/db/meta/model.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4480 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/meta/relations.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3596 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/django_sorcery/db/middleware.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3114 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/mixins.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    12813 2019-04-16 14:47:54.000000 django-sorcery-0.9.3/django_sorcery/db/models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     8922 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/profiler.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     7905 2019-04-13 23:23:37.000000 django-sorcery-0.9.3/django_sorcery/db/query.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    10163 2019-04-16 15:14:05.000000 django-sorcery-0.9.3/django_sorcery/db/relations.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2858 2019-04-28 11:58:22.000000 django-sorcery-0.9.3/django_sorcery/db/session.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3513 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/signals.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     9539 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/django_sorcery/db/sqlalchemy.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1393 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/transaction.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5970 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/db/url.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3612 2019-06-01 19:47:16.000000 django-sorcery-0.9.3/django_sorcery/db/utils.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2935 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/exceptions.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6823 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/fields.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    13494 2019-06-24 10:31:18.000000 django-sorcery-0.9.3/django_sorcery/forms.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/formsets/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      156 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/formsets/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6481 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/formsets/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3584 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/formsets/inline.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/management/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      142 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6130 2019-04-23 12:29:18.000000 django-sorcery-0.9.3/django_sorcery/management/alembic.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2319 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/base.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/management/commands/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      893 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      999 2019-04-23 12:29:18.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_createall.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1565 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_current.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2341 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_downgrade.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      976 2019-04-23 12:29:18.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_dropall.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1750 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_heads.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1974 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_history.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4254 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_revision.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1720 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_stamp.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2348 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_upgrade.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      551 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/pytest_plugin.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    11557 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/routers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1551 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/shortcuts.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2130 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/testing.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2070 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/utils.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/validators/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      189 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/validators/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     7916 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/validators/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1259 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/validators/runner.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/views/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      212 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/views/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     8182 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/views/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2736 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/views/detail.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5535 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/views/edit.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3545 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/views/list.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery/viewsets/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      338 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/viewsets/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6135 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/viewsets/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    10740 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/django_sorcery/viewsets/mixins.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/
--rw-r--r--   0 serkan    (1000) serkan    (1000)    26015 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/PKG-INFO
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5001 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/SOURCES.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)        1 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/dependency_links.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)       58 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/entry_points.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)       72 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/requires.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)       15 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/django_sorcery.egg-info/top_level.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)      240 2019-06-24 10:31:18.000000 django-sorcery-0.9.3/requirements.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)      489 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/setup.cfg
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2921 2019-04-23 12:44:42.000000 django-sorcery-0.9.3/setup.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      250 2019-06-24 10:31:18.000000 django-sorcery-0.9.3/tests/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      867 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/base.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/db/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/__init__.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/db/alembic/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/alembic/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1356 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/alembic/test_base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1709 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/alembic/test_signals.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/db/meta/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/meta/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      539 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/meta/test_base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    15772 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/db/meta/test_column.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3882 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/meta/test_composite.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     7088 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/meta/test_model.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4275 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/meta/test_relations.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2537 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_composites.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    10399 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_fields.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5461 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/db/test_middleware.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5171 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_mixins.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    21999 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/db/test_models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2735 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_profiler.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4623 2019-04-13 23:23:37.000000 django-sorcery-0.9.3/tests/db/test_query.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3177 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_relations.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3448 2019-04-28 11:58:22.000000 django-sorcery-0.9.3/tests/db/test_session.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      253 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_signals.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2778 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_sqlalchemy.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1711 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_transaction.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5604 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/db/test_url.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4639 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/db/test_utils.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/formsets/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/formsets/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    16778 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/formsets/test_base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     9591 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/formsets/test_inline.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/management/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/__init__.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/management/commands/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      583 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1583 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3447 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_current.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3570 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_downgrade.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2575 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_heads.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2826 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_history.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2626 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_revision.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1781 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_stamp.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3575 2019-04-28 11:58:22.000000 django-sorcery-0.9.3/tests/management/commands/test_sorcery_upgrade.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1847 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/management/test_base.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/minimalapp/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/minimalapp/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      230 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/minimalapp/apps.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1599 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/minimalapp/models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1939 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/models_backpop.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      640 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/models_multidb.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      677 2019-04-13 23:26:39.000000 django-sorcery-0.9.3/tests/models_terrible_relations.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/otherapp/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/otherapp/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      224 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/otherapp/apps.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/otherapp/migrations/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/otherapp/migrations/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      361 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/otherapp/models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2652 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/settings.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/templates/
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       11 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/owner_confirm_delete.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)       18 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/owner_detail.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)       14 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/owner_form.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)       57 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/owner_list.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)       14 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/tests.testapp/vehicle_form.html
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/templates/views/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       11 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/views/edit.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)       52 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/templates/views/list.html
--rw-r--r--   0 serkan    (1000) serkan    (1000)      298 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_compat.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2940 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_exceptions.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6928 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_fields.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    25619 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_forms.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1490 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_pytest_plugin.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     5918 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_routers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1588 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_shortcuts.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      986 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_utils.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     6415 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/test_validators.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/testapp/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/testapp/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      257 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/testapp/apps.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/testapp/migrations/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/testapp/migrations/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     8178 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/testapp/models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2462 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/testapp/views.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2321 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/urls.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/views/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/views/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3075 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/views/test_base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3109 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/views/test_detail.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4276 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/views/test_edit.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4342 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/views/test_list.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:30:14.000000 django-sorcery-0.9.3/tests/viewsets/
--rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/viewsets/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1059 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/viewsets/test_base.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    11119 2019-04-12 23:53:43.000000 django-sorcery-0.9.3/tests/viewsets/test_mixins.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      115 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/AUTHORS.rst
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    13783 2019-07-14 23:15:07.000000 django-sorcery-0.9.4/HISTORY.rst
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      152 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/MANIFEST.in
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    26015 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/PKG-INFO
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    19456 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/README.rst
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      190 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      241 2019-07-14 23:15:07.000000 django-sorcery-0.9.4/django_sorcery/__version__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      348 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/compat.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/db/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5345 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/__init__.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/db/alembic/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      157 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/alembic/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1059 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/alembic/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      495 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/alembic/script.py.mako
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      998 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/alembic/signals.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3379 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/composites.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    11997 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/fields.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/db/meta/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      315 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      708 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    16753 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/column.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4249 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/composite.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    13314 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/model.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4480 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/meta/relations.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3635 2019-07-14 23:14:46.000000 django-sorcery-0.9.4/django_sorcery/db/middleware.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3114 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/mixins.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    12813 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     8922 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/profiler.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     7905 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/query.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    10163 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/relations.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2858 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/session.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3513 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/signals.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     9539 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/sqlalchemy.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1393 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/transaction.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5970 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/url.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3612 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/db/utils.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2935 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/exceptions.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6823 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/fields.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    13494 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/forms.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/formsets/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      156 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/formsets/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6481 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/formsets/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3584 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/formsets/inline.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/management/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      142 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6130 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/alembic.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2319 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/base.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/management/commands/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      893 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      999 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_createall.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1565 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_current.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2341 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_downgrade.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      976 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_dropall.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1750 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_heads.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1974 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_history.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4254 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_revision.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1720 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_stamp.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2348 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_upgrade.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      551 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/pytest_plugin.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    11557 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/routers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1551 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/shortcuts.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2130 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/testing.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2070 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/utils.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/validators/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      189 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/validators/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     7916 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/validators/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1259 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/validators/runner.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/views/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      212 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/views/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     8182 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/views/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2736 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/views/detail.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5535 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/views/edit.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3545 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/views/list.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery/viewsets/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      338 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/viewsets/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6135 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/viewsets/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    10740 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/django_sorcery/viewsets/mixins.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    26015 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/PKG-INFO
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5001 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/SOURCES.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)        1 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/dependency_links.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       58 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/entry_points.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       72 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/requires.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       15 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/django_sorcery.egg-info/top_level.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      240 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/requirements.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      489 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/setup.cfg
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2921 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/setup.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      250 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      867 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/base.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/db/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/__init__.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/db/alembic/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/alembic/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1356 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/alembic/test_base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1709 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/alembic/test_signals.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/db/meta/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      539 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/test_base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    15772 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/test_column.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3882 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/test_composite.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     7088 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/test_model.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4275 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/meta/test_relations.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2537 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_composites.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    10399 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_fields.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5761 2019-07-14 23:14:46.000000 django-sorcery-0.9.4/tests/db/test_middleware.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5171 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_mixins.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    21999 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2735 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_profiler.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4623 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_query.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3177 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_relations.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3448 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_session.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      253 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_signals.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2778 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_sqlalchemy.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1711 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_transaction.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5604 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_url.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4639 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/db/test_utils.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/formsets/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/formsets/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    16778 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/formsets/test_base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     9591 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/formsets/test_inline.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/management/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/__init__.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/management/commands/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      583 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1583 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3447 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_current.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3570 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_downgrade.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2575 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_heads.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2826 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_history.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2626 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_revision.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1781 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_stamp.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3575 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/commands/test_sorcery_upgrade.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1847 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/management/test_base.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/minimalapp/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/minimalapp/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      230 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/minimalapp/apps.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1599 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/minimalapp/models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1939 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/models_backpop.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      640 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/models_multidb.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      677 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/models_terrible_relations.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/otherapp/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/otherapp/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      224 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/otherapp/apps.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/otherapp/migrations/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/otherapp/migrations/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      361 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/otherapp/models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2652 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/settings.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/templates/
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       11 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/owner_confirm_delete.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       18 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/owner_detail.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       14 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/owner_form.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       57 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/owner_list.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       14 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/tests.testapp/vehicle_form.html
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/templates/views/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       11 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/views/edit.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       52 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/templates/views/list.html
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      298 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_compat.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2940 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_exceptions.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6928 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_fields.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    25619 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_forms.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1490 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_pytest_plugin.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     5918 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_routers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1588 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_shortcuts.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      986 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_utils.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     6415 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/test_validators.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/testapp/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/testapp/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      257 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/testapp/apps.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/testapp/migrations/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     8178 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/testapp/models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2462 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/testapp/views.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2321 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/urls.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/views/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/views/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3075 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/views/test_base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3109 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/views/test_detail.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4276 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/views/test_edit.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4342 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/views/test_list.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-07-14 23:15:47.000000 django-sorcery-0.9.4/tests/viewsets/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       97 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/viewsets/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1059 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/viewsets/test_base.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    11119 2019-07-14 14:14:50.000000 django-sorcery-0.9.4/tests/viewsets/test_mixins.py
```

### Comparing `django-sorcery-0.9.3/HISTORY.rst` & `django-sorcery-0.9.4/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
-0.9.3 (2019-06-26)
+0.9.4 (2019-07-14)
 -----------------------------
+- Fix middleware response return (#143) [Serkan Hosca]
+- Use python/black (#141) [Serkan Hosca]
+
+
+0.9.3 (2019-06-27)
+------------------
 - Defining test matrix in tox and switchint to tox-travis (#140)
   [Miroslav Shubernetskiy]
 - Increase build matrix (#139) [Serkan Hosca]
 - Update pre-commit (#138) [Serkan Hosca]
 
 
 0.9.2 (2019-05-10)
```

### Comparing `django-sorcery-0.9.3/PKG-INFO` & `django-sorcery-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-sorcery
-Version: 0.9.3
+Version: 0.9.4
 Summary: Django and SQLAlchemy integration
 Home-page: https://github.com/shosca/django-sorcery
 Author: Serkan Hosca
 Author-email: serkan@hosca.com
 License: MIT
 Project-URL: Documentation, https://django-sorcery.readthedocs.io
 Project-URL: Source, https://github.com/shosca/django-sorcery
```

### Comparing `django-sorcery-0.9.3/README.rst` & `django-sorcery-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/__init__.py` & `django-sorcery-0.9.4/django_sorcery/db/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/alembic/base.py` & `django-sorcery-0.9.4/django_sorcery/db/alembic/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/alembic/signals.py` & `django-sorcery-0.9.4/django_sorcery/db/alembic/signals.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/composites.py` & `django-sorcery-0.9.4/django_sorcery/db/composites.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/fields.py` & `django-sorcery-0.9.4/django_sorcery/db/fields.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/meta/base.py` & `django-sorcery-0.9.4/django_sorcery/db/meta/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/meta/column.py` & `django-sorcery-0.9.4/django_sorcery/db/meta/column.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/meta/composite.py` & `django-sorcery-0.9.4/django_sorcery/db/meta/composite.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/meta/model.py` & `django-sorcery-0.9.4/django_sorcery/db/meta/model.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/meta/relations.py` & `django-sorcery-0.9.4/django_sorcery/db/meta/relations.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/middleware.py` & `django-sorcery-0.9.4/django_sorcery/db/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,17 +53,18 @@
 
         try:
             self.flush(request=request, response=response)
             self.commit(request=request, response=response)
         except Exception:
             self.logger.error("Error during flush or commit")
             self.rollback(request=request, response=response)
-            raise
-        finally:
             self.return_response(request, response)
+            raise
+
+        return self.return_response(request, response)
 
     def return_response(self, request, response):
         """
         Hook for adding arbitrary logic to response processing
         """
         self.remove(request=request, response=response)
```

### Comparing `django-sorcery-0.9.3/django_sorcery/db/mixins.py` & `django-sorcery-0.9.4/django_sorcery/db/mixins.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/models.py` & `django-sorcery-0.9.4/django_sorcery/db/models.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/profiler.py` & `django-sorcery-0.9.4/django_sorcery/db/profiler.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/query.py` & `django-sorcery-0.9.4/django_sorcery/db/query.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/relations.py` & `django-sorcery-0.9.4/django_sorcery/db/relations.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/session.py` & `django-sorcery-0.9.4/django_sorcery/db/session.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/signals.py` & `django-sorcery-0.9.4/django_sorcery/db/signals.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/sqlalchemy.py` & `django-sorcery-0.9.4/django_sorcery/db/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/transaction.py` & `django-sorcery-0.9.4/django_sorcery/db/transaction.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/url.py` & `django-sorcery-0.9.4/django_sorcery/db/url.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/db/utils.py` & `django-sorcery-0.9.4/django_sorcery/db/utils.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/exceptions.py` & `django-sorcery-0.9.4/django_sorcery/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/fields.py` & `django-sorcery-0.9.4/django_sorcery/fields.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/forms.py` & `django-sorcery-0.9.4/django_sorcery/forms.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/formsets/base.py` & `django-sorcery-0.9.4/django_sorcery/formsets/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/formsets/inline.py` & `django-sorcery-0.9.4/django_sorcery/formsets/inline.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/alembic.py` & `django-sorcery-0.9.4/django_sorcery/management/alembic.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/base.py` & `django-sorcery-0.9.4/django_sorcery/management/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_createall.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_createall.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_current.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_current.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_downgrade.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_downgrade.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_dropall.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_dropall.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_heads.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_heads.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_history.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_history.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_revision.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_revision.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_stamp.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_stamp.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/management/commands/sorcery_upgrade.py` & `django-sorcery-0.9.4/django_sorcery/management/commands/sorcery_upgrade.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/pytest_plugin.py` & `django-sorcery-0.9.4/django_sorcery/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/routers.py` & `django-sorcery-0.9.4/django_sorcery/routers.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/shortcuts.py` & `django-sorcery-0.9.4/django_sorcery/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/testing.py` & `django-sorcery-0.9.4/django_sorcery/testing.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/utils.py` & `django-sorcery-0.9.4/django_sorcery/utils.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/validators/base.py` & `django-sorcery-0.9.4/django_sorcery/validators/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/validators/runner.py` & `django-sorcery-0.9.4/django_sorcery/validators/runner.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/views/base.py` & `django-sorcery-0.9.4/django_sorcery/views/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/views/detail.py` & `django-sorcery-0.9.4/django_sorcery/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/views/edit.py` & `django-sorcery-0.9.4/django_sorcery/views/edit.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/views/list.py` & `django-sorcery-0.9.4/django_sorcery/views/list.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/viewsets/base.py` & `django-sorcery-0.9.4/django_sorcery/viewsets/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery/viewsets/mixins.py` & `django-sorcery-0.9.4/django_sorcery/viewsets/mixins.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/django_sorcery.egg-info/PKG-INFO` & `django-sorcery-0.9.4/django_sorcery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-sorcery
-Version: 0.9.3
+Version: 0.9.4
 Summary: Django and SQLAlchemy integration
 Home-page: https://github.com/shosca/django-sorcery
 Author: Serkan Hosca
 Author-email: serkan@hosca.com
 License: MIT
 Project-URL: Documentation, https://django-sorcery.readthedocs.io
 Project-URL: Source, https://github.com/shosca/django-sorcery
```

### Comparing `django-sorcery-0.9.3/django_sorcery.egg-info/SOURCES.txt` & `django-sorcery-0.9.4/django_sorcery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/setup.py` & `django-sorcery-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/base.py` & `django-sorcery-0.9.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/alembic/test_base.py` & `django-sorcery-0.9.4/tests/db/alembic/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/alembic/test_signals.py` & `django-sorcery-0.9.4/tests/db/alembic/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/meta/test_base.py` & `django-sorcery-0.9.4/tests/db/meta/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/meta/test_column.py` & `django-sorcery-0.9.4/tests/db/meta/test_column.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/meta/test_composite.py` & `django-sorcery-0.9.4/tests/db/meta/test_composite.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/meta/test_model.py` & `django-sorcery-0.9.4/tests/db/meta/test_model.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/meta/test_relations.py` & `django-sorcery-0.9.4/tests/db/meta/test_relations.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_composites.py` & `django-sorcery-0.9.4/tests/db/test_composites.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_fields.py` & `django-sorcery-0.9.4/tests/db/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_middleware.py` & `django-sorcery-0.9.4/tests/db/test_middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,43 +49,48 @@
 class TestBaseMiddleware(unittest.TestCase):
     def setUp(self):
         super(TestBaseMiddleware, self).setUp()
         self.middleware = DummyMiddeware(get_response=get_response)
 
     def test_process_request(self):
         self.middleware.dummy = "abcd"
-        self.middleware(Request())
+        response = self.middleware(Request())
+        self.assertIsNotNone(response)
         self.assertFalse(self.middleware.rollback_called)
         self.assertFalse(self.middleware.flush_called)
         self.assertFalse(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_success(self):
-        self.middleware(Request())
+        response = self.middleware(Request())
+        self.assertIsNotNone(response)
         self.assertFalse(self.middleware.rollback_called)
         self.assertTrue(self.middleware.flush_called)
         self.assertTrue(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_redirect(self):
-        self.middleware(Request(status_code=300))
+        response = self.middleware(Request(status_code=300))
+        self.assertIsNotNone(response)
         self.assertFalse(self.middleware.rollback_called)
         self.assertTrue(self.middleware.flush_called)
         self.assertTrue(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_bad_request(self):
-        self.middleware(Request(status_code=400))
+        response = self.middleware(Request(status_code=400))
+        self.assertIsNotNone(response)
         self.assertTrue(self.middleware.rollback_called)
         self.assertFalse(self.middleware.flush_called)
         self.assertFalse(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_server_error(self):
-        self.middleware(Request(status_code=400))
+        response = self.middleware(Request(status_code=400))
+        self.assertIsNotNone(response)
         self.assertTrue(self.middleware.rollback_called)
         self.assertFalse(self.middleware.flush_called)
         self.assertFalse(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_flush_error(self):
         self.middleware.flush_error = RuntimeError
@@ -93,15 +98,16 @@
             self.middleware(Request(status_code=200))
         self.assertTrue(self.middleware.rollback_called)
         self.assertTrue(self.middleware.flush_called)
         self.assertFalse(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
     def test_other_methods(self):
-        self.middleware(Request(method="HEAD"))
+        response = self.middleware(Request(method="HEAD"))
+        self.assertIsNotNone(response)
         self.assertTrue(self.middleware.rollback_called)
         self.assertFalse(self.middleware.flush_called)
         self.assertFalse(self.middleware.commit_called)
         self.assertTrue(self.middleware.remove_called)
 
 
 class TestSQLAlchemyDBMiddleware(unittest.TestCase):
```

### Comparing `django-sorcery-0.9.3/tests/db/test_mixins.py` & `django-sorcery-0.9.4/tests/db/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_models.py` & `django-sorcery-0.9.4/tests/db/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_profiler.py` & `django-sorcery-0.9.4/tests/db/test_profiler.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_query.py` & `django-sorcery-0.9.4/tests/db/test_query.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_relations.py` & `django-sorcery-0.9.4/tests/db/test_relations.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_session.py` & `django-sorcery-0.9.4/tests/db/test_session.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_sqlalchemy.py` & `django-sorcery-0.9.4/tests/db/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_transaction.py` & `django-sorcery-0.9.4/tests/db/test_transaction.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_url.py` & `django-sorcery-0.9.4/tests/db/test_url.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/db/test_utils.py` & `django-sorcery-0.9.4/tests/db/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/formsets/test_base.py` & `django-sorcery-0.9.4/tests/formsets/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/formsets/test_inline.py` & `django-sorcery-0.9.4/tests/formsets/test_inline.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/base.py` & `django-sorcery-0.9.4/tests/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_current.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_current.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_downgrade.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_downgrade.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_heads.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_heads.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_history.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_history.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_revision.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_revision.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_stamp.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_stamp.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/commands/test_sorcery_upgrade.py` & `django-sorcery-0.9.4/tests/management/commands/test_sorcery_upgrade.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/management/test_base.py` & `django-sorcery-0.9.4/tests/management/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/minimalapp/models.py` & `django-sorcery-0.9.4/tests/minimalapp/models.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/models_backpop.py` & `django-sorcery-0.9.4/tests/models_backpop.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/models_multidb.py` & `django-sorcery-0.9.4/tests/models_multidb.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/models_terrible_relations.py` & `django-sorcery-0.9.4/tests/models_terrible_relations.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/settings.py` & `django-sorcery-0.9.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_exceptions.py` & `django-sorcery-0.9.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_fields.py` & `django-sorcery-0.9.4/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_forms.py` & `django-sorcery-0.9.4/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_pytest_plugin.py` & `django-sorcery-0.9.4/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_routers.py` & `django-sorcery-0.9.4/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_shortcuts.py` & `django-sorcery-0.9.4/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_utils.py` & `django-sorcery-0.9.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/test_validators.py` & `django-sorcery-0.9.4/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/testapp/models.py` & `django-sorcery-0.9.4/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/testapp/views.py` & `django-sorcery-0.9.4/tests/testapp/views.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/urls.py` & `django-sorcery-0.9.4/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/views/test_base.py` & `django-sorcery-0.9.4/tests/views/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/views/test_detail.py` & `django-sorcery-0.9.4/tests/views/test_detail.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/views/test_edit.py` & `django-sorcery-0.9.4/tests/views/test_edit.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/views/test_list.py` & `django-sorcery-0.9.4/tests/views/test_list.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/viewsets/test_base.py` & `django-sorcery-0.9.4/tests/viewsets/test_base.py`

 * *Files identical despite different names*

### Comparing `django-sorcery-0.9.3/tests/viewsets/test_mixins.py` & `django-sorcery-0.9.4/tests/viewsets/test_mixins.py`

 * *Files identical despite different names*

