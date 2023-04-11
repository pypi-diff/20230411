# Comparing `tmp/tracuni-0.4.8.tar.gz` & `tmp/tracuni-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tracuni-0.4.8.tar", last modified: Mon Nov 18 13:17:24 2019, max compression
+gzip compressed data, was "dist/tracuni-0.4.9.tar", last modified: Wed Feb 12 11:25:00 2020, max compression
```

## Comparing `tracuni-0.4.8.tar` & `tracuni-0.4.9.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/
--rw-r--r--   0 tova      (1000) tova      (1001)     1862 2019-11-18 13:17:23.000000 tracuni-0.4.8/HISTORY.rst
--rw-r--r--   0 tova      (1000) tova      (1001)      312 2019-11-18 13:17:23.000000 tracuni-0.4.8/MANIFEST.in
--rw-r--r--   0 tova      (1000) tova      (1001)     3685 2019-11-18 13:17:24.000000 tracuni-0.4.8/PKG-INFO
--rw-r--r--   0 tova      (1000) tova      (1001)      428 2019-11-18 13:17:23.000000 tracuni-0.4.8/README.rst
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/docs/
--rw-r--r--   0 tova      (1000) tova      (1001)      609 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/Makefile
--rwxr-xr-x   0 tova      (1000) tova      (1001)     4969 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/conf.py
--rw-r--r--   0 tova      (1000) tova      (1001)       28 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/history.rst
--rw-r--r--   0 tova      (1000) tova      (1001)      299 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/index.rst
--rw-r--r--   0 tova      (1000) tova      (1001)     1114 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/installation.rst
--rw-r--r--   0 tova      (1000) tova      (1001)      770 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/make.bat
--rw-r--r--   0 tova      (1000) tova      (1001)       27 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/readme.rst
--rw-r--r--   0 tova      (1000) tova      (1001)      297 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/tooling.rst
--rw-r--r--   0 tova      (1000) tova      (1001)    10569 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/tox.todo.rst
--rw-r--r--   0 tova      (1000) tova      (1001)       71 2019-11-18 13:17:23.000000 tracuni-0.4.8/docs/usage.rst
--rw-r--r--   0 tova      (1000) tova      (1001)      323 2019-11-18 13:17:23.000000 tracuni-0.4.8/requirements.txt
--rw-r--r--   0 tova      (1000) tova      (1001)      486 2019-11-18 13:17:23.000000 tracuni-0.4.8/requirements_dev.txt
--rw-r--r--   0 tova      (1000) tova      (1001)      741 2019-11-18 13:17:24.000000 tracuni-0.4.8/setup.cfg
--rw-r--r--   0 tova      (1000) tova      (1001)     1664 2019-11-18 13:17:23.000000 tracuni-0.4.8/setup.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/
--rw-r--r--   0 tova      (1000) tova      (1001)      562 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/conftest.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/define/
--rw-r--r--   0 tova      (1000) tova      (1001)     3627 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/define/test_const.py
--rw-r--r--   0 tova      (1000) tova      (1001)    21723 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/define/test_type.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/fixtures/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/fixtures/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1814 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/fixtures/fixture_engine.py
--rw-r--r--   0 tova      (1000) tova      (1001)     7086 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/fixtures/fixture_engine_schemas.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4300 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/fixtures/fixture_engine_structures.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/
--rw-r--r--   0 tova      (1000) tova      (1001)      390 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/Pipfile
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2594 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/app.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4073 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/amqp_server.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3821 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/app.py
--rw-r--r--   0 tova      (1000) tova      (1001)      383 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/component.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3844 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/db.py
--rw-r--r--   0 tova      (1000) tova      (1001)      378 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/error.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1675 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/handler.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5240 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/helper.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2183 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/http_client.py
--rw-r--r--   0 tova      (1000) tova      (1001)     6045 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/http_server.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5123 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/amqp_handler.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2581 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/http_handler.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1047 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/http_router.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/lib/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/lib/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4826 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/lib/helper.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/models/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/models/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1456 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/app/models/tasks_db.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/config/
--rw-r--r--   0 tova      (1000) tova      (1001)     2493 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/config/error_conf.json
--rw-r--r--   0 tova      (1000) tova      (1001)     1808 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/config/main.json
--rw-r--r--   0 tova      (1000) tova      (1001)     2006 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/config/main.json.sample
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/logs/
--rw-r--r--   0 tova      (1000) tova      (1001)       71 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/logs/.gitignore
--rw-r--r--   0 tova      (1000) tova      (1001)     1222 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/main.py
--rw-r--r--   0 tova      (1000) tova      (1001)       96 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095/requirements.txt
--rw-r--r--   0 tova      (1000) tova      (1001)     1812 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/sample/srv_aio_8095.json
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tests/schema/
--rw-r--r--   0 tova      (1000) tova      (1001)     6678 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/schema/test_engine_cache.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5568 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/schema/test_engine_feed.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5468 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/schema/test_engine_instance.py
--rw-r--r--   0 tova      (1000) tova      (1001)    15713 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/schema/test_engine_run.py
--rw-r--r--   0 tova      (1000) tova      (1001)      689 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/test_point_accessor.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1044 2019-11-18 13:17:23.000000 tracuni-0.4.8/tests/test_trac_uni.py
--rw-r--r--   0 tova      (1000) tova      (1001)      729 2019-11-18 13:17:23.000000 tracuni-0.4.8/tox.ini
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/
--rw-r--r--   0 tova      (1000) tova      (1001)     4816 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)    12054 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/adapter.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3794 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/adapter_tornado.py
--rw-r--r--   0 tova      (1000) tova      (1001)      479 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/cli.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/define/
--rw-r--r--   0 tova      (1000) tova      (1001)       50 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/define/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5864 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/define/const.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1926 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/define/errors.py
--rw-r--r--   0 tova      (1000) tova      (1001)    22713 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/define/type.py
--rw-r--r--   0 tova      (1000) tova      (1001)     9053 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/intercept.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/misc/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/misc/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4997 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/misc/helper.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2719 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/misc/keep_tornado.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1575 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/misc/select_coroutine.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/point/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/point/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)    11304 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/point/accessor.py
--rw-r--r--   0 tova      (1000) tova      (1001)     8779 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/point/span_general.py
--rw-r--r--   0 tova      (1000) tova      (1001)     7042 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/point/span_stages.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/__init__.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/builtin/
--rw-r--r--   0 tova      (1000) tova      (1001)     1715 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/__init__.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/builtin/core/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     6495 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_amqp_in.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3978 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_amqp_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4140 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_db_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)    12050 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_in.py
--rw-r--r--   0 tova      (1000) tova      (1001)    12567 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_in_headers.py
--rw-r--r--   0 tova      (1000) tova      (1001)    10993 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1679 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/core/ext_retry_out.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4225 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_amqp_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4177 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_db_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)    11383 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_http_in.py
--rw-r--r--   0 tova      (1000) tova      (1001)    11471 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_http_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1366 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_inner_retry_in.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2006 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_inner_retry_out.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3257 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/builtin/tornado/log_out.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/engine/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/engine/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)    12013 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/engine/engine.py
--rw-r--r--   0 tova      (1000) tova      (1001)    14868 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/engine/feed.py
--rw-r--r--   0 tova      (1000) tova      (1001)     6823 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/engine/pool.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/schema/lib/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3348 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/catch_essential.py
--rw-r--r--   0 tova      (1000) tova      (1001)     1663 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/debug.py
--rw-r--r--   0 tova      (1000) tova      (1001)      778 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/make_cut.py
--rw-r--r--   0 tova      (1000) tova      (1001)     4939 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/mask_secret.py
--rw-r--r--   0 tova      (1000) tova      (1001)      551 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/lib/pick_items.py
--rw-r--r--   0 tova      (1000) tova      (1001)    18604 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/pipe_methods.py
--rw-r--r--   0 tova      (1000) tova      (1001)     3469 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/shared_rules.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5105 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/schema/standard.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/side_steps/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/__init__.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/side_steps/db_logger/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/db_logger/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     2977 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/db_logger/logger.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni/side_steps/stat/
--rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/stat/__init__.py
--rw-r--r--   0 tova      (1000) tova      (1001)     7268 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/stat/adapter.py
--rw-r--r--   0 tova      (1000) tova      (1001)     5398 2019-11-18 13:17:23.000000 tracuni-0.4.8/tracuni/side_steps/stat/send.py
-drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/
--rw-r--r--   0 tova      (1000) tova      (1001)     3685 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/PKG-INFO
--rw-r--r--   0 tova      (1000) tova      (1001)     3990 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/SOURCES.txt
--rw-r--r--   0 tova      (1000) tova      (1001)        1 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/dependency_links.txt
--rw-r--r--   0 tova      (1000) tova      (1001)       46 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/entry_points.txt
--rw-r--r--   0 tova      (1000) tova      (1001)        1 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/not-zip-safe
--rw-r--r--   0 tova      (1000) tova      (1001)       94 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/requires.txt
--rw-r--r--   0 tova      (1000) tova      (1001)        8 2019-11-18 13:17:24.000000 tracuni-0.4.8/tracuni.egg-info/top_level.txt
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/
+-rw-r--r--   0 tova      (1000) tova      (1001)     1862 2019-11-06 12:51:14.000000 tracuni-0.4.9/HISTORY.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)      312 2018-12-21 13:23:51.000000 tracuni-0.4.9/MANIFEST.in
+-rw-r--r--   0 tova      (1000) tova      (1001)     3685 2020-02-12 11:25:00.000000 tracuni-0.4.9/PKG-INFO
+-rw-r--r--   0 tova      (1000) tova      (1001)      428 2019-01-30 12:32:19.000000 tracuni-0.4.9/README.rst
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/docs/
+-rw-r--r--   0 tova      (1000) tova      (1001)      609 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/Makefile
+-rwxr-xr-x   0 tova      (1000) tova      (1001)     4969 2019-03-06 07:00:40.000000 tracuni-0.4.9/docs/conf.py
+-rw-r--r--   0 tova      (1000) tova      (1001)       28 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/history.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)      299 2018-12-21 13:50:07.000000 tracuni-0.4.9/docs/index.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)     1114 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/installation.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)      770 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/make.bat
+-rw-r--r--   0 tova      (1000) tova      (1001)       27 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/readme.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)      297 2018-12-21 13:51:00.000000 tracuni-0.4.9/docs/tooling.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)    10569 2019-03-06 07:00:40.000000 tracuni-0.4.9/docs/tox.todo.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)       71 2018-12-20 11:13:41.000000 tracuni-0.4.9/docs/usage.rst
+-rw-r--r--   0 tova      (1000) tova      (1001)      323 2019-02-01 13:39:55.000000 tracuni-0.4.9/requirements.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)      486 2019-01-23 08:13:56.000000 tracuni-0.4.9/requirements_dev.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)      741 2020-02-12 11:25:00.000000 tracuni-0.4.9/setup.cfg
+-rw-r--r--   0 tova      (1000) tova      (1001)     1664 2020-02-12 11:22:55.000000 tracuni-0.4.9/setup.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/
+-rw-r--r--   0 tova      (1000) tova      (1001)      562 2019-01-18 15:25:04.000000 tracuni-0.4.9/tests/conftest.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/define/
+-rw-r--r--   0 tova      (1000) tova      (1001)     3627 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/define/test_const.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    21723 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/define/test_type.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/fixtures/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-01-18 15:04:38.000000 tracuni-0.4.9/tests/fixtures/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1814 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/fixtures/fixture_engine.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     7086 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/fixtures/fixture_engine_schemas.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4300 2019-08-28 14:28:03.000000 tracuni-0.4.9/tests/fixtures/fixture_engine_structures.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/
+-rw-r--r--   0 tova      (1000) tova      (1001)      390 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/Pipfile
+-rw-r--r--   0 tova      (1000) tova      (1001)    13992 2019-01-24 06:44:44.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/Pipfile.lock
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2594 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/app.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4073 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/amqp_server.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3821 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/app.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      383 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/component.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3844 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/db.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      378 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/error.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1675 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/handler.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5240 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/helper.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2183 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/http_client.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     6045 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/http_server.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5123 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/amqp_handler.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2581 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/http_handler.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1047 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/http_router.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/lib/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/lib/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4826 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/lib/helper.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/models/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/models/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1456 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/app/models/tasks_db.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/config/
+-rw-r--r--   0 tova      (1000) tova      (1001)     2493 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/config/error_conf.json
+-rw-r--r--   0 tova      (1000) tova      (1001)     1808 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/config/main.json
+-rw-r--r--   0 tova      (1000) tova      (1001)     2006 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/config/main.json.sample
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/logs/
+-rw-r--r--   0 tova      (1000) tova      (1001)       71 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/logs/.gitignore
+-rw-r--r--   0 tova      (1000) tova      (1001)     1222 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/main.py
+-rw-r--r--   0 tova      (1000) tova      (1001)       96 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095/requirements.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)     1812 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/sample/srv_aio_8095.json
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tests/schema/
+-rw-r--r--   0 tova      (1000) tova      (1001)     6678 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/schema/test_engine_cache.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5568 2019-02-01 13:39:55.000000 tracuni-0.4.9/tests/schema/test_engine_feed.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5468 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/schema/test_engine_instance.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    15713 2019-02-08 15:59:30.000000 tracuni-0.4.9/tests/schema/test_engine_run.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      689 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/test_point_accessor.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1044 2019-02-01 12:17:52.000000 tracuni-0.4.9/tests/test_trac_uni.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      729 2019-01-23 16:41:29.000000 tracuni-0.4.9/tox.ini
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/
+-rw-r--r--   0 tova      (1000) tova      (1001)     4816 2020-02-12 11:22:55.000000 tracuni-0.4.9/tracuni/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    12054 2019-04-29 14:47:31.000000 tracuni-0.4.9/tracuni/adapter.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3794 2019-04-17 10:21:56.000000 tracuni-0.4.9/tracuni/adapter_tornado.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      479 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/cli.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/define/
+-rw-r--r--   0 tova      (1000) tova      (1001)       50 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/define/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5864 2019-10-31 11:05:59.000000 tracuni-0.4.9/tracuni/define/const.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1926 2019-06-14 08:40:22.000000 tracuni-0.4.9/tracuni/define/errors.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    22713 2019-08-07 16:37:53.000000 tracuni-0.4.9/tracuni/define/type.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     9053 2019-08-08 11:45:09.000000 tracuni-0.4.9/tracuni/intercept.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/misc/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/misc/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4997 2019-05-06 09:00:44.000000 tracuni-0.4.9/tracuni/misc/helper.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2719 2019-03-05 17:28:16.000000 tracuni-0.4.9/tracuni/misc/keep_tornado.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1575 2019-03-07 12:00:26.000000 tracuni-0.4.9/tracuni/misc/select_coroutine.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/point/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 13:39:55.000000 tracuni-0.4.9/tracuni/point/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    11304 2019-10-31 11:24:42.000000 tracuni-0.4.9/tracuni/point/accessor.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     8779 2019-05-16 12:25:27.000000 tracuni-0.4.9/tracuni/point/span_general.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     7042 2019-05-06 08:47:51.000000 tracuni-0.4.9/tracuni/point/span_stages.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/__init__.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/builtin/
+-rw-r--r--   0 tova      (1000) tova      (1001)     1715 2019-08-06 15:17:32.000000 tracuni-0.4.9/tracuni/schema/builtin/__init__.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/builtin/core/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 13:39:55.000000 tracuni-0.4.9/tracuni/schema/builtin/core/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     6495 2019-06-11 13:23:51.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_amqp_in.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3978 2019-04-29 14:47:31.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_amqp_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4140 2019-03-11 17:33:37.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_db_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    12050 2019-11-06 12:37:13.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_in.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    12567 2019-11-06 12:39:46.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_in_headers.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    10993 2019-10-31 11:04:58.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1679 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/builtin/core/ext_retry_out.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-04 10:01:32.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4225 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_amqp_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4177 2019-03-11 17:33:37.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_db_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    11383 2019-11-18 13:14:19.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_http_in.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    11575 2020-02-12 11:15:52.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_http_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1366 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_inner_retry_in.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2006 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_inner_retry_out.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3257 2019-05-06 08:56:42.000000 tracuni-0.4.9/tracuni/schema/builtin/tornado/log_out.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/engine/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/engine/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    12013 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/engine/engine.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    14868 2019-02-01 13:39:55.000000 tracuni-0.4.9/tracuni/schema/engine/feed.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     6823 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/engine/pool.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/schema/lib/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/lib/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3348 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/lib/catch_essential.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     1663 2019-03-06 07:04:41.000000 tracuni-0.4.9/tracuni/schema/lib/debug.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      778 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/schema/lib/make_cut.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     4939 2019-10-31 10:58:54.000000 tracuni-0.4.9/tracuni/schema/lib/mask_secret.py
+-rw-r--r--   0 tova      (1000) tova      (1001)      551 2019-08-08 11:54:01.000000 tracuni-0.4.9/tracuni/schema/lib/pick_items.py
+-rw-r--r--   0 tova      (1000) tova      (1001)    18688 2020-02-12 10:38:27.000000 tracuni-0.4.9/tracuni/schema/pipe_methods.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     3469 2019-04-29 15:19:55.000000 tracuni-0.4.9/tracuni/schema/shared_rules.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5105 2019-08-07 19:00:02.000000 tracuni-0.4.9/tracuni/schema/standard.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/side_steps/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/side_steps/__init__.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/side_steps/db_logger/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/side_steps/db_logger/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     2977 2019-03-06 07:05:29.000000 tracuni-0.4.9/tracuni/side_steps/db_logger/logger.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni/side_steps/stat/
+-rw-r--r--   0 tova      (1000) tova      (1001)        0 2019-02-01 12:17:52.000000 tracuni-0.4.9/tracuni/side_steps/stat/__init__.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     7268 2019-07-18 14:35:53.000000 tracuni-0.4.9/tracuni/side_steps/stat/adapter.py
+-rw-r--r--   0 tova      (1000) tova      (1001)     5398 2019-08-08 11:22:33.000000 tracuni-0.4.9/tracuni/side_steps/stat/send.py
+drwxr-xr-x   0 tova      (1000) tova      (1001)        0 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/
+-rw-r--r--   0 tova      (1000) tova      (1001)     3685 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/PKG-INFO
+-rw-r--r--   0 tova      (1000) tova      (1001)     4029 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/SOURCES.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)        1 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/dependency_links.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)       46 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/entry_points.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)        1 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/not-zip-safe
+-rw-r--r--   0 tova      (1000) tova      (1001)       94 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/requires.txt
+-rw-r--r--   0 tova      (1000) tova      (1001)        8 2020-02-12 11:25:00.000000 tracuni-0.4.9/tracuni.egg-info/top_level.txt
```

### Comparing `tracuni-0.4.8/HISTORY.rst` & `tracuni-0.4.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/PKG-INFO` & `tracuni-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tracuni
-Version: 0.4.8
+Version: 0.4.9
 Summary: Convenient library to plug in tracer to incoming and outgoing points and extract data from there
 Home-page: https://github.com/hastly/tracuni
 Author: Konstantin Gonciarou
 Author-email: konstantin.goncharov@inplat.ru
 License: UNKNOWN
 Description: ========
         trac_uni
