# Comparing `tmp/hcs-cli-0.1.26.tar.gz` & `tmp/hcs-cli-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.26.tar", last modified: Mon Apr 10 19:18:24 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.27.tar", last modified: Tue Apr 11 01:05:06 2023, max compression
```

## Comparing `hcs-cli-0.1.26.tar` & `hcs-cli-0.1.27.tar`

### file list

```diff
@@ -1,124 +1,128 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.707967 hcs-cli-0.1.26/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.26/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.26/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.26/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     1957 2023-04-10 19:18:24.707583 hcs-cli-0.1.26/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1188 2023-04-08 01:25:45.000000 hcs-cli-0.1.26/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.597969 hcs-cli-0.1.26/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1957 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2738 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.26/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.26/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-10 19:18:24.708530 hcs-cli-0.1.26/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-10 17:59:22.000000 hcs-cli-0.1.26/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.601120 hcs-cli-0.1.26/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.26/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.26/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.603270 hcs-cli-0.1.26/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.26/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.604548 hcs-cli-0.1.26/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.26/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.614493 hcs-cli-0.1.26/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.617700 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.618803 hcs-cli-0.1.26/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.26/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.620694 hcs-cli-0.1.26/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.624157 hcs-cli-0.1.26/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.625572 hcs-cli-0.1.26/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.628937 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.631383 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.26/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.633484 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.637570 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      129 2023-04-07 18:26:44.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.644247 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      644 2023-04-10 18:54:41.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      352 2023-04-07 18:24:18.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-10 19:14:17.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1260 2023-04-07 18:57:03.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.653177 hcs-cli-0.1.26/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.656115 hcs-cli-0.1.26/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.26/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.661446 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     1960 2023-04-10 18:54:37.000000 hcs-cli-0.1.26/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.664761 hcs-cli-0.1.26/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.678871 hcs-cli-0.1.26/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.26/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.682829 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4097 2023-04-10 19:00:11.000000 hcs-cli-0.1.26/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.26/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.26/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.26/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-10 19:10:32.000000 hcs-cli-0.1.26/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.26/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.26/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.690491 hcs-cli-0.1.26/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3879 2023-04-10 18:18:13.000000 hcs-cli-0.1.26/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.26/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.26/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.694245 hcs-cli-0.1.26/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.26/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.702797 hcs-cli-0.1.26/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.26/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.26/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     2777 2023-04-10 18:36:25.000000 hcs-cli-0.1.26/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.26/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.26/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.705710 hcs-cli-0.1.26/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.26/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.26/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.155745 hcs-cli-0.1.27/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.27/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.27/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.27/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 01:05:06.155325 hcs-cli-0.1.27/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.27/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.077664 hcs-cli-0.1.27/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2782 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.058620 hcs-cli-0.1.27/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.078530 hcs-cli-0.1.27/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.27/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.27/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.27/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-11 01:05:06.156946 hcs-cli-0.1.27/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-11 01:05:02.000000 hcs-cli-0.1.27/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.080202 hcs-cli-0.1.27/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.27/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.27/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.081255 hcs-cli-0.1.27/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.27/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.081856 hcs-cli-0.1.27/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.27/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.084990 hcs-cli-0.1.27/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.086622 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.087292 hcs-cli-0.1.27/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.27/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.088410 hcs-cli-0.1.27/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.090302 hcs-cli-0.1.27/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.090855 hcs-cli-0.1.27/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.093681 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.096148 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.27/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.097537 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.101967 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      380 2023-04-11 01:00:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.107843 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1289 2023-04-11 00:52:05.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-10 19:14:17.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1693 2023-04-10 21:48:05.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.111851 hcs-cli-0.1.27/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.113119 hcs-cli-0.1.27/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.27/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.115770 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2381 2023-04-10 22:35:04.000000 hcs-cli-0.1.27/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.116993 hcs-cli-0.1.27/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.129155 hcs-cli-0.1.27/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.27/vhcs/common/ctxp/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.132440 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4097 2023-04-10 19:00:11.000000 hcs-cli-0.1.27/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.27/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.27/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.27/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-10 19:10:32.000000 hcs-cli-0.1.27/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.27/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.27/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.138679 hcs-cli-0.1.27/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3866 2023-04-10 22:09:28.000000 hcs-cli-0.1.27/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.27/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.27/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.140877 hcs-cli-0.1.27/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.27/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.148875 hcs-cli-0.1.27/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.27/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.27/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3199 2023-04-11 01:04:04.000000 hcs-cli-0.1.27/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.27/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.27/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.154451 hcs-cli-0.1.27/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2160 2023-04-10 21:32:09.000000 hcs-cli-0.1.27/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.27/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.27/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.26/.gitignore` & `hcs-cli-0.1.27/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/Makefile` & `hcs-cli-0.1.27/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/PKG-INFO` & `hcs-cli-0.1.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.26
+Version: 0.1.27
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
@@ -74,7 +74,17 @@
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
 hcs pki sign-resource-cert my-res1
 ```
+
+LCM command examples
+```
+hcs lcm template create < payload/lcm/zero.json
+hcs lcm template wait --timeout=1m10s <template-id>
+hcs lcm template list --type ZEROCLOUD | jq ".|map(.id)"
+hcs lcm template get <template-id>
+hcs lcm template delete <template-id>
+hcs lcm provider list --type ZEROCLOUD
+```
```

