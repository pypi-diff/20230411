# Comparing `tmp/pop-create-idem-3.2.0.tar.gz` & `tmp/pop-create-idem-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.2.0.tar", last modified: Fri Apr  7 17:25:28 2023, max compression
+gzip compressed data, was "pop-create-idem-3.2.1.tar", last modified: Tue Apr 11 20:29:41 2023, max compression
```

## Comparing `pop-create-idem-3.2.0.tar` & `pop-create-idem-3.2.1.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.496761 pop-create-idem-3.2.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-07 17:25:28.496761 pop-create-idem-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3539 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2091 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      793 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      762 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1474 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5708 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)    12344 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      587 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.488761 pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-07 17:25:27.000000 pop-create-idem-3.2.0/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 17:25:28.492761 pop-create-idem-3.2.0/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3939 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-07 17:25:28.000000 pop-create-idem-3.2.0/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 17:25:28.496761 pop-create-idem-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-07 17:25:14.000000 pop-create-idem-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8546 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3552 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)    12404 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4232 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/setup.py
```

### Comparing `pop-create-idem-3.2.0/LICENSE` & `pop-create-idem-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/PKG-INFO` & `pop-create-idem-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.2.0
+Version: 3.2.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.2.0/README.rst` & `pop-create-idem-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/cloudspec/__init__.py` & `pop-create-idem-3.2.1/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/cloudspec/conf.py` & `pop-create-idem-3.2.1/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import pathlib
+import timeit
 from typing import List
 
 from cloudspec import CloudSpec
 
 
 def __init__(hub):
     hub.pop.sub.add(dyne_name="tool")
@@ -37,16 +38,17 @@
 
 def run(
     hub,
     ctx,
     root_directory: pathlib.Path,
     create_plugins: List[str],
 ):
-
+    start_time = timeit.default_timer()
     for create_plugin in create_plugins:
         try:
             hub.log.info(f"Running create plugin: {create_plugin}")
             hub.cloudspec.create[create_plugin].run(ctx, root_directory)
         except Exception as e:
             hub.log.error(f"Failed to run create plugin: {create_plugin}")
             hub.log.error(e)
             raise
+    print(f"Total Duration: {timeit.default_timer() - start_time} seconds")
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 CREATE = """
 async def {{function.name}}(
     hub,
     ctx,
-    name: str,
+    name: str
     {% if function.header_params %}
         {{function.header_params}}
-    {% endif -%}
+    {% endif -%},
+    **kwargs
 ) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         Resource State:
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Templates for state modules
 """
 
 PRESENT_FUNCTION = """
 async def {{function.name}}(
     hub,
-    ctx{{function.header_params}}
+    ctx,
+    name: str,
+    resource_id: str= None,
+    **kwargs
 ) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         .. code-block:: sls
@@ -17,15 +20,21 @@
             resource_is_{{function.name}}:
               {{ function.ref }}.{{ function.name }}:
                 - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
     '''
 """
 
 ABSENT_FUNCTION = """
-async def {{function.name}}(hub, ctx{{function.header_params}})  -> Dict[str, Any]:
+async def {{function.name}}(
+    hub,
+    ctx,
+    name: str = None,
+    resource_id: str = None,
+    **kwargs
+)  -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         .. code-block:: sls
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/conf.py` & `pop-create-idem-3.2.1/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-import aiohttp
+import base64
+
+DEFAULT_ENDPOINT_URL = "{{cookiecutter.servers|first}}"
 
 
 async def gather(hub):
     """
     Authenticate with a username and password to the given endpoint url.
     Any extra parameters will be saved as part of the profile.
 
     Example:
 
     .. code-block:: sls
 