```

### Comparing `tracuni-0.4.8/docs/Makefile` & `tracuni-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/docs/conf.py` & `tracuni-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/docs/installation.rst` & `tracuni-0.4.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/docs/make.bat` & `tracuni-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/docs/tox.todo.rst` & `tracuni-0.4.9/docs/tox.todo.rst`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/setup.cfg` & `tracuni-0.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.8
+current_version = 0.4.9
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `tracuni-0.4.8/setup.py` & `tracuni-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     name='tracuni',
     packages=find_packages(),
     python_requires='>=3.5.3',
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hastly/tracuni',
-    version='0.4.8',
+    version='0.4.9',
     zip_safe=False,
 )
```

### Comparing `tracuni-0.4.8/tests/conftest.py` & `tracuni-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/define/test_const.py` & `tracuni-0.4.9/tests/define/test_const.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/define/test_type.py` & `tracuni-0.4.9/tests/define/test_type.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/fixtures/fixture_engine.py` & `tracuni-0.4.9/tests/fixtures/fixture_engine.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/fixtures/fixture_engine_schemas.py` & `tracuni-0.4.9/tests/fixtures/fixture_engine_schemas.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/fixtures/fixture_engine_structures.py` & `tracuni-0.4.9/tests/fixtures/fixture_engine_structures.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/app.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/app.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/amqp_server.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/amqp_server.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/app.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/app.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/db.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/db.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/handler.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/handler.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/helper.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/helper.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/http_client.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/http_client.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/core/http_server.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/core/http_server.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/amqp_handler.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/amqp_handler.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/http_handler.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/handlers/http_router.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/handlers/http_router.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/lib/helper.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/lib/helper.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/app/models/tasks_db.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/app/models/tasks_db.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/config/error_conf.json` & `tracuni-0.4.9/tests/sample/srv_aio_8095/config/error_conf.json`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/config/main.json` & `tracuni-0.4.9/tests/sample/srv_aio_8095/config/main.json`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/config/main.json.sample` & `tracuni-0.4.9/tests/sample/srv_aio_8095/config/main.json.sample`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095/main.py` & `tracuni-0.4.9/tests/sample/srv_aio_8095/main.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/sample/srv_aio_8095.json` & `tracuni-0.4.9/tests/sample/srv_aio_8095.json`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/schema/test_engine_cache.py` & `tracuni-0.4.9/tests/schema/test_engine_cache.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/schema/test_engine_feed.py` & `tracuni-0.4.9/tests/schema/test_engine_feed.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/schema/test_engine_instance.py` & `tracuni-0.4.9/tests/schema/test_engine_instance.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/schema/test_engine_run.py` & `tracuni-0.4.9/tests/schema/test_engine_run.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/test_point_accessor.py` & `tracuni-0.4.9/tests/test_point_accessor.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tests/test_trac_uni.py` & `tracuni-0.4.9/tests/test_trac_uni.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tox.ini` & `tracuni-0.4.9/tox.ini`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/__init__.py` & `tracuni-0.4.9/tracuni/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     SpanSide,
     APIKind,
     Part,
 )
 
 __author__ = """Konstantin Gonciarou"""
 __email__ = 'konstantin.goncharov@inplat.ru'
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 
 __all__ = (
     # interceptor
     'fab_tracer',  # инициализация адаптера для работы с aiohttp приложением
     'init_tornado_loop',  # инициализация для работы с Tornado приложением
     'tracer_point',  # декоратор перехвата вызова точки и запуска извлечения
     # Types
```

