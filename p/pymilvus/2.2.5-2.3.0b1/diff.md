# Comparing `tmp/pymilvus-2.2.5.tar.gz` & `tmp/pymilvus-2.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.2.5.tar", last modified: Tue Apr 11 06:35:53 2023, max compression
+gzip compressed data, was "pymilvus-2.3.0b1.tar", last modified: Mon Mar 20 10:23:59 2023, max compression
```

## Comparing `pymilvus-2.2.5.tar` & `pymilvus-2.3.0b1.tar`

### file list

```diff
@@ -1,166 +1,163 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.112802 pymilvus-2.2.5/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/.github/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      817 2023-04-06 02:38:41.000000 pymilvus-2.2.5/.github/mergify.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/.github/workflows/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      730 2023-04-06 02:38:41.000000 pymilvus-2.2.5/.github/workflows/check_milvus_proto.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      685 2023-04-11 03:16:40.000000 pymilvus-2.2.5/.github/workflows/code_checker.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/workflows/doc_update_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.github/workflows/nightly_ci.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-04-11 03:16:40.000000 pymilvus-2.2.5/.github/workflows/publish_dev_package.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      744 2023-04-06 02:38:41.000000 pymilvus-2.2.5/.github/workflows/pull_request.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2022-11-21 06:54:31.000000 pymilvus-2.2.5/.github/workflows/release_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2022-11-09 07:08:42.000000 pymilvus-2.2.5/.gitignore
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2023-03-28 09:37:32.000000 pymilvus-2.2.5/.gitmodules
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2022-11-09 07:08:42.000000 pymilvus-2.2.5/CONTRIBUTING.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2022-11-09 07:08:42.000000 pymilvus-2.2.5/CONTRIBUTING_CN.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2022-11-09 07:08:42.000000 pymilvus-2.2.5/Dockerfile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2023-04-10 06:47:08.000000 pymilvus-2.2.5/LICENSE
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2022-12-06 08:37:06.000000 pymilvus-2.2.5/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2022-11-09 07:08:42.000000 pymilvus-2.2.5/OWNERS
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-04-11 06:35:53.112802 pymilvus-2.2.5/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-04-06 02:38:41.000000 pymilvus-2.2.5/README.md
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2023-03-28 09:37:32.000000 pymilvus-2.2.5/check_proto_product.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.092803 pymilvus-2.2.5/ci/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.092803 pymilvus-2.2.5/ci/docker/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/ci/docker/milvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2022-11-09 07:08:42.000000 pymilvus-2.2.5/ci/docker/milvus/docker-compose.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/ci/scripts/
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2022-11-09 07:08:42.000000 pymilvus-2.2.5/ci/scripts/docker_image_find_tag.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.096803 pymilvus-2.2.5/docs/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/make.bat
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.100803 pymilvus-2.2.5/docs/source/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.100803 pymilvus-2.2.5/docs/source/_templates/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/_templates/autosummaryclass.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/_templates/layout.html
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/about.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.100803 pymilvus-2.2.5/docs/source/api/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-03-28 09:37:32.000000 pymilvus-2.2.5/docs/source/api/api.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8038 2023-04-06 02:38:41.000000 pymilvus-2.2.5/docs/source/api/collection.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/api/connections.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/api/future.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/api/milvus_index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4010 2023-04-06 02:38:41.000000 pymilvus-2.2.5/docs/source/api/partition.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/api/schema.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/api/search.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2023-03-28 09:37:32.000000 pymilvus-2.2.5/docs/source/api/utility.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/changes.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2023-03-28 09:37:32.000000 pymilvus-2.2.5/docs/source/conf.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/contribute.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/faq.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/install.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/param.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.100803 pymilvus-2.2.5/docs/source/res/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/res/Intro_to_Indexes.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/res/about_documentation.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/results.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2022-11-09 07:08:42.000000 pymilvus-2.2.5/docs/source/tutorial.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.104803 pymilvus-2.2.5/examples/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.104803 pymilvus-2.2.5/examples/cert/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/cert/ca.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/cert/client.key
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/cert/client.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/cert/server.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11523 2023-04-06 02:38:41.000000 pymilvus-2.2.5/examples/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/example_bulkinsert.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/example_tls1.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/example_tls2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/films.csv
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/hello_milvus.ipynb
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/multithreading_hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/old_style_example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/old_style_example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/old_style_example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2022-11-09 07:08:42.000000 pymilvus-2.2.5/examples/old_style_query.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2977 2023-04-06 02:38:41.000000 pymilvus-2.2.5/examples/resource_group.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6680 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/role_and_privilege.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2023-03-28 09:37:32.000000 pymilvus-2.2.5/examples/user.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pylint.conf
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.104803 pymilvus-2.2.5/pymilvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3188 2023-04-03 09:35:35.000000 pymilvus-2.2.5/pymilvus/__init__.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.108802 pymilvus-2.2.5/pymilvus/client/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28616 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/abstract.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10675 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/asynch.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/blob.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11884 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/client/check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      242 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/configs.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      231 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/client/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3144 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/entity_helper.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    59258 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/client/grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/interceptor.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    39574 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/client/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/singleton_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58555 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/client/stub.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2812 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/client/ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19370 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/client/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4563 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/client/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6414 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6265 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/exceptions.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.108802 pymilvus-2.2.5/pymilvus/grpc_gen/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      116 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/grpc_gen/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13533 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/common_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11829 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/common_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    64751 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/milvus_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    81759 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   111564 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1264 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/python_gen.sh
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5774 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/schema_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7923 2023-04-11 03:16:40.000000 pymilvus-2.2.5/pymilvus/grpc_gen/schema_pb2.pyi
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.112802 pymilvus-2.2.5/pymilvus/orm/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2022-11-09 07:08:42.000000 pymilvus-2.2.5/pymilvus/orm/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    50279 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/orm/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14956 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      842 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/default_config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2022-11-09 07:08:42.000000 pymilvus-2.2.5/pymilvus/orm/future.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5680 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/mutation.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    25748 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/orm/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3482 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/orm/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7911 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/role.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14632 2023-04-06 02:38:41.000000 pymilvus-2.2.5/pymilvus/orm/schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7478 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/search.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4318 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/orm/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    45623 2023-03-29 13:13:56.000000 pymilvus-2.2.5/pymilvus/orm/utility.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1926 2023-03-28 09:37:32.000000 pymilvus-2.2.5/pymilvus/settings.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.104803 pymilvus-2.2.5/pymilvus.egg-info/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-04-11 06:35:53.000000 pymilvus-2.2.5/pymilvus.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3721 2023-04-11 06:35:53.000000 pymilvus-2.2.5/pymilvus.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-04-11 06:35:53.000000 pymilvus-2.2.5/pymilvus.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       91 2023-04-11 06:35:53.000000 pymilvus-2.2.5/pymilvus.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-04-11 06:35:53.000000 pymilvus-2.2.5/pymilvus.egg-info/top_level.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.2.5/pyproject.toml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      601 2023-04-11 03:16:40.000000 pymilvus-2.2.5/requirements.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-04-11 06:35:53.112802 pymilvus-2.2.5/setup.cfg
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1110 2023-04-11 03:16:40.000000 pymilvus-2.2.5/setup.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-11 06:35:53.112802 pymilvus-2.2.5/tests/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/conftest.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/mock_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/mock_result.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2022-11-09 07:08:42.000000 pymilvus-2.2.5/tests/pytest.ini
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5828 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13787 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4283 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/test_create_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5529 2023-03-29 13:13:56.000000 pymilvus-2.2.5/tests/test_grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4490 2023-03-28 09:37:32.000000 pymilvus-2.2.5/tests/test_prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6417 2023-04-06 02:38:41.000000 pymilvus-2.2.5/tests/test_schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/test_ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4330 2023-04-11 03:16:40.000000 pymilvus-2.2.5/tests/test_types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-03-17 10:50:05.000000 pymilvus-2.2.5/tests/utils.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      823 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/mergify.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/workflows/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      733 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      596 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/code_checker.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/publish_dev_package.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      747 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/pull_request.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2022-11-21 06:54:31.000000 pymilvus-2.3.0b1/.github/workflows/release_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.gitignore
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/.gitmodules
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING_CN.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/Dockerfile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/LICENSE
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2022-12-06 08:37:06.000000 pymilvus-2.3.0b1/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/OWNERS
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/README.md
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/check_proto_product.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/docker/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/docker/milvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/scripts/
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/docs/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/README.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/make.bat
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/_templates/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/autosummaryclass.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/layout.html
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/about.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/api/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/docs/source/api/api.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8339 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/collection.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/connections.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/future.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/milvus_index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4253 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/partition.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/schema.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/search.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/api/utility.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/changes.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/conf.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/contribute.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/faq.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/install.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/param.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/res/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/about_documentation.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/results.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/tutorial.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/cert/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/ca.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.key
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/server.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11469 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example_bulkinsert.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls1.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/films.csv
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/hello_milvus.ipynb
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-02-20 09:16:24.000000 pymilvus-2.3.0b1/examples/hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_query.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2701 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/resource_group.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6680 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/role_and_privilege.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/user.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pylint.conf
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3188 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/__init__.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/client/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28616 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/pymilvus/client/abstract.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10675 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/asynch.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/blob.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11932 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      242 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/configs.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      200 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/client/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3144 2023-03-17 10:58:42.000000 pymilvus-2.3.0b1/pymilvus/client/entity_helper.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    59059 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/interceptor.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    37767 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/singleton_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58555 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pymilvus/client/stub.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2781 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19426 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/client/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6421 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6414 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6423 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/exceptions.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/grpc_gen/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      116 2023-03-17 10:56:09.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    23471 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/common_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   120931 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   109919 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)      967 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/python_gen.sh
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10854 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/schema_pb2.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/orm/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    52636 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14956 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/orm/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      842 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/default_config.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/future.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5680 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/mutation.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28312 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3691 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7911 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/role.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14893 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7478 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/search.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4318 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    44273 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/utility.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1926 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/settings.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus.egg-info/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3622 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/dependency_links.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      175 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/requires.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/top_level.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pyproject.toml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      617 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/requirements.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/setup.cfg
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1096 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/setup.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/tests/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/conftest.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_result.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/tests/pytest.ini
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5828 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13787 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4283 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_create_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4163 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4490 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5437 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4292 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/utils.py
```

### Comparing `pymilvus-2.2.5/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/.github/mergify.yml` & `pymilvus-2.3.0b1/.github/mergify.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
       label:
         add:
           - ci-passed
   - name: Add needs-dco label when DCO check failed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - -status-success=DCO
     actions:
       label:
         remove:
           - dco-passed
         add:
           - needs-dco
 
   - name: Add dco-passed label when DCO check passed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - status-success=DCO
     actions:
       label:
         remove:
           - needs-dco
         add:
           - dco-passed
