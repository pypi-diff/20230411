# Comparing `tmp/managesf-0.31.0.tar.gz` & `tmp/managesf-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "managesf-0.31.0.tar", last modified: Tue Jan 10 10:28:28 2023, max compression
+gzip compressed data, was "managesf-0.32.0.tar", last modified: Tue Apr 11 12:32:50 2023, max compression
```

## Comparing `managesf-0.31.0.tar` & `managesf-0.32.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.832748 managesf-0.31.0/
--rw-r--r--   0 root         (0) root         (0)     1471 2023-01-10 10:28:03.000000 managesf-0.31.0/.zuul.yaml
--rw-r--r--   0 root         (0) root         (0)      967 2023-01-10 10:28:28.000000 managesf-0.31.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    26137 2023-01-10 10:28:02.000000 managesf-0.31.0/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    19643 2023-01-10 10:28:28.000000 managesf-0.31.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11339 2023-01-10 10:28:02.000000 managesf-0.31.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      115 2023-01-10 10:28:02.000000 managesf-0.31.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1328 2023-01-10 10:28:28.832748 managesf-0.31.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-01-10 10:28:02.000000 managesf-0.31.0/README.md
--rw-r--r--   0 root         (0) root         (0)      126 2023-01-10 10:28:02.000000 managesf-0.31.0/app.wsgi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.814747 managesf-0.31.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6779 2023-01-10 10:28:02.000000 managesf-0.31.0/docs/Makefile
--rwxr-xr-x   0 root         (0) root         (0)     3559 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/generate-resources-docs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.815748 managesf-0.31.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)     8317 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/contribute.rst
--rw-r--r--   0 root         (0) root         (0)      287 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      898 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/install.rst
--rw-r--r--   0 root         (0) root         (0)     2045 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/plugins.rst
--rw-r--r--   0 root         (0) root         (0)      258 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/source/restapi.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.815748 managesf-0.31.0/docs/swagger/
--rw-r--r--   0 root         (0) root         (0)    91523 2023-01-10 10:28:03.000000 managesf-0.31.0/docs/swagger/managesf.v2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.815748 managesf-0.31.0/etc/
--rw-r--r--   0 root         (0) root         (0)     1223 2023-01-10 10:28:03.000000 managesf-0.31.0/etc/sf-policy.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.816748 managesf-0.31.0/managesf/
--rw-r--r--   0 root         (0) root         (0)       34 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.818748 managesf-0.31.0/managesf/api/
--rw-r--r--   0 root         (0) root         (0)      578 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.818748 managesf-0.31.0/managesf/api/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3122 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/base.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.818748 managesf-0.31.0/managesf/api/v2/resources/
--rw-r--r--   0 root         (0) root         (0)     1179 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.819748 managesf-0.31.0/managesf/api/v2/resources/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/resources/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/api/v2/resources/services/manageSF.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.819748 managesf-0.31.0/managesf/cmds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/cmds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/cmds/keycloak.py
--rw-r--r--   0 root         (0) root         (0)     9348 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/cmds/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.820748 managesf-0.31.0/managesf/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.820748 managesf-0.31.0/managesf/controllers/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.821748 managesf-0.31.0/managesf/controllers/api/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/api/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6133 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/api/v2/base.py
--rw-r--r--   0 root         (0) root         (0)    32426 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/api/v2/configurations.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/api/v2/resources.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/controllers/introspection.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/controllers/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.821748 managesf-0.31.0/managesf/lib/
--rw-r--r--   0 root         (0) root         (0)      578 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.822748 managesf-0.31.0/managesf/lib/auth/
--rw-r--r--   0 root         (0) root         (0)      709 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/lib/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/lib/auth/base.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/lib/auth/keycloak.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/lib/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.822748 managesf-0.31.0/managesf/model/
--rw-r--r--   0 root         (0) root         (0)    13321 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.823748 managesf-0.31.0/managesf/model/yamlbkd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/model/yamlbkd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29608 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/engine.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.824748 managesf-0.31.0/managesf/model/yamlbkd/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/connection.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/dummy.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/gitacls.py
--rw-r--r--   0 root         (0) root         (0)    15105 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/gitrepository.py
--rw-r--r--   0 root         (0) root         (0)    10055 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/group.py
--rw-r--r--   0 root         (0) root         (0)     6050 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/project.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/resources/tenant.py
--rw-r--r--   0 root         (0) root         (0)    10590 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/model/yamlbkd/yamlbackend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.825748 managesf-0.31.0/managesf/policies/
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/policies/base.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policies/config.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policies/hooks.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policies/localuser.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policies/resources.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policies/services_users.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.826748 managesf-0.31.0/managesf/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6109 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/base.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/services/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.827748 managesf-0.31.0/managesf/services/gerrit/
--rw-r--r--   0 root         (0) root         (0)     1964 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/gerrit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/gerrit/group.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-01-10 10:28:02.000000 managesf-0.31.0/managesf/services/gerrit/project.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/gerrit/review.py
--rw-r--r--   0 root         (0) root         (0)     5780 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/gerrit/user.py
--rw-r--r--   0 root         (0) root         (0)    18360 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/gerrit/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.827748 managesf-0.31.0/managesf/services/keycloak/
--rw-r--r--   0 root         (0) root         (0)    11907 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/services/keycloak/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/sfauth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.830748 managesf-0.31.0/managesf/tests/
--rw-r--r--   0 root         (0) root         (0)     2574 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.830748 managesf-0.31.0/managesf/tests/apiv2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/apiv2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/apiv2/test_app.py
--rw-r--r--   0 root         (0) root         (0)     4886 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/apiv2/test_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.831748 managesf-0.31.0/managesf/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      701 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/fixtures/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.831748 managesf-0.31.0/managesf/tests/fixtures/nodepool/
--rw-r--r--   0 root         (0) root         (0)      322 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/fixtures/nodepool/_nodepool.yaml
--rw-r--r--   0 root         (0) root         (0)      650 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/fixtures/nodepool/nodepool.yaml
--rw-r--r--   0 root         (0) root         (0)    13518 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/fixtures/sf_resources.py
--rw-r--r--   0 root         (0) root         (0)    19456 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/fixtures/zuul_sql_reporter.sqlite3
--rw-r--r--   0 root         (0) root         (0)     2120 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/resources_test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_apiv2.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_app.py
--rw-r--r--   0 root         (0) root         (0)    30726 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_gerrit_utils.py
--rw-r--r--   0 root         (0) root         (0)    16973 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_policy.py
--rw-r--r--   0 root         (0) root         (0)    48674 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_engine.py
--rw-r--r--   0 root         (0) root         (0)    71918 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_engine_real.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_gitacls.py
--rw-r--r--   0 root         (0) root         (0)    15837 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_gitrepo.py
--rw-r--r--   0 root         (0) root         (0)    13497 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_group.py
--rw-r--r--   0 root         (0) root         (0)     9251 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_model.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_resources_project.py
--rw-r--r--   0 root         (0) root         (0)     2197 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_service.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_service_gerrit.py
--rw-r--r--   0 root         (0) root         (0)     6879 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_service_keycloak.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_sfauth.py
--rw-r--r--   0 root         (0) root         (0)    12416 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf/tests/test_yamlbackend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.818748 managesf-0.31.0/managesf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1328 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3926 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      461 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      152 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-10 10:28:28.000000 managesf-0.31.0/managesf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      414 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf.service
--rw-r--r--   0 root         (0) root         (0)     4552 2023-01-10 10:28:03.000000 managesf-0.31.0/managesf.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.810747 managesf-0.31.0/releasenotes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 10:28:28.832748 managesf-0.31.0/releasenotes/notes/
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-10 10:28:03.000000 managesf-0.31.0/releasenotes/notes/add-project-resources-options-attribute-ac62c9885cbd71c1.yaml
--rw-r--r--   0 root         (0) root         (0)       92 2023-01-10 10:28:03.000000 managesf-0.31.0/releasenotes/notes/change-to-pymysql-4256873574e76488.yaml
--rw-r--r--   0 root         (0) root         (0)      115 2023-01-10 10:28:03.000000 managesf-0.31.0/releasenotes/notes/new-connection-resources-object-f71f7bcd95ac22bd.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-01-10 10:28:03.000000 managesf-0.31.0/releasenotes/notes/new-tenant-resources-object-cb89ef2bd341263e.yaml
--rw-r--r--   0 root         (0) root         (0)       92 2023-01-10 10:28:03.000000 managesf-0.31.0/releasenotes/notes/remove-htp-controller-2669de12052ecb74.yaml
--rw-r--r--   0 root         (0) root         (0)      229 2023-01-10 10:28:03.000000 managesf-0.31.0/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      780 2023-01-10 10:28:03.000000 managesf-0.31.0/run_tests.sh
--rw-r--r--   0 root         (0) root         (0)      682 2023-01-10 10:28:28.833748 managesf-0.31.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      967 2023-01-10 10:28:03.000000 managesf-0.31.0/setup.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-10 10:28:03.000000 managesf-0.31.0/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)      429 2023-01-10 10:28:03.000000 managesf-0.31.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.055447 managesf-0.32.0/
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-11 12:31:30.000000 managesf-0.32.0/.zuul.yaml
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-11 12:32:49.000000 managesf-0.32.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    26137 2023-04-11 12:31:30.000000 managesf-0.32.0/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    19726 2023-04-11 12:32:49.000000 managesf-0.32.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11339 2023-04-11 12:31:30.000000 managesf-0.32.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      115 2023-04-11 12:31:30.000000 managesf-0.32.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-11 12:32:50.055447 managesf-0.32.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-04-11 12:31:30.000000 managesf-0.32.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-11 12:31:30.000000 managesf-0.32.0/app.wsgi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.039447 managesf-0.32.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/Makefile
+-rwxr-xr-x   0 root         (0) root         (0)     3559 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/generate-resources-docs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.041447 managesf-0.32.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)     8317 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/contribute.rst
+-rw-r--r--   0 root         (0) root         (0)      287 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/install.rst
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/plugins.rst
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/source/restapi.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.041447 managesf-0.32.0/docs/swagger/
+-rw-r--r--   0 root         (0) root         (0)    91523 2023-04-11 12:31:30.000000 managesf-0.32.0/docs/swagger/managesf.v2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.041447 managesf-0.32.0/etc/
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-04-11 12:31:30.000000 managesf-0.32.0/etc/sf-policy.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.042447 managesf-0.32.0/managesf/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.043447 managesf-0.32.0/managesf/api/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.043447 managesf-0.32.0/managesf/api/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/base.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.043447 managesf-0.32.0/managesf/api/v2/resources/
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.044447 managesf-0.32.0/managesf/api/v2/resources/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/resources/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/api/v2/resources/services/manageSF.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.044447 managesf-0.32.0/managesf/cmds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/cmds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/cmds/keycloak.py
+-rw-r--r--   0 root         (0) root         (0)     9348 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/cmds/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.044447 managesf-0.32.0/managesf/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.045447 managesf-0.32.0/managesf/controllers/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.045447 managesf-0.32.0/managesf/controllers/api/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/api/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/api/v2/base.py
+-rw-r--r--   0 root         (0) root         (0)    32426 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/api/v2/configurations.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/api/v2/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/introspection.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/controllers/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.046447 managesf-0.32.0/managesf/lib/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.046447 managesf-0.32.0/managesf/lib/auth/
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/lib/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/lib/auth/base.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/lib/auth/keycloak.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/lib/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.046447 managesf-0.32.0/managesf/model/
+-rw-r--r--   0 root         (0) root         (0)    13321 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.047447 managesf-0.32.0/managesf/model/yamlbkd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29608 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/engine.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.048447 managesf-0.32.0/managesf/model/yamlbkd/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/connection.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/dummy.py
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/gitacls.py
+-rw-r--r--   0 root         (0) root         (0)    15105 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/gitrepository.py
+-rw-r--r--   0 root         (0) root         (0)    10055 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/group.py
+-rw-r--r--   0 root         (0) root         (0)     6050 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/project.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/resources/tenant.py
+-rw-r--r--   0 root         (0) root         (0)    10590 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/model/yamlbkd/yamlbackend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.049447 managesf-0.32.0/managesf/policies/
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/base.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/config.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/localuser.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policies/services_users.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.049447 managesf-0.32.0/managesf/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/base.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.050447 managesf-0.32.0/managesf/services/gerrit/
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/group.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/project.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/review.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/user.py
+-rw-r--r--   0 root         (0) root         (0)    18360 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/gerrit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.050447 managesf-0.32.0/managesf/services/keycloak/
+-rw-r--r--   0 root         (0) root         (0)    11907 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/services/keycloak/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/sfauth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.053447 managesf-0.32.0/managesf/tests/
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.053447 managesf-0.32.0/managesf/tests/apiv2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/apiv2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/apiv2/test_app.py
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/apiv2/test_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.054447 managesf-0.32.0/managesf/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      701 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/fixtures/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.054447 managesf-0.32.0/managesf/tests/fixtures/nodepool/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/fixtures/nodepool/_nodepool.yaml
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/fixtures/nodepool/nodepool.yaml
+-rw-r--r--   0 root         (0) root         (0)    13518 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/fixtures/sf_resources.py
+-rw-r--r--   0 root         (0) root         (0)    19456 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/fixtures/zuul_sql_reporter.sqlite3
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/resources_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_apiv2.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_app.py
+-rw-r--r--   0 root         (0) root         (0)    30726 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_gerrit_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16973 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_policy.py
+-rw-r--r--   0 root         (0) root         (0)    48674 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_engine.py
+-rw-r--r--   0 root         (0) root         (0)    71918 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_engine_real.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_gitacls.py
+-rw-r--r--   0 root         (0) root         (0)    15837 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_gitrepo.py
+-rw-r--r--   0 root         (0) root         (0)    13497 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_group.py
+-rw-r--r--   0 root         (0) root         (0)     9251 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_model.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_resources_project.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_service.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_service_gerrit.py
+-rw-r--r--   0 root         (0) root         (0)     6879 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_service_keycloak.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_sfauth.py
+-rw-r--r--   0 root         (0) root         (0)    12416 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf/tests/test_yamlbackend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.043447 managesf-0.32.0/managesf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-11 12:32:49.000000 managesf-0.32.0/managesf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf.service
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-04-11 12:31:30.000000 managesf-0.32.0/managesf.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.035447 managesf-0.32.0/releasenotes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:32:50.055447 managesf-0.32.0/releasenotes/notes/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-11 12:31:30.000000 managesf-0.32.0/releasenotes/notes/add-project-resources-options-attribute-ac62c9885cbd71c1.yaml
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-11 12:31:30.000000 managesf-0.32.0/releasenotes/notes/change-to-pymysql-4256873574e76488.yaml
+-rw-r--r--   0 root         (0) root         (0)      115 2023-04-11 12:31:30.000000 managesf-0.32.0/releasenotes/notes/new-connection-resources-object-f71f7bcd95ac22bd.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-11 12:31:30.000000 managesf-0.32.0/releasenotes/notes/new-tenant-resources-object-cb89ef2bd341263e.yaml
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-11 12:31:30.000000 managesf-0.32.0/releasenotes/notes/remove-htp-controller-2669de12052ecb74.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-11 12:31:30.000000 managesf-0.32.0/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      780 2023-04-11 12:31:30.000000 managesf-0.32.0/run_tests.sh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-11 12:32:50.055447 managesf-0.32.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-11 12:31:30.000000 managesf-0.32.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-11 12:31:30.000000 managesf-0.32.0/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      429 2023-04-11 12:31:30.000000 managesf-0.32.0/tox.ini
```

### Comparing `managesf-0.31.0/.zuul.yaml` & `managesf-0.32.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/AUTHORS` & `managesf-0.32.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/CHANGELOG` & `managesf-0.32.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/ChangeLog` & `managesf-0.32.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.32.0
+------
+
+* Since Gerrit 3.3 'Non-Interactive Users' is not a default group'
+
 0.31.0
 ------
 
 * Fix preferred\_username claim condition for default zuul tenant admin rule
 * Add managesf-keycloak CLI command
 * More cauth removal