-        {{cookiecutter.service_name}}.basic_auth:
+        {{cookiecutter.service_name}}:
           profile_name:
             username: my_user
             password: my_token
             endpoint_url: https://{{cookiecutter.service_name}}.com
     """
     sub_profiles = {}
     for profile, ctx in hub.acct.PROFILES.get(
         "{{cookiecutter.service_name}}.basic_auth", {}
     ).items():
+        creds = f"{ctx.pop('username')}:{ctx.pop('password')}"
         sub_profiles[profile] = dict(
             endpoint_url=ctx.pop("endpoint_url"),
-            auth=aiohttp.BasicAuth(ctx.pop("username"), ctx.pop("password")),
+            headers={
+                "Authorization": f"Basic {base64.b64encode(creds.encode('utf-8')).decode('ascii')}"
+            },
             **ctx
         )
 
     return sub_profiles
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
     hub.exec.{{cookiecutter.service_name}}.ACCT = ["{{cookiecutter.acct_plugin}}"]
 
     def _get_version_sub(ctx, *args, **kwargs):
         api_version = ctx.acct.get("api_version", "latest")
         return hub.exec.{{cookiecutter.service_name}}
 
     # Get the version sub dynamically from the ctx variable/acct
-    hub.pop.sub.dynamic(hub.exec.{{cookiecutter.service_name}}, _get_version_sub)
+    #hub.pop.sub.dynamic(hub.exec.{{cookiecutter.service_name}}, _get_version_sub)
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,40 +11,44 @@
     if ctx.get("simple_service_name"):
         ctx.service_name = ctx.simple_service_name
     elif not ctx.get("service_name"):
         ctx.service_name = (
             ctx.clean_name.replace("idem", "").replace("cloud", "").strip("_")
         )
 
-    ctx.clean_api_version = ctx.get("clean_api_version")
-    ctx.cloud_api_version = ctx.get("cloud_api_version")
-    ctx.servers = ctx.get("servers", [""])
     ctx.has_acct_plugin = bool(ctx.acct_plugin)
     if not ctx.has_acct_plugin:
         # Create auth plugins
         ctx.acct_plugin = ctx.service_name
 
-    # Read the spec from URL or local file
+    # Read the spec from URL or local file (Yaml)
     spec = hub.pop_create.openapi3.init.read(source=ctx.specification)
     api = openapi3.OpenAPI(spec, validate=True)
     errors = api.errors()
     if errors:
         for e in errors:
             hub.log.warning(e)
 
     # list these as defaults in the acct plugin
     if api.servers:
         ctx.servers = [x.url for x in api.servers]
     else:
-        ctx.servers = ["https://"]
+        ctx.servers = ctx.get("servers", [""])
 
     hub.log.debug(f"Working with openapi spec version: {api.openapi}")
+
     ctx.cloud_api_version = api.info.version or "latest"
     ctx.clean_api_version = hub.tool.format.case.snake(ctx.cloud_api_version).strip("_")
 
+    if not ctx.clean_api_version:
+        ctx.clean_api_version = ctx.get("clean_api_version")
+
+    if not ctx.cloud_api_version:
+        ctx.cloud_api_version = ctx.get("cloud_api_version")
+
     # If the api version starts with a digit then make sure it can be used for python namespacing
     if ctx.clean_api_version[0].isdigit():
         ctx.clean_api_version = "v" + ctx.clean_api_version
 
     # Get function plugins
     plugins = hub.pop_create.openapi3.parse.plugins(ctx, api)
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 from typing import Any
 from typing import Dict
 
 import openapi3.object_base
 import tqdm
 
 __func_alias__ = {"type_": "type"}
@@ -26,54 +25,45 @@
                 continue
             subs = [hub.tool.format.case.snake(sub) for sub in func.tags]
             if not subs:
                 plugin = "init"
             else:
                 plugin = subs.pop()
 
-            refs = [ctx.service_name] + subs + [plugin]
+            # service name is already added in pop-create
+            refs = subs + [plugin]
             ref = ".".join(refs)
             if ref not in ret:
                 # This is the first time we have looked at this plugin
                 ret[ref] = {
                     "functions": {},
                     "doc": "",
                     "imports": [
-                        "from typing import *",
+                        "from typing import Any",
+                        "from typing import Dict",
                         "import dict_tools.differ as differ",
                     ],
                 }
 
             # See if this function will be reserved CRUD operations, if so change the name
-            known_func_name = None
-
-            # e.g. /pets
-            if name.endswith(plugin):
-                # list/post
-                if request_type == "get":
-                    known_func_name = "list"
-                elif request_type == "post":
-                    known_func_name = "create"
-            # e.g.: /pets/{id}
-            elif re.match(".*(id})$", name.lower()) and name.rsplit("/", 1)[0].endswith(
-                plugin
-            ):
-                # get/list/put
-                if request_type == "get":
-                    known_func_name = "get"
-                elif request_type == "put" or request_type == "patch":
-                    known_func_name = "update"
-                elif request_type == "delete":
-                    known_func_name = "delete"
+            reserved_func_name = (
+                hub.pop_create.openapi3.parse.resolve_reserved_function_name(
+                    name, plugin, request_type, func
+                )
+            )
 
+            # Anything that doesn't resolved in reserved function name, would go into tools/{resource_name}/*
             func_name = (
-                hub.pop_create.openapi3.parse.resolve_function_name(name, func)
-                if not known_func_name
-                else known_func_name
+                hub.pop_create.openapi3.parse.resolve_function_name(name, plugin, func)
+                if not reserved_func_name
+                else reserved_func_name
             )
+
+            # print(f"{func_name}: {name}: {plugin}")
+
             func_data = hub.pop_create.openapi3.parse.function(func, api)
             func_data["hardcoded"] = {
                 "method": request_type,
                 "path": name.split(" ")[0],
                 "service_name": ctx.service_name,
                 "resource_name": plugin,
             }
@@ -90,16 +80,18 @@
 
     params = {}
     for p in func.parameters:
         # TODO: openapi3.general.Reference is unsupported at the moment
         if isinstance(p, openapi3.paths.Parameter):
             params[p.name] = hub.pop_create.openapi3.parse.parameter(p)
 
+    deprecated_text = "\nDEPRECATED" if func.deprecated else ""
+
     return {
-        "doc": f"{func.summary}\n    {func.description}".strip(),
+        "doc": f"{func.summary}\n    {func.description}    {deprecated_text}".strip(),
         "params": params,
     }
 
 
 def parameter(hub, parameter: openapi3.paths.Parameter):
     if parameter.in_ == "query":
         target_type = "mapping"
@@ -130,31 +122,66 @@
         return "int"
     elif "boolean" == param_type:
         return "bool"
     elif "number" == param_type:
         return "float"
     elif "string" == param_type:
         return "str"
+    elif "array" == param_type:
+        return "list"
     else:
         return ""
 
 
-def resolve_function_name(hub, name: str, func: openapi3.paths.Operation):
+def resolve_reserved_function_name(
+    hub, name: str, plugin: str, request_type: str, func: openapi3.paths.Operation
+):
+    # Do not make deprecated API paths into CRUDs and throw them into tools/*
+    if not func.deprecated:
+        # e.g. plugin: pets, path: /pets
+        if name.endswith(plugin):
+            # list/post
+            if request_type == "get":
+                return "list"
+            elif request_type == "post":
+                return "create"
+        # e.g.: plugin: pets, path: /pets/{id}
+        elif name.rsplit("/", 1)[0].endswith(plugin):
+            # get/list/put
+            if request_type == "get":
+                return "get"
+            elif request_type == "put" or request_type == "patch":
+                return "update"
+            elif request_type == "delete":
+                return "delete"
+
+    return None
+
+
+def resolve_function_name(hub, name: str, plugin: str, func: openapi3.paths.Operation):
     # This is the preferred way to get a function name
-    func_name = func.operationId
+    # However, some APIs can just put reserved/known operationId which is not helpful here in parsing and codegen
+    # Also, we always handle reserved/known operation names in different way
+    func_name = (
+        func.operationId
+        if func.operationId
+        not in ["get", "list", "create", "patch", "update", "put", "delete"]
+        else None
+    )
 
     # Fallback function name based on the pets example
     if not func_name and " " in name:
         func_name = "_".join(name.split(" ")[1:]).lower()
 
+    if not func_name:
+        # Truncate it to 10 characters and add plugin name in the end
+        func_name = f"{func.summary[:10]}_{plugin}"
+
     if not func_name and func.extensions:
         func_name = func.extensions[sorted(func.extensions.keys())[0]]
 
-    if not func_name:
-        func_name = func.summary
-
     # Maybe we need more fallbacks, you tell me
     if not func_name:
         # Maybe a fallback based on the path and method?
         raise AttributeError(f"Not sure how to find func name for {name}, help me out")
 
     return hub.tool.format.case.snake(func_name)
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/openapi3/template.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,84 +1,88 @@
 GET_REQUEST_FORMAT = """
     result = dict(comment=[], ret=None, result=True)
 
     # TODO: Change function methods params if needed