```

### Comparing `pymilvus-2.2.5/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Check proto on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
   build:
     name: Run Check Proto
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `pymilvus-2.2.5/.github/workflows/code_checker.yml` & `pymilvus-2.3.0b1/.github/workflows/pull_request.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-name: Code checker on pull request
+name: Test on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  code-lint:
-    name: Code lint check
+  build:
+    name: Run Python Tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
+        python-version: [3.8]
+
     steps:
-      - name: Checkout code
-        uses: actions/checkout@v2
-      - name: Set up python
-        uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: check setup.py install
-        run: |
-          python setup.py install
-      - name: Install requirements
-        run: |
-          pip install -r requirements.txt
-      - name: Run pylint
-        shell: bash
-        run: |
-          make lint
+    - uses: actions/checkout@v2
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Fetch tags
+      run: |
+        git fetch --prune --unshallow --tags
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install pytest
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+
+    - name: Test with pytest
+      run: |
+        make unittest
```

### Comparing `pymilvus-2.2.5/.github/workflows/doc_update_event.yml` & `pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/.github/workflows/nightly_ci.yml` & `pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/.github/workflows/pull_request.yml` & `pymilvus-2.3.0b1/.github/workflows/code_checker.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-name: Test on pull request
+name: Code checker on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  build:
-    name: Run Python Tests
+  code-lint:
+    name: Code lint check
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.8]
-
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Fetch tags
-      run: |
-        git fetch --prune --unshallow --tags
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-
-    - name: Test with pytest
-      run: |
-        make unittest
+      - name: Checkout code
+        uses: actions/checkout@v2
+      - name: Set up python
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install requirements
+        run: |
+          pip install -r requirements.txt
+      - name: Run pylint
+        shell: bash
+        run: |
+          make lint
```

### Comparing `pymilvus-2.2.5/.github/workflows/release_event.yml` & `pymilvus-2.3.0b1/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/CONTRIBUTING.md` & `pymilvus-2.3.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/CONTRIBUTING_CN.md` & `pymilvus-2.3.0b1/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/LICENSE` & `pymilvus-2.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/Makefile` & `pymilvus-2.3.0b1/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/PKG-INFO` & `pymilvus-2.3.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.5
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.5/README.md` & `pymilvus-2.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/check_proto_product.sh` & `pymilvus-2.3.0b1/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/Makefile` & `pymilvus-2.3.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/README.md` & `pymilvus-2.3.0b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/make.bat` & `pymilvus-2.3.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/collection.rst` & `pymilvus-2.3.0b1/docs/source/api/collection.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Collection.insert>`_                     | Insert data into collection.                                             |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Collection.delete>`_                     | Delete entities with an expression condition.                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Collection.search>`_                     | Vector similarity search with an optional boolean expression as filters. |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_                     | Upsert data of collection.                                                                  |
++---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Collection.query>`_                       | Query with a set of criteria.                                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `partition() <#pymilvus.Collection.partition>`_               | Return the partition corresponding to name.                              |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `create_partition() <#pymilvus.Collection.create_partition>`_ | Create the partition for the collection.                                 |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `has_partition() <#pymilvus.Collection.has_partition>`_       | Checks if a specified partition exists.                                  |
```

### Comparing `pymilvus-2.2.5/docs/source/api/connections.rst` & `pymilvus-2.3.0b1/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/future.rst` & `pymilvus-2.3.0b1/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/milvus_index.rst` & `pymilvus-2.3.0b1/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/partition.rst` & `pymilvus-2.3.0b1/docs/source/api/partition.rst`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `release() <#pymilvus.Partition.release>`_ | Release the Partition from memory.                                       |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Partition.insert>`_   | Insert data into partition.                                              |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Partition.delete>`_   | Delete entities with an expression condition.                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_  |Upsert data of collection.                                               |
++--------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Partition.search>`_   | Vector similarity search with an optional boolean expression as filters. |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Partition.query>`_     | Query with a set of criteria.                                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
 
 API Refereences
 ---------------
```

### Comparing `pymilvus-2.2.5/docs/source/api/schema.rst` & `pymilvus-2.3.0b1/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/search.rst` & `pymilvus-2.3.0b1/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/api/utility.rst` & `pymilvus-2.3.0b1/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/conf.py` & `pymilvus-2.3.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/contribute.rst` & `pymilvus-2.3.0b1/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/faq.rst` & `pymilvus-2.3.0b1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/index.rst` & `pymilvus-2.3.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/install.rst` & `pymilvus-2.3.0b1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/res/about_documentation.md` & `pymilvus-2.3.0b1/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/results.rst` & `pymilvus-2.3.0b1/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/docs/source/tutorial.rst` & `pymilvus-2.3.0b1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/cert/ca.pem` & `pymilvus-2.3.0b1/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/cert/client.key` & `pymilvus-2.3.0b1/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/cert/client.pem` & `pymilvus-2.3.0b1/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/cert/server.pem` & `pymilvus-2.3.0b1/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/collection.py` & `pymilvus-2.3.0b1/examples/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,14 @@
 
     print("\nlist collections:")
     print(utility.list_collections())
     assert utility.has_collection(old_collection)
 
     utility.rename_collection(old_collection, new_collection)
     assert utility.has_collection(new_collection)