```

### Comparing `managesf-0.31.0/LICENSE` & `managesf-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/README.md` & `managesf-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/Makefile` & `managesf-0.32.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/generate-resources-docs.py` & `managesf-0.32.0/docs/generate-resources-docs.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/source/conf.py` & `managesf-0.32.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/source/contribute.rst` & `managesf-0.32.0/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/source/install.rst` & `managesf-0.32.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/source/plugins.rst` & `managesf-0.32.0/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/docs/swagger/managesf.v2.yaml` & `managesf-0.32.0/docs/swagger/managesf.v2.yaml`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/etc/sf-policy.yaml` & `managesf-0.32.0/etc/sf-policy.yaml`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/api/__init__.py` & `managesf-0.32.0/managesf/api/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/api/v2/base.py` & `managesf-0.32.0/managesf/api/v2/base.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/api/v2/managers.py` & `managesf-0.32.0/managesf/api/v2/managers.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/api/v2/resources/__init__.py` & `managesf-0.32.0/managesf/api/v2/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/api/v2/resources/services/manageSF.py` & `managesf-0.32.0/managesf/api/v2/resources/services/manageSF.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/app.py` & `managesf-0.32.0/managesf/app.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/cmds/keycloak.py` & `managesf-0.32.0/managesf/cmds/keycloak.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/cmds/resources.py` & `managesf-0.32.0/managesf/cmds/resources.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/controllers/api/v2/base.py` & `managesf-0.32.0/managesf/controllers/api/v2/base.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/controllers/api/v2/configurations.py` & `managesf-0.32.0/managesf/controllers/api/v2/configurations.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/controllers/api/v2/resources.py` & `managesf-0.32.0/managesf/controllers/api/v2/resources.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/controllers/introspection.py` & `managesf-0.32.0/managesf/controllers/introspection.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/controllers/root.py` & `managesf-0.32.0/managesf/controllers/root.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/lib/__init__.py` & `managesf-0.32.0/managesf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/lib/auth/__init__.py` & `managesf-0.32.0/managesf/lib/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/lib/auth/base.py` & `managesf-0.32.0/managesf/lib/auth/base.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/lib/auth/keycloak.py` & `managesf-0.32.0/managesf/lib/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/lib/common.py` & `managesf-0.32.0/managesf/lib/common.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/__init__.py` & `managesf-0.32.0/managesf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/engine.py` & `managesf-0.32.0/managesf/model/yamlbkd/engine.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resource.py` & `managesf-0.32.0/managesf/model/yamlbkd/resource.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/connection.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/connection.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/dummy.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/dummy.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/gitacls.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/gitacls.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
     def __init__(self, conf, new):
         self.conf = conf
         self.new = new
 
     def extra_validations(self, **kwargs):
         default_groups = ('Service Users',
-                          'Non-Interactive Users',
                           'Administrators',
                           'Registered Users',
                           'Anonymous Users')
         logs = []
         acls = kwargs['file']
         groups = kwargs['groups']
         name = kwargs['name']
