# Comparing `tmp/ansible-risk-insight-0.1.2.tar.gz` & `tmp/ansible-risk-insight-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.2.tar", last modified: Tue Apr 11 08:46:19 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.2rc1.tar", last modified: Mon Apr 10 02:38:49 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.2.tar` & `ansible-risk-insight-0.1.2rc1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.097323 ansible-risk-insight-0.1.2/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.032280 ansible-risk-insight-0.1.2/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.038473 ansible-risk-insight-0.1.2/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.2/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-04-11 08:46:19.097172 ansible-risk-insight-0.1.2/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.050806 ansible-risk-insight-0.1.2/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      659 2023-04-11 08:43:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.053965 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.059036 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9100 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.059206 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7294 2023-04-11 08:43:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.061003 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31556 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-10 01:04:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    10390 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    59635 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    73975 2023-04-10 01:06:00.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5452 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    40317 2023-04-11 08:43:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8059 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.076005 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4041 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-03 07:57:55.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46288 2023-04-11 08:43:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38620 2023-04-11 08:43:40.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.051882 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-11 08:46:18.000000 ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.033085 ansible-risk-insight-0.1.2/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.084660 ansible-risk-insight-0.1.2/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.089109 ansible-risk-insight-0.1.2/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.2/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.2/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.092694 ansible-risk-insight-0.1.2/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.093334 ansible-risk-insight-0.1.2/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.093720 ansible-risk-insight-0.1.2/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.094055 ansible-risk-insight-0.1.2/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.2/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-11 08:46:19.097379 ansible-risk-insight-0.1.2/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.094383 ansible-risk-insight-0.1.2/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.034285 ansible-risk-insight-0.1.2/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.033812 ansible-risk-insight-0.1.2/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.095250 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.033962 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.034195 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.095562 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.095810 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.096103 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.034341 ansible-risk-insight-0.1.2/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.034568 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.096392 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.096650 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-11 08:46:19.096888 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.2/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.711360 ansible-risk-insight-0.1.2rc1/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.640038 ansible-risk-insight-0.1.2rc1/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.650149 ansible-risk-insight-0.1.2rc1/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.2rc1/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.711165 ansible-risk-insight-0.1.2rc1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.662224 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-10 02:37:44.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.666080 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673412 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9100 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673765 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7085 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.676236 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31556 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-10 01:04:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    10390 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    59635 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    73975 2023-04-10 01:06:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5452 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    40173 2023-04-10 02:35:50.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8059 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.695936 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4041 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-03 07:57:55.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46105 2023-04-04 16:17:13.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38570 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.663637 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.641546 ansible-risk-insight-0.1.2rc1/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.698915 ansible-risk-insight-0.1.2rc1/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.701207 ansible-risk-insight-0.1.2rc1/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.2rc1/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.2rc1/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706182 ansible-risk-insight-0.1.2rc1/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706828 ansible-risk-insight-0.1.2rc1/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707275 ansible-risk-insight-0.1.2rc1/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707614 ansible-risk-insight-0.1.2rc1/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.2rc1/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-10 02:38:49.711431 ansible-risk-insight-0.1.2rc1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707948 ansible-risk-insight-0.1.2rc1/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643942 ansible-risk-insight-0.1.2rc1/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643004 ansible-risk-insight-0.1.2rc1/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.708757 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643287 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643774 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709171 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709470 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709826 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644092 ansible-risk-insight-0.1.2rc1/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644604 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710133 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710436 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710765 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.2rc1/tox.ini
```

### Comparing `ansible-risk-insight-0.1.2/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/.github/workflows/test.yml` & `ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/.gitignore` & `ansible-risk-insight-0.1.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/CONTRIBUTING.md` & `ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/LICENSE` & `ansible-risk-insight-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/README.md` & `ansible-risk-insight-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.1.2-rc1"
```

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         parser.add_argument("--taskfile-only", action="store_true", help="if true, don't load playbooks/roles arround the specified taskfile")
         parser.add_argument("--skip-install", action="store_true", help="if true, skip install for the specified target")
         parser.add_argument("--dependency-dir", nargs="?", help="path to a directory that have dependencies for the target")
         parser.add_argument("--collection-name", nargs="?", help="if provided, use it as a collection name")
         parser.add_argument("--role-name", nargs="?", help="if provided, use it as a role name")
         parser.add_argument("--source", help="source server name in ansible config file (if empty, use public ansible galaxy)")
         parser.add_argument("--without-ram", action="store_true", help="if true, RAM data is not used and not even updated")
-        parser.add_argument("--read-only-ram", action="store_true", help="if true, RAM data is used but not updated")
         parser.add_argument("--read-ram-for-dependency", action="store_true", help="if true, RAM data is used only for dependency")
         parser.add_argument("--update-ram", action="store_true", help="if true, RAM data is not used for scan but updated with the scan result")
         parser.add_argument("--include-tests", action="store_true", help='if true, load test contents in "tests/integration/targets"')
         parser.add_argument("--silent", action="store_true", help='if true, do not print anything"')
         parser.add_argument("--objects", action="store_true", help="if true, output objects.json to the output directory")
         parser.add_argument("--show-all", action="store_true", help="if true, show findings even if missing dependencies are found")
         parser.add_argument("--json", help="if specified, show findings in json format")
@@ -115,17 +114,14 @@
 
         read_ram = True
         write_ram = True
         read_ram_for_dependency = False
         if args.without_ram:
             read_ram = False
             write_ram = False
-        elif args.read_only_ram:
-            read_ram = True
-            write_ram = False
         elif args.update_ram:
             read_ram = False
             write_ram = True
         elif args.read_ram_for_dependency:
             read_ram_for_dependency = True
             read_ram = False
             write_ram = False
```

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,16 @@
                 self.role_index = json.load(file)
 
         taskfile_index_path = os.path.join(self.root_dir, "indices", taskfile_index_name)
         if os.path.exists(taskfile_index_path):
             with open(taskfile_index_path, "r") as file:
                 self.taskfile_index = json.load(file)
 