-    get = hub.tool.{{ function.hardcoded.service_name }}.session.request(
+    get = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
-        path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}".format(
+        path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
         data={{ parameter.mapping.header|default({}) }}
     )
 
     if not get["result"]:
         # Send empty result for not found
-        if err.status == 404:
+        if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             return result
 
         result["comment"].append(get["comment"])
         result["result"] = False
         return result
 
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(
             f"Get '{name}' result is empty"
         )
         return result
 
+    # TODO: Make sure resource_id is mapped in get response
+    get["ret"]["resource_id"] = resource_id
     result["ret"] = get["ret"]
     return result
 """
 
 LIST_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
     # TODO: Change function methods params if needed
-    list = hub.tool.{{ function.hardcoded.service_name }}.session.request(
+    list = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
-        path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}",
+        path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
         data={{ parameter.mapping.header|default({}) }}
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
 
     for resource in list["ret"]:
+        # TODO: Map resource_id from response
+        resource["resource_id"] = ""
         result["ret"].append(resource)
     return result
 """
 
 CREATE_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
     # TODO: Change function methods params if needed.
-    create = hub.tool.{{ function.hardcoded.service_name }}.session.request(
+    create = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
-        path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}",
+        path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
         data={{ parameter.mapping.header|default({}) }}
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(f"Created {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} '{name}'",)
 