-    assert not utility.has_collection(old_collection)
 
 
 if __name__ == "__main__":
     print("test collection and get an existing collection")
     name = test_create_collection()
     print("test an existing collection")
     test_exist_collection(name)
```

### Comparing `pymilvus-2.2.5/examples/example.py` & `pymilvus-2.3.0b1/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/example_bulkinsert.py` & `pymilvus-2.3.0b1/examples/example_bulkinsert.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/example_index.py` & `pymilvus-2.3.0b1/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/example_str.py` & `pymilvus-2.3.0b1/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/example_tls1.py` & `pymilvus-2.3.0b1/examples/example_tls1.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/example_tls2.py` & `pymilvus-2.3.0b1/examples/example_tls2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/films.csv` & `pymilvus-2.3.0b1/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/hello_milvus.ipynb` & `pymilvus-2.3.0b1/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/hello_milvus.py` & `pymilvus-2.3.0b1/examples/hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/multithreading_hello_milvus.py` & `pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/old_style_example.py` & `pymilvus-2.3.0b1/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/old_style_example_index.py` & `pymilvus-2.3.0b1/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/old_style_example_str.py` & `pymilvus-2.3.0b1/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/old_style_query.py` & `pymilvus-2.3.0b1/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/partition.py` & `pymilvus-2.3.0b1/examples/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/resource_group.py` & `pymilvus-2.3.0b1/examples/resource_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,22 +49,20 @@
 
 def transfer_replica(source, target, collection_name, num_replica):
     print(
         f"transfer {num_replica} replicas in {collection_name} from {source} to {target}")
     utility.transfer_replica(
         source, target, collection_name, num_replica, using=_CONNECTION_NAME)
     
-
 def run(): 
     create_connection("root", "123456")
     coll = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
     vectors = insert(coll, 10000, _DIM)
     coll.flush()
     create_index(coll, _VECTOR_FIELD_NAME)
-    load_collection(coll)
     
     create_resource_group("rg")
     list_resource_groups()
     describe_resource_group("rg")
     transfer_node(DEFAULT_RESOURCE_GROUP, "rg", 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
@@ -76,20 +74,14 @@
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
    
     drop_resource_group("rg")
     release_collection(coll)
     drop_collection(_COLLECTION_NAME)
 
 if __name__ == "__main__":
```

### Comparing `pymilvus-2.2.5/examples/role_and_privilege.py` & `pymilvus-2.3.0b1/examples/role_and_privilege.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/examples/user.py` & `pymilvus-2.3.0b1/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pylint.conf` & `pymilvus-2.3.0b1/pylint.conf`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/__init__.py` & `pymilvus-2.3.0b1/pymilvus/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/__init__.py` & `pymilvus-2.3.0b1/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/abstract.py` & `pymilvus-2.3.0b1/pymilvus/client/abstract.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/asynch.py` & `pymilvus-2.3.0b1/pymilvus/client/asynch.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/blob.py` & `pymilvus-2.3.0b1/pymilvus/client/blob.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/check.py` & `pymilvus-2.3.0b1/pymilvus/client/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,25 +215,26 @@
     return True
 
 def is_legal_replica_number(replica_number: int) -> bool:
     return isinstance(replica_number, int)
 
 # https://milvus.io/cn/docs/v1.0.0/metric.md#floating
 def is_legal_index_metric_type(index_type: str, metric_type: str) -> bool:
-    if index_type not in ("FLAT",
+    if index_type not in ("GPU_FLAT",
+                          "GPU_IVF_FLAT",
+                          "GPU_IVF_SQ8",
+                          "GPU_IVF_PQ",
+                          "RAFT_IVF_FLAT",
+                          "RAFT_IVF_PQ",
+                          "FLAT",
                           "IVF_FLAT",
                           "IVF_SQ8",
-                          # "IVF_SQ8_HYBRID",
                           "IVF_PQ",
                           "HNSW",
-                          # "NSG",
                           "ANNOY",
-                          "RHNSW_FLAT",
-                          "RHNSW_PQ",
-                          "RHNSW_SQ",
                           "AUTOINDEX",
                           "DISKANN"):
         return False
     if metric_type not in ("L2", "IP"):
         return False
     return True
```

### Comparing `pymilvus-2.2.5/pymilvus/client/entity_helper.py` & `pymilvus-2.3.0b1/pymilvus/client/entity_helper.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/grpc_handler.py` & `pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,40 +349,47 @@
         response = future.result()
         status = response.status
         if status.error_code == 0:
             return response.stats
 
         raise MilvusException(status.error_code, status.reason)
 
-    def _prepare_batch_insert_request(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
-        insert_param = kwargs.get('insert_param', None)
+    def _prepare_batch_insert_or_upsert_request(self, collection_name, entities, partition_name=None, timeout=None, isInsert=True, **kwargs):
+        param = kwargs.get('insert_param', None)
 
-        if insert_param and not isinstance(insert_param, milvus_types.RowBatch):
-            raise ParamError(message="The value of key 'insert_param' is invalid")
+        if not isInsert:
+            param = kwargs.get('upsert_param', None)
+
+        if param and not isinstance(param, milvus_types.RowBatch):
+            if isInsert:
+                raise ParamError(message="The value of key 'insert_param' is invalid")
+            raise ParamError(message="The value of key 'upsert_param' is invalid")
         if not isinstance(entities, list):
             raise ParamError(message="None entities, please provide valid entities.")
 
         collection_schema = kwargs.get("schema", None)
         if not collection_schema:
-            collection_schema = self.describe_collection(collection_name, timeout=timeout, **kwargs)
+            collection_schema = self.describe_collection(
+                collection_name, timeout=timeout, **kwargs)
 
         fields_info = collection_schema["fields"]
 
-        request = insert_param if insert_param \
-            else Prepare.batch_insert_param(collection_name, entities, partition_name, fields_info)
+        request = param if param \
+            else Prepare.batch_insert_or_upsert_param(collection_name, entities, partition_name, fields_info, isInsert)
 
         return request
 
     @retry_on_rpc_failure()
     def batch_insert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
         if not check_invalid_binary_vector(entities):
             raise ParamError(message="Invalid binary vector data exists")
 
         try:
-            request = self._prepare_batch_insert_request(collection_name, entities, partition_name, timeout, **kwargs)
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, **kwargs)
             rf = self._stub.Insert.future(request, timeout=timeout)
             if kwargs.get("_async", False) is True:
                 cb = kwargs.get("_callback", None)
                 f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
                 f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
                 return f
 
@@ -419,14 +426,42 @@
 
             raise MilvusException(response.status.error_code, response.status.reason)
         except Exception as err:
             if kwargs.get("_async", False):
                 return MutationFuture(None, None, err)
             raise err
 
+    @retry_on_rpc_failure()
+    def upsert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
+        if not check_invalid_binary_vector(entities):
+            raise ParamError(message="Invalid binary vector data exists")
+
+        try:
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, False, **kwargs)
+            rf = self._stub.Upsert.future(request, timeout=timeout)
+            if kwargs.get("_async", False) is True:
+                cb = kwargs.get("_callback", None)
+                f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
+                f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
+                return f
+
+            response = rf.result()
+            if response.status.error_code == 0:
+                m = MutationResult(response)
+                ts_utils.update_collection_ts(collection_name, m.timestamp)
+                return m
+
+            raise MilvusException(
+                response.status.error_code, response.status.reason)
+        except Exception as err:
+            if kwargs.get("_async", False):
+                return MutationFuture(None, None, err)
+            raise err
+
     def _execute_search_requests(self, requests, timeout=None, **kwargs):
         auto_id = kwargs.get("auto_id", True)
 
         try:
             if kwargs.get("_async", False):
                 futures = []
                 for request in requests:
