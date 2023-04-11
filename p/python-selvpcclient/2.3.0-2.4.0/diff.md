# Comparing `tmp/python-selvpcclient-2.3.0.tar.gz` & `tmp/python-selvpcclient-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selvpcclient-2.3.0.tar", last modified: Tue Apr 11 13:41:04 2023, max compression
+gzip compressed data, was "python-selvpcclient-2.4.0.tar", last modified: Tue Apr 11 13:41:40 2023, max compression
```

## Comparing `python-selvpcclient-2.3.0.tar` & `python-selvpcclient-2.4.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.686641 python-selvpcclient-2.3.0/
--rw-r--r--   0 vitaliy    (501) staff       (20)      185 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/.flake8
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.605704 python-selvpcclient-2.3.0/.github/
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.613395 python-selvpcclient-2.3.0/.github/workflows/
--rw-r--r--   0 vitaliy    (501) staff       (20)      549 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/.github/workflows/checks.yml
--rw-r--r--   0 vitaliy    (501) staff       (20)      549 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/LICENSE
--rw-r--r--   0 vitaliy    (501) staff       (20)     1566 2023-04-11 13:41:04.686832 python-selvpcclient-2.3.0/PKG-INFO
--rw-r--r--   0 vitaliy    (501) staff       (20)      835 2023-04-11 13:40:43.000000 python-selvpcclient-2.3.0/README.md
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.616410 python-selvpcclient-2.3.0/docs/
--rw-r--r--   0 vitaliy    (501) staff       (20)        9 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/.gitignore
--rw-r--r--   0 vitaliy    (501) staff       (20)     7851 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/Makefile
--rw-r--r--   0 vitaliy    (501) staff       (20)     9419 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/conf.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.617379 python-selvpcclient-2.3.0/docs/devref/
--rw-r--r--   0 vitaliy    (501) staff       (20)     4944 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/devref/cli_option_guideline.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)      811 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/devref/client_command_extensions.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)      700 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/index.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)     7208 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/make.bat
--rw-r--r--   0 vitaliy    (501) staff       (20)       52 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/docs/requirements.txt
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.619039 python-selvpcclient-2.3.0/docs/usage/
--rw-r--r--   0 vitaliy    (501) staff       (20)     4079 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/docs/usage/cli.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)     5413 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/docs/usage/commands.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)     4457 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/docs/usage/library.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)      635 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/docs/usage/man.rst
--rw-r--r--   0 vitaliy    (501) staff       (20)      208 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/env.example.bat
--rw-r--r--   0 vitaliy    (501) staff       (20)      238 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/env.example.sh
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.606619 python-selvpcclient-2.3.0/examples/
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.619494 python-selvpcclient-2.3.0/examples/first_project/
--rw-r--r--   0 vitaliy    (501) staff       (20)     2116 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/examples/first_project/main.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.621772 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/
--rw-r--r--   0 vitaliy    (501) staff       (20)     1566 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/PKG-INFO
--rw-r--r--   0 vitaliy    (501) staff       (20)     2869 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 vitaliy    (501) staff       (20)        1 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 vitaliy    (501) staff       (20)       51 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/entry_points.txt
--rw-r--r--   0 vitaliy    (501) staff       (20)        1 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/not-zip-safe
--rw-r--r--   0 vitaliy    (501) staff       (20)       47 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/pbr.json
--rw-r--r--   0 vitaliy    (501) staff       (20)       84 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/requires.txt
--rw-r--r--   0 vitaliy    (501) staff       (20)       19 2023-04-11 13:41:04.000000 python-selvpcclient-2.3.0/python_selvpcclient.egg-info/top_level.txt
--rw-r--r--   0 vitaliy    (501) staff       (20)       84 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/requirements.txt
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.625056 python-selvpcclient-2.3.0/selvpcclient/
--rw-r--r--   0 vitaliy    (501) staff       (20)       20 2023-04-11 12:55:46.000000 python-selvpcclient-2.3.0/selvpcclient/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)    10075 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/selvpcclient/base.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2854 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/client.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.633268 python-selvpcclient-2.3.0/selvpcclient/commands/
--rw-r--r--   0 vitaliy    (501) staff       (20)     1950 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/commands/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2823 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/capabilities.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3223 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/customization.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4123 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/floatingips.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4481 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/commands/keypair.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4183 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/license.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1192 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/commands/limit.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     6790 2023-04-11 12:55:46.000000 python-selvpcclient-2.3.0/selvpcclient/commands/project.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3612 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/commands/quotas.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3594 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/role.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4404 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/subnet.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1782 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/token.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4422 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/user.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     5047 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/commands/vrrp.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.634591 python-selvpcclient-2.3.0/selvpcclient/exceptions/
--rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/exceptions/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      464 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/exceptions/base.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     7851 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/selvpcclient/exceptions/http.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1494 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/formatters.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     6514 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/httpclient.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.639916 python-selvpcclient-2.3.0/selvpcclient/resources/
--rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      632 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/capabilities.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2611 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/customization.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3329 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/floatingips.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2724 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/resources/keypairs.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3476 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/licenses.py
--rw-r--r--   0 vitaliy    (501) staff       (20)    13477 2023-04-11 12:55:46.000000 python-selvpcclient-2.3.0/selvpcclient/resources/projects.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4391 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/selvpcclient/resources/quotas.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3358 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/roles.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3186 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/subnets.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1667 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/tokens.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     6740 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/users.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3363 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/selvpcclient/resources/vrrp.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3363 2023-02-22 13:04:39.000000 python-selvpcclient-2.3.0/selvpcclient/shell.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     9430 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/selvpcclient/util.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      930 2023-04-11 13:41:04.687662 python-selvpcclient-2.3.0/setup.cfg
--rwxr-xr-x   0 vitaliy    (501) staff       (20)      171 2023-04-11 13:14:16.000000 python-selvpcclient-2.3.0/setup.py
--rw-r--r--   0 vitaliy    (501) staff       (20)       58 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/test-requirements.txt
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.640513 python-selvpcclient-2.3.0/tests/
--rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/__init__.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.676620 python-selvpcclient-2.3.0/tests/cli/
--rw-r--r--   0 vitaliy    (501) staff       (20)     1263 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/tests/cli/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      203 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/tests/cli/conftest.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1649 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_capabilities.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2576 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_customization.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3096 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_floatingip.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1571 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/cli/test_keypairs.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3290 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_license.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      355 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/cli/test_limit.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4051 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/cli/test_project.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1170 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/cli/test_quota.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1898 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_role.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3311 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_subnet.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1215 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_token.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2755 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_user.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2010 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/cli/test_vrrp.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.683942 python-selvpcclient-2.3.0/tests/rest/
--rw-r--r--   0 vitaliy    (501) staff       (20)      566 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/tests/rest/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      121 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/tests/rest/conftest.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      695 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_capabilities.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      471 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_customization.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3488 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_floatingips.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2522 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_keypairs.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3349 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_licenses.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     8761 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/rest/test_projects.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4628 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/rest/test_quotas.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2870 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_roles.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     3248 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_subnets.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      908 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_tokens.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     5300 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_users.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     2728 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/rest/test_vrrp.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     4956 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/test_util.py
-drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:04.686278 python-selvpcclient-2.3.0/tests/util/
--rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/util/__init__.py
--rw-r--r--   0 vitaliy    (501) staff       (20)    27904 2023-02-01 13:21:24.000000 python-selvpcclient-2.3.0/tests/util/answers.py
--rw-r--r--   0 vitaliy    (501) staff       (20)     1418 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/util/logo.jpg
--rw-r--r--   0 vitaliy    (501) staff       (20)     1761 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/util/params.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      515 2022-11-07 12:40:07.000000 python-selvpcclient-2.3.0/tests/util/temp_files.py
--rw-r--r--   0 vitaliy    (501) staff       (20)      180 2023-04-11 12:55:41.000000 python-selvpcclient-2.3.0/tox.ini
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.329677 python-selvpcclient-2.4.0/
+-rw-r--r--   0 vitaliy    (501) staff       (20)      185 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/.flake8
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.294460 python-selvpcclient-2.4.0/.github/
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.300160 python-selvpcclient-2.4.0/.github/workflows/
+-rw-r--r--   0 vitaliy    (501) staff       (20)      549 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/.github/workflows/checks.yml
+-rw-r--r--   0 vitaliy    (501) staff       (20)      549 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/LICENSE
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1464 2023-04-11 13:41:40.329863 python-selvpcclient-2.4.0/PKG-INFO
+-rw-r--r--   0 vitaliy    (501) staff       (20)      694 2023-04-11 13:41:25.000000 python-selvpcclient-2.4.0/README.md
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.301807 python-selvpcclient-2.4.0/docs/
+-rw-r--r--   0 vitaliy    (501) staff       (20)        9 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/.gitignore
+-rw-r--r--   0 vitaliy    (501) staff       (20)     7851 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/Makefile
+-rw-r--r--   0 vitaliy    (501) staff       (20)     9419 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/conf.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.302354 python-selvpcclient-2.4.0/docs/devref/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4944 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/devref/cli_option_guideline.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)      811 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/devref/client_command_extensions.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)      700 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/index.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)     7208 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/make.bat
+-rw-r--r--   0 vitaliy    (501) staff       (20)       52 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/docs/requirements.txt
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.303660 python-selvpcclient-2.4.0/docs/usage/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4079 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/docs/usage/cli.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)     5413 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/docs/usage/commands.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4457 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/docs/usage/library.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)      635 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/docs/usage/man.rst
+-rw-r--r--   0 vitaliy    (501) staff       (20)      208 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/env.example.bat
+-rw-r--r--   0 vitaliy    (501) staff       (20)      238 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/env.example.sh
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.295182 python-selvpcclient-2.4.0/examples/
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.304110 python-selvpcclient-2.4.0/examples/first_project/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2116 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/examples/first_project/main.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.307370 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1464 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2869 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaliy    (501) staff       (20)        1 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaliy    (501) staff       (20)       51 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 vitaliy    (501) staff       (20)        1 2023-04-11 13:41:04.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/not-zip-safe
+-rw-r--r--   0 vitaliy    (501) staff       (20)       46 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/pbr.json
+-rw-r--r--   0 vitaliy    (501) staff       (20)       84 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/requires.txt
+-rw-r--r--   0 vitaliy    (501) staff       (20)       19 2023-04-11 13:41:40.000000 python-selvpcclient-2.4.0/python_selvpcclient.egg-info/top_level.txt
+-rw-r--r--   0 vitaliy    (501) staff       (20)       84 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/requirements.txt
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.309513 python-selvpcclient-2.4.0/selvpcclient/
+-rw-r--r--   0 vitaliy    (501) staff       (20)       20 2023-04-11 12:55:46.000000 python-selvpcclient-2.4.0/selvpcclient/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)    10075 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/selvpcclient/base.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2854 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/client.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.314456 python-selvpcclient-2.4.0/selvpcclient/commands/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1950 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/commands/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2823 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/capabilities.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3223 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/customization.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4123 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/floatingips.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4481 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/commands/keypair.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4183 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/license.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1192 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/commands/limit.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     6790 2023-04-11 12:55:46.000000 python-selvpcclient-2.4.0/selvpcclient/commands/project.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3612 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/commands/quotas.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3594 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/role.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4404 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/subnet.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1782 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/token.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4422 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/user.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     5047 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/commands/vrrp.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.315261 python-selvpcclient-2.4.0/selvpcclient/exceptions/
+-rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/exceptions/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      464 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/exceptions/base.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     7851 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/selvpcclient/exceptions/http.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1494 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/formatters.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     6514 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/httpclient.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.318825 python-selvpcclient-2.4.0/selvpcclient/resources/
+-rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      632 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/capabilities.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2611 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/customization.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3329 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/floatingips.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2724 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/resources/keypairs.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3476 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/licenses.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)    13477 2023-04-11 12:55:46.000000 python-selvpcclient-2.4.0/selvpcclient/resources/projects.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4391 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/selvpcclient/resources/quotas.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3358 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/roles.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3186 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/subnets.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1667 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/tokens.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     6740 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/users.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3363 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/selvpcclient/resources/vrrp.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3363 2023-02-22 13:04:39.000000 python-selvpcclient-2.4.0/selvpcclient/shell.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     9430 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/selvpcclient/util.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      982 2023-04-11 13:41:40.330656 python-selvpcclient-2.4.0/setup.cfg
+-rwxr-xr-x   0 vitaliy    (501) staff       (20)      171 2023-04-11 13:14:16.000000 python-selvpcclient-2.4.0/setup.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)       58 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/test-requirements.txt
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.319312 python-selvpcclient-2.4.0/tests/
+-rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/__init__.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.323421 python-selvpcclient-2.4.0/tests/cli/
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1263 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/tests/cli/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      203 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/tests/cli/conftest.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1649 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_capabilities.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2576 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_customization.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3096 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_floatingip.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1571 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/cli/test_keypairs.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3290 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_license.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      355 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/cli/test_limit.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4051 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/cli/test_project.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1170 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/cli/test_quota.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1898 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_role.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3311 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_subnet.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1215 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_token.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2755 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_user.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2010 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/cli/test_vrrp.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.327831 python-selvpcclient-2.4.0/tests/rest/
+-rw-r--r--   0 vitaliy    (501) staff       (20)      566 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/tests/rest/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      121 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/tests/rest/conftest.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      695 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_capabilities.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      471 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_customization.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3488 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_floatingips.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2522 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_keypairs.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3349 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_licenses.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     8761 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/rest/test_projects.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4628 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/rest/test_quotas.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2870 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_roles.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     3248 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_subnets.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      908 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_tokens.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     5300 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_users.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     2728 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/rest/test_vrrp.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     4956 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/test_util.py
+drwxr-xr-x   0 vitaliy    (501) staff       (20)        0 2023-04-11 13:41:40.329375 python-selvpcclient-2.4.0/tests/util/
+-rw-r--r--   0 vitaliy    (501) staff       (20)        0 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/util/__init__.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)    27904 2023-02-01 13:21:24.000000 python-selvpcclient-2.4.0/tests/util/answers.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1418 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/util/logo.jpg
+-rw-r--r--   0 vitaliy    (501) staff       (20)     1761 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/util/params.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      515 2022-11-07 12:40:07.000000 python-selvpcclient-2.4.0/tests/util/temp_files.py
+-rw-r--r--   0 vitaliy    (501) staff       (20)      180 2023-04-11 12:55:41.000000 python-selvpcclient-2.4.0/tox.ini
```

### Comparing `python-selvpcclient-2.3.0/.github/workflows/checks.yml` & `python-selvpcclient-2.4.0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/LICENSE` & `python-selvpcclient-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/PKG-INFO` & `python-selvpcclient-2.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: python-selvpcclient
-Version: 2.3.0
+Version: 2.4.0
 Summary: Client for the Selectel Virtual Private Cloud API.
 Home-page: https://github.com/selectel/python-selvpcclient
 Author: Selectel
 Author-email: m.kalinin@selectel.ru
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-selvpcclient
 