```

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/gitrepository.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/gitrepository.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/group.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/group.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/project.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/project.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/resources/tenant.py` & `managesf-0.32.0/managesf/model/yamlbkd/resources/tenant.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/model/yamlbkd/yamlbackend.py` & `managesf-0.32.0/managesf/model/yamlbkd/yamlbackend.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/__init__.py` & `managesf-0.32.0/managesf/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/base.py` & `managesf-0.32.0/managesf/policies/base.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/config.py` & `managesf-0.32.0/managesf/policies/config.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/hooks.py` & `managesf-0.32.0/managesf/policies/hooks.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/localuser.py` & `managesf-0.32.0/managesf/policies/localuser.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/resources.py` & `managesf-0.32.0/managesf/policies/resources.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policies/services_users.py` & `managesf-0.32.0/managesf/policies/services_users.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/policy.py` & `managesf-0.32.0/managesf/policy.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/base.py` & `managesf-0.32.0/managesf/services/base.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/exceptions.py` & `managesf-0.32.0/managesf/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/__init__.py` & `managesf-0.32.0/managesf/services/gerrit/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/group.py` & `managesf-0.32.0/managesf/services/gerrit/group.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/project.py` & `managesf-0.32.0/managesf/services/gerrit/project.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/review.py` & `managesf-0.32.0/managesf/services/gerrit/review.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/user.py` & `managesf-0.32.0/managesf/services/gerrit/user.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/gerrit/utils.py` & `managesf-0.32.0/managesf/services/gerrit/utils.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/services/keycloak/__init__.py` & `managesf-0.32.0/managesf/services/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/sfauth.py` & `managesf-0.32.0/managesf/sfauth.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/__init__.py` & `managesf-0.32.0/managesf/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/apiv2/test_app.py` & `managesf-0.32.0/managesf/tests/apiv2/test_app.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/apiv2/test_resources.py` & `managesf-0.32.0/managesf/tests/apiv2/test_resources.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/fixtures/__init__.py` & `managesf-0.32.0/managesf/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/fixtures/nodepool/nodepool.yaml` & `managesf-0.32.0/managesf/tests/fixtures/nodepool/nodepool.yaml`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/fixtures/sf_resources.py` & `managesf-0.32.0/managesf/tests/fixtures/sf_resources.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/fixtures/zuul_sql_reporter.sqlite3` & `managesf-0.32.0/managesf/tests/fixtures/zuul_sql_reporter.sqlite3`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/resources_test_utils.py` & `managesf-0.32.0/managesf/tests/resources_test_utils.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_apiv2.py` & `managesf-0.32.0/managesf/tests/test_apiv2.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_app.py` & `managesf-0.32.0/managesf/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_configuration.py` & `managesf-0.32.0/managesf/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_gerrit_utils.py` & `managesf-0.32.0/managesf/tests/test_gerrit_utils.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_policy.py` & `managesf-0.32.0/managesf/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_engine.py` & `managesf-0.32.0/managesf/tests/test_resources_engine.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_engine_real.py` & `managesf-0.32.0/managesf/tests/test_resources_engine_real.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_gitacls.py` & `managesf-0.32.0/managesf/tests/test_resources_gitacls.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_gitrepo.py` & `managesf-0.32.0/managesf/tests/test_resources_gitrepo.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_group.py` & `managesf-0.32.0/managesf/tests/test_resources_group.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_model.py` & `managesf-0.32.0/managesf/tests/test_resources_model.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_resources_project.py` & `managesf-0.32.0/managesf/tests/test_resources_project.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_service.py` & `managesf-0.32.0/managesf/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_service_gerrit.py` & `managesf-0.32.0/managesf/tests/test_service_gerrit.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_service_keycloak.py` & `managesf-0.32.0/managesf/tests/test_service_keycloak.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_sfauth.py` & `managesf-0.32.0/managesf/tests/test_sfauth.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf/tests/test_yamlbackend.py` & `managesf-0.32.0/managesf/tests/test_yamlbackend.py`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf.egg-info/SOURCES.txt` & `managesf-0.32.0/managesf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/managesf.spec` & `managesf-0.32.0/managesf.spec`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/run_tests.sh` & `managesf-0.32.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/setup.cfg` & `managesf-0.32.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `managesf-0.31.0/setup.py` & `managesf-0.32.0/setup.py`

 * *Files identical despite different names*