@@ -1254,52 +1289,7 @@
 
     @retry_on_rpc_failure()
     def transfer_replica(self, source, target, collection_name, num_replica, timeout=None, **kwargs):
         req = Prepare.transfer_replica(source, target, collection_name, num_replica)
         resp = self._stub.TransferReplica(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
-
-    @retry_on_rpc_failure()
-    def get_flush_all_state(self, flush_all_ts, timeout=None, **kwargs):
-        req = Prepare.get_flush_all_state_request(flush_all_ts)
-        response = self._stub.GetFlushAllState(req, timeout=timeout)
-        status = response.status
-        if status.error_code == 0:
-            return response.flushed
-        raise MilvusException(status.error_code, status.reason)
-
-    def _wait_for_flush_all(self, flush_all_ts, timeout=None, **kwargs):
-        flush_ret = False
-        start = time.time()
-        while not flush_ret:
-            flush_ret = self.get_flush_all_state(flush_all_ts, timeout, **kwargs)
-            end = time.time()
-            if timeout is not None:
-                if end - start > timeout:
-                    raise MilvusException(message=f"wait for flush all timeout, flush_all_ts: {flush_all_ts}")
-
-            if not flush_ret:
-                time.sleep(5)
-
-    @retry_on_rpc_failure()
-    def flush_all(self, timeout=None, **kwargs):
-        request = Prepare.flush_all_request()
-        future = self._stub.FlushAll.future(request, timeout=timeout)
-        response = future.result()
-        if response.status.error_code != 0:
-            raise MilvusException(response.status.error_code, response.status.reason)
-
-        def _check():
-            self._wait_for_flush_all(response.flush_all_ts, timeout, **kwargs)
-
-        if kwargs.get("_async", False):
-            flush_future = FlushFuture(future)
-            flush_future.add_callback(_check)
-
-            user_cb = kwargs.get("_callback", None)
-            if user_cb:
-                flush_future.add_callback(user_cb)
-
-            return flush_future
-
-        _check()
```

### Comparing `pymilvus-2.2.5/pymilvus/client/interceptor.py` & `pymilvus-2.3.0b1/pymilvus/client/interceptor.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/prepare.py` & `pymilvus-2.3.0b1/pymilvus/client/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import ujson
 
 from . import blob
 from . import entity_helper
 from .check import check_pass_param, is_legal_collection_properties
 from .types import DataType, PlaceholderType, get_consistency_level
+from .utils import traverse_info
 from .constants import DEFAULT_CONSISTENCY_LEVEL
 from ..exceptions import ParamError, DataNotMatchException, ExceptionsMessage
 from ..orm.schema import CollectionSchema
 
 from ..grpc_gen import common_pb2 as common_types
 from ..grpc_gen import schema_pb2 as schema_types
 from ..grpc_gen import milvus_pb2 as milvus_types
@@ -243,66 +244,30 @@
             raise ParamError(message="collection_name must be of str type")
         if not isinstance(partition_name, str):
             raise ParamError(message="partition_name must be of str type")
         return milvus_types.PartitionName(collection_name=collection_name,
                                           tag=partition_name)
 
     @classmethod
-    def batch_insert_param(cls, collection_name, entities, partition_name, fields_info=None, **kwargs):
-        # insert_request.hash_keys won't be filled in client. It will be filled in proxy.
+    def batch_insert_or_upsert_param(cls, collection_name, entities, partition_name, fields_info=None, isInsert=True, **kwargs):
+        # insert_request.hash_keys and upsert_request.hash_keys won't be filled in client. It will be filled in proxy.
 
-        tag = partition_name or "_default" # should here?
-        insert_request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
+        tag = partition_name or "_default"  # should here?
+        request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
+
+        if not isInsert:
+            request = milvus_types.UpsertRequest(collection_name=collection_name, partition_name=tag)
 
         for entity in entities:
             if not entity.get("name", None) or not entity.get("values", None) or not entity.get("type", None):
                 raise ParamError(message="Missing param in entities, a field must have type, name and values")
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
-        location, primary_key_loc, auto_id_loc = {}, None, None
-        for i, field in enumerate(fields_info):
-            if field.get("is_primary", False):
-                primary_key_loc = i
-
-            if field.get("auto_id", False):
-                auto_id_loc = i
-                continue
-
-            match_flag = False
-            field_name = field["name"]
-            field_type = field["type"]
-
-            for entity in entities:
-                entity_name, entity_type = entity["name"], entity["type"]
-
-                if field_name == entity_name:
-                    if field_type != entity_type:
-                        raise ParamError(message=f"Collection field type is {field_type}"
-                                         f", but entities field type is {entity_type}")
-
-                    entity_dim, field_dim = 0, 0
-                    if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
-                        field_dim = field["params"]["dim"]
-                        entity_dim = len(entity["values"][0])
-
-                    if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim}")
-
-                    if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim * 8}")
-
-                    location[field["name"]] = i
-                    match_flag = True
-                    break
-
-            if not match_flag:
-                raise ParamError(message=f"Field {field['name']} don't match in entities")
+        location, primary_key_loc, auto_id_loc = traverse_info(fields_info, entities)
 
         # though impossible from sdk
         if primary_key_loc is None:
             raise ParamError(message="primary key not found")
 
         if auto_id_loc is None and len(entities) != len(fields_info):
             raise ParamError(message=f"number of fields: {len(fields_info)}, number of entities: {len(entities)}")
@@ -314,21 +279,21 @@
         try:
             for entity in entities:
                 current = len(entity.get("values"))
                 if row_num not in (0, current):
                     raise ParamError(message="row num misaligned current[{current}]!= previous[{row_num}]")
                 row_num = current
                 field_data = entity_helper.entity_to_field_data(entity, fields_info[location[entity.get("name")]])
-                insert_request.fields_data.append(field_data)
+                request.fields_data.append(field_data)
         except (TypeError, ValueError) as e:
             raise DataNotMatchException(message=ExceptionsMessage.DataTypeInconsistent) from e
 
-        insert_request.num_rows = row_num
+        request.num_rows = row_num
 
-        return insert_request
+        return request
 
     @classmethod
     def delete_request(cls, collection_name, partition_name, expr):
         def check_str(instr, prefix):
             if instr is None:
                 raise ParamError(message=f"{prefix} cannot be None")
             if not isinstance(instr, str):
@@ -855,15 +820,7 @@
     def transfer_replica(cls, source, target, collection_name, num_replica):
         check_pass_param(resource_group_name=source)
         check_pass_param(resource_group_name=target)
         return milvus_types.TransferReplicaRequest(source_resource_group=source,
                                                    target_resource_group=target,
                                                    collection_name=collection_name,
                                                    num_replica=num_replica)
-
-    @classmethod
-    def flush_all_request(cls):
-        return milvus_types.FlushAllRequest()
-
-    @classmethod
-    def get_flush_all_state_request(cls, flush_all_ts):
-        return milvus_types.GetFlushAllStateRequest(flush_all_ts=flush_all_ts)
```

### Comparing `pymilvus-2.2.5/pymilvus/client/stub.py` & `pymilvus-2.3.0b1/pymilvus/client/stub.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/client/ts_utils.py` & `pymilvus-2.3.0b1/pymilvus/client/ts_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import threading
 import datetime
 
 from .singleton_utils import Singleton
 from .utils import hybridts_to_unixtime
 from .constants import EVENTUALLY_TS, BOUNDED_TS
 
-from ..grpc_gen import common_pb2
-
-ConsistencyLevel = common_pb2.ConsistencyLevel
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 
 
 class GTsDict(metaclass=Singleton):
     def __init__(self):
         # collection id -> last write ts
         self._last_write_ts_dict = {}
         self._last_write_ts_dict_lock = threading.Lock()
```

### Comparing `pymilvus-2.2.5/pymilvus/client/types.py` & `pymilvus-2.3.0b1/pymilvus/client/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import time
 from enum import IntEnum
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 from ..grpc_gen import common_pb2
 from ..exceptions import (
     AutoIDException,
     ExceptionsMessage,
     InvalidConsistencyLevel,
 )
 from ..grpc_gen import milvus_pb2 as milvus_types
 
 