### Comparing `tracuni-0.4.8/tracuni/adapter.py` & `tracuni-0.4.9/tracuni/adapter.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/adapter_tornado.py` & `tracuni-0.4.9/tracuni/adapter_tornado.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/define/const.py` & `tracuni-0.4.9/tracuni/define/const.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/define/errors.py` & `tracuni-0.4.9/tracuni/define/errors.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/define/type.py` & `tracuni-0.4.9/tracuni/define/type.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/intercept.py` & `tracuni-0.4.9/tracuni/intercept.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/misc/helper.py` & `tracuni-0.4.9/tracuni/misc/helper.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/misc/keep_tornado.py` & `tracuni-0.4.9/tracuni/misc/keep_tornado.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/misc/select_coroutine.py` & `tracuni-0.4.9/tracuni/misc/select_coroutine.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/point/accessor.py` & `tracuni-0.4.9/tracuni/point/accessor.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/point/span_general.py` & `tracuni-0.4.9/tracuni/point/span_general.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/point/span_stages.py` & `tracuni-0.4.9/tracuni/point/span_stages.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/__init__.py` & `tracuni-0.4.9/tracuni/schema/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_amqp_in.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_amqp_in.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_amqp_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_amqp_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_db_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_db_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_in.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_in.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_in_headers.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_in_headers.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_http_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_http_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/core/ext_retry_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/core/ext_retry_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_amqp_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_amqp_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_db_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_db_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_http_in.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_http_in.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_http_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_http_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,18 +189,21 @@
             pipe_dump,
             pipe_mask_secret_catch_essentials,
             pipe_head,
         ),
         origins=(
             Origin(
                 OriginSection.REUSE,
-                lambda data: data['request']['headers'],
+                lambda data: data['response'].get(
+                    'request_headers',
+                    data['request'].get('headers')
+                ),
             ),
         ),