### Comparing `hcs-cli-0.1.26/README.md` & `hcs-cli-0.1.27/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -56,7 +56,17 @@
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
 hcs pki sign-resource-cert my-res1
 ```
+
+LCM command examples
+```
+hcs lcm template create < payload/lcm/zero.json
+hcs lcm template wait --timeout=1m10s <template-id>
+hcs lcm template list --type ZEROCLOUD | jq ".|map(.id)"
+hcs lcm template get <template-id>
+hcs lcm template delete <template-id>
+hcs lcm provider list --type ZEROCLOUD
+```
```

### Comparing `hcs-cli-0.1.26/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.27/hcs_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.26
+Version: 0.1.27
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
@@ -74,7 +74,17 @@
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
 hcs pki sign-resource-cert my-res1
 ```
+
+LCM command examples
+```
+hcs lcm template create < payload/lcm/zero.json
+hcs lcm template wait --timeout=1m10s <template-id>
+hcs lcm template list --type ZEROCLOUD | jq ".|map(.id)"
+hcs lcm template get <template-id>
+hcs lcm template delete <template-id>
+hcs lcm provider list --type ZEROCLOUD
+```
```

### Comparing `hcs-cli-0.1.26/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.27/hcs_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 hcs_cli.egg-info/PKG-INFO
 hcs_cli.egg-info/SOURCES.txt
 hcs_cli.egg-info/dependency_links.txt
 hcs_cli.egg-info/entry_points.txt
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
+payload/lcm/zero.json
 tests/__init__.py
 tests/conftest.py
 tests/test_utils.py
 tests/vhcs/__init__.py
 tests/vhcs/cli/__init__.py
 tests/vhcs/cli/cmds/__init__.py
 tests/vhcs/cli/cmds/test_auth.py
@@ -87,10 +88,11 @@
 vhcs/service/__init__.py
 vhcs/service/_util.py
 vhcs/service/admin.py
 vhcs/service/lcm.py
 vhcs/service/pki.py
 vhcs/service/vmhub.py
 vhcs/util/__init__.py
+vhcs/util/duration.py
 vhcs/util/pki_util.py
 vhcs/util/query_util.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.26/pyproject.toml` & `hcs-cli-0.1.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/setup.py` & `hcs-cli-0.1.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.26"
+VERSION = "0.1.27"
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
     return version
```

### Comparing `hcs-cli-0.1.26/tests/test_utils.py` & `hcs-cli-0.1.27/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-import sys
 import click
 from vhcs.service import lcm
-
-
-@click.command()
-@click.option(
-    "--file",
-    "-f",
-    type=click.File("r"),
-    default=sys.stdin,
-    help="Specify the template file name. If not specified, STDIN will be used.",
-)
-@click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
-def create(file: str, type: str, wait: str):
-    """Create a template"""
-
-    with file:
-        payload = file.read()
-    return lcm.template.create(payload, type)
+from vhcs.util import duration
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@click.option("--status", "-s", type=str, required=False, help="The target status to wait for.")
-@click.option("--timeout", "-t", type=str, required=False, help="Timeout. Examples: '2m', '30s', '1h30m'")
+@click.option("--status", "-s", 
+              type=click.Choice(["READY", "ERROR", "DELETING", "EXPANDING", "SHRINKING", "CUSTOMIZING", "MAINTENANCE"]), 
+              required=False, 
+              default="READY",
+              help="The target status to wait for.")
+@click.option("--timeout", "-t", type=str, required=False, default="1m",
+              help="Timeout. Examples: '2m', '30s', '1h30m'")
 @click.option(
-    "--fail-on-other-termination-status",
+    "--fail-fast/--fail-timeout-only",
     "-f",
     type=bool,
     default=True,
     required=False,
     help="Stop waiting if the template reached to non-expected terminal states, e.g. waiting for ERROR but template is READY, or waiting for READY and template is ERROR.",
 )
-def wait(id: str, status: str, timeout: str, fail_on_other_termination_status: bool):
+@click.option("--silent/--return-template", type=bool, required=False, default=True,
+              help="Slient mode will has no output on success. Otherwise the full template is returned")
+def wait(id: str, status: str, timeout: str, fail_fast: bool, silent: bool):
     """Wait for a template to transit to specific status. If the template"""
 