-ConsistencyLevel = common_pb2.ConsistencyLevel
-
 class Status:
     """
     :attribute code: int (optional) default as ok
 
     :attribute message: str (optional) current status message
     """
 
@@ -694,20 +693,20 @@
         self._num_available_node = resource_group.num_available_node
         self._num_loaded_replica = resource_group.num_loaded_replica
         self._num_outgoing_node = resource_group.num_outgoing_node
         self._num_incoming_node = resource_group.num_incoming_node
 
     def __repr__(self) -> str:
         s = f"""ResourceGroupInfo:
-<name:{self.name}>,
-<capacity:{self.capacity}>,
-<num_available_node:{self.num_available_node}>,
-<num_loaded_replica:{self.num_loaded_replica}>,
-<num_outgoing_node:{self.num_outgoing_node}>,
-<num_incoming_node:{self.num_incoming_node}>"""
+        <name:{self.name}>, 
+        <capacity:{self.capacity}>, 
+        <num_available_node:{self.num_available_node}>, 
+        <num_loaded_replica:{self.num_loaded_replica}>, 
+        <num_outgoing_node:{self.num_outgoing_node}>, 
+        <num_incoming_node:{self.num_incoming_node}>"""
         return s
 
 
     @property
     def name(self):
         return self._name
```

### Comparing `pymilvus-2.2.5/pymilvus/client/utils.py` & `pymilvus-2.3.0b1/pymilvus/client/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import datetime
 
 from .types import DataType
 from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
-from ..exceptions import MilvusException
+from ..exceptions import ParamError, MilvusException
 
 valid_index_types = [
+    "GPU_FLAT",
+    "GPU_IVF_FLAT",
+    "GPU_IVF_SQ8",
+    "GPU_IVF_PQ",
+    "RAFT_IVF_FLAT",
+    "RAFT_IVF_PQ",
     "FLAT",
     "IVF_FLAT",
     "IVF_SQ8",
-    # "IVF_SQ8_HYBRID",
     "IVF_PQ",
     "HNSW",
-    # "NSG",
     "ANNOY",
-    "RHNSW_FLAT",
-    "RHNSW_PQ",
-    "RHNSW_SQ",
     "BIN_FLAT",
     "BIN_IVF_FLAT",
     "DISKANN",
     "AUTOINDEX"
 ]
 
 valid_index_params_keys = [
@@ -145,7 +146,53 @@
                 raise MilvusException(message=f"Invalid vector length: total_len={total_len}, dim={dim}")
             return int(total_len / dim)
 
         total_len = len(field_data.vectors.binary_vector)
         return int(total_len / (dim / 8))
 
     raise MilvusException(message="Unknown data type")
+
+
+def traverse_info(fields_info, entities):
+    location, primary_key_loc, auto_id_loc = {}, None, None
+    for i, field in enumerate(fields_info):
+        if field.get("is_primary", False):
+            primary_key_loc = i
+
+        if field.get("auto_id", False):
+            auto_id_loc = i
+            continue
+
+        match_flag = False
+        field_name = field["name"]
+        field_type = field["type"]
+
+        for entity in entities:
+            entity_name, entity_type = entity["name"], entity["type"]
+
+            if field_name == entity_name:
+                if field_type != entity_type:
+                    raise ParamError(message=f"Collection field type is {field_type}"
+                                     f", but entities field type is {entity_type}")
+
+                entity_dim, field_dim = 0, 0
+                if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
+                    field_dim = field["params"]["dim"]
+                    entity_dim = len(entity["values"][0])
+
+                if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
+                    raise ParamError(message=f"Collection field dim is {field_dim}"
+                                     f", but entities field dim is {entity_dim}")
+
+                if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
+                    raise ParamError(message=f"Collection field dim is {field_dim}"
+                                     f", but entities field dim is {entity_dim * 8}")
+
+                location[field["name"]] = i
+                match_flag = True
+                break
+
+        if not match_flag:
+            raise ParamError(
+                message=f"Field {field['name']} don't match in entities")
+
+    return location, primary_key_loc, auto_id_loc
```

### Comparing `pymilvus-2.2.5/pymilvus/decorators.py` & `pymilvus-2.3.0b1/pymilvus/decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/exceptions.py` & `pymilvus-2.3.0b1/pymilvus/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,18 @@
     """ Raise when autoID is invalid """
 
 
 class InvalidConsistencyLevel(MilvusException):
     """ Raise when consistency level is invalid """
 
 
+class UpsertAutoIDTrueException(MilvusException):
+    """ Raise when upsert autoID is true """
+
+
 class ExceptionsMessage:
     NoHostPort = "connection configuration must contain 'host' and 'port'."
     HostType = "Type of 'host' must be str."
     PortType = "Type of 'port' must be str or int."
     ConnDiffConf = "Alias of %r already creating connections, but the configure is not the same as passed in."
     AliasType = "Alias should be string, but %r is given."
     ConnLackConf = "You need to pass in the configuration of the connection named %r ."
@@ -161,7 +165,8 @@
     CollectionType = "The type of collection must be pymilvus.Collection."
     FieldsType = "The fields of schema must be type list."
     FieldType = "The field of schema type must be FieldSchema."
     FieldDtype = "Field dtype must be of DataType"
     ExprType = "The type of expr must be string ,but %r is given."
     EnvConfigErr = "Environment variable %s has a wrong format, please check it: %s"
     AmbiguousIndexName = "There are multiple indexes, please specify the index_name."
+    UpsertAutoIDTrue = "Upsert don't support autoid == true"
```

### Comparing `pymilvus-2.2.5/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,19 @@
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Delete',
                 request_serializer=milvus__pb2.DeleteRequest.SerializeToString,
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
+        self.Upsert = channel.unary_unary(
+                '/milvus.proto.milvus.MilvusService/Upsert',
+                request_serializer=milvus__pb2.UpsertRequest.SerializeToString,
+                response_deserializer=milvus__pb2.MutationResult.FromString,
+                )
         self.Search = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Search',
                 request_serializer=milvus__pb2.SearchRequest.SerializeToString,
                 response_deserializer=milvus__pb2.SearchResults.FromString,
                 )
         self.Flush = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Flush',
@@ -171,29 +176,19 @@
                 response_deserializer=milvus__pb2.QueryResults.FromString,
                 )
         self.CalcDistance = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/CalcDistance',
                 request_serializer=milvus__pb2.CalcDistanceRequest.SerializeToString,
                 response_deserializer=milvus__pb2.CalcDistanceResults.FromString,
                 )
-        self.FlushAll = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/FlushAll',
-                request_serializer=milvus__pb2.FlushAllRequest.SerializeToString,
-                response_deserializer=milvus__pb2.FlushAllResponse.FromString,
-                )
         self.GetFlushState = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetFlushState',
                 request_serializer=milvus__pb2.GetFlushStateRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetFlushStateResponse.FromString,
                 )
-        self.GetFlushAllState = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-                request_serializer=milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-                response_deserializer=milvus__pb2.GetFlushAllStateResponse.FromString,
-                )
         self.GetPersistentSegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetPersistentSegmentInfo',
                 request_serializer=milvus__pb2.GetPersistentSegmentInfoRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetPersistentSegmentInfoResponse.FromString,
                 )
         self.GetQuerySegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetQuerySegmentInfo',
@@ -531,56 +526,50 @@
 
     def Delete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Search(self, request, context):
+    def Upsert(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Flush(self, request, context):
+    def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Query(self, request, context):
+    def Flush(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalcDistance(self, request, context):
+    def Query(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FlushAll(self, request, context):
+    def CalcDistance(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFlushState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetFlushAllState(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetPersistentSegmentInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetQuerySegmentInfo(self, request, context):
@@ -925,14 +914,19 @@
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=milvus__pb2.DeleteRequest.FromString,
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
+            'Upsert': grpc.unary_unary_rpc_method_handler(
+                    servicer.Upsert,
+                    request_deserializer=milvus__pb2.UpsertRequest.FromString,
+                    response_serializer=milvus__pb2.MutationResult.SerializeToString,
+            ),
             'Search': grpc.unary_unary_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=milvus__pb2.SearchRequest.FromString,
                     response_serializer=milvus__pb2.SearchResults.SerializeToString,
             ),
             'Flush': grpc.unary_unary_rpc_method_handler(
                     servicer.Flush,
@@ -945,29 +939,19 @@
                     response_serializer=milvus__pb2.QueryResults.SerializeToString,
             ),
             'CalcDistance': grpc.unary_unary_rpc_method_handler(
                     servicer.CalcDistance,
                     request_deserializer=milvus__pb2.CalcDistanceRequest.FromString,
                     response_serializer=milvus__pb2.CalcDistanceResults.SerializeToString,
             ),
-            'FlushAll': grpc.unary_unary_rpc_method_handler(
-                    servicer.FlushAll,
-                    request_deserializer=milvus__pb2.FlushAllRequest.FromString,
-                    response_serializer=milvus__pb2.FlushAllResponse.SerializeToString,
-            ),
             'GetFlushState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFlushState,
                     request_deserializer=milvus__pb2.GetFlushStateRequest.FromString,
                     response_serializer=milvus__pb2.GetFlushStateResponse.SerializeToString,
             ),
-            'GetFlushAllState': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetFlushAllState,
-                    request_deserializer=milvus__pb2.GetFlushAllStateRequest.FromString,
-                    response_serializer=milvus__pb2.GetFlushAllStateResponse.SerializeToString,
-            ),
             'GetPersistentSegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPersistentSegmentInfo,
                     request_deserializer=milvus__pb2.GetPersistentSegmentInfoRequest.FromString,
                     response_serializer=milvus__pb2.GetPersistentSegmentInfoResponse.SerializeToString,
             ),
             'GetQuerySegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetQuerySegmentInfo,
@@ -1617,14 +1601,31 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Delete',
             milvus__pb2.DeleteRequest.SerializeToString,
             milvus__pb2.MutationResult.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def Upsert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Upsert',
+            milvus__pb2.UpsertRequest.SerializeToString,
+            milvus__pb2.MutationResult.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Search(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1685,31 +1686,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/CalcDistance',
             milvus__pb2.CalcDistanceRequest.SerializeToString,
             milvus__pb2.CalcDistanceResults.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FlushAll(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/FlushAll',
-            milvus__pb2.FlushAllRequest.SerializeToString,
-            milvus__pb2.FlushAllResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetFlushState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1719,31 +1703,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushState',
             milvus__pb2.GetFlushStateRequest.SerializeToString,
             milvus__pb2.GetFlushStateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetFlushAllState(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-            milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-            milvus__pb2.GetFlushAllStateResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetPersistentSegmentInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `pymilvus-2.2.5/pymilvus/orm/__init__.py` & `pymilvus-2.3.0b1/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/collection.py` & `pymilvus-2.3.0b1/pymilvus/orm/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 import json
-from typing import List
+from typing import List, Union
 import pandas
 
 from .connections import connections
 from .schema import (
     CollectionSchema,
     FieldSchema,
     parse_fields_from_data,
-    check_insert_data_schema,
+    check_insert_or_upsert_data_schema,
     check_schema,
 )
 from .prepare import Prepare
 from .partition import Partition
 from .index import Index
 from .search import SearchResult
 from .mutation import MutationResult
@@ -384,15 +384,15 @@
             >>> collection.create_index("films", {"index_type": "FLAT", "metric_type": "L2", "params": {}})
             >>> collection.load()
             >>> collection.release()
         """
         conn = self._get_connection()
         conn.release_collection(self._name, timeout=timeout, **kwargs)
 