-        stage=Stage.PRE,
+        stage=Stage.POST,
     ),
     Rule(
         description="Разделитель запроса и ответа",
         destination=Destination(
             DestinationSection.SPAN_LOGS,
             'divider',
         ),
```

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_inner_retry_in.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_inner_retry_in.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/ext_inner_retry_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/ext_inner_retry_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/builtin/tornado/log_out.py` & `tracuni-0.4.9/tracuni/schema/builtin/tornado/log_out.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/engine/engine.py` & `tracuni-0.4.9/tracuni/schema/engine/engine.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/engine/feed.py` & `tracuni-0.4.9/tracuni/schema/engine/feed.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/engine/pool.py` & `tracuni-0.4.9/tracuni/schema/engine/pool.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/lib/catch_essential.py` & `tracuni-0.4.9/tracuni/schema/lib/catch_essential.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/lib/debug.py` & `tracuni-0.4.9/tracuni/schema/lib/debug.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/lib/make_cut.py` & `tracuni-0.4.9/tracuni/schema/lib/make_cut.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/lib/mask_secret.py` & `tracuni-0.4.9/tracuni/schema/lib/mask_secret.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/lib/pick_items.py` & `tracuni-0.4.9/tracuni/schema/lib/pick_items.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/pipe_methods.py` & `tracuni-0.4.9/tracuni/schema/pipe_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,18 +666,19 @@
 
 def pipe_get_send_request_tornado(point_args):
     url = getattr(point_args, 'url', None)
     parsed_url = urlparse(url)
     url_hostname = parsed_url.hostname
     url_address = ''.join([parsed_url[0], '://', *urlparse(url)[1]])
     url_path = parsed_url[2] or '/'
-    body = getattr(point_args, 'req', None)
+    body_var_a = getattr(point_args, 'req', None)
+    body_var_b = getattr(point_args, 'request_arr', None)
     query = getattr(point_args, 'body', None)
     return {
-        "body": body,
+        "body": body_var_a or body_var_b,
         "query": query,
         "url": url,
         "url_hostname": url_hostname,
         "url_address": url_address,
         "url_path": url_path,
         "method": getattr(point_args, 'method', 'POST'),
         "headers": getattr(point_args, 'headers', None),
```

### Comparing `tracuni-0.4.8/tracuni/schema/shared_rules.py` & `tracuni-0.4.9/tracuni/schema/shared_rules.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/schema/standard.py` & `tracuni-0.4.9/tracuni/schema/standard.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/side_steps/db_logger/logger.py` & `tracuni-0.4.9/tracuni/side_steps/db_logger/logger.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/side_steps/stat/adapter.py` & `tracuni-0.4.9/tracuni/side_steps/stat/adapter.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni/side_steps/stat/send.py` & `tracuni-0.4.9/tracuni/side_steps/stat/send.py`

 * *Files identical despite different names*

### Comparing `tracuni-0.4.8/tracuni.egg-info/PKG-INFO` & `tracuni-0.4.9/tracuni.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tracuni
-Version: 0.4.8
+Version: 0.4.9
 Summary: Convenient library to plug in tracer to incoming and outgoing points and extract data from there
 Home-page: https://github.com/hastly/tracuni
 Author: Konstantin Gonciarou
 Author-email: konstantin.goncharov@inplat.ru
 License: UNKNOWN
 Description: ========
         trac_uni
```

### Comparing `tracuni-0.4.8/tracuni.egg-info/SOURCES.txt` & `tracuni-0.4.9/tracuni.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 tests/define/test_type.py
 tests/fixtures/__init__.py
 tests/fixtures/fixture_engine.py
 tests/fixtures/fixture_engine_schemas.py
 tests/fixtures/fixture_engine_structures.py
 tests/sample/srv_aio_8095.json
 tests/sample/srv_aio_8095/Pipfile
+tests/sample/srv_aio_8095/Pipfile.lock
 tests/sample/srv_aio_8095/main.py
 tests/sample/srv_aio_8095/requirements.txt
 tests/sample/srv_aio_8095/app/__init__.py
 tests/sample/srv_aio_8095/app/app.py
 tests/sample/srv_aio_8095/app/core/__init__.py
 tests/sample/srv_aio_8095/app/core/amqp_server.py
 tests/sample/srv_aio_8095/app/core/app.py
```