+        self.init_findings_json_list_cache()
+
     def clear_old_cache(self):
         size = self.max_cache_size
         self._remove_old_item(self.findings_cache, size)
         self._remove_old_item(self.findings_search_cache, size)
         self._remove_old_item(self.module_search_cache, size)
         self._remove_old_item(self.role_search_cache, size)
         self._remove_old_item(self.taskfile_search_cache, size)
@@ -769,16 +771,14 @@
         search_patterns = os.path.join(self.root_dir, "roles", "findings", "*", "*", "*", "findings.json")
         findings_json_list_role = safe_glob(search_patterns)
         findings_json_list_role = sort_by_version(findings_json_list_role)
         findings_json_list = findings_json_list_coll + findings_json_list_role
         self.findings_json_list_cache = findings_json_list
 
     def list_all_ram_metadata(self):
-        if not self.findings_json_list_cache:
-            self.init_findings_json_list_cache()
         findings_json_list = self.findings_json_list_cache
 
         metadata_list = []
         for findings_path in findings_json_list:
             parts = findings_path.split("/")
 
             metadata_list.append(
@@ -788,16 +788,14 @@
                     "version": parts[-3],
                     "hash": parts[-2],
                 }
             )
         return metadata_list
 
     def search_findings(self, target_name, target_version, target_type=None):
-        if not self.findings_json_list_cache:
-            self.init_findings_json_list_cache()
         args_str = json.dumps([target_name, target_version, target_type])
         if args_str in self.findings_search_cache:
             return self.findings_search_cache[args_str]
 
         if not target_name:
             raise ValueError("target name must be specified for searching RAM data")
         if not target_version:
```

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,15 +723,15 @@
     root_dir: str = ""
     rules_dir: str = ""
     rules: list = field(default_factory=list)
 
     ram_client: RAMClient = None
     read_ram: bool = True
     read_ram_for_dependency: bool = True
-    write_ram: bool = False
+    write_ram: bool = True
 
     persist_dependency_cache: bool = False
 
     skip_playbook_format_error: bool = (True,)
     skip_task_format_error: bool = (True,)
 
     use_ansible_doc: bool = True
@@ -840,15 +840,15 @@
             _parser=self._parser,
         )
         self._current = scandata
         self.record_end(time_records, "scandata_init")
 
         self.record_begin(time_records, "metadata_load")
         metdata_loaded = False
-        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
+        if self.read_ram:
             loaded, metadata, dependencies = self.load_metadata_from_ram(scandata.type, scandata.name, scandata.version)
             logger.debug(f"metadata loaded: {loaded}")
             if loaded:
                 scandata.set_metadata(metadata, dependencies)
                 metdata_loaded = True
                 if not self.silent:
                     logger.debug(f'Use metadata for "{scandata.name}" in RAM DB')
@@ -948,15 +948,15 @@
         # scandata.prm["playbooks"] = playbooks
         # scandata.prm["roles"] = roles
         # scandata.prm["modules"] = modules
         self.record_end(time_records, "prm_load")
 
         loaded = False
         self.record_begin(time_records, "target_load")
-        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
+        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE]:
             loaded, root_defs = self.load_definitions_from_ram(scandata.type, scandata.name, scandata.version, scandata.hash, allow_unresolved=True)
             logger.debug(f"spec data loaded: {loaded}")
             if loaded:
                 scandata.root_definitions = root_defs
                 if not self.silent:
                     logger.info("Use spec data in RAM DB")
         self.record_end(time_records, "target_load")
@@ -1019,15 +1019,15 @@
         dep_num, ext_counts, root_counts = scandata.count_definitions()
         if not self.silent:
             print("# of dependencies:", dep_num)
             # print("ext definitions:", ext_counts)
             # print("root definitions:", root_counts)
 
         # save RAM data
-        if self.write_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
+        if self.write_ram:
             self.register_findings_to_ram(scandata.findings)
             self.register_indices_to_ram(scandata.findings, include_test_contents)
 
         if scandata.out_dir is not None and scandata.out_dir != "":
             self.save_rule_result(scandata.findings, scandata.out_dir)
             if not self.silent:
                 print("The rule result is saved at {}".format(scandata.out_dir))
```

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,21 +488,19 @@
     def _recursive_get_calls(self, key, caller=None, handover={}, index=0, history=[]):
         obj_list = ObjectList()
         obj = self.get_object(key)
         if obj is None:
             return obj_list
         if key in history:
             return obj_list
-        _history = []
-        if history:
-            _history = [h for h in history]
+        _history = deepcopy(history)
         call_obj = call_obj_from_spec(spec=obj, caller=caller, index=index)
         if call_obj is not None:
             obj_list.add(call_obj, update_dict=False)
-            _history.append(key)
+            history.append(key)
         children_keys, from_ram, handover = self._get_children_keys(obj, handover_from_upper_node=handover)
         for i, c_key in enumerate(children_keys):
             child_objects = self._recursive_get_calls(
                 c_key,
                 call_obj,
                 handover,
                 i,
```

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/data-struct.txt` & `ansible-risk-insight-0.1.2rc1/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/annotation.md` & `ansible-risk-insight-0.1.2rc1/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/customize_rules.md` & `ansible-risk-insight-0.1.2rc1/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/example/readme.md` & `ansible-risk-insight-0.1.2rc1/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/example/sample.py` & `ansible-risk-insight-0.1.2rc1/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/mkdocs.yml` & `ansible-risk-insight-0.1.2rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/pyproject.toml` & `ansible-risk-insight-0.1.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/test/test_scanner.py` & `ansible-risk-insight-0.1.2rc1/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2/tox.ini` & `ansible-risk-insight-0.1.2rc1/tox.ini`

 * *Files identical despite different names*