-    def insert(self, data: [List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
+    def insert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
         """ Insert data into the collection.
 
         Args:
             data (``list/tuple/pandas.DataFrame``): The specified data to insert
             partition_name (``str``): The partition name which the data will be inserted to,
                 if partition name is not passed, then the data will be inserted to "_default" partition
             timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
@@ -419,16 +419,16 @@
             ... ]
             >>> res = collection.insert(data)
             >>> res.insert_count
             10
         """
         if data is None:
             return MutationResult(data)
-        check_insert_data_schema(self._schema, data)
-        entities = Prepare.prepare_insert_data(data, self._schema)
+        check_insert_or_upsert_data_schema(self._schema, data)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema)
 
         conn = self._get_connection()
         res = conn.batch_insert(self._name, entities, partition_name,
                                 timeout=timeout, schema=self._schema_dict, **kwargs)
 
         if kwargs.get("_async", False):
             return MutationFuture(res)
@@ -473,14 +473,60 @@
 
         conn = self._get_connection()
         res = conn.delete(self._name, expr, partition_name, timeout=timeout, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
+    def upsert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
+        """ Upsert data into the collection.
+
+        Args:
+            data (``list/tuple/pandas.DataFrame``): The specified data to upsert
+            partition_name (``str``): The partition name which the data will be upserted at,
+                if partition name is not passed, then the data will be upserted in "_default" partition
+            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
+                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
+        Returns:
+            MutationResult: contains 2 properties `upsert_count`, and, `primary_keys`
+                `upsert_count`: how may entites have been upserted at Milvus,
+                `primary_keys`: list of primary keys of the upserted entities
+        Raises:
+            MilvusException: If anything goes wrong.
+
+        Examples:
+            >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
+            >>> import random
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_collection_upsert", schema)
+            >>> data = [
+            ...     [random.randint(1, 100) for _ in range(10)],
+            ...     [[random.random() for _ in range(2)] for _ in range(10)],
+            ... ]
+            >>> res = collection.upsert(data)
+            >>> res.upsert_count
+            10
+        """
+        if data is None:
+            return MutationResult(data)
+        check_insert_or_upsert_data_schema(self._schema, data, False)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema, False)
+
+        conn = self._get_connection()
+        res = conn.upsert(self._name, entities, partition_name,
+                                timeout=timeout, schema=self._schema_dict, **kwargs)
+
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
     def search(self, data, anns_field, param, limit, expr=None, partition_names=None,
                output_fields=None, timeout=None, round_decimal=-1, **kwargs):
         """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
             data (``List[List[float]]``): The vectors of search data.
                 the length of data is number of query (nq), and the dim of every vector in data must be equal to
```

### Comparing `pymilvus-2.2.5/pymilvus/orm/connections.py` & `pymilvus-2.3.0b1/pymilvus/orm/connections.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/constants.py` & `pymilvus-2.3.0b1/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/default_config.py` & `pymilvus-2.3.0b1/pymilvus/orm/default_config.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/future.py` & `pymilvus-2.3.0b1/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/index.py` & `pymilvus-2.3.0b1/pymilvus/orm/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/mutation.py` & `pymilvus-2.3.0b1/pymilvus/orm/mutation.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/partition.py` & `pymilvus-2.3.0b1/pymilvus/orm/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             >>> partition.num_entities
             10
         """
         conn = self._get_connection()
         if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
             raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
         # TODO: check insert data schema here?
-        entities = Prepare.prepare_insert_data(data, self._collection.schema)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema)
         res = conn.batch_insert(self._collection.name, entities=entities, partition_name=self._name,
             timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
     def delete(self, expr, timeout=None, **kwargs):
@@ -344,14 +344,67 @@
 
         conn = self._get_connection()
         res = conn.delete(self._collection.name, expr, self.name, timeout=timeout, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
+    def upsert(self, data, timeout=None, **kwargs):
+        """
+        Upsert data into partition.
+
+        :param data: The specified data to upsert, the dimension of data needs to align with column
+                     number
+        :type  data: list-like(list, tuple) object or pandas.DataFrame
+
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *timeout* (``float``) --
+              An optional duration of time in seconds to allow for the RPC. When timeout
+              is set to None, client waits until server response or error occur.
+
+        :return: A MutationResult object contains a property named `upsert_count` represents how many
+        entities have been upserted at milvus and a property named `primary_keys` is a list of primary
+        keys of the upserted entities.
+        :rtype: MutationResult
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_upsert", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.upsert(data)
+            >>> partition.num_entities
+            10
+        """
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
+            raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
+        # TODO: check upsert data schema here?
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema,False)
+        res = conn.upsert(self._collection.name, entities=entities, partition_name=self._name,
+            timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
     def search(self, data, anns_field, param, limit,
                expr=None, output_fields=None, timeout=None, round_decimal=-1, **kwargs):
         """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
             data (``List[List[float]]``): The vectors of search data.
                 the length of data is number of query (nq), and the dim of every vector in data must be equal to
```

### Comparing `pymilvus-2.2.5/pymilvus/orm/prepare.py` & `pymilvus-2.3.0b1/pymilvus/orm/prepare.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,36 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 import copy
 
 import numpy
 import pandas
 
-from ..exceptions import DataNotMatchException, DataTypeNotSupportException, ExceptionsMessage
+from ..exceptions import (
+    DataNotMatchException,
+    DataTypeNotSupportException,
+    ExceptionsMessage,
+    UpsertAutoIDTrueException,
+)
 
 
 class Prepare:
     @classmethod
-    def prepare_insert_data(cls, data, schema):
+    def prepare_insert_or_upsert_data(cls, data, schema, isInsert = True):
         if not isinstance(data, (list, tuple, pandas.DataFrame)):
             raise DataTypeNotSupportException(message=ExceptionsMessage.DataTypeNotSupport)
 
         fields = schema.fields
         entities = []  # Entities
         raw_lengths = []  # Check if each row has the same numbers.
 
         if isinstance(data, pandas.DataFrame):
             if schema.auto_id:
+                if isInsert is False:
+                    raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
                 if schema.primary_field.name in data:
                     if len(fields) != len(data.columns):
                         raise DataNotMatchException(message=ExceptionsMessage.FieldsNumInconsistent)
                     if not data[schema.primary_field.name].isnull().all():
                         raise DataNotMatchException(message=ExceptionsMessage.AutoIDWithData)
                 else:
                     if len(fields) != len(data.columns) + 1:
```

### Comparing `pymilvus-2.2.5/pymilvus/orm/role.py` & `pymilvus-2.3.0b1/pymilvus/orm/role.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/schema.py` & `pymilvus-2.3.0b1/pymilvus/orm/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
-from typing import List
+from typing import List, Union
 import pandas
 from pandas.api.types import is_list_like
 
 from .constants import COMMON_TYPE_PARAMS
 from .types import DataType, map_numpy_dtype_to_datatype, infer_dtype_bydata
 from ..exceptions import (
     CannotInferSchemaException,
@@ -23,14 +23,15 @@
     PrimaryKeyException,
     FieldsTypeException,
     FieldTypeException,
     AutoIDException,
     ExceptionsMessage,
     DataNotMatchException,
     SchemaNotReadyException,
+    UpsertAutoIDTrueException
 )
 
 
 class CollectionSchema:
     def __init__(self, fields, description="", **kwargs):
         if not isinstance(fields, list):
             raise FieldsTypeException(message=ExceptionsMessage.FieldsType)
@@ -162,18 +163,18 @@
             "description": self._description,
             "fields": [s.to_dict() for s in self._fields],
         }
         return _dict
 
 
 class FieldSchema:
-    def __init__(self, name: str, dtype: DataType, description="", **kwargs):
+    def __init__(self, name, dtype, description="", **kwargs):
         self.name = name
         try:
-            dtype = DataType(dtype)
+            DataType(dtype)
         except ValueError:
             raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype) from None
         if dtype == DataType.UNKNOWN:
             raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype)
         self._dtype = dtype
         self._description = description
         self._type_params = {}
@@ -281,38 +282,41 @@
         >>> fvec_field = FieldSchema("fvec", DataType.FLOAT_VECTOR, is_primary=False, dim=128)
         >>> fvec_field.params
         {'dim': 128}
         """
         return self._type_params
 
     @property
-    def dtype(self) -> DataType:
+    def dtype(self):
         return self._dtype
 
 
-def check_insert_data_schema(schema: CollectionSchema, data: [List[List], pandas.DataFrame]) -> None:
-    """ check if the insert data is consist with the collection schema
+def check_insert_or_upsert_data_schema(schema: CollectionSchema, data: Union[List[List], pandas.DataFrame], isInsert=True) -> None:
+    """ check if the insert or upsert data is consist with the collection schema
 
     Args:
         schema (CollectionSchema): the schema of the collection
-        data (List[List], pandas.DataFrame): the data to be inserted
+        data (List[List], pandas.DataFrame): the data to be inserted or upserted
 
     Raise:
         SchemaNotReadyException: if the schema is None
+        UpsertAutoIDTrueException: if autoid option is true
         DataNotMatchException: if the data is in consist with the schema
     """
     if schema is None:
         raise SchemaNotReadyException(message="Schema shouldn't be None")
     if schema.auto_id:
-        if isinstance(data, pandas.DataFrame):
-            if schema.primary_field.name in data:
-                if not data[schema.primary_field.name].isnull().all():
-                    raise DataNotMatchException(message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
-                data = data.drop(schema.primary_field.name, axis=1)
-
+        if isInsert:
+            if isinstance(data, pandas.DataFrame):
+                if schema.primary_field.name in data:
+                    if not data[schema.primary_field.name].isnull().all():
+                        raise DataNotMatchException(message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
+                    data = data.drop(schema.primary_field.name, axis=1)
+        else:
+            raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
     infer_fields = parse_fields_from_data(data)
     tmp_fields = copy.deepcopy(schema.fields)
 
     for i, field in enumerate(schema.fields):
         if field.is_primary and field.auto_id:
             tmp_fields.pop(i)
 
@@ -325,15 +329,15 @@
     for x, y in zip(infer_fields, tmp_fields):
         if x.dtype != y.dtype:
             raise DataNotMatchException(message=f"The data type of field {y.name} doesn't match, expected: {y.dtype.name}, got {x.dtype.name}")
         if isinstance(data, pandas.DataFrame) and x.name != y.name:
             raise DataNotMatchException(message=f"The name of field don't match, expected: {y.name}, got {x.name}")
 
 
-def parse_fields_from_data(data: [List[List], pandas.DataFrame]) -> List[FieldSchema]:
+def parse_fields_from_data(data: Union[List[List], pandas.DataFrame]) -> List[FieldSchema]:
     if not isinstance(data, (pandas.DataFrame, list)):
         raise DataTypeNotSupportException(message="The type of data should be list or pandas.DataFrame")
 
     if isinstance(data, pandas.DataFrame):
         return parse_fields_from_dataframe(data)
 
     for d in data:
```

### Comparing `pymilvus-2.2.5/pymilvus/orm/search.py` & `pymilvus-2.3.0b1/pymilvus/orm/search.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/types.py` & `pymilvus-2.3.0b1/pymilvus/orm/types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus/orm/utility.py` & `pymilvus-2.3.0b1/pymilvus/orm/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1032,35 +1032,7 @@
 
     :example:
         >>> from pymilvus import connections, utility
         >>> connections.connect()
         >>> rgs = utility.transfer_replica(source, target, collection_name, num_replica)
     """
     return _get_connection(using).transfer_replica(source_group, target_group, collection_name, num_replicas, timeout)
-
-def flush_all(using="default", timeout=None, **kwargs):
-    """ Flush all collections. All insertions, deletions, and upserts before `flush_all` will be synced.
-
-    Args:
-        timeout (float): an optional duration of time in seconds to allow for the RPCs.
-            If timeout is not set, the client keeps waiting until the server responds or an error occurs.
-            **kwargs (``dict``, optional):
-
-        * *_async*(``bool``)
-            Indicate if invoke asynchronously. Default `False`.
-
-    Examples:
-        >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType, utility
-        >>> connections.connect()
-        >>> fields = [
-        ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
-        ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=128)
-        ... ]
-        >>> schema = CollectionSchema(fields=fields)
-        >>> collection = Collection(name="test_collection_flush", schema=schema)
-        >>> collection.insert([[1, 2], [[1.0, 2.0], [3.0, 4.0]]])
-        >>> utility.flush_all(_async=False) # synchronized flush_all
-        >>> # or use `future` to flush_all asynchronously
-        >>> future = utility.flush_all(_async=True)
-        >>> future.done() # flush_all finished
-    """
-    return _get_connection(using).flush_all(timeout=timeout, **kwargs)
```

### Comparing `pymilvus-2.2.5/pymilvus/settings.py` & `pymilvus-2.3.0b1/pymilvus/settings.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.5
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.5/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -98,21 +98,18 @@
 pymilvus/client/singleton_utils.py
 pymilvus/client/stub.py
 pymilvus/client/ts_utils.py
 pymilvus/client/types.py
 pymilvus/client/utils.py
 pymilvus/grpc_gen/__init__.py
 pymilvus/grpc_gen/common_pb2.py
-pymilvus/grpc_gen/common_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2.py
-pymilvus/grpc_gen/milvus_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2_grpc.py
 pymilvus/grpc_gen/python_gen.sh
 pymilvus/grpc_gen/schema_pb2.py
-pymilvus/grpc_gen/schema_pb2.pyi
 pymilvus/orm/__init__.py
 pymilvus/orm/collection.py
 pymilvus/orm/connections.py
 pymilvus/orm/constants.py
 pymilvus/orm/default_config.py
 pymilvus/orm/future.py
 pymilvus/orm/index.py
```

### Comparing `pymilvus-2.2.5/requirements.txt` & `pymilvus-2.3.0b1/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 build==0.4.0
-certifi==2021.5.30
+certifi==2022.12.7
 chardet==4.0.0
-grpcio==1.53.0
-grpcio-testing==1.53.0
-grpcio-tools==1.53.0
+grpcio==1.47.0
+grpcio-testing==1.47.0
+grpcio-tools==1.47.0
 protobuf>=3.17.1
 idna==2.10
-mmh3>=2.0
+mmh3>=2.0,<=3.0.0
 packaging==20.9
 pep517==0.10.0
 pyparsing==2.4.7
 six==1.16.0
 toml==0.10.2
-ujson>=2.0.0
+ujson>=2.0.0,<=5.4.0
 urllib3==1.26.5
 sklearn==0.0
 m2r==0.3.1
 Sphinx==4.0.0
 sphinx-copybutton
 sphinx-rtd-theme
 sphinxcontrib-applehelp
```

### Comparing `pymilvus-2.2.5/setup.py` & `pymilvus-2.3.0b1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,22 @@
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/milvus-io/pymilvus',
     license="Apache-2.0",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
-        "grpcio>=1.49.1,<=1.53.0",
-        "grpcio-tools>=1.49.1,<=1.53.0",
-        "mmh3>=2.0",
-        "ujson>=2.0.0",
-        "pandas>=1.2.4",
+        "grpcio>=1.47.0,<=1.48.0",
+        "grpcio-tools>=1.47.0, <=1.48.0",
+        "ujson>=2.0.0,<=5.4.0",
+        "mmh3>=2.0,<=3.0.0",
+        "pandas==1.1.5; python_version<'3.7'",
+        "pandas>=1.2.4; python_version>'3.6'",
     ],
     classifiers=[
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
 
-    python_requires='>=3.7'
+    python_requires='>=3.6'
 )
```

### Comparing `pymilvus-2.2.5/tests/conftest.py` & `pymilvus-2.3.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/mock_milvus.py` & `pymilvus-2.3.0b1/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/mock_result.py` & `pymilvus-2.3.0b1/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_check.py` & `pymilvus-2.3.0b1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_collection.py` & `pymilvus-2.3.0b1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_connections.py` & `pymilvus-2.3.0b1/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_create_collection.py` & `pymilvus-2.3.0b1/tests/test_create_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_decorators.py` & `pymilvus-2.3.0b1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_grpc_handler.py` & `pymilvus-2.3.0b1/tests/test_grpc_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,44 +106,7 @@
             status=common_pb2.Status(error_code=common_pb2.Success),
             version=version,
         )
         rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
 
         got_result = get_version_future.result()
         assert got_result == version