-    result["ret"] = create
+    result["ret"] = create["ret"]
     return result
 """
 
 UPDATE_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {"name": name, "resource_id": resource_id, **kwargs}
@@ -89,42 +93,42 @@
 
     parameters_to_update = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
             parameters_to_update[resource_to_raw_input_mapping[key]] = desired_state.get(key)
 
     if parameters_to_update:
-        update = hub.tool.{{ function.hardcoded.service_name }}.session.request(
+        update = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
             ctx,
             method="{{ function.hardcoded.method }}",
-            path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}".format(
+            path="{{ function.hardcoded.path }}".format(
                 **{{ parameter.mapping.path|default({}) }}
             ),
             query_params={{ parameter.mapping.query|default({}) }},
             data={{ parameter.mapping.header|default({}) }}
         )
 
         if not create["result"]:
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
-        result["ret"] = update
+        result["ret"] = update["ret"]
         result["comment"].append(f"Updated {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} '{name}'",)
 
     return result
 """
 
 DELETE_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
-    delete = hub.tool.{{ function.hardcoded.service_name }}.session.request(
+    delete = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
-        path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}".format(
+        path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
         data={{ parameter.mapping.header|default({}) }}
     )
 
     if not delete["result"]:
@@ -138,15 +142,15 @@
 
 OTHER_FUNCTION_REQUEST_FORMAT = """
     result = dict(comment=[], ret=None, result=True)
 
     ret = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
-        path=ctx.acct.endpoint_url + "{{ function.hardcoded.path }}".format(
+        path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
         data={{ parameter.mapping.header|default({}) }}
     )
 
     if not ret["result"]:
@@ -216,15 +220,14 @@
             )
             result["comment"] = (f"Would create {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} {name}",)
             return result
         else:
             create_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.create(
                 ctx,
                 name=name,
-                resource_id=resource_id,
                 **kwargs
                 # TODO: Add other required parameters from: **{{ parameter.mapping.kwargs|default({})}}
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
                 result["comment"].append(f"Created '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}'")
@@ -307,16 +310,16 @@
 
     if not ret or not ret["result"]:
         hub.log.debug(f"Could not describe {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
         # TODO: Look for respective identifier in **{{ function.hardcoded.resource_attributes }}
-        resource_id = resource.get("TODO: Replace with resource identifier")
+        resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "{{ function.hardcoded.resource_name }}.present": [
+            "{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
 """
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.2.1/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.2.1/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.2.1/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.0/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.2.1/pop_create_idem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.2.0
+Version: 3.2.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.2.0/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-3.2.1/pop_create_idem.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
 pop_create_idem/pop_create/openapi3/init.py
 pop_create_idem/pop_create/openapi3/parse.py
 pop_create_idem/pop_create/openapi3/template.py
 pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
 pop_create_idem/pop_create/rest/init.py
 pop_create_idem/pop_create/swagger/init.py
 pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
 pop_create_idem/tool/gradle.py
 pop_create_idem/tool/jinja.py
 pop_create_idem/tool/format/case.py
 pop_create_idem/tool/format/html.py
```

### Comparing `pop-create-idem-3.2.0/setup.py` & `pop-create-idem-3.2.1/setup.py`

 * *Files identical despite different names*