-[![Build Status](https://travis-ci.org/selectel/python-selvpcclient.svg?branch=master)](https://travis-ci.org/selectel/python-selvpcclient)
-
 This is a client for the Selectel VPC API. There is a Python API
 (the selvpcclient module), and command-line script (installed as **selvpc**).
 
 ## Overview
 
 - [Selectel VPC REST API documentation](https://developers.selectel.ru/docs/selectel-cloud-platform/main-services/selectel_cloud_management_api/)
 - [PyPi](https://pypi.org/project/python-selvpcclient)
@@ -36,8 +35,7 @@
 
         pip install -U python-selvpcclient
 
 License
 -------
 
 Apache 2.0
-
```

### Comparing `python-selvpcclient-2.3.0/README.md` & `python-selvpcclient-2.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # python-selvpcclient
 
-[![Build Status](https://travis-ci.org/selectel/python-selvpcclient.svg?branch=master)](https://travis-ci.org/selectel/python-selvpcclient)
-
 This is a client for the Selectel VPC API. There is a Python API
 (the selvpcclient module), and command-line script (installed as **selvpc**).
 
 ## Overview
 
 - [Selectel VPC REST API documentation](https://developers.selectel.ru/docs/selectel-cloud-platform/main-services/selectel_cloud_management_api/)
 - [PyPi](https://pypi.org/project/python-selvpcclient)
```

### Comparing `python-selvpcclient-2.3.0/docs/Makefile` & `python-selvpcclient-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/conf.py` & `python-selvpcclient-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/devref/cli_option_guideline.rst` & `python-selvpcclient-2.4.0/docs/devref/cli_option_guideline.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/devref/client_command_extensions.rst` & `python-selvpcclient-2.4.0/docs/devref/client_command_extensions.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/index.rst` & `python-selvpcclient-2.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/make.bat` & `python-selvpcclient-2.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/usage/cli.rst` & `python-selvpcclient-2.4.0/docs/usage/cli.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/usage/commands.rst` & `python-selvpcclient-2.4.0/docs/usage/commands.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/usage/library.rst` & `python-selvpcclient-2.4.0/docs/usage/library.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/docs/usage/man.rst` & `python-selvpcclient-2.4.0/docs/usage/man.rst`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/examples/first_project/main.py` & `python-selvpcclient-2.4.0/examples/first_project/main.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/python_selvpcclient.egg-info/PKG-INFO` & `python-selvpcclient-2.4.0/python_selvpcclient.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: python-selvpcclient
-Version: 2.3.0
+Version: 2.4.0
 Summary: Client for the Selectel Virtual Private Cloud API.
 Home-page: https://github.com/selectel/python-selvpcclient
 Author: Selectel
 Author-email: m.kalinin@selectel.ru
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-selvpcclient
 
-[![Build Status](https://travis-ci.org/selectel/python-selvpcclient.svg?branch=master)](https://travis-ci.org/selectel/python-selvpcclient)
-
 This is a client for the Selectel VPC API. There is a Python API
 (the selvpcclient module), and command-line script (installed as **selvpc**).
 
 ## Overview
 
 - [Selectel VPC REST API documentation](https://developers.selectel.ru/docs/selectel-cloud-platform/main-services/selectel_cloud_management_api/)
 - [PyPi](https://pypi.org/project/python-selvpcclient)
@@ -36,8 +35,7 @@
 
         pip install -U python-selvpcclient
 
 License
 -------
 
 Apache 2.0
-
```

### Comparing `python-selvpcclient-2.3.0/python_selvpcclient.egg-info/SOURCES.txt` & `python-selvpcclient-2.4.0/python_selvpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/base.py` & `python-selvpcclient-2.4.0/selvpcclient/base.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/client.py` & `python-selvpcclient-2.4.0/selvpcclient/client.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/__init__.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/capabilities.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/capabilities.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/customization.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/customization.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/floatingips.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/floatingips.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/keypair.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/keypair.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/license.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/license.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/limit.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/limit.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/project.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/project.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/quotas.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/quotas.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/role.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/role.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/subnet.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/subnet.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/token.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/token.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/user.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/user.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/commands/vrrp.py` & `python-selvpcclient-2.4.0/selvpcclient/commands/vrrp.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/exceptions/http.py` & `python-selvpcclient-2.4.0/selvpcclient/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/formatters.py` & `python-selvpcclient-2.4.0/selvpcclient/formatters.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/httpclient.py` & `python-selvpcclient-2.4.0/selvpcclient/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/capabilities.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/capabilities.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/customization.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/customization.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/floatingips.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/floatingips.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/keypairs.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/keypairs.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/licenses.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/licenses.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/projects.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/projects.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/quotas.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/quotas.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/roles.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/roles.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/subnets.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/subnets.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/tokens.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/tokens.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/users.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/users.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/resources/vrrp.py` & `python-selvpcclient-2.4.0/selvpcclient/resources/vrrp.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/shell.py` & `python-selvpcclient-2.4.0/selvpcclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/selvpcclient/util.py` & `python-selvpcclient-2.4.0/selvpcclient/util.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/setup.cfg` & `python-selvpcclient-2.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [metadata]
 name = python-selvpcclient
 author = Selectel
 author-email = m.kalinin@selectel.ru
 summary = Client for the Selectel Virtual Private Cloud API.
-description-file = README.md
+long_description = file: README.md
+long_description_content_type = text/markdown
 home-page = https://github.com/selectel/python-selvpcclient
 license = Apache License, Version 2.0
 classifier = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
```

### Comparing `python-selvpcclient-2.3.0/tests/cli/__init__.py` & `python-selvpcclient-2.4.0/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_capabilities.py` & `python-selvpcclient-2.4.0/tests/cli/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_customization.py` & `python-selvpcclient-2.4.0/tests/cli/test_customization.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_floatingip.py` & `python-selvpcclient-2.4.0/tests/cli/test_floatingip.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_keypairs.py` & `python-selvpcclient-2.4.0/tests/cli/test_keypairs.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_license.py` & `python-selvpcclient-2.4.0/tests/cli/test_license.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_project.py` & `python-selvpcclient-2.4.0/tests/cli/test_project.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_quota.py` & `python-selvpcclient-2.4.0/tests/cli/test_quota.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_role.py` & `python-selvpcclient-2.4.0/tests/cli/test_role.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_subnet.py` & `python-selvpcclient-2.4.0/tests/cli/test_subnet.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_token.py` & `python-selvpcclient-2.4.0/tests/cli/test_token.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_user.py` & `python-selvpcclient-2.4.0/tests/cli/test_user.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/cli/test_vrrp.py` & `python-selvpcclient-2.4.0/tests/cli/test_vrrp.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/__init__.py` & `python-selvpcclient-2.4.0/tests/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_capabilities.py` & `python-selvpcclient-2.4.0/tests/rest/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_floatingips.py` & `python-selvpcclient-2.4.0/tests/rest/test_floatingips.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_keypairs.py` & `python-selvpcclient-2.4.0/tests/rest/test_keypairs.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_licenses.py` & `python-selvpcclient-2.4.0/tests/rest/test_licenses.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_projects.py` & `python-selvpcclient-2.4.0/tests/rest/test_projects.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_quotas.py` & `python-selvpcclient-2.4.0/tests/rest/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_roles.py` & `python-selvpcclient-2.4.0/tests/rest/test_roles.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_subnets.py` & `python-selvpcclient-2.4.0/tests/rest/test_subnets.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_tokens.py` & `python-selvpcclient-2.4.0/tests/rest/test_tokens.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_users.py` & `python-selvpcclient-2.4.0/tests/rest/test_users.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/rest/test_vrrp.py` & `python-selvpcclient-2.4.0/tests/rest/test_vrrp.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/test_util.py` & `python-selvpcclient-2.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/util/answers.py` & `python-selvpcclient-2.4.0/tests/util/answers.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/util/logo.jpg` & `python-selvpcclient-2.4.0/tests/util/logo.jpg`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/util/params.py` & `python-selvpcclient-2.4.0/tests/util/params.py`

 * *Files identical despite different names*

### Comparing `python-selvpcclient-2.3.0/tests/util/temp_files.py` & `python-selvpcclient-2.4.0/tests/util/temp_files.py`

 * *Files identical despite different names*