-
-    @pytest.mark.parametrize("_async", [True])
-    def test_flush_all(self, channel, client_thread, _async):
-        handler = GrpcHandler(channel=channel)
-
-        flush_all_future = client_thread.submit(
-            handler.flush_all, _async=_async, timeout=10)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['FlushAll']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.FlushAllResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flush_all_ts=100,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flush_all_future is not None
-
-    def test_get_flush_all_state(self, channel, client_thread):
-        handler = GrpcHandler(channel=channel)
-
-        flushed = client_thread.submit(
-            handler.get_flush_all_state, flush_all_ts=100)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['GetFlushAllState']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.GetFlushStateResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flushed=True,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flushed.result() is True
```

### Comparing `pymilvus-2.2.5/tests/test_index.py` & `pymilvus-2.3.0b1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_partition.py` & `pymilvus-2.3.0b1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_prepare.py` & `pymilvus-2.3.0b1/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_schema.py` & `pymilvus-2.3.0b1/tests/test_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy
 import pytest
 
-from pymilvus import CollectionSchema, FieldSchema, DataType, MilvusException
+from pymilvus import CollectionSchema, FieldSchema, DataType
 from utils import *
-from pymilvus.orm import schema as s
 
 
 class TestCollectionSchema:
     @pytest.fixture(scope="function")
     def raw_dict(self):
         _dict = {}
         _dict["description"] = "TestCollectionSchema_description"