-    print("TODO")
+    timeout_seconds = duration.to_seconds(timeout)
+    expected_status = status.upper().split(",")
+    exclude_status = []
+    if fail_fast:
+        if "READY" not in expected_status:
+            exclude_status.append("READY")
+        if "ERROR" not in expected_status:
+            exclude_status.append("ERROR")
+    try:
+        template = lcm.template.wait(id, expected_status, timeout_seconds, exclude_status)
+        return template if not silent else None
+    except Exception as e:
+        return str(e), 1
```

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/cli/main.py` & `hcs-cli-0.1.27/vhcs/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env -S python3 -W ignore
 
 import sys
+import json
+import httpx
 import click
 import os.path as path
 import logging
 
 _script_dir = path.abspath(path.join(path.dirname(path.realpath(__file__)), "."))
 _module_dir = path.dirname(_script_dir)
 if __name__ == "__main__":
@@ -52,11 +54,24 @@
 def main():
     try:
         commands_dir = path.join(_module_dir, "cli/cmds")
         config_path = path.join(_module_dir, "config")
         ctxp.init(cli_name="hcs", main_cli=cli, commands_dir=commands_dir, config_path=config_path)
     except ctxp.CtxpException as e:
         ctxp.panic(e)
+    except httpx.HTTPStatusError as e:
+        import traceback
+        traceback.print_exc()
+        try:
+            err = json.loads(e.response.text)
+        except:
+            err = {
+                "message": str(e),
+                "response": e.response.text,
+                "resource": str(e.request.url)
+            }
+        text = json.dumps(err, indent=4)
+        ctxp.panic(text)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.27/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.27/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/logger.py` & `hcs-cli-0.1.27/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.27/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.27/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.27/vhcs/common/sglib/ez_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def _raise_on_4xx_5xx(response: httpx.Response):
     
     if not response.is_success:
         response.read()
         if len(response.text) > 0:
             text = _try_formatting_json(response.text)
-            print(text, file=sys.stderr)
+            log.debug(text)
 
     response.raise_for_status()
 
 
 def _try_formatting_json(text: str):
     try:
         return json.dumps(json.loads(text), indent=4)
```

### Comparing `hcs-cli-0.1.26/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.27/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.27/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/service/_util.py` & `hcs-cli-0.1.27/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/service/admin.py` & `hcs-cli-0.1.27/vhcs/service/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/service/lcm.py` & `hcs-cli-0.1.27/vhcs/service/lcm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import json
 from ._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
 
 
 class template:
@@ -22,24 +23,23 @@
             #filter_fn = lambda t : t.name.find(name) >= 0
             def filter_fn(t):
                 return t.name.find(name) >= 0
             ret = list(filter(filter_fn, ret))
         return ret
 
     @staticmethod
-    def delete(id: str, force: bool):
-        return _client.delete(f"/v1/templates/{id}?force={force}")
+    def delete(id: str, org_id: str, force: bool):
+        resp = _client.delete(f"/v1/templates/{id}?org_id={org_id}&force={force}")
+        return _convert_resp(resp)
 
     @staticmethod
-    def create(payload: str, type: str):
+    def create(template: dict):
         url = "/v1/templates"
-        if type:
-            url += "/" + type
-
-        return _client.post(url, payload)
+        url += "/" + template['providerType'].lower()
+        return _client.post(url=url, json=template)
 
     @staticmethod
     def wait(
         id: str,
         expected_status: list,
         timeout_seconds: int,
         exclude_status: list = ["ERROR"],
@@ -86,12 +86,26 @@
             url = "/v1/providers?" + query_string
             return _client.get(url)
 
         return PageRequest(_get_page, limit, **kwargs).get()
 
     @staticmethod
     def delete(id: str):
-        return _client.delete(f"/v1/providers/{id}")
+        resp = _client.delete(f"/v1/providers/{id}")
+        return _convert_resp(resp)
 
 
+    @staticmethod
+    def create(data: dict):
+        url = "/v1/providers/" + data['type'].lower()
+        return _client.post(url, json=data)
+
+def _convert_resp(resp):
+    if resp:
+        resp.read()
+        try:
+            json.loads(resp.text)
+        except:
+            return resp.text
+        
 def test():
     print("test")
```

### Comparing `hcs-cli-0.1.26/vhcs/service/pki.py` & `hcs-cli-0.1.27/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/service/vmhub.py` & `hcs-cli-0.1.27/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/util/pki_util.py` & `hcs-cli-0.1.27/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/util/query_util.py` & `hcs-cli-0.1.27/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.26/vhcs/util/versions.py` & `hcs-cli-0.1.27/vhcs/util/versions.py`

 * *Files identical despite different names*