@@ -140,27 +139,7 @@
 
     #  def test_parse_fields_from_dataframe(self, dataframe1):
     #      fields = parse_fields_from_dataframe(dataframe1)
     #      assert len(fields) == len(dataframe1.columns)
     #      for f in fields:
     #          if f.dtype == DataType.FLOAT_VECTOR:
     #              assert f.dim == len(dataframe1['float_vec'].values[0])
-
-class TestCheckInsertDataSchema:
-    def test_check_insert_data_schema_issue1324(self):
-        schema = CollectionSchema([
-            FieldSchema(name="id", dtype=DataType.INT64, descrition="int64", is_primary=True, auto_id=True),
-            FieldSchema(name="embedding", dtype=DataType.FLOAT_VECTOR, descrition="float vector", dim=2),
-            FieldSchema(name="work_id2", dtype=5, descrition="work id"),
-            FieldSchema(name='path', dtype=DataType.VARCHAR, description='path to image', max_length=200),
-            FieldSchema(name="uid", dtype=DataType.INT64, descrition="user id"),
-        ])
-
-        data = [
-            [[0.003984056, 0.05035976]],
-            ['15755403'],
-            ['https://xxx.com/app/works/105149/2023-01-11/w_63be653c4643b/963be653c8aa8c.jpg'],
-            ['105149'],
-        ]
-
-        with pytest.raises(MilvusException):
-            s.check_insert_data_schema(schema, data)
```

### Comparing `pymilvus-2.2.5/tests/test_ts_utils.py` & `pymilvus-2.3.0b1/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.5/tests/test_types.py` & `pymilvus-2.3.0b1/tests/test_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under the License.
 
 from pymilvus import DataType, DEFAULT_RESOURCE_GROUP
 from pymilvus.exceptions import InvalidConsistencyLevel
 from pymilvus.client.types import (
-    get_consistency_level, Shard, Group, Replica, ConsistencyLevel
+    get_consistency_level, ConsistencyLevel,
+    Shard, Group, Replica
 )
 
-from pymilvus.grpc_gen import common_pb2
-
 import pytest
 import pandas as pd
 import numpy as np
 
 
 @pytest.mark.xfail
 class TestTypes:
```

### Comparing `pymilvus-2.2.5/tests/utils.py` & `pymilvus-2.3.0b1/tests/utils.py`

 * *Files identical despite different names*

