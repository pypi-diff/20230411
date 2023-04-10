# Comparing `tmp/iambic_core-0.1.186.tar.gz` & `tmp/iambic_core-0.1.198.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.1.186.tar", max compression
+gzip compressed data, was "iambic_core-0.1.198.tar", max compression
```

## Comparing `iambic_core-0.1.186.tar` & `iambic_core-0.1.198.tar`

### file list

```diff
@@ -1,151 +1,150 @@
--rw-r--r--   0        0        0    11356 2023-03-30 00:04:26.638385 iambic_core-0.1.186/LICENSE.md
--rw-r--r--   0        0        0     9395 2023-03-31 02:03:03.449971 iambic_core-0.1.186/README.md
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.836548 iambic_core-0.1.186/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.836659 iambic_core-0.1.186/iambic/config/__init__.py
--rw-r--r--   0        0        0    20072 2023-03-28 21:23:30.300844 iambic_core-0.1.186/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-03-07 17:56:58.837134 iambic_core-0.1.186/iambic/config/templates.py
--rw-r--r--   0        0        0     1755 2023-03-28 21:23:30.301364 iambic_core-0.1.186/iambic/config/utils.py
--rw-r--r--   0        0        0    67720 2023-03-28 22:59:25.918655 iambic_core-0.1.186/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.837983 iambic_core-0.1.186/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-03-15 23:50:56.365863 iambic_core-0.1.186/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-03-14 00:53:04.719470 iambic_core-0.1.186/iambic/core/context.py
--rw-r--r--   0        0        0      451 2023-03-07 17:56:58.838334 iambic_core-0.1.186/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-03-28 21:23:30.302234 iambic_core-0.1.186/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-03-28 21:54:29.527958 iambic_core-0.1.186/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-03-28 21:23:30.302397 iambic_core-0.1.186/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-03-07 17:56:58.838997 iambic_core-0.1.186/iambic/core/logger.py
--rw-r--r--   0        0        0    23878 2023-03-30 00:04:26.647877 iambic_core-0.1.186/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-03-07 17:56:58.839309 iambic_core-0.1.186/iambic/core/noq_json.py
--rw-r--r--   0        0        0     4016 2023-03-07 17:56:58.839416 iambic_core-0.1.186/iambic/core/parser.py
--rw-r--r--   0        0        0    42095 2023-03-28 21:54:29.528195 iambic_core-0.1.186/iambic/core/template_generation.py
--rw-r--r--   0        0        0    24151 2023-03-30 00:04:26.648377 iambic_core-0.1.186/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.841073 iambic_core-0.1.186/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-03-07 17:56:58.841236 iambic_core-0.1.186/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-03-30 00:04:26.648749 iambic_core-0.1.186/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-03-15 23:50:56.367291 iambic_core-0.1.186/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-03-07 17:56:58.841927 iambic_core-0.1.186/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-03-07 17:56:58.842093 iambic_core-0.1.186/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.842199 iambic_core-0.1.186/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-03-14 00:53:04.721758 iambic_core-0.1.186/iambic/lambda/app.py
--rw-r--r--   0        0        0    13622 2023-03-30 00:04:26.649186 iambic_core-0.1.186/iambic/main.py
--rw-r--r--   0        0        0      626 2023-03-30 00:04:26.649419 iambic_core-0.1.186/iambic/output/__init__.py
--rw-r--r--   0        0        0     2667 2023-03-30 00:04:26.649554 iambic_core-0.1.186/iambic/output/filters.py
--rw-r--r--   0        0        0      489 2023-03-30 00:04:26.649778 iambic_core-0.1.186/iambic/output/markdown.py
--rw-r--r--   0        0        0    12407 2023-03-30 00:04:26.649930 iambic_core-0.1.186/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-03-30 00:04:26.650200 iambic_core-0.1.186/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-03-30 00:04:26.650940 iambic_core-0.1.186/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-03-30 00:04:26.651124 iambic_core-0.1.186/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1049 2023-03-30 00:04:26.651221 iambic_core-0.1.186/iambic/output/text.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.842549 iambic_core-0.1.186/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-03-07 17:56:58.842663 iambic_core-0.1.186/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.842738 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.842825 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1670 2023-03-07 17:56:58.842988 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     1715 2023-03-15 23:50:56.367954 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     1888 2023-03-07 17:56:58.843184 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-03-07 17:56:58.843284 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    12863 2023-03-09 22:35:37.339953 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.843531 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-03-19 19:43:57.432601 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    28181 2023-03-30 00:04:26.651628 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.843943 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.844073 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10710 2023-03-30 00:04:26.653781 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17636 2023-03-28 21:54:29.530096 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    12688 2023-03-30 00:04:26.654012 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-03-28 21:23:30.306170 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.844785 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15807 2023-03-30 00:04:26.654213 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17497 2023-03-30 00:04:26.654782 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10302 2023-03-30 00:04:26.655061 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-03-28 21:23:30.307348 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16988 2023-03-30 00:04:26.655452 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21318 2023-03-28 21:54:29.530515 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    22587 2023-03-30 00:04:26.655669 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.845855 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14755 2023-03-30 00:04:26.655830 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20576 2023-03-28 21:54:29.530804 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    21317 2023-03-30 00:04:26.656019 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4307 2023-03-28 21:23:30.309772 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-03-07 17:56:58.846909 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.846955 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.847040 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    29917 2023-03-30 00:04:26.656185 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20166 2023-03-28 21:54:29.530992 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    34960 2023-03-30 00:04:26.656487 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    26580 2023-03-29 02:14:19.005542 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-03-07 17:56:58.848567 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.848675 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.848752 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0        0 2023-03-15 23:50:56.370636 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    31917 2023-03-15 20:12:13.923966 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/broken_test_access_model.py
--rw-r--r--   0        0        0    11950 2023-03-28 21:23:30.313929 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-03-28 21:23:30.315138 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    12087 2023-03-28 21:54:29.531772 iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-03-28 21:23:30.316766 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 21:23:30.316852 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13619 2023-03-29 02:14:19.006683 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-03-28 21:54:29.531940 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14928 2023-03-30 00:04:26.657263 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-03-28 21:23:30.319207 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-03-28 21:23:30.319707 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8282 2023-03-28 21:23:30.319954 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-03-28 21:23:30.320025 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8629 2023-03-29 02:14:19.008082 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-03-28 21:54:29.532057 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7180 2023-03-30 00:04:26.657669 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-03-28 21:23:30.321323 iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-03-07 17:56:58.849037 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.849083 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-03-07 17:56:58.849189 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      788 2023-03-15 20:18:50.019550 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.849387 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-03-28 21:23:30.321597 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.849590 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     1690 2023-03-28 21:23:30.321863 iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      195 2023-03-07 17:56:58.849840 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.849887 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-03-30 00:04:26.658146 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-03-30 00:04:26.658521 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-03-28 21:23:30.322725 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-03-15 20:23:29.389228 iambic_core-0.1.186/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-03-09 14:55:43.896928 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 14:55:43.897014 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9835 2023-03-30 00:04:26.659022 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-03-28 21:54:29.532299 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-03-30 00:04:26.659876 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-03-09 14:55:43.897451 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5066 2023-03-28 21:23:30.323431 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-03-28 21:23:30.323595 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-03-09 14:55:43.897824 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 21:23:30.323647 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7797 2023-03-28 21:23:30.323776 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-03-28 21:23:30.323888 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-03-29 02:14:19.010096 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-03-28 21:23:30.324622 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-03-28 21:23:30.324743 iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.853172 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.853664 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9430 2023-03-30 00:04:26.660104 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-03-28 21:54:29.532804 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17908 2023-03-30 00:04:26.660387 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-03-07 17:56:58.854799 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.854896 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11241 2023-03-30 00:04:26.660932 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-03-28 21:54:29.533054 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    19760 2023-03-30 00:04:26.661582 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-03-09 14:55:43.898504 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2732 2023-03-29 02:14:19.016571 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-03-29 02:14:19.017140 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-03-07 17:56:58.855691 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.855783 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9337 2023-03-30 00:04:26.661925 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-03-28 21:54:29.533322 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13806 2023-03-30 00:04:26.662332 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-03-18 20:44:10.215825 iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 17:56:58.857082 iambic_core-0.1.186/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      878 2023-03-07 17:56:58.857188 iambic_core-0.1.186/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-03-28 21:23:30.328662 iambic_core-0.1.186/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-03-28 21:23:30.328787 iambic_core-0.1.186/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0     1924 2023-03-31 02:03:03.451857 iambic_core-0.1.186/pyproject.toml
--rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 iambic_core-0.1.186/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-10 23:07:45.632792 iambic_core-0.1.198/LICENSE.md
+-rw-r--r--   0        0        0     9696 2023-04-10 23:07:45.632792 iambic_core-0.1.198/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20072 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/templates.py
+-rw-r--r--   0        0        0     1755 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/utils.py
+-rw-r--r--   0        0        0    67671 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/context.py
+-rw-r--r--   0        0        0      451 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/logger.py
+-rw-r--r--   0        0        0    24753 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     4744 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/parser.py
+-rw-r--r--   0        0        0    42095 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    24381 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13644 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/main.py
+-rw-r--r--   0        0        0      628 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2763 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/text.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1670 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     1715 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     1888 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    12863 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    29881 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10478 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17642 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13596 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15802 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17502 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10795 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16584 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21322 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    22598 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    15144 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20581 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    21982 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4307 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    29547 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20166 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35114 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    26441 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    12155 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13737 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8455 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8619 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      788 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     1690 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      195 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5066 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9404 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11354 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    19759 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2687 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9307 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13806 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      878 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0     1924 2023-04-10 23:07:45.664792 iambic_core-0.1.198/pyproject.toml
+-rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 iambic_core-0.1.198/PKG-INFO
```

### Comparing `iambic_core-0.1.186/LICENSE.md` & `iambic_core-0.1.198/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/README.md` & `iambic_core-0.1.198/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
+[![codecov.io](https://codecov.io/github/noqdev/iambic/coverage.svg?branch=main)](https://codecov.io/github/noqdev/iambic?branch=main)
 
 # IAMbic: Cloud IAM as Code
 
 "IAMbic: the Terraform of Cloud IAM"
 
 Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://www.iambic.org](https://www.iambic.org).
 
@@ -17,14 +18,24 @@
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
 ## Getting Started
 
 Dive into IAMbic with our [quick-start guide](http://iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
+## Installing IAMbic and Supported Versions
+
+IAMbic is available on PyPI:
+
+```console
+python -m pip install iambic-core
+```
+
+IAMbic officially supports Python 3.9+.
+
 ### Template Examples
 
 Here are some examples showcasing IAMbic's capabilities:
 
 #### AWS Multi-Account Cloudwatch Role
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
```

### Comparing `iambic_core-0.1.186/iambic/config/dynamic_config.py` & `iambic_core-0.1.198/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/config/utils.py` & `iambic_core-0.1.198/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/config/wizard.py` & `iambic_core-0.1.198/iambic/config/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,17 +741,18 @@
             )
             return
 
         is_hub_account = bool(
             not self.config.aws.accounts and not self.config.aws.organizations
         )
         requires_sync = bool(
-            not is_hub_account and (
-                    len(self.config.aws.accounts)
-                    > self.config.aws.min_accounts_required_for_wildcard_included_accounts
+            not is_hub_account
+            and (
+                len(self.config.aws.accounts)
+                > self.config.aws.min_accounts_required_for_wildcard_included_accounts
             )
         )
 
         if is_hub_account:
             account_id = self.hub_account_id
             account_name = set_required_text_value(
                 "What is the name of the AWS Account?"
@@ -846,17 +847,15 @@
             iambic_managed=IambicManaged.READ_AND_WRITE,
             aws_profile=profile_name,
         )
         if is_hub_account:
             account.hub_role_arn = get_hub_role_arn(account_id)
         # account.partition = set_aws_account_partition(account.partition)
 
-        confirm_command_exe(
-            "AWS Account", Operation.ADDED, requires_sync=requires_sync
-        )
+        confirm_command_exe("AWS Account", Operation.ADDED, requires_sync=requires_sync)
 
         self.config.aws.accounts.append(account)
 
         if is_hub_account:
             check_and_update_resource_limit(self.config)
             asyncio.run(self.run_import_aws_resources())
         else:
@@ -1025,15 +1024,14 @@
         if not created_successfully:
             log.error("Failed to create the required IAMbic roles. Exiting.")
             sys.exit(0)
 
         aws_org = AWSOrganization(
             org_id=org_id,
             org_account_id=account_id,
-            region=org_region,
             default_rule=BaseAWSOrgRule(),
             hub_role_arn=get_hub_role_arn(account_id),
             aws_profile=profile_name,
         )
         aws_org.default_rule.iambic_managed = IambicManaged.READ_AND_WRITE
 
         self.config.aws.organizations.append(aws_org)
```

### Comparing `iambic_core-0.1.186/iambic/core/aio_utils/__init__.py` & `iambic_core-0.1.198/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/git.py` & `iambic_core-0.1.198/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/iambic_enum.py` & `iambic_core-0.1.198/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/iambic_plugin.py` & `iambic_core-0.1.198/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/logger.py` & `iambic_core-0.1.198/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/models.py` & `iambic_core-0.1.198/iambic/core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import inspect
 import itertools
 import json
 import os
 import typing
 from enum import Enum
 from hashlib import md5
+from pathlib import Path
 from types import GenericAlias
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
@@ -25,15 +26,15 @@
 
 import aiofiles
 import dateparser
 from deepdiff.model import PrettyOrderedSet
 from git import Repo
 from jinja2 import BaseLoader, Environment
 from pydantic import BaseModel as PydanticBaseModel
-from pydantic import Extra, Field, root_validator, schema,  validate_model, validator
+from pydantic import Extra, Field, root_validator, schema, validate_model, validator
 from pydantic.fields import ModelField
 
 from iambic.core.iambic_enum import Command, ExecutionStatus, IambicManaged
 from iambic.core.logger import log
 from iambic.core.utils import (
     apply_to_provider,
     create_commented_map,
@@ -341,28 +342,40 @@
             else:
                 self.proposed_changes.append(change)
 
 
 class TemplateChangeDetails(PydanticBaseModel):
     resource_id: str
     resource_type: str
-    template_path: str
+    template_path: Union[str, Path]
     # Supports multi-account providers and single-account providers
     proposed_changes: list[Union[AccountChangeDetails, ProposedChange]] = []
     exceptions_seen: list[Union[AccountChangeDetails, ProposedChange]] = Field(
         default=[]
     )
 
     class Config:
         json_encoders = {PrettyOrderedSet: list}
         extra = Extra.forbid
 
+    @validator("template_path")
+    def validate_template_path(cls, v: Union[str, Path]):
+        return str(v)
+
     def extend_changes(self, changes: list[ProposedChange]):
         for change in changes:
             if change.exceptions_seen:
+                if isinstance(change, AccountChangeDetails) and change.proposed_changes:
+                    # If there was a partial failure then split the successes into their own change
+                    proposed_change = change.copy()
+                    proposed_change.exceptions_seen = []
+                    self.proposed_changes.append(proposed_change)
+                    change.proposed_changes = (
+                        []
+                    )  # Remove the proposed changes from the original change
                 self.exceptions_seen.append(change)
             elif isinstance(change, AccountChangeDetails) and change.proposed_changes:
                 self.proposed_changes.append(change)
             elif isinstance(change, ProposedChange):
                 self.proposed_changes.append(change)
 
     def dict(
@@ -464,15 +477,15 @@
         )
 
 
 class BaseTemplate(
     BaseModel,
 ):
     template_type: str
-    file_path: str = Field(..., hidden_from_schema=True)
+    file_path: Union[str, Path] = Field(..., hidden_from_schema=True)
     owner: Optional[str]
     iambic_managed: Optional[IambicManaged] = Field(
         IambicManaged.UNDEFINED,
         description="Controls the directionality of Iambic changes",
     )
 
     def dict(
@@ -532,15 +545,21 @@
 
     def delete(self):
         log.info("Deleting template file", file_path=self.file_path)
         try:
             repo = Repo(self.file_path, search_parent_directories=True)
             # why force=True? Expire could have modified the local contents
             # without force=True, git rm would not be able to remove the file
-            repo.index.remove([self.file_path], working_tree=True, force=True)
+            repo.index.remove(
+                [
+                    str(self.file_path)
+                ],  # manual cast to str is necessary because git library only accepts str and not FilePath
+                working_tree=True,
+                force=True,
+            )
         except Exception as e:
             log.error(
                 "Unable to remove file from local Git repo. Deleting manually",
                 error=e,
                 file_path=self.file_path,
             )
             os.remove(self.file_path)
```

### Comparing `iambic_core-0.1.186/iambic/core/noq_json.py` & `iambic_core-0.1.198/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/parser.py` & `iambic_core-0.1.198/iambic/core/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import json
 import traceback
+from functools import partial
+from multiprocessing import Pool, cpu_count
 from typing import Union
 
 from pydantic import ValidationError
 from ruamel.yaml.scanner import ScannerError
 
 from iambic.config.templates import TEMPLATES
 from iambic.core.logger import log
@@ -61,42 +63,59 @@
         return "\n".join(lines)
     except Exception:
         # need to still return something to avoid to downstream formatting
         captured_traceback = traceback.format_exc()
         return f"Unable to compute hints: {captured_traceback}"
 
 
+def load_template(template_path: str, raise_validation_err: bool = True) -> dict:
+    try:
+        template_dict = transform_comments(yaml.load(open(template_path)))
+        template_type = template_dict.get("template_type")
+        if template_type and template_type not in ["NOQ::Core::Config"]:
+            template_dict["file_path"] = template_path
+            return template_dict
+    except ScannerError as err:
+        log.critical(
+            "Invalid template structure", file_path=template_path, error=repr(err)
+        )
+        if raise_validation_err:
+            raise ValueError(f"{template_path} template has validation error.") from err
+
+
 def load_templates(
     template_paths: list[str], raise_validation_err: bool = True
 ) -> list[BaseTemplate]:
     templates = []
+    load_template_fn = partial(load_template, raise_validation_err=raise_validation_err)
+    with Pool(max(1, cpu_count() // 2)) as p:
+        template_dicts = p.map(load_template_fn, template_paths)
+
+    for template_dict in template_dicts:
+        if not template_dict:
+            continue
 
-    for template_path in template_paths:
         try:
-            template_dict = transform_comments(yaml.load(open(template_path)))
-            if template_dict["template_type"] in ["NOQ::Core::Config"]:
-                continue
             template_cls = TEMPLATES.template_map[template_dict["template_type"]]
             template_cls.update_forward_refs()
-            templates.append(template_cls(file_path=template_path, **template_dict))
+            templates.append(template_cls(**template_dict))
         except KeyError:
             log.critical(
                 "Invalid template type",
-                file_path=template_path,
+                file_path=template_dict["file_path"],
                 template_type=template_dict["template_type"],
             )
             # We should allow to continue to allow unknown template type; otherwise,
             # we cannot support forward or backward compatibility during version changes.
-        except (ValidationError, ScannerError) as err:
+        except ValidationError as err:
             log.critical(
-                "Invalid template structure", file_path=template_path, error=repr(err)
+                "Invalid template structure",
+                file_path=template_dict["file_path"],
+                error=repr(err),
             )
             if raise_validation_err:
-                if isinstance(err, ValidationError):
-                    hints = format_validation_error(err, template_dict)
-                else:
-                    hints = ""
+                hints = format_validation_error(err, template_dict)
                 raise ValueError(
-                    f"{template_path} template has validation error. \n{hints}"
+                    f"{template_dict['file_path']} template has validation error. \n{hints}"
                 ) from err
 
     return templates
```

### Comparing `iambic_core-0.1.186/iambic/core/template_generation.py` & `iambic_core-0.1.198/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/core/utils.py` & `iambic_core-0.1.198/iambic/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
-import glob
 import os
 import pathlib
 import re
 import sys
 import tempfile
 import typing
 from datetime import date, datetime
 from io import StringIO
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Coroutine, Optional, Union
 from urllib.parse import unquote_plus
 
 import aiofiles
 from asgiref.sync import sync_to_async
 from ruamel.yaml import YAML
 
@@ -78,21 +78,20 @@
     ).title()  # normalize string and add required case convention
     return str_obj.replace("_", "")  # Remove underscores
 
 
 async def plugin_apply_wrapper(
     apply_awaitable: Coroutine, proposed_changes: list[ProposedChange]
 ) -> list[ProposedChange]:
-    exceptions = []
     try:
         await apply_awaitable
     except Exception as e:
-        exceptions.append(str(e))
-    for change in proposed_changes:
-        change.exceptions_seen = exceptions
+        for change in proposed_changes:
+            change.exceptions_seen.append(str(e))
+
     return proposed_changes
 
 
 async def resource_file_upsert(
     file_path: Union[str, pathlib.Path],
     content_as_dict: dict,
     replace_file: bool = False,
@@ -123,39 +122,48 @@
             content_dict = json.loads(await f.read())
             content_as_dict = {**content_dict, **content_as_dict}
 
     async with aiofiles.open(file_path, mode="w") as f:
         await f.write(json.dumps(content_as_dict, indent=2))
 
 
-async def file_regex_search(file_path: str, re_pattern: str) -> Union[str, None]:
+async def file_regex_search(
+    file_path: Union[str, Path], re_pattern: str
+) -> Union[str, None]:
     async with aiofiles.open(file_path, mode="r") as f:
         file_content = await f.read()
         if re.search(re_pattern, file_content):
             return file_path
 
 
 async def gather_templates(repo_dir: str, template_type: str = None) -> list[str]:
+    repo_dir_path = Path(repo_dir)
+    if not repo_dir_path.is_dir():
+        raise ValueError(f"{repo_dir_path} is not a directory")
+
     if template_type and template_type.startswith("NOQ::"):
         # Strip the prefix, so it plays nice with NOQ_TEMPLATE_REGEX
         template_type = template_type.replace("NOQ::", "")
 
     regex_pattern = (
         rf"{NOQ_TEMPLATE_REGEX}.*{template_type}"
         if template_type
         else NOQ_TEMPLATE_REGEX
     )
+    # since multiple glob pattern can potential intersect, we use a set data structure
+    # to suppress any duplicate for defensive measure
     # Support both yaml and yml extensions for templates
-    file_paths = glob.glob(f"{repo_dir}/**/*.yaml", recursive=True)
-    file_paths += glob.glob(f"{repo_dir}*.yaml", recursive=True)
-    file_paths += glob.glob(f"{repo_dir}/**/*.yml", recursive=True)
-    file_paths += glob.glob(f"{repo_dir}*.yml", recursive=True)
+    file_path_set = set()
+    # >>> glob.glob('**/*.txt', recursive=True)
+    # ['2.txt', 'sub/3.txt']
+    file_path_set.update(repo_dir_path.glob("**/*.yaml"))
+    file_path_set.update(repo_dir_path.glob("**/*.yml"))
 
     file_paths = await gather_limit(
-        *[file_regex_search(fp, regex_pattern) for fp in file_paths],
+        *[file_regex_search(fp, regex_pattern) for fp in file_path_set],
         limit=int(os.environ.get("IAMBIC_GATHER_TEMPLATES_LIMIT", 10)),
     )
     return [fp for fp in file_paths if fp]
 
 
 async def aio_wrapper(fnc, *args, **kwargs):
     thread_sensitive = kwargs.pop("thread_sensitive", False)
@@ -207,15 +215,15 @@
             return_exceptions=return_exceptions,
         )
 
 
 async def async_batch_processor(
     tasks: list,
     batch_size: int,
-    seconds_between_process: Union[int, float] = 1,
+    seconds_between_process: Union[int, float, None] = None,
     return_exceptions: bool = False,
 ) -> list:
     """
     Batches up tasks in an effort to prevent rate limiting
     """
     if len(tasks) <= batch_size:
         return await asyncio.gather(*tasks, return_exceptions=return_exceptions)
```

### Comparing `iambic_core-0.1.186/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.1.198/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.1.198/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.1.198/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/github/templates/iambic-import.yml` & `iambic_core-0.1.198/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/github/utils.py` & `iambic_core-0.1.198/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/lambda/app.py` & `iambic_core-0.1.198/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/main.py` & `iambic_core-0.1.198/iambic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,23 @@
 from iambic.config.wizard import ConfigurationWizard
 from iambic.core.context import ctx
 from iambic.core.git import clone_git_repos
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage, TemplateChangeDetails
 from iambic.core.parser import load_templates
-from iambic.core.utils import exceptions_in_proposed_changes, gather_templates, init_writable_directory
-from iambic.output.text import file_render_resource_changes, screen_render_resource_changes
+from iambic.core.utils import (
+    exceptions_in_proposed_changes,
+    gather_templates,
+    init_writable_directory,
+)
+from iambic.output.text import (
+    file_render_resource_changes,
+    screen_render_resource_changes,
+)
 from iambic.request_handler.expire_resources import flag_expired_resources
 from iambic.request_handler.git_apply import apply_git_changes
 from iambic.request_handler.git_plan import plan_git_changes
 
 warnings.filterwarnings("ignore", category=FutureWarning, module="botocore.client")
 
 os.environ.setdefault("IAMBIC_REPO_DIR", str(pathlib.Path.cwd()))
@@ -43,17 +50,15 @@
         output_path = "proposed_changes.txt"
     if template_changes:
         log.info(f"A detailed summary of changes has been saved to {output_path}")
         file_render_resource_changes(output_path, template_changes)
 
     json_filepath = pathlib.Path(output_path).with_suffix(".json")
     with open(str(json_filepath), "w") as fp:
-        json.dump(
-            [template_change.dict() for template_change in template_changes], fp
-        )
+        json.dump([template_change.dict() for template_change in template_changes], fp)
 
     if exceptions_in_proposed_changes([change.dict() for change in template_changes]):
         log.error(
             "Exceptions encountered. Some operations failed. Please read proposed_changes for details."
         )
         if exit_on_error:
             raise SystemExit(1)
@@ -349,15 +354,17 @@
     config_path = asyncio.run(resolve_config_template_path(repo_dir))
     config = asyncio.run(load_config(config_path))
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.APPLY
     )
     asyncio.run(flag_expired_resources(templates))
     ctx.eval_only = True
-    template_changes = asyncio.run(config.run_apply(exe_message, load_templates(templates)))
+    template_changes = asyncio.run(
+        config.run_apply(exe_message, load_templates(templates))
+    )
     output_proposed_changes(template_changes)
     screen_render_resource_changes(template_changes)
 
 
 @cli.command()
 @click.option(
     "--repo-dir",
```

### Comparing `iambic_core-0.1.186/iambic/output/__init__.py` & `iambic_core-0.1.198/iambic/output/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pathlib
+
 from jinja2 import Environment, FileSystemLoader
+
 from iambic.output.filters import (
     rich_format,
     rich_text,
     rich_text_table,
     rich_tree_exception,
     rich_tree_summary,
 )
```

### Comparing `iambic_core-0.1.186/iambic/output/filters.py` & `iambic_core-0.1.198/iambic/output/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from io import StringIO
 from typing import List
-from rich.console import Console    
+
+from rich.console import Console
 from rich.style import Style
-from rich.text import Text
 from rich.table import Table
+from rich.text import Text
 from rich.tree import Tree
-from iambic.output.models import ActionSummary, ExceptionSummary
 
+from iambic.output.models import ActionSummary, ExceptionSummary
 
 console = Console()
+
+
 def rich_format(value: str, style_str: str) -> str:
     style = Style.parse(style_str)
     return console.render_str(str(value), style=style)
 
 
 def rich_text(text: str, style_str: str) -> str:
     style = Style.parse(style_str)
@@ -31,15 +34,18 @@
 def rich_tree_summary(action_summary: ActionSummary):
     action_summary_tree = Tree(action_summary.action, expanded=True)
     for template in action_summary.templates:
         template_tree = action_summary_tree.add(template.template_path, expanded=True)
         for account in template.accounts:
             account_tree = template_tree.add(account.account, expanded=True)
             for change in account.changes:
-                change_tree = account_tree.add(f"{change.change.resource_type} // {change.change.resource_id}", expanded=True)
+                change_tree = account_tree.add(
+                    f"{change.change.resource_type} // {change.change.resource_id}",
+                    expanded=True,
+                )
                 if change.change.diff:
                     change_tree.add(change.change.diff_plus_minus)
     console = Console(file=StringIO(), force_terminal=True)
     console.print(action_summary_tree)
     output = console.file.getvalue()
     return output
 
@@ -47,15 +53,17 @@
 def rich_tree_exception(exceptions: ExceptionSummary):
     exception_tree = Tree(exceptions.action, expanded=True)
     for template in exceptions.templates:
         template_tree = exception_tree.add(template.template_path, expanded=True)
         for account in template.accounts:
             account_tree = template_tree.add(account.account, expanded=True)
             for change in account.changes:
-                change_tree = account_tree.add(str(change.change.change_type), expanded=True)
+                change_tree = account_tree.add(
+                    str(change.change.change_type), expanded=True
+                )
                 change_tree.add(change.change.resource_id)
                 change_tree.add(change.change.resource_type)
                 change_tree.add(str(change.change.change_type.value))
                 if change.change.diff:
                     change_tree.add("* " + "\n* ".join(change.change.diff_plus_minus))
     console = Console(file=StringIO(), force_terminal=True)
     console.print(exception_tree)
```

### Comparing `iambic_core-0.1.186/iambic/output/models.py` & `iambic_core-0.1.198/iambic/output/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-import json
 
+import json
 import pathlib
 from typing import Any, Dict, List, Optional, Set
 
 from dictdiffer import diff
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Field
 
@@ -34,32 +34,33 @@
         "group_email": "GroupEmail",
         "assignments": "Assignment",
         "domain": "Domain",
         "group": "Group",
         "groups": "Group",
         "users": "User",
         "user": "User",
-
     }
 
     def __init__(self, proposed_change: ProposedChange) -> None:
         super().__init__(**proposed_change.dict())
         try:
             object_attribute = camel_to_snake(self.attribute)
         except TypeError:
             object_attribute = None
         if self.current_value is None:
             self.current_value = {}
         if self.new_value is None:
             self.new_value = {}
         if isinstance(self.current_value, dict):
-            self.diff = list(diff(self.current_value.get(object_attribute, {}), self.new_value))
+            self.diff = list(
+                diff(self.current_value.get(object_attribute, {}), self.new_value)
+            )
         else:
             self.diff = list(diff(self.current_value, self.new_value))
-        
+
     @property
     def diff_plus_minus(self) -> List[str]:
         diff_plus_minus = ""
         for x in self.diff:
             label = self.attribute
             if x[0] == "change":
                 if isinstance(x[2], list) or isinstance(x[2], tuple):
@@ -67,22 +68,28 @@
                     change_to = x[2][1]
                 else:
                     change_from = x[2]
                     change_to = x[2]
                 if change_to:
                     diff_plus_minus += f"{label}:\n-(From)\n{json.dumps(change_from, indent=2)}\n+(To)\n{json.dumps(change_to, indent=2)}"
                 else:
-                    diff_plus_minus += f"{label}:\n-(Remove)\n{json.dumps(change_from, indent=2)}"
-                diff_plus_minus.rstrip('\n')
+                    diff_plus_minus += (
+                        f"{label}:\n-(Remove)\n{json.dumps(change_from, indent=2)}"
+                    )
+                diff_plus_minus.rstrip("\n")
             elif x[0] == "add":
-                diff_plus_minus += f"{label}:\n+(Add)\n{json.dumps([y[1] for y in x[2]], indent=2)}"
-                diff_plus_minus.rstrip('\n')
+                diff_plus_minus += (
+                    f"{label}:\n+(Add)\n{json.dumps([y[1] for y in x[2]], indent=2)}"
+                )
+                diff_plus_minus.rstrip("\n")
             elif x[0] == "remove":
-                diff_plus_minus += f"{label}:\n-(Remove)\n{json.dumps([y[1] for y in x[2]], indent=2)}"
-                diff_plus_minus.rstrip('\n')
+                diff_plus_minus += (
+                    f"{label}:\n-(Remove)\n{json.dumps([y[1] for y in x[2]], indent=2)}"
+                )
+                diff_plus_minus.rstrip("\n")
         return diff_plus_minus
 
 
 class ApplicableChange(PydanticBaseModel):
     account: Optional[str]
     change: Optional[ProposedChange]
     template_change: Optional[TemplateChangeDetails]
```

### Comparing `iambic_core-0.1.186/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.1.198/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.1.198/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.1.198/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/output/text.py` & `iambic_core-0.1.198/iambic/output/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 from typing import List
 
 import rich
 
-from iambic.core.models import (
-    TemplateChangeDetails,
-)
+from iambic.core.models import TemplateChangeDetails
 from iambic.output import get_template_env
 from iambic.output.models import get_template_data
 
 
 def file_render_resource_changes(
     filepath: str,
     resource_changes: List[TemplateChangeDetails],
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import base64
 import json
 import uuid
+from itertools import chain
 from typing import TYPE_CHECKING, Union
 
 import boto3
 
 from iambic.config.dynamic_config import ExtendsConfig, ExtendsConfigKey
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
@@ -36,15 +37,15 @@
     generate_aws_role_templates,
 )
 from iambic.plugins.v0_1_0.aws.iam.user.template_generation import (
     collect_aws_users,
     generate_aws_user_templates,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
-    AwsIdentityCenterPermissionSetTemplate,
+    AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.template_generation import (
     collect_aws_permission_sets,
     generate_aws_permission_set_templates,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.utils import (
     generate_permission_set_map,
@@ -107,63 +108,117 @@
         *[account.get_boto3_client("iam") for account in config.accounts],
         return_exceptions=True,
     )
 
     return config
 
 
-async def apply(
+async def apply_identity_center_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     templates: list[BaseTemplate],
     remote_worker=None,
 ) -> list[TemplateChangeDetails]:
     """
-    The async_apply_callable for the AWS IambicPlugin class.
+    The async_apply_callable for IdentityCenter (SSO) resources.
 
     :param exe_message: Execution context
     :param config: The config object.
     :param templates: The list of templates to apply.
     :param remote_worker: The remote worker to use for applying templates.
     """
-    # TODO: Leverage exe_message as part of a distributed execution
-    # TODO: Leverage remote_worker as part of a distributed execution
+    return await async_batch_processor(
+        [template.apply(config) for template in templates],
+        5,
+        0.5,
+    )
 
-    if any(
-        isinstance(template, AwsIdentityCenterPermissionSetTemplate)
-        for template in templates
-    ):
-        await generate_permission_set_map(config.accounts, templates)
+
+async def apply_iam_templates(
+    exe_message: ExecutionMessage,
+    config: AWSConfig,
+    templates: list[BaseTemplate],
+    remote_worker=None,
+) -> list[TemplateChangeDetails]:
+    """
+    The async_apply_callable for IAM resource.
+
+    :param exe_message: Execution context
+    :param config: The config object.
+    :param templates: The list of templates to apply.
+    :param remote_worker: The remote worker to use for applying templates.
+    """
+    await generate_permission_set_map(config.accounts, templates)
 
     template_changes: list[TemplateChangeDetails] = []
 
     if managed_policy_tasks := [
         template.apply(config)
         for template in templates
         if template.template_type == AWS_MANAGED_POLICY_TEMPLATE_TYPE
     ]:
-        template_changes.extend(
-            await async_batch_processor(managed_policy_tasks, 50, 0)
-        )
+        template_changes.extend(await async_batch_processor(managed_policy_tasks, 40))
         if len(template_changes) > len(managed_policy_tasks):
             # There are other template changes that could rely on the managed policy
             # Give a few seconds to allow the managed policies to be created in AWS
             await asyncio.sleep(10)
 
     template_changes.extend(
         await async_batch_processor(
             [
                 template.apply(config)
                 for template in templates
                 if template.template_type != AWS_MANAGED_POLICY_TEMPLATE_TYPE
             ],
-            50,
-            0,
+            30,
         )
     )
+    return template_changes
+
+
+async def apply(
+    exe_message: ExecutionMessage,
+    config: AWSConfig,
+    templates: list[BaseTemplate],
+    remote_worker=None,
+) -> list[TemplateChangeDetails]:
+    """
+    The async_apply_callable for the AWS IambicPlugin class.
+
+    :param exe_message: Execution context
+    :param config: The config object.
+    :param templates: The list of templates to apply.
+    :param remote_worker: The remote worker to use for applying templates.
+    """
+    # TODO: Leverage exe_message as part of a distributed execution
+    # TODO: Leverage remote_worker as part of a distributed execution
+
+    identity_center_templates = []
+    iam_templates = []
+    tasks = []
+
+    for template in templates:
+        if template.template_type == AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE:
+            identity_center_templates.append(template)
+        else:
+            iam_templates.append(template)
+
+    if identity_center_templates:
+        tasks.append(
+            apply_identity_center_templates(
+                exe_message, config, identity_center_templates, remote_worker
+            )
+        )
+
+    if iam_templates:
+        tasks.append(
+            apply_iam_templates(exe_message, config, iam_templates, remote_worker)
+        )
+
+    template_changes = list(chain.from_iterable(await asyncio.gather(*tasks)))
 
     return [
         template_change
         for template_change in template_changes
         if template_change.proposed_changes or template_change.exceptions_seen
     ]
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+from itertools import chain
 from typing import Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
@@ -20,15 +21,15 @@
     apply_group_managed_policies,
     delete_iam_group,
     get_group,
 )
 from iambic.plugins.v0_1_0.aws.iam.models import Path
 from iambic.plugins.v0_1_0.aws.iam.policy.models import ManagedPolicyRef, PolicyDocument
 from iambic.plugins.v0_1_0.aws.models import AccessModel, AWSAccount, AWSTemplate
-from iambic.plugins.v0_1_0.aws.utils import boto_crud_call, remove_expired_resources
+from iambic.plugins.v0_1_0.aws.utils import boto_crud_call
 
 AWS_IAM_GROUP_TEMPLATE_TYPE = "NOQ::AWS::IAM::Group"
 
 
 class GroupProperties(BaseModel):
     group_name: str = Field(
         description="Name of the group",
@@ -90,22 +91,21 @@
             or self.iambic_managed == IambicManaged.IMPORT_ONLY
         )
 
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
+
+        # Marking for deletion. This shouldn't be done on the fly.
+        # self = await remove_expired_resources(
+        #     self, self.resource_type, self.resource_id
+        # )
         account_group = self.apply_resource_dict(aws_account)
 
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
         group_name = account_group["GroupName"]
         account_change_details = AccountChangeDetails(
             account=str(aws_account),
             resource_id=group_name,
             resource_type=self.resource_type,
             new_value=dict(**account_group),
             proposed_changes=[],
@@ -142,15 +142,15 @@
                         resource_id=group_name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "Active resource found with deleted=false."
                 if ctx.execute and not iambic_import_only:
                     log_str = f"{log_str} Deleting resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
 
                 if ctx.execute:
                     await delete_iam_group(group_name, client, log_params)
 
             return account_change_details
 
         group_exists = bool(current_group)
@@ -182,45 +182,45 @@
                         ProposedChange(
                             change_type=ProposedChangeType.UPDATE,
                             resource_id=group_name,
                             resource_type=self.resource_type,
                         )
                     ]
                     if ctx.execute:
-                        log.info(
+                        log.debug(
                             f"{log_str} Updating resource...",
                             **update_resource_log_params,
                         )
                         apply_awaitable = boto_crud_call(
                             client.update_group,
                             RoleName=group_name,
                             **update_group_params,
                         )
                         tasks.append(
                             plugin_apply_wrapper(apply_awaitable, proposed_changes)
                         )
                     else:
-                        log.info(log_str, **update_resource_log_params)
+                        log.debug(log_str, **update_resource_log_params)
                         account_change_details.proposed_changes.extend(proposed_changes)
             else:
                 account_change_details.proposed_changes.append(
                     ProposedChange(
                         change_type=ProposedChangeType.CREATE,
                         resource_id=group_name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "New resource found in code."
                 if not ctx.execute:
-                    log.info(log_str, **log_params)
+                    log.debug(log_str, **log_params)
                     # Exit now because apply functions won't work if resource doesn't exist
                     return account_change_details
 
                 log_str = f"{log_str} Creating resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
                 await boto_crud_call(client.create_group, **account_group)
         except Exception as e:
             log.error("Unable to generate tasks for resource", error=e, **log_params)
             return account_change_details
 
         tasks.extend(
             [
@@ -237,46 +237,40 @@
                     inline_policies,
                     existing_inline_policies,
                     log_params,
                 ),
             ]
         )
         try:
-            results: list[list[ProposedChange]] = await asyncio.gather(
-                *tasks, return_exceptions=True
-            )
-
-            # separate out the success versus failure calls
-            exceptions: list[ProposedChange] = []
-            changes_made: list[ProposedChange] = []
-            for result in results:
-                for r in result:
-                    if isinstance(r, ProposedChange):
-                        if len(r.exceptions_seen) == 0:
-                            changes_made.append(r)
-                        else:
-                            exceptions.append(r)
+            changes_made = await asyncio.gather(*tasks, return_exceptions=True)
+            if any(changes_made):
+                account_change_details.extend_changes(
+                    list(chain.from_iterable(changes_made))
+                )
 
         except Exception as e:
             log.exception("Unable to apply changes to resource", error=e, **log_params)
             return account_change_details
-        if any(changes_made):
-            account_change_details.proposed_changes.extend(changes_made)
-        if any(exceptions):
-            account_change_details.exceptions_seen.extend(exceptions)
-
-        if ctx.execute:
-            if self.deleted:
-                self.delete()
-            self.write()
+
+        if ctx.execute and not account_change_details.exceptions_seen:
+            # if self.deleted:
+            #     self.delete()
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
+        elif account_change_details.exceptions_seen:
+            log.error(
+                "Unable to finish execution on account for resource",
+                exceptions_seen=[
+                    cd.exceptions_seen for cd in account_change_details.exceptions_seen
+                ],
+                **log_params,
+            )
         else:
             log.debug(
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     group_resource_file_upsert_semaphore = NoqSemaphore(resource_file_upsert, 10)
     messages = []
 
     response = dict(account_id=aws_account.account_id, groups=[])
     iam_client = await aws_account.get_boto3_client("iam")
     account_groups = await list_groups(iam_client)
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Groups.",
         account_id=aws_account.account_id,
         account_name=aws_account.account_name,
         group_count=len(account_groups),
     )
 
     for account_group in account_groups:
@@ -107,15 +107,15 @@
             }
         )
         messages.append(
             dict(file_path=group_path, content_as_dict=account_group, replace_file=True)
         )
 
     await group_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Groups.",
         account_id=aws_account.account_id,
         group_count=len(account_groups),
     )
 
     return response
 
@@ -132,15 +132,15 @@
     response = []
 
     group_across_accounts = await get_group_across_accounts(
         aws_accounts, group_name, False
     )
     group_across_accounts = {k: v for k, v in group_across_accounts.items() if v}
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Group for all accounts.",
         group_name=group_name,
         total_accounts=len(group_across_accounts),
     )
 
     for account_id, account_group in group_across_accounts.items():
         group_path = os.path.join(
@@ -155,15 +155,15 @@
             }
         )
         messages.append(
             dict(file_path=group_path, content_as_dict=account_group, replace_file=True)
         )
 
     await group_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Group for all accounts.",
         group_name=group_name,
         total_accounts=len(group_across_accounts),
     )
 
     return response
 
@@ -458,15 +458,15 @@
         base_output_dir, AWS_IAM_GROUP_TEMPLATE_TYPE
     )
     group_dir = get_template_dir(base_output_dir)
     account_groups = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
-    log.info("Grouping groups")
+    log.debug("Grouping groups")
     # Move everything to required structure
     for account_group_elem in range(len(account_groups)):
         for group_elem in range(len(account_groups[account_group_elem]["groups"])):
             group_name = account_groups[account_group_elem]["groups"][group_elem].pop(
                 "name"
             )
             account_groups[account_group_elem]["groups"][group_elem][
@@ -475,15 +475,15 @@
 
         account_groups[account_group_elem]["resources"] = account_groups[
             account_group_elem
         ].pop("groups", [])
 
     grouped_group_map = await base_group_str_attribute(aws_account_map, account_groups)
 
-    log.info("Writing templated groups")
+    log.debug("Writing templated groups")
     all_resource_ids = set()
     for group_name, group_refs in grouped_group_map.items():
         resource_template = await create_templated_group(
             aws_account_map,
             group_name,
             group_refs,
             group_dir,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,61 +131,65 @@
     new_managed_policies = [
         policy_arn
         for policy_arn in template_policies
         if policy_arn not in existing_managed_policies
     ]
     if new_managed_policies:
         log_str = "New managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Attaching managed policies..."
+
         for policy_arn in new_managed_policies:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.ATTACH,
                     resource_type="aws:policy_document",
                     resource_id=policy_arn,
                     attribute="managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Attaching managed policies..."
                 apply_awaitable = boto_crud_call(
                     iam_client.attach_group_policy,
                     GroupName=group_name,
                     PolicyArn=policy_arn,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, managed_policies=new_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=new_managed_policies, **log_params)
 
     # Delete existing managed policies not in template
     existing_managed_policies = [
         policy_arn
         for policy_arn in existing_managed_policies
         if policy_arn not in template_policies
     ]
     if existing_managed_policies:
         log_str = "Stale managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Detaching managed policies..."
+
         for policy_arn in existing_managed_policies:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DETACH,
                     resource_type="aws:policy_document",
                     resource_id=policy_arn,
                     attribute="managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Detaching managed policies..."
                 apply_awaitable = boto_crud_call(
                     iam_client.detach_group_policy,
                     GroupName=group_name,
                     PolicyArn=policy_arn,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, managed_policies=existing_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=existing_managed_policies, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
@@ -193,15 +197,16 @@
 async def apply_group_inline_policies(
     group_name,
     iam_client,
     template_policies: list[dict],
     existing_policies: list[dict],
     log_params: dict,
 ) -> list[ProposedChange]:
-    tasks = []
+    apply_tasks = []
+    delete_tasks = []
     response = []
     template_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in template_policies
     }
     existing_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
@@ -225,16 +230,18 @@
                 log_str = f"{log_str} Removing inline policy..."
 
                 apply_awaitable = boto_crud_call(
                     iam_client.delete_group_policy,
                     GroupName=group_name,
                     PolicyName=policy_name,
                 )
-                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-            log.info(log_str, policy_name=policy_name, **log_params)
+                delete_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                )
+            log.debug(log_str, policy_name=policy_name, **log_params)
 
     for policy_name, policy_document in template_policy_map.items():
         existing_policy_doc = existing_policy_map.get(policy_name)
         policy_drift = None
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
@@ -284,67 +291,90 @@
                 log_str = f"{log_str} {boto_action} inline policy..."
                 apply_awaitable = boto_crud_call(
                     iam_client.put_group_policy,
                     GroupName=group_name,
                     PolicyName=policy_name,
                     PolicyDocument=json.dumps(policy_document),
                 )
-                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
+                apply_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                )
 
-            log.info(log_str, policy_name=policy_name, **log_params)
+            log.debug(log_str, policy_name=policy_name, **log_params)
+
+    if apply_tasks or delete_tasks:
+        results: list[list[ProposedChange]] = []
+        if delete_tasks:
+            results.extend(await asyncio.gather(*delete_tasks))
+            if apply_tasks:
+                # Wait for the policy deletion to propagate before applying new policies
+                # Otherwise a max policy limit error may be thrown
+                await asyncio.sleep(3)
+
+        if apply_tasks:
+            results.extend(await asyncio.gather(*apply_tasks))
 
-    if tasks:
-        results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
 
 async def delete_iam_group(group_name: str, iam_client, log_params: dict):
     tasks = []
     # Remove users from group
     attached_users = await list_users_in_group(group_name, iam_client)
-    attached_users = [attached_user["UserName"] for attached_user in attached_users]
-    log.info("Removing users from group.", attached_users=attached_users, **log_params)
-    for attached_user in attached_users:
-        tasks.append(
-            boto_crud_call(
-                iam_client.remove_user_from_group,
-                GroupName=group_name,
-                UserName=attached_user,
-            )
+    if attached_users:
+        attached_users = [attached_user["UserName"] for attached_user in attached_users]
+        log.debug(
+            "Removing users from group.", attached_users=attached_users, **log_params
         )
-    await asyncio.gather(*tasks)
+        for attached_user in attached_users:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.remove_user_from_group,
+                    GroupName=group_name,
+                    UserName=attached_user,
+                )
+            )
+        await asyncio.gather(*tasks)
 
     tasks = []
     # Detach managed policies
     managed_policies = await get_group_managed_policies(group_name, iam_client)
-    managed_policies = [policy["PolicyArn"] for policy in managed_policies]
-    log.info(
-        "Detaching managed policies.", managed_policies=managed_policies, **log_params
-    )
-    for policy in managed_policies:
-        tasks.append(
-            boto_crud_call(
-                iam_client.detach_group_policy, GroupName=group_name, PolicyArn=policy
-            )
+    if managed_policies:
+        managed_policies = [policy["PolicyArn"] for policy in managed_policies]
+        log.debug(
+            "Detaching managed policies.",
+            managed_policies=managed_policies,
+            **log_params,
         )
+        for policy in managed_policies:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.detach_group_policy,
+                    GroupName=group_name,
+                    PolicyArn=policy,
+                )
+            )
 
     # Delete inline policies
     inline_policies = await get_group_inline_policies(group_name, iam_client)
-    inline_policies = list(inline_policies.keys())
-    log.info(
-        "Deleting inline policies.", managed_policies=inline_policies, **log_params
-    )
-    for policy_name in inline_policies:
-        tasks.append(
-            boto_crud_call(
-                iam_client.delete_group_policy,
-                GroupName=group_name,
-                PolicyName=policy_name,
-            )
+    if inline_policies:
+        inline_policies = list(inline_policies.keys())
+        log.debug(
+            "Deleting inline policies.", managed_policies=inline_policies, **log_params
         )
+        for policy_name in inline_policies:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.delete_group_policy,
+                    GroupName=group_name,
+                    PolicyName=policy_name,
+                )
+            )
+
+    if managed_policies or inline_policies:
+        # Actually perform the deletion of Managed & Inline policies
+        await asyncio.gather(*tasks)
 
-    # Actually perform the deletion of Managed & Inline policies
-    await asyncio.gather(*tasks)
     # Now that everything has been removed from the group, delete the group itself
     await boto_crud_call(iam_client.delete_group, GroupName=group_name)
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import json
+from itertools import chain
 from typing import Callable, List, Optional, Union
 
 from jinja2 import BaseLoader, Environment
 from pydantic import Field, constr, validator
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
@@ -363,15 +364,15 @@
                         resource_id=policy_name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "Active resource found with deleted=false."
                 if not is_iambic_import_only:
                     log_str = f"{log_str} Deleting resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
 
                 if not is_iambic_import_only:
                     await delete_managed_policy(client, policy_arn, log_params)
 
             return account_change_details
 
         if current_policy:
@@ -390,31 +391,22 @@
                     account_policy.get("Tags", []),
                     current_policy.get("Tags", []),
                     is_iambic_import_only,
                     log_params,
                 ),
             ]
 
-            results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
-
-            # separate out the success versus failure calls
-            exceptions: list[ProposedChange] = []
-            changes_made: list[ProposedChange] = []
-            for result in results:
-                for r in result:
-                    if isinstance(r, ProposedChange):
-                        if len(r.exceptions_seen) == 0:
-                            changes_made.append(r)
-                        else:
-                            exceptions.append(r)
-
+            changes_made: list[list[ProposedChange]] = await asyncio.gather(
+                *tasks, return_exceptions=True
+            )
             if any(changes_made):
-                account_change_details.proposed_changes.extend(changes_made)
-            if any(exceptions):
-                account_change_details.exceptions_seen.extend(exceptions)
+                account_change_details.extend_changes(
+                    list(chain.from_iterable(changes_made))
+                )
+
         else:
             account_change_details.proposed_changes.append(
                 ProposedChange(
                     change_type=ProposedChangeType.CREATE,
                     resource_id=policy_name,
                     resource_type=self.resource_type,
                 )
@@ -423,22 +415,32 @@
             if not is_iambic_import_only:
                 log_str = f"{log_str} Creating resource..."
                 if isinstance(account_policy["PolicyDocument"], dict):
                     account_policy["PolicyDocument"] = json.dumps(
                         account_policy["PolicyDocument"]
                     )
                 await boto_crud_call(client.create_policy, **account_policy)
-            log.info(log_str, **log_params)
+            log.debug(log_str, **log_params)
 
-        if not is_iambic_import_only:
+        if ctx.execute and not account_change_details.exceptions_seen:
+            # if self.deleted:
+            #     self.delete()
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
+        elif account_change_details.exceptions_seen:
+            log.error(
+                "Unable to finish execution on account for resource",
+                exceptions_seen=[
+                    cd.exceptions_seen for cd in account_change_details.exceptions_seen
+                ],
+                **log_params,
+            )
         else:
             log.debug(
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     resource_file_upsert_semaphore = NoqSemaphore(resource_file_upsert, 10)
     messages = []
 
     response = dict(account_id=aws_account.account_id, managed_policies=[])
     iam_client = await aws_account.get_boto3_client("iam")
     account_managed_policies = await list_managed_policies(iam_client)
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Managed Policies.",
         account_id=aws_account.account_id,
         account_name=aws_account.account_name,
         managed_policy_count=len(account_managed_policies),
     )
 
     for managed_policy in account_managed_policies:
@@ -108,15 +108,15 @@
         messages.append(
             dict(
                 file_path=policy_path, content_as_dict=managed_policy, replace_file=True
             )
         )
 
     await resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Managed Policies.",
         account_id=aws_account.account_id,
         managed_policy_count=len(account_managed_policies),
     )
 
     return response
 
@@ -136,15 +136,15 @@
     response = []
 
     mp_across_accounts = await get_managed_policy_across_accounts(
         aws_accounts, policy_path, policy_name
     )
     mp_across_accounts = {k: v for k, v in mp_across_accounts.items() if v}
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Managed Policy for all accounts.",
         policy_name=policy_name,
         policy_path=policy_path,
         total_accounts=len(mp_across_accounts),
     )
 
     for account_id, managed_policy in mp_across_accounts.items():
@@ -164,15 +164,15 @@
         messages.append(
             dict(
                 file_path=policy_path, content_as_dict=managed_policy, replace_file=True
             )
         )
 
     await mp_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Managed Policy for all accounts.",
         policy_name=policy_name,
         policy_path=policy_path,
         total_accounts=len(mp_across_accounts),
     )
 
     return response
@@ -468,15 +468,15 @@
             "resources"
         ] = account_managed_policies[account_mp_elem].pop("managed_policies", [])
 
     grouped_managed_policy_map = await base_group_str_attribute(
         aws_account_map, account_managed_policies
     )
 
-    log.info("Writing templated managed policies")
+    log.debug("Writing templated managed policies")
     all_resource_ids = set()
     for policy_name, policy_refs in grouped_managed_policy_map.items():
         resource_template = await create_templated_managed_policy(
             aws_account_map,
             policy_name,
             policy_refs,
             resource_dir,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             'PolicyUsers': [{'UserName': 'string', 'UserId': 'string'}],
             'PolicyRoles': [{'RoleName': 'string', 'RoleId': 'string'}]
         }
     """
     return await paginated_search(
         iam_client.list_entities_for_policy,
         response_keys=["PolicyGroups", "PolicyRoles", "PolicyUsers"],
+        retain_key=True,
         PolicyArn=policy_arn,
     )
 
 
 async def get_managed_policy(iam_client, policy_arn: str, **kwargs) -> dict:
     try:
         response = (
@@ -112,27 +113,41 @@
             for policy in managed_policies
         ]
     )
 
 
 async def delete_managed_policy(iam_client, policy_arn: str, log_params: dict):
     policy_attachments = await get_managed_policy_attachments(iam_client, policy_arn)
+    policy_versions = await list_managed_policy_versions(iam_client, policy_arn)
     tasks = []
 
     for detachment_type in ["User", "Role", "Group"]:
         for entity in policy_attachments[f"Policy{detachment_type}s"]:
             tasks.append(
                 boto_crud_call(
                     getattr(iam_client, f"detach_{detachment_type.lower()}_policy"),
                     PolicyArn=policy_arn,
                     **{f"{detachment_type}Name": entity[f"{detachment_type}Name"]},
                 )
             )
 
-    log.info(
+    if len(policy_versions) > 1:
+        for version in policy_versions:
+            if version["IsDefaultVersion"]:
+                continue
+
+            tasks.append(
+                boto_crud_call(
+                    iam_client.delete_policy_version,
+                    PolicyArn=policy_arn,
+                    VersionId=version["VersionId"],
+                )
+            )
+
+    log.debug(
         "Detaching managed policy from resources.",
         policy_arn=policy_arn,
         **log_params,
     )
     await asyncio.gather(*tasks)
     await boto_crud_call(iam_client.delete_policy, PolicyArn=policy_arn)
 
@@ -183,15 +198,15 @@
                     template_policy_document,
                     policy_drift,
                     log_str,
                     log_params,
                 )
                 return await plugin_apply_wrapper(apply_awaitable, proposed_changes)
 
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
     return response
 
 
 async def new_policy_version(
     iam_client, policy_arn, template_policy_document, policy_drift, log_str, log_params
 ):
     if policy_drift:
@@ -205,15 +220,15 @@
 
     log_str = f"{log_str} Updating PolicyDocument..."
     await boto_crud_call(
         iam_client.create_policy_version,
         PolicyArn=policy_arn,
         PolicyDocument=json.dumps(template_policy_document),
     )
-    log.info(log_str, **log_params)
+    log.debug(log_str, **log_params)
 
 
 async def apply_managed_policy_tags(
     iam_client,
     policy_arn: str,
     template_tags: list[dict],
     existing_tags: list[dict],
@@ -249,15 +264,15 @@
             log_str = f"{log_str} Removing tags..."
             apply_awaitable = boto_crud_call(
                 iam_client.untag_policy,
                 PolicyArn=policy_arn,
                 TagKeys=tags_to_remove,
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, tags=tags_to_remove, **log_params)
+        log.debug(log_str, tags=tags_to_remove, **log_params)
 
     if tags_to_apply:
         log_str = "New tags discovered in AWS."
         proposed_changes = [
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
                 resource_type="aws:policy_document",
@@ -270,15 +285,15 @@
         response.extend(proposed_changes)
         if ctx.execute:
             log_str = f"{log_str} Adding tags..."
             apply_awaitable = boto_crud_call(
                 iam_client.tag_policy, PolicyArn=policy_arn, Tags=tags_to_apply
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, tags=tags_to_apply, **log_params)
+        log.debug(log_str, tags=tags_to_apply, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import json
+from itertools import chain
 from typing import Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
@@ -38,15 +39,15 @@
 from iambic.plugins.v0_1_0.aws.models import (
     AccessModel,
     AWSAccount,
     AWSTemplate,
     Description,
     Tag,
 )
-from iambic.plugins.v0_1_0.aws.utils import boto_crud_call, remove_expired_resources
+from iambic.plugins.v0_1_0.aws.utils import boto_crud_call
 
 AWS_IAM_ROLE_TEMPLATE_TYPE = "NOQ::AWS::IAM::Role"
 
 
 class RoleAccess(ExpiryModel, AccessModel):
     users: list[str] = Field(
         [],
@@ -215,22 +216,15 @@
             or self.iambic_managed == IambicManaged.IMPORT_ONLY
         )
 
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
         account_role = self.apply_resource_dict(aws_account)
-
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
         role_name = account_role["RoleName"]
         account_change_details = AccountChangeDetails(
             account=str(aws_account),
             resource_id=role_name,
             resource_type=self.resource_type,
             new_value=dict(**account_role),
             proposed_changes=[],
@@ -265,15 +259,15 @@
                         resource_id=role_name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "Active resource found with deleted=false."
                 if ctx.execute and not iambic_import_only:
                     log_str = f"{log_str} Deleting resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
 
                 if ctx.execute:
                     await delete_iam_role(role_name, client, log_params)
 
             return account_change_details
 
         role_exists = bool(current_role)
@@ -321,15 +315,15 @@
                             old_value=current_role.get(k), new_value=account_role.get(k)
                         )
                         update_role_params[k] = current_role.get(k)
 
                 if update_role_params:
                     log_str = "Out of date resource found."
                     if ctx.execute:
-                        log.info(
+                        log.debug(
                             f"{log_str} Updating resource...",
                             **update_resource_log_params,
                         )
 
                         async def update_role():
                             exceptions = []
                             try:
@@ -350,15 +344,15 @@
                                     resource_type=self.resource_type,
                                     exceptions_seen=exceptions,
                                 )
                             ]
 
                         tasks.append(update_role())
                     else:
-                        log.info(log_str, **update_resource_log_params)
+                        log.debug(log_str, **update_resource_log_params)
                         account_change_details.proposed_changes.append(
                             ProposedChange(
                                 change_type=ProposedChangeType.UPDATE,
                                 resource_id=role_name,
                                 resource_type=self.resource_type,
                             )
                         )
@@ -368,32 +362,33 @@
                         change_type=ProposedChangeType.CREATE,
                         resource_id=role_name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "New resource found in code."
                 if not ctx.execute:
-                    log.info(log_str, **log_params)
+                    log.debug(log_str, **log_params)
                     # Exit now because apply functions won't work if resource doesn't exist
                     return account_change_details
 
                 log_str = f"{log_str} Creating resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
                 account_role["AssumeRolePolicyDocument"] = json.dumps(
                     account_role["AssumeRolePolicyDocument"]
                 )
                 if account_role.get("PermissionsBoundary"):
                     account_role["PermissionsBoundary"] = account_role[
                         "PermissionsBoundary"
                     ]["PolicyArn"]
 
                 await boto_crud_call(client.create_role, **account_role)
         except Exception as e:
             log.error("Unable to generate tasks for resource", error=e, **log_params)
-            return account_change_details
+            # return account_change_details
+            raise
 
         tasks.extend(
             [
                 apply_role_managed_policies(
                     role_name,
                     client,
                     managed_policies,
@@ -406,46 +401,40 @@
                     inline_policies,
                     existing_inline_policies,
                     log_params,
                 ),
             ]
         )
         try:
-            results: list[list[ProposedChange]] = await asyncio.gather(
+            changes_made: list[list[ProposedChange]] = await asyncio.gather(
                 *tasks, return_exceptions=True
             )
-
-            # separate out the success versus failure calls
-            exceptions: list[ProposedChange] = []
-            changes_made: list[ProposedChange] = []
-            for result in results:
-                for r in result:
-                    if isinstance(r, ProposedChange):
-                        if len(r.exceptions_seen) == 0:
-                            changes_made.append(r)
-                        else:
-                            exceptions.append(r)
+            if any(changes_made):
+                account_change_details.extend_changes(
+                    list(chain.from_iterable(changes_made))
+                )
 
         except Exception as e:
             log.exception("Unable to apply changes to resource", error=e, **log_params)
             return account_change_details
-        if any(changes_made):
-            account_change_details.proposed_changes.extend(changes_made)
-        if any(exceptions):
-            account_change_details.exceptions_seen.extend(exceptions)
-
-        if ctx.execute:
-            if self.deleted:
-                self.delete()
-            self.write()
+
+        if ctx.execute and not account_change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
+        elif account_change_details.exceptions_seen:
+            log.error(
+                "Unable to finish execution on account for resource",
+                exceptions_seen=[
+                    cd.exceptions_seen for cd in account_change_details.exceptions_seen
+                ],
+                **log_params,
+            )
         else:
             log.debug(
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     role_resource_file_upsert_semaphore = NoqSemaphore(resource_file_upsert, 10)
     messages = []
 
     response = dict(account_id=aws_account.account_id, roles=[])
     iam_client = await aws_account.get_boto3_client("iam")
     account_roles = await list_roles(iam_client)
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Roles.",
         account_id=aws_account.account_id,
         account_name=aws_account.account_name,
         role_count=len(account_roles),
     )
 
     for account_role in account_roles:
@@ -109,15 +109,15 @@
             }
         )
         messages.append(
             dict(file_path=role_path, content_as_dict=account_role, replace_file=True)
         )
 
     await role_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Roles.",
         account_id=aws_account.account_id,
         role_count=len(account_roles),
     )
 
     return response
 
@@ -136,15 +136,15 @@
     response = []
 
     role_across_accounts = await get_role_across_accounts(
         aws_accounts, role_name, False
     )
     role_across_accounts = {k: v for k, v in role_across_accounts.items() if v}
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Role for all accounts.",
         role_name=role_name,
         total_accounts=len(role_across_accounts),
     )
 
     for account_id, account_role in role_across_accounts.items():
         role_path = os.path.join(
@@ -159,15 +159,15 @@
             }
         )
         messages.append(
             dict(file_path=role_path, content_as_dict=account_role, replace_file=True)
         )
 
     await role_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Role for all accounts.",
         role_name=role_name,
         total_accounts=len(role_across_accounts),
     )
 
     return response
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                     attribute="tags",
                     resource_type="aws:iam:role",
                     resource_id=role_name,
                     change_summary={"TagKeys": tags_to_remove},
                 )
             )
 
-        log.info(log_str, tags=tags_to_remove, **log_params)
+        log.debug(log_str, tags=tags_to_remove, **log_params)
 
     if tags_to_apply:
         log_str = "New tags discovered in AWS."
 
         if ctx.execute:
             log_str = f"{log_str} Adding tags..."
 
@@ -239,15 +239,15 @@
                         change_type=ProposedChangeType.ATTACH,
                         attribute="tags",
                         resource_type="aws:iam:role",
                         resource_id=role_name,
                         new_value=tag,
                     )
                 )
-        log.info(log_str, tags=tags_to_apply, **log_params)
+        log.debug(log_str, tags=tags_to_apply, **log_params)
 
     if tasks and ctx.execute:
         results: list[list[ProposedChange]] = await asyncio.gather(
             *tasks, return_exceptions=True
         )
         for r in results:
             response.extend(r)
@@ -311,15 +311,15 @@
             boto_action = "Creating" if existing_policy_document else "Updating"
             log_str = f"{log_str} {boto_action} AssumeRolePolicyDocument..."
             await boto_crud_call(
                 iam_client.update_assume_role_policy,
                 RoleName=role_name,
                 PolicyDocument=json.dumps(template_policy_document),
             )
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
 
     return response
 
 
 async def apply_role_managed_policies(
     role_name,
     iam_client,
@@ -355,15 +355,15 @@
                 boto_crud_call(
                     iam_client.attach_role_policy,
                     RoleName=role_name,
                     PolicyArn=policy_arn,
                 )
                 for policy_arn in new_managed_policies
             ]
-        log.info(log_str, managed_policies=new_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=new_managed_policies, **log_params)
 
     # Delete existing managed policies not in template
     existing_managed_policies = [
         policy_arn
         for policy_arn in existing_managed_policies
         if policy_arn not in template_policies
     ]
@@ -386,15 +386,15 @@
                         iam_client.detach_role_policy,
                         RoleName=role_name,
                         PolicyArn=policy_arn,
                     )
                     for policy_arn in existing_managed_policies
                 ]
             )
-        log.info(log_str, managed_policies=existing_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=existing_managed_policies, **log_params)
 
     if tasks:
         await asyncio.gather(*tasks)
 
     return response
 
 
@@ -439,15 +439,15 @@
                         RoleName=role_name,
                         PermissionsBoundary=template_boundary_policy_arn,
                     ),
                     proposed_changes,
                 )
             ]
 
-        log.info(
+        log.debug(
             log_str, permission_boundary=template_boundary_policy_arn, **log_params
         )
 
     # Detach permission boundary not in template
     if template_boundary_policy_arn is None and (
         existing_boundary_policy_arn != template_boundary_policy_arn
     ):
@@ -474,15 +474,15 @@
                             RoleName=role_name,
                         ),
                         proposed_changes,
                     )
                 ]
             )
 
-        log.info(
+        log.debug(
             log_str, permission_boundary=existing_boundary_policy_arn, **log_params
         )
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
@@ -523,15 +523,15 @@
                 tasks.append(
                     boto_crud_call(
                         iam_client.delete_role_policy,
                         RoleName=role_name,
                         PolicyName=policy_name,
                     )
                 )
-            log.info(log_str, policy_name=policy_name, **log_params)
+            log.debug(log_str, policy_name=policy_name, **log_params)
 
     for policy_name, policy_document in template_policy_map.items():
         existing_policy_doc = existing_policy_map.get(policy_name)
         policy_drift = None
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
@@ -583,15 +583,15 @@
                         iam_client.put_role_policy,
                         RoleName=role_name,
                         PolicyName=policy_name,
                         PolicyDocument=json.dumps(policy_document),
                     )
                 )
 
-            log.info(log_str, policy_name=policy_name, **log_params)
+            log.debug(log_str, policy_name=policy_name, **log_params)
 
     if tasks:
         await asyncio.gather(*tasks)
 
     return response
 
 
@@ -619,28 +619,28 @@
         )
     await asyncio.gather(*tasks)
 
     tasks = []
     # Detach managed policies
     managed_policies = await get_role_managed_policies(role_name, iam_client)
     managed_policies = [policy["PolicyArn"] for policy in managed_policies]
-    log.info(
+    log.debug(
         "Detaching managed policies.", managed_policies=managed_policies, **log_params
     )
     for policy in managed_policies:
         tasks.append(
             boto_crud_call(
                 iam_client.detach_role_policy, RoleName=role_name, PolicyArn=policy
             )
         )
 
     # Delete inline policies
     inline_policies = await get_role_inline_policies(role_name, iam_client)
     inline_policies = list(inline_policies.keys())
-    log.info(
+    log.debug(
         "Deleting inline policies.", managed_policies=inline_policies, **log_params
     )
     for policy_name in inline_policies:
         tasks.append(
             boto_crud_call(
                 iam_client.delete_role_policy,
                 RoleName=role_name,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from __future__ import annotations
 
 import asyncio
+from itertools import chain
 from typing import Any, Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
     ProposedChange,
     ProposedChangeType,
 )
+from iambic.core.utils import plugin_apply_wrapper
 from iambic.plugins.v0_1_0.aws.iam.models import Path, PermissionBoundary
 from iambic.plugins.v0_1_0.aws.iam.policy.models import ManagedPolicyRef, PolicyDocument
 from iambic.plugins.v0_1_0.aws.iam.user.utils import (
     apply_user_groups,
     apply_user_inline_policies,
     apply_user_managed_policies,
     apply_user_permission_boundary,
     apply_user_tags,
     delete_iam_user,
     get_user,
 )
 from iambic.plugins.v0_1_0.aws.models import AccessModel, AWSAccount, AWSTemplate, Tag
-from iambic.plugins.v0_1_0.aws.utils import boto_crud_call, remove_expired_resources
+from iambic.plugins.v0_1_0.aws.utils import boto_crud_call
 
 AWS_IAM_USER_TEMPLATE_TYPE = "NOQ::AWS::IAM::User"
 
 
 class Group(ExpiryModel, AccessModel):
     group_name: str
-    
+
     # All excluded fields are populated by the API and not required in the template
     # We are not tracking those, but we do allow them to be imported in order to
     # pass validation.
     arn: Optional[str] = Field("", description="ARN of the group", exclude=True)
-    create_date: Optional[str] = Field("", description="Date the group was created", exclude=True)
+    create_date: Optional[str] = Field(
+        "", description="Date the group was created", exclude=True
+    )
     group_id: Optional[str] = Field("", description="ID of the group", exclude=True)
     path: Optional[str] = Field("", description="Path of the group", exclude=True)
     extra: Any = Field(None, description=("Extra attributes to store"), exclude=True)
 
     @property
     def resource_type(self):
         return "aws:iam:group"
@@ -155,17 +159,14 @@
             or self.iambic_managed == IambicManaged.IMPORT_ONLY
         )
 
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
         account_user = self.apply_resource_dict(aws_account)
 
         user_name = account_user["UserName"]
         account_change_details = AccountChangeDetails(
             account=str(aws_account),
             resource_id=user_name,
             resource_type=self.resource_type,
@@ -175,44 +176,55 @@
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=user_name,
             account=str(aws_account),
         )
         iambic_import_only = self._is_iambic_import_only(aws_account)
-        current_user = await get_user(user_name, client)
+        deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
+        try:
+            current_user = await get_user(
+                user_name, client, include_policies=bool(not deleted)
+            )
+        except Exception as err:
+            log.error("Failed to retrieve user", **log_params, error=err)
+            return account_change_details
+
         if current_user:
             account_change_details.current_value = {**current_user}  # Create a new dict
 
             if ctx.command == Command.CONFIG_DISCOVERY:
                 # Don't overwrite a resource during config discovery
                 account_change_details.new_value = {}
                 return account_change_details
 
-        deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_user:
                 account_change_details.new_value = None
-                account_change_details.proposed_changes.append(
+                log_str = "Active resource found with deleted=false."
+                if ctx.execute and not iambic_import_only:
+                    log_str = f"{log_str} Deleting resource..."
+                log.debug(log_str, **log_params)
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=user_name,
                         resource_type=self.resource_type,
                     )
-                )
-                log_str = "Active resource found with deleted=false."
-                if ctx.execute and not iambic_import_only:
-                    log_str = f"{log_str} Deleting resource..."
-                log.info(log_str, **log_params)
+                ]
 
                 if ctx.execute:
-                    await delete_iam_user(user_name, client, log_params)
+                    proposed_changes = await plugin_apply_wrapper(
+                        delete_iam_user(user_name, client, log_params), proposed_changes
+                    )
+
+                account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         user_exists = bool(current_user)
         inline_policies = account_user.pop("InlinePolicies", [])
         managed_policies = account_user.pop("ManagedPolicies", [])
         groups = account_user.pop("Groups", [])
@@ -251,15 +263,15 @@
                         update_resource_log_params[k] = dict(
                             old_value=current_user.get(k), new_value=account_user.get(k)
                         )
                         update_user_params[f"New{k}"] = account_user.get(k)
                 if update_user_params:
                     log_str = "Out of date resource found."
                     if ctx.execute:
-                        log.info(
+                        log.debug(
                             f"{log_str} Updating resource...",
                             **update_resource_log_params,
                         )
 
                         async def update_user():
                             exceptions = []
                             try:
@@ -280,44 +292,50 @@
                                     resource_type=self.resource_type,
                                     exceptions_seen=exceptions,
                                 )
                             ]
 
                         tasks.append(update_user())
                     else:
-                        log.info(log_str, **update_resource_log_params)
+                        log.debug(log_str, **update_resource_log_params)
                         account_change_details.proposed_changes.append(
                             ProposedChange(
                                 change_type=ProposedChangeType.UPDATE,
                                 resource_id=user_name,
                                 resource_type=self.resource_type,
                             )
                         )
             else:
-                account_change_details.proposed_changes.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.CREATE,
                         resource_id=user_name,
                         resource_type=self.resource_type,
                     )
-                )
+                ]
                 log_str = "New resource found in code."
                 if not ctx.execute:
-                    log.info(log_str, **log_params)
+                    account_change_details.proposed_changes.extend(proposed_changes)
+                    log.debug(log_str, **log_params)
                     # Exit now because apply functions won't work if resource doesn't exist
                     return account_change_details
 
                 log_str = f"{log_str} Creating resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
                 if account_user.get("PermissionsBoundary"):
                     account_user["PermissionsBoundary"] = account_user[
                         "PermissionsBoundary"
                     ]["PolicyArn"]
 
-                await boto_crud_call(client.create_user, **account_user)
+                account_change_details.proposed_changes.extend(
+                    await plugin_apply_wrapper(
+                        boto_crud_call(client.create_user, **account_user),
+                        proposed_changes,
+                    )
+                )
         except Exception as e:
             log.error("Unable to generate tasks for resource", error=e, **log_params)
             return account_change_details
 
         tasks.extend(
             [
                 apply_user_managed_policies(
@@ -340,46 +358,40 @@
                     groups,
                     existing_groups,
                     log_params,
                 ),
             ]
         )
         try:
-            results: list[list[ProposedChange]] = await asyncio.gather(
+            changes_made: list[list[ProposedChange]] = await asyncio.gather(
                 *tasks, return_exceptions=True
             )
-
-            # separate out the success versus failure calls
-            exceptions: list[ProposedChange] = []
-            changes_made: list[ProposedChange] = []
-            for result in results:
-                for r in result:
-                    if isinstance(r, ProposedChange):
-                        if len(r.exceptions_seen) == 0:
-                            changes_made.append(r)
-                        else:
-                            exceptions.append(r)
+            if any(changes_made):
+                account_change_details.extend_changes(
+                    list(chain.from_iterable(changes_made))
+                )
 
         except Exception as e:
             log.exception("Unable to apply changes to resource", error=e, **log_params)
             return account_change_details
-        if any(changes_made):
-            account_change_details.proposed_changes.extend(changes_made)
-        if any(exceptions):
-            account_change_details.exceptions_seen.extend(exceptions)
-
-        if ctx.execute:
-            if self.deleted:
-                self.delete()
-            self.write()
+
+        if ctx.execute and not account_change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
+        elif account_change_details.exceptions_seen:
+            log.error(
+                "Unable to finish execution on account for resource",
+                exceptions_seen=[
+                    cd.exceptions_seen for cd in account_change_details.exceptions_seen
+                ],
+                **log_params,
+            )
         else:
             log.debug(
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     user_resource_file_upsert_semaphore = NoqSemaphore(resource_file_upsert, 10)
     messages = []
 
     response = dict(account_id=aws_account.account_id, users=[])
     iam_client = await aws_account.get_boto3_client("iam")
     account_users = await list_users(iam_client)
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM Users.",
         account_id=aws_account.account_id,
         account_name=aws_account.account_name,
         user_count=len(account_users),
     )
 
     for account_user in account_users:
@@ -109,15 +109,15 @@
             }
         )
         messages.append(
             dict(file_path=user_path, content_as_dict=account_user, replace_file=True)
         )
 
     await user_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM Users.",
         account_id=aws_account.account_id,
         user_count=len(account_users),
     )
 
     return response
 
@@ -134,15 +134,15 @@
     response = []
 
     user_across_accounts = await get_user_across_accounts(
         aws_accounts, user_name, False
     )
     user_across_accounts = {k: v for k, v in user_across_accounts.items() if v}
 
-    log.info(
+    log.debug(
         "Retrieved AWS IAM User for all accounts.",
         user_name=user_name,
         total_accounts=len(user_across_accounts),
     )
 
     for account_id, account_user in user_across_accounts.items():
         user_path = os.path.join(
@@ -157,15 +157,15 @@
             }
         )
         messages.append(
             dict(file_path=user_path, content_as_dict=account_user, replace_file=True)
         )
 
     await user_resource_file_upsert_semaphore.process(messages)
-    log.info(
+    log.debug(
         "Finished caching AWS IAM User for all accounts.",
         user_name=user_name,
         total_accounts=len(user_across_accounts),
     )
 
     return response
 
@@ -562,15 +562,15 @@
 
         account_users[account_user_elem]["resources"] = account_users[
             account_user_elem
         ].pop("users", [])
 
     grouped_user_map = await base_group_str_attribute(aws_account_map, account_users)
 
-    log.info("Writing templated users")
+    log.debug("Writing templated users")
     all_resource_ids = set()
     for user_name, user_refs in grouped_user_map.items():
         resource_template = await create_templated_user(
             aws_account_map,
             user_name,
             user_refs,
             user_dir,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             apply_awaitable = boto_crud_call(
                 iam_client.untag_user,
                 UserName=user_name,
                 TagKeys=tags_to_remove,
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-        log.info(log_str, tags=tags_to_remove, **log_params)
+        log.debug(log_str, tags=tags_to_remove, **log_params)
 
     if tags_to_apply:
         log_str = "New tags discovered in AWS."
 
         proposed_changes = [
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
@@ -193,15 +193,15 @@
         if ctx.execute:
             log_str = f"{log_str} Adding tags..."
             apply_awaitable = boto_crud_call(
                 iam_client.tag_user, UserName=user_name, Tags=tags_to_apply
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-        log.info(log_str, tags=tags_to_apply, **log_params)
+        log.debug(log_str, tags=tags_to_apply, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
@@ -247,15 +247,15 @@
                         UserName=user_name,
                         PermissionsBoundary=template_boundary_policy_arn,
                     ),
                     proposed_changes,
                 )
             ]
 
-        log.info(
+        log.debug(
             log_str, permission_boundary=template_boundary_policy_arn, **log_params
         )
 
     # Detach permission boundary not in template
     if template_boundary_policy_arn is None and (
         existing_boundary_policy_arn != template_boundary_policy_arn
     ):
@@ -282,15 +282,15 @@
                             UserName=user_name,
                         ),
                         proposed_changes,
                     )
                 ]
             )
 
-        log.info(
+        log.debug(
             log_str, permission_boundary=existing_boundary_policy_arn, **log_params
         )
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
@@ -347,15 +347,15 @@
                             attribute="managed_policies",
                         )
                     ],
                 )
                 for policy_arn in new_managed_policies
             ]
 
-        log.info(log_str, managed_policies=new_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=new_managed_policies, **log_params)
 
     # Delete existing managed policies not in template
     existing_managed_policies = [
         policy_arn
         for policy_arn in existing_managed_policies
         if policy_arn not in template_policies
     ]
@@ -393,15 +393,15 @@
                             )
                         ],
                     )
                     for policy_arn in existing_managed_policies
                 ]
             )
 
-        log.info(log_str, managed_policies=existing_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=existing_managed_policies, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
@@ -444,15 +444,15 @@
                 apply_awaitable = boto_crud_call(
                     iam_client.delete_user_policy,
                     UserName=user_name,
                     PolicyName=policy_name,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-            log.info(log_str, policy_name=policy_name, **log_params)
+            log.debug(log_str, policy_name=policy_name, **log_params)
 
     for policy_name, policy_document in template_policy_map.items():
         existing_policy_doc = existing_policy_map.get(policy_name)
         policy_drift = None
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
@@ -505,15 +505,15 @@
                     iam_client.put_user_policy,
                     UserName=user_name,
                     PolicyName=policy_name,
                     PolicyDocument=json.dumps(policy_document),
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-            log.info(log_str, policy_name=policy_name, **log_params)
+            log.debug(log_str, policy_name=policy_name, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
@@ -548,21 +548,20 @@
                 apply_awaitable = boto_crud_call(
                     iam_client.add_user_to_group,
                     GroupName=group,
                     UserName=user_name,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-            log.info(log_str, group_name=group, **log_params)
+            log.debug(log_str, group_name=group, **log_params)
 
     # Remove stale groups
     for group in existing_groups:
         if group not in template_groups:
             log_str = "Stale groups discovered."
-
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DELETE,
                     resource_type="aws:iam:group",
                     resource_id=group,
                     attribute="groups",
                 )
@@ -573,50 +572,68 @@
                 apply_awaitable = boto_crud_call(
                     iam_client.remove_user_from_group,
                     GroupName=group,
                     UserName=user_name,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
 
-            log.info(log_str, group_name=group, **log_params)
+            log.debug(log_str, group_name=group, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
 
 async def delete_iam_user(user_name: str, iam_client, log_params: dict):
     tasks = []
     # Detach managed policies
     managed_policies = await get_user_managed_policies(user_name, iam_client)
-    managed_policies = [policy["PolicyArn"] for policy in managed_policies]
-    log.info(
-        "Detaching managed policies.", managed_policies=managed_policies, **log_params
-    )
-    for policy in managed_policies:
-        tasks.append(
-            boto_crud_call(
-                iam_client.detach_user_policy, UserName=user_name, PolicyArn=policy
-            )
+    if managed_policies:
+        managed_policies = [policy["PolicyArn"] for policy in managed_policies]
+        log.debug(
+            "Detaching managed policies.",
+            managed_policies=managed_policies,
+            **log_params,
         )
+        for policy in managed_policies:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.detach_user_policy, UserName=user_name, PolicyArn=policy
+                )
+            )
 
     # Delete inline policies
     inline_policies = await get_user_inline_policies(user_name, iam_client)
-    inline_policies = list(inline_policies.keys())
-    log.info(
-        "Deleting inline policies.", managed_policies=inline_policies, **log_params
-    )
-    for policy_name in inline_policies:
-        tasks.append(
-            boto_crud_call(
-                iam_client.delete_user_policy,
-                UserName=user_name,
-                PolicyName=policy_name,
-            )
+    if inline_policies:
+        inline_policies = list(inline_policies.keys())
+        log.debug(
+            "Deleting inline policies.", managed_policies=inline_policies, **log_params
         )
+        for policy_name in inline_policies:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.delete_user_policy,
+                    UserName=user_name,
+                    PolicyName=policy_name,
+                )
+            )
+
+    # Remove groups
+    user_groups = await get_user_groups(user_name, iam_client)
+    if user_groups:
+        user_groups = sorted(list(user_groups.keys()))
+        log.debug("Removing user groups.", groups=user_groups, **log_params)
+        for group in user_groups:
+            tasks.append(
+                boto_crud_call(
+                    iam_client.remove_user_from_group,
+                    UserName=user_name,
+                    GroupName=group,
+                )
+            )
 
     # Actually perform the deletion of Managed & Inline policies
     await asyncio.gather(*tasks)
     # Now that everything has been removed from the user, delete the user itself
     await boto_crud_call(iam_client.delete_user, UserName=user_name)
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import re
+from itertools import chain
 from typing import TYPE_CHECKING, Callable, List, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
@@ -34,15 +35,15 @@
     AccessModel,
     AWSAccount,
     AWSTemplate,
     Description,
     ExpiryModel,
     Tag,
 )
-from iambic.plugins.v0_1_0.aws.utils import boto_crud_call, remove_expired_resources
+from iambic.plugins.v0_1_0.aws.utils import boto_crud_call
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 
 AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE = (
     "NOQ::AWS::IdentityCenter::PermissionSet"
 )
@@ -415,17 +416,18 @@
         """
 
         identity_center_client = await aws_account.get_boto3_client(
             "sso-admin", region_name=aws_account.identity_center_details.region_name
         )
         instance_arn = aws_account.identity_center_details.instance_arn
         permission_set_arn = None
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
+        # Marking for deletion. This shouldn't be done on the fly.
+        # self = await remove_expired_resources(
+        #     self, self.resource_type, self.resource_id
+        # )
         template_permission_set = self.apply_resource_dict(aws_account)
         name = template_permission_set["Name"]
         template_account_assignments = await self._verbose_access_rules(aws_account)
         account_change_details = AccountChangeDetails(
             org_id=aws_account.org_id,
             account=str(aws_account),
             resource_id=name,
@@ -495,26 +497,25 @@
                         resource_id=name,
                         resource_type=self.resource_type,
                     )
                 )
                 log_str = "Active resource found with deleted=false."
                 if ctx.execute and not read_only:
                     log_str = f"{log_str} Deleting resource..."
-                log.info(log_str, **log_params)
+                log.debug(log_str, **log_params)
 
                 if ctx.execute:
                     await delete_permission_set(
                         identity_center_client,
                         instance_arn,
                         permission_set_arn,
                         current_permission_set,
                         current_account_assignments,
                         log_params,
                     )
-                    self.delete()
 
             return account_change_details
 
         permission_set_exists = bool(current_permission_set)
         tasks = []
         try:
             if permission_set_exists:
@@ -649,50 +650,38 @@
                     template_permission_set.get("PermissionsBoundary", {}),
                     current_permission_set.get("PermissionsBoundary", {}),
                     log_params,
                 ),
             ]
         )
         try:
-            results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
+            changes_made: list[list[ProposedChange]] = await asyncio.gather(*tasks)
 
             # apply_account_assignments is a dedicated call due to the request limit on CreateAccountAssignment
             #   per https://docs.aws.amazon.com/singlesignon/latest/userguide/limits.html
-            results.append(
+            changes_made.append(
                 await apply_account_assignments(
                     identity_center_client,
                     instance_arn,
                     permission_set_arn,
                     template_account_assignments,
                     current_account_assignments,
                     log_params,
                 )
             )
+            if any(changes_made):
+                account_change_details.extend_changes(
+                    list(chain.from_iterable(changes_made))
+                )
         except Exception as e:
             log.error("Unable to apply changes to resource", error=e, **log_params)
             return account_change_details
 
-        # separate out the success versus failure calls
-        exceptions: list[ProposedChange] = []
-        changes_made: list[ProposedChange] = []
-        for result in results:
-            for r in result:
-                if isinstance(r, ProposedChange):
-                    if len(r.exceptions_seen) == 0:
-                        changes_made.append(r)
-                    else:
-                        exceptions.append(r)
-
-        if any(changes_made):
-            account_change_details.proposed_changes.extend(changes_made)
-        if any(exceptions):
-            account_change_details.exceptions_seen.extend(exceptions)
-
-        if ctx.execute:
-            if any(changes_made):
+        if ctx.execute and not account_change_details.exceptions_seen:
+            if any(changes_made) and not self.deleted:
                 res = await boto_crud_call(
                     identity_center_client.provision_permission_set,
                     InstanceArn=instance_arn,
                     PermissionSetArn=permission_set_arn,
                     TargetType="ALL_PROVISIONED_ACCOUNTS",
                 )
 
@@ -709,84 +698,90 @@
                         provision_status["PermissionSetProvisioningStatus"]["Status"]
                         != "IN_PROGRESS"
                     ):
                         break
 
                     await asyncio.sleep(1)
                     continue
-            if self.deleted:
-                self.delete()
-            self.write()  # why are writing the template here?
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
+        elif account_change_details.exceptions_seen:
+            log.error(
+                "Unable to finish execution on account for resource",
+                exceptions_seen=[
+                    cd.exceptions_seen for cd in account_change_details.exceptions_seen
+                ],
+                **log_params,
+            )
         else:
             log.debug(
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
 
-        # If changes are detected they are to be executed then call provision_permission_set
         return account_change_details
 
     async def apply(self, config: AWSConfig) -> TemplateChangeDetails:
         tasks = []
         template_changes = TemplateChangeDetails(
             resource_id=self.resource_id,
             resource_type=self.resource_type,
             template_path=self.file_path,
             exceptions_seen=[],
         )
         log_params = dict(
             resource_type=self.resource_type, resource_id=self.resource_id
         )
+        relevant_accounts = []
 
         for account in config.accounts:
             if not account.identity_center_details:
                 continue
 
             if evaluate_on_provider(self, account):
-                if ctx.execute:
-                    log_str = "Applying changes to resource."
-                else:
-                    log_str = "Detecting changes for resource."
-                log.info(log_str, account=str(account), **log_params)
+                relevant_accounts.append(str(account))
                 tasks.append(self._apply_to_account(account))
 
+        if not relevant_accounts:
+            return template_changes
+
+        if ctx.execute:
+            log_str = "Applying changes to resource."
+        else:
+            log_str = "Detecting changes for resource."
+
+        log.info(log_str, accounts=relevant_accounts, **log_params)
+
         account_changes = await asyncio.gather(*tasks)
-        template_changes.proposed_changes = [
-            account_change
-            for account_change in account_changes
-            if any(account_change.proposed_changes)
-        ]
-        # aggregate exceptions
-        template_changes.exceptions_seen = [
-            account_change
-            for account_change in account_changes
-            if any(account_change.exceptions_seen)
-        ]
-
-        proposed_changes = [x for x in account_changes if x.proposed_changes]
-
-        if proposed_changes and ctx.execute:
-            log.info(
-                "Successfully applied all or some resource changes to all AWS accounts. Any unapplied resources will have an accompanying error message.",
-                **log_params,
-            )
-        elif proposed_changes and not ctx.execute:
-            log.info(
-                "Successfully detected all or some required resource changes on all AWS accounts. Any unapplied resources will have an accompanying error message.",
-                **log_params,
-            )
+        template_changes.extend_changes(account_changes)
+
+        if template_changes.exceptions_seen:
+            if self.deleted:
+                cmd_verb = "removing"
+            elif ctx.execute:
+                cmd_verb = "applying"
+            else:
+                cmd_verb = "detecting"
+            log_str = f"Error encountered when {cmd_verb} resource changes."
+        elif account_changes and ctx.execute:
+            if self.deleted:
+                self.delete()
+                log_str = "Successfully removed resource."
+            else:
+                log_str = "Successfully applied resource changes."
+        elif account_changes:
+            log_str = "Successfully detected required resource changes."
         else:
-            log.debug("No changes detected for resource on any account.", **log_params)
+            log_str = "No changes detected for resource."
 
+        log.info(log_str, accounts=relevant_accounts, **log_params)
         return template_changes
 
     @property
     def included_children(self):
         return []
 
     def set_included_children(self, value):
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
                 response_key="AccountAssignments",
                 AccountId=account_id,
                 **query_params,
             )
             for account_id in instance_accounts
         ],
         15,
+        1,
         return_exceptions=True,
     )
 
     for account_assignments in all_account_assignments:
         for aa in account_assignments:
             response[aa["PrincipalType"].lower()][aa["PrincipalId"]]["accounts"].append(
                 aa["AccountId"]
@@ -508,15 +509,19 @@
         f"{ea['account_id']}:{ea['resource_type']}:{ea['resource_id']}": ea
         for ea in existing_assignments
     }
 
     for assignment_id, assignment in existing_assignment_map.items():
         if not template_assignment_map.get(assignment_id):
             log_str = "Stale assignments discovered."
-            resource_type="arn:aws:iam::aws:user" if assignment["resource_type"] == "USER" else "arn:aws:iam::aws:group"
+            resource_type = (
+                "arn:aws:iam::aws:user"
+                if assignment["resource_type"] == "USER"
+                else "arn:aws:iam::aws:group"
+            )
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DELETE,
                     account=assignment["account_name"],
                     resource_id=assignment["resource_name"],
                     resource_type=resource_type,
                     attribute="account_assignment",
@@ -536,15 +541,19 @@
                     log_params=log_params,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
             log.info(log_str, details=assignment, **log_params)
 
     for assignment_id, assignment in template_assignment_map.items():
         if not existing_assignment_map.get(assignment_id):
-            resource_type="arn:aws:iam::aws:user" if assignment["resource_type"] == "USER" else "arn:aws:iam::aws:group"
+            resource_type = (
+                "arn:aws:iam::aws:user"
+                if assignment["resource_type"] == "USER"
+                else "arn:aws:iam::aws:group"
+            )
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.CREATE,
                     account=assignment["account_name"],
                     resource_id=assignment["resource_name"],
                     resource_type=resource_type,
                     attribute="account_assignment",
@@ -565,15 +574,15 @@
                     resource_name=assignment["resource_name"],
                     log_params=log_params,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
             log.info(log_str, details=assignment, **log_params)
 
     if tasks:
-        results: list[list[ProposedChange]] = await async_batch_processor(tasks, 10)
+        results: list[list[ProposedChange]] = await async_batch_processor(tasks, 10, 1)
         return list(chain.from_iterable(results))
     else:
         return response
 
 
 async def apply_permission_set_inline_policy(
     identity_center_client,
@@ -631,15 +640,15 @@
             log_str = f"{log_str} {boto_action} InlinePolicyDocument..."
             await boto_crud_call(
                 identity_center_client.put_inline_policy_to_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
                 InlinePolicy=json.dumps(template_inline_policy),
             )
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
     elif not template_inline_policy and existing_inline_policy:
         log_str = "Stale InlinePolicyDocument."
         response.append(
             ProposedChange(
                 change_type=ProposedChangeType.DELETE,
                 attribute="inline_policy",
                 resource_type="aws:identity_center:permission_set",
@@ -650,15 +659,15 @@
         if ctx.execute:
             log_str = f"{log_str} Removing InlinePolicyDocument..."
             await boto_crud_call(
                 identity_center_client.delete_inline_policy_from_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
             )
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
 
     return response
 
 
 async def apply_permission_set_permission_boundary(
     identity_center_client,
     instance_arn: str,
@@ -711,15 +720,15 @@
             log_str = f"{log_str} {boto_action} PermissionsBoundary..."
             await boto_crud_call(
                 identity_center_client.put_permissions_boundary_to_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
                 PermissionsBoundary=template_permission_boundary,
             )
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
     elif existing_permission_boundary and not template_permission_boundary:
         log_str = "Removing PermissionsBoundary discovered."
         response.append(
             ProposedChange(
                 change_type=ProposedChangeType.DELETE,
                 resource_type="aws:identity_center:permission_set",
                 resource_id=permission_set_arn,
@@ -731,15 +740,15 @@
         if ctx.execute:
             log_str = f"{log_str} Deleting PermissionsBoundary..."
             await boto_crud_call(
                 identity_center_client.delete_permissions_boundary_from_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
             )
-        log.info(log_str, **log_params)
+        log.debug(log_str, **log_params)
 
     return response
 
 
 async def apply_permission_set_tags(
     identity_center_client,
     instance_arn: str,
@@ -777,15 +786,15 @@
             apply_awaitable = boto_crud_call(
                 identity_center_client.untag_resource,
                 InstanceArn=instance_arn,
                 ResourceArn=permission_set_arn,
                 TagKeys=tags_to_remove,
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, tags=tags_to_remove, **log_params)
+        log.debug(log_str, tags=tags_to_remove, **log_params)
 
     if tags_to_apply:
         log_str = "New tags discovered in AWS."
         proposed_changes = [
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
                 resource_type="aws:identity_center:permission_set",
@@ -802,15 +811,15 @@
             apply_awaitable = boto_crud_call(
                 identity_center_client.tag_resource,
                 InstanceArn=instance_arn,
                 ResourceArn=permission_set_arn,
                 Tags=tags_to_apply,
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, tags=tags_to_apply, **log_params)
+        log.debug(log_str, tags=tags_to_apply, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
@@ -904,15 +913,15 @@
                 identity_center_client.untag_resource,
                 InstanceArn=instance_arn,
                 ResourceArn=permission_set_arn,
                 TagKeys=tags_to_remove,
             )
         )
 
-    log.info(
+    log.debug(
         "Detaching resources from the permission set.",
         permission_set_arn=permission_set_arn,
         **log_params,
     )
     await async_batch_processor(tasks, 10, 1)
 
     retry_count = 0
@@ -926,15 +935,15 @@
         except ClientError as err:
             err_response = err.response["Error"]
             if (
                 "PermissionSet has ApplicationProfile associated with it."
                 in err_response["Message"]
             ) and retry_count < 10:
                 # Wait for the detached resources to be deleted so that the permission set can be deleted.
-                log.info(
+                log.debug(
                     "Waiting for resources to be detached from the permission set.",
                     **log_params,
                 )
                 retry_count += 1
                 await asyncio.sleep(5)
             elif err_response["Code"] == "ResourceNotFoundException":
                 return
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -718,51 +718,54 @@
             resource_id=self.resource_id,
             resource_type=self.resource_type,
             template_path=self.file_path,
         )
         log_params = dict(
             resource_type=self.resource_type, resource_id=self.resource_id
         )
+        relevant_accounts = []
+
         for account in config.accounts:
             if evaluate_on_provider(self, account):
-                if ctx.execute:
-                    log_str = "Applying changes to resource."
-                else:
-                    log_str = "Detecting changes for resource."
-                log.info(log_str, account=str(account), **log_params)
+                relevant_accounts.append(str(account))
                 tasks.append(self._apply_to_account(account))
 
+        if not relevant_accounts:
+            return template_changes
+
+        if ctx.execute:
+            log_str = "Applying changes to resource."
+        else:
+            log_str = "Detecting changes for resource."
+
+        log.info(log_str, accounts=relevant_accounts, **log_params)
+
         account_changes: list[AccountChangeDetails] = await asyncio.gather(*tasks)
-        template_changes.proposed_changes = [
-            account_change
-            for account_change in account_changes
-            if any(account_change.proposed_changes)
-        ]
-        # aggregate exceptions
-        template_changes.exceptions_seen = [
-            account_change
-            for account_change in account_changes
-            if any(account_change.exceptions_seen)
-        ]
-
-        proposed_changes = [x for x in account_changes if x.proposed_changes]
-
-        if proposed_changes and ctx.execute:
-            log.info(
-                "Successfully applied all or some resource changes to all aws_accounts. Any unapplied resources will have an accompanying error message.",
-                **log_params,
-            )
-        elif proposed_changes and not ctx.execute:
-            log.info(
-                "Successfully detected all or some required resource changes on all aws_accounts. Any unapplied resources will have an accompanying error message.",
-                **log_params,
-            )
+        template_changes.extend_changes(account_changes)
+
+        if template_changes.exceptions_seen:
+            if self.deleted:
+                cmd_verb = "removing"
+            elif ctx.execute:
+                cmd_verb = "applying"
+            else:
+                cmd_verb = "detecting"
+            log_str = f"Error encountered when {cmd_verb} resource changes."
+        elif account_changes and ctx.execute:
+            if self.deleted:
+                self.delete()
+                log_str = "Successfully removed resource."
+            else:
+                log_str = "Successfully applied resource changes."
+        elif account_changes:
+            log_str = "Successfully detected required resource changes."
         else:
-            log.debug("No changes detected for resource on any account.", **log_params)
+            log_str = "No changes detected for resource."
 
+        log.info(log_str, accounts=relevant_accounts, **log_params)
         return template_changes
 
     @property
     def resource_id(self):
         return self.properties.resource_id
 
     @property
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         try:
             return await aio_wrapper(boto_fnc, **kwargs)
         except ClientError as err:
             if "Throttling" in err.response["Error"]["Code"]:
                 if retry_count >= 10:
                     raise
                 retry_count += 1
-                await asyncio.sleep(retry_count / 2)
+                log.warning(f"Throttling error on {str(boto_fnc)}")
+                await asyncio.sleep(retry_count / 4)
                 continue
             elif "AccessDenied" in err.response["Error"]["Code"]:
                 raise
             else:
                 raise
         except NoCredentialsError as exc:
             log.error(
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,57 +111,87 @@
         description="The rule that determines members for this group if the group is a dynamic group."
     )
     members: Optional[List[Member]] = Field(
         [], description="A list of users in the group"
     )
 
     classification: Optional[str] = Field(
-        None, description="Classification of the group", exclude=True,
+        None,
+        description="Classification of the group",
+        exclude=True,
     )
     created_date_time: Optional[str] = Field(
-        None, description="Date and time when the group was created", exclude=True,
+        None,
+        description="Date and time when the group was created",
+        exclude=True,
     )
     creation_options: Optional[List[str]] = Field(
-        None, description="Specifies the group type and its membership", exclude=True,
+        None,
+        description="Specifies the group type and its membership",
+        exclude=True,
     )
     deleted_date_time: Optional[str] = Field(
-        None, description="Date and time when the group was deleted", exclude=True,
+        None,
+        description="Date and time when the group was deleted",
+        exclude=True,
     )
     expiration_date_time: Optional[str] = Field(
-        None, description="Date and time when the group expires", exclude=True,
+        None,
+        description="Date and time when the group expires",
+        exclude=True,
     )
     membership_rule_processing_state: Optional[str] = Field(
         None,
         description="Indicates whether the group is a dynamic group or not",
         exclude=True,
     )
     preferred_data_location: Optional[str] = Field(
-        None, description="Preferred data location of the group", exclude=True,
+        None,
+        description="Preferred data location of the group",
+        exclude=True,
     )
     preferred_language: Optional[str] = Field(
-        None, description="Preferred language of the group", exclude=True,
+        None,
+        description="Preferred language of the group",
+        exclude=True,
     )
     proxy_addresses: Optional[List[str]] = Field(
-        None, description="Proxy addresses of the group", exclude=True,
+        None,
+        description="Proxy addresses of the group",
+        exclude=True,
     )
     renewed_date_time: Optional[str] = Field(
-        None, description="Date and time when the group was renewed", exclude=True,
+        None,
+        description="Date and time when the group was renewed",
+        exclude=True,
     )
     resource_behavior_options: Optional[List[str]] = Field(
-        None, description="Resource behavior options of the group", exclude=True,
+        None,
+        description="Resource behavior options of the group",
+        exclude=True,
     )
     resource_provisioning_options: Optional[List[str]] = Field(
-        None, description="Resource provisioning options of the group", exclude=True,
+        None,
+        description="Resource provisioning options of the group",
+        exclude=True,
     )
     security_identifier: Optional[str] = Field(
-        None, description="Security identifier of the group", exclude=True,
+        None,
+        description="Security identifier of the group",
+        exclude=True,
+    )
+    theme: Optional[str] = Field(
+        None,
+        description="Theme of the group",
+        exclude=True,
     )
-    theme: Optional[str] = Field(None, description="Theme of the group", exclude=True,)
     visibility: Optional[str] = Field(
-        None, description="Visibility of the group", exclude=True,
+        None,
+        description="Visibility of the group",
+        exclude=True,
     )
     extra: Any = Field(None, description=("Extra attributes to store"), exclude=True)
 
     def __init__(self, **data):
         if "mail_nickname" not in data:
             data["mail_nickname"] = data.get("name")
         super().__init__(**data)
@@ -176,16 +206,20 @@
 
     @classmethod
     def from_azure_response(cls, azure_response: dict):
         azure_response = normalize_dict_keys(azure_response)
         # Filter unwanted keys
         group_id = azure_response.pop("id")
         name = azure_response.pop("display_name")
-        azure_response = {x: y for x, y in azure_response.items() if not x.startswith('@odata')}
-        azure_response = {x: y for x, y in azure_response.items() if not x.startswith('on_premises')}
+        azure_response = {
+            x: y for x, y in azure_response.items() if not x.startswith("@odata")
+        }
+        azure_response = {
+            x: y for x, y in azure_response.items() if not x.startswith("on_premises")
+        }
         return cls(
             group_id=group_id,
             name=name,
             members=[],
             **azure_response,
         )
 
@@ -348,18 +382,14 @@
 
         if ctx.execute and not change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
-            # TODO: Check if deleted, remove git commit the change to ratify it
-            if self.deleted:
-                self.delete()
-            self.write()
         elif change_details.exceptions_seen:
             cmd_verb = "apply" if ctx.execute else "scan for"
             log.error(
                 f"Failed to successfully {cmd_verb} resource changes",
                 **log_params,
             )
         else:
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from typing import TYPE_CHECKING, List, Optional
 
 from aiohttp import ClientResponseError
-from pydantic import ValidationError
 
 from iambic.core.context import ctx
 from iambic.core.logger import log
 from iambic.core.models import ProposedChange, ProposedChangeType
 from iambic.core.utils import GlobalRetryController, snake_to_camelback
 from iambic.plugins.v0_1_0.azure_ad.group.models import (
     GroupTemplateProperties,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import msal
 from pydantic import BaseModel, Field, SecretStr
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate, TemplateChangeDetails
-from iambic.core.utils import exceptions_in_proposed_changes
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.azure_ad.iambic_plugin import AzureADConfig
 
     MappingIntStrAny = typing.Mapping[int | str, any]
     AbstractSetIntStr = typing.AbstractSet[int | str]
 
@@ -191,25 +190,32 @@
                 log_str = "Detecting changes for resource."
             log.info(log_str, idp_name=azure_ad_organization.idp_name, **log_params)
             tasks.append(self._apply_to_account(azure_ad_organization))
 
         account_changes = list(await asyncio.gather(*tasks))
         template_changes.extend_changes(account_changes)
 
-        if exceptions_in_proposed_changes(template_changes.dict()):
+        if template_changes.exceptions_seen:
             cmd_verb = "applying" if ctx.execute else "detecting"
             log.error(
                 f"Error encountered when {cmd_verb} resource changes.",
                 **log_params,
             )
         elif account_changes and ctx.execute:
-            log.info(
-                "Successfully applied resource changes to all Azure AD organizations.",
-                **log_params,
-            )
+            if self.deleted:
+                self.delete()
+                log.info(
+                    "Successfully removed resource from all Azure AD organizations.",
+                    **log_params,
+                )
+            else:
+                log.info(
+                    "Successfully applied resource changes to all Azure AD organizations.",
+                    **log_params,
+                )
         elif account_changes:
             log.info(
                 "Successfully detected required resource changes on all Azure AD organizations.",
                 **log_params,
             )
         else:
             log.debug(
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,41 +41,64 @@
     mail_nickname: Optional[str]
     given_name: Optional[str]
     employee_id: Optional[str]
     domain: Optional[str]
     fullname: Optional[str]
     status: Optional[UserStatus]
 
-    business_phones: Optional[list[str]] = Field([], description="List of business phone numbers", exclude=True)
-    id: Optional[str] = Field(None, description="Unique identifier for the user", exclude=True)
-    job_title: Optional[str] = Field(None, description="Job title of the user", exclude=True)
-    mail: Optional[str] = Field(None, description="Email address of the user", exclude=True)
-    mobile_phone: Optional[str] = Field(None, description="Mobile phone number of the user", exclude=True)
-    office_location: Optional[str] = Field(None, description="Office location of the user", exclude=True)
-    preferred_language: Optional[str] = Field(None, description="Preferred language of the user", exclude=True)
-    surname: Optional[str] = Field(None, description="Surname of the user", exclude=True)
-    user_principal_name: Optional[str] = Field(None, description="User principal name of the user", exclude=True)
+    business_phones: Optional[list[str]] = Field(
+        [], description="List of business phone numbers", exclude=True
+    )
+    id: Optional[str] = Field(
+        None, description="Unique identifier for the user", exclude=True
+    )
+    job_title: Optional[str] = Field(
+        None, description="Job title of the user", exclude=True
+    )
+    mail: Optional[str] = Field(
+        None, description="Email address of the user", exclude=True
+    )
+    mobile_phone: Optional[str] = Field(
+        None, description="Mobile phone number of the user", exclude=True
+    )
+    office_location: Optional[str] = Field(
+        None, description="Office location of the user", exclude=True
+    )
+    preferred_language: Optional[str] = Field(
+        None, description="Preferred language of the user", exclude=True
+    )
+    surname: Optional[str] = Field(
+        None, description="Surname of the user", exclude=True
+    )
+    user_principal_name: Optional[str] = Field(
+        None, description="User principal name of the user", exclude=True
+    )
 
     @property
     def resource_type(self) -> str:
         return "azure_ad:user"
 
     @property
     def resource_id(self) -> str:
         return self.username
 
     @classmethod
     def from_azure_response(cls, azure_response: dict) -> UserTemplateProperties:
         unwanted_keys = [
             "password_profile",
+            "account_enabled",
         ]
         azure_response = normalize_dict_keys(azure_response)
         # Filter unwanted keys
-        azure_response = {x: y for x, y in azure_response.items() if x not in unwanted_keys}
-        azure_response = {x: y for x, y in azure_response.items() if not x.startswith('@odata')}
+        azure_response = {
+            x: y for x, y in azure_response.items() if x not in unwanted_keys
+        }
+        azure_response = {
+            x: y for x, y in azure_response.items() if not x.startswith("@odata")
+        }
 
         return cls(
             user_id=azure_response.get("id"),
             username=azure_response.get("user_principal_name"),
             **azure_response,
         )
 
@@ -144,16 +167,14 @@
                     ]
                 )
                 return change_details
 
         user_exists = bool(cloud_user)
         tasks = []
 
-        await self.remove_expired_resources()
-
         if not user_exists and not self.deleted:
             log_str = "New resource found in code."
             change_details.extend_changes(
                 [
                     ProposedChange(
                         change_type=ProposedChangeType.CREATE,
                         resource_id=self.resource_id,
@@ -212,18 +233,14 @@
 
         if ctx.execute and not change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
-            # TODO: Check if deleted, remove git commit the change to ratify it
-            if self.deleted:
-                self.delete()
-            self.write()
         elif change_details.exceptions_seen:
             cmd_verb = "apply" if ctx.execute else "scan for"
             log.error(
                 f"Failed to successfully {cmd_verb} resource changes",
                 **log_params,
             )
         else:
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     - allow_template_ref: If True, attempt to resolve the user by loading the IAMbic template
 
     Returns:
     - The `User` instance, representing the user in Azure AD.
     """
     assert user_id or username
 
-
     if user_id:
         async with GlobalRetryController(
             fn_identifier="azure_ad.get_user"
         ) as retry_controller:
             fn = functools.partial(azure_ad_organization.get, f"users/{user_id}")
             user = await retry_controller(fn)
             return UserTemplateProperties.from_azure_response(user)
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,23 +235,21 @@
                     google_project,
                     log_params,
                 ),
                 maybe_delete_group(
                     self,
                     google_project,
                     log_params,
-                )
+                ),
             ]
         )
 
         changes_made = await asyncio.gather(*tasks)
         if any(changes_made):
-            change_details.extend_changes(
-                list(chain.from_iterable(changes_made))
-            )
+            change_details.extend_changes(list(chain.from_iterable(changes_made)))
 
         if ctx.execute:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,17 @@
             AsyncMock(return_value=mock_service),
         )
         self.google_workspace_config.workspaces = [
             self.google_project1,
             self.google_project2,
         ]
 
+    def tearDown(self):
+        ctx.eval_only = False
+
     async def test_apply_with_projects(self):
         ctx.eval_only = True
         google_workspace_config = copy.deepcopy(self.google_workspace_config)
         template_changes = await self.template.apply(google_workspace_config)
 
         self.assertIsInstance(template_changes, TemplateChangeDetails)
         self.assertEqual(template_changes.resource_id, "test@example.com")
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     AccountChangeDetails,
     BaseModel,
     BaseTemplate,
     ExpiryModel,
     TemplateChangeDetails,
 )
 from iambic.core.utils import NoqSemaphore
-from iambic.plugins.v0_1_0.aws.utils import remove_expired_resources
 from iambic.plugins.v0_1_0.okta.app.utils import (
     get_app,
     maybe_delete_app,
     update_app_assignments,
     update_app_name,
 )
 from iambic.plugins.v0_1_0.okta.models import App, Assignment, Status
@@ -181,17 +180,18 @@
                 # Don't overwrite a resource during config discovery
                 change_details.new_value = {}
                 return change_details
 
         app_exists = bool(current_app)
         tasks = []
 
-        self = await remove_expired_resources(
-            self, self.resource_type, self.resource_id
-        )
+        # Marking for deletion. This shouldn't be done on the fly.
+        # self = await remove_expired_resources(
+        #     self, self.resource_type, self.resource_id
+        # )
 
         if not app_exists and not self.deleted:
             log.error(
                 "Iambic does not support creating new apps. "
                 "Please create the app in Okta and then import it.",
                 **log_params,
             )
@@ -229,17 +229,15 @@
                     log_params,
                 ),
             ]
         )
 
         changes_made = await asyncio.gather(*tasks)
         if any(changes_made):
-            change_details.extend_changes(
-                list(chain.from_iterable(changes_made))
-            )
+            change_details.extend_changes(list(chain.from_iterable(changes_made)))
 
         if ctx.execute:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                 change_summary={
                     "AssignmentsToUnassign": {
                         "user_assignments_to_unassign": user_assignments_to_unassign,
                         "group_assignments_to_unassign": group_assignments_to_unassign,
                     }
                 },
                 current_value=current_user_assignments + current_group_assignments,
-                new_value = desired_user_assignments + desired_group_assignments,
+                new_value=desired_user_assignments + desired_group_assignments,
             )
         )
 
     if assignments_to_assign:
         response.append(
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,45 @@
 OKTA_GROUP_TEMPLATE_TYPE = "NOQ::Okta::Group"
 
 
 class UserSimple(BaseModel, ExpiryModel):
     username: str
     status: Optional[UserStatus] = UserStatus.active
 
-    background_check_status: Optional[bool] = Field(False, description="Background check status for the group", exclude=True)
-    created: Optional[str] = Field(None, description="Created date for the group", exclude=True)
-    domain: Optional[str] = Field(None, description="Domain for the group", exclude=True)
+    background_check_status: Optional[bool] = Field(
+        False, description="Background check status for the group", exclude=True
+    )
+    created: Optional[str] = Field(
+        None, description="Created date for the group", exclude=True
+    )
+    domain: Optional[str] = Field(
+        None, description="Domain for the group", exclude=True
+    )
     extra: Any = Field(None, description=("Extra attributes to store"), exclude=True)
-    fullname: Optional[str] = Field(None, description="Full name for the group", exclude=True)
-    groups: Optional[List[str]] = Field(None, description="Groups for the group", exclude=True)
-    idp_name: Optional[str] = Field(None, description="IDP name for the group", exclude=True)
-    profile: Optional[Any] = Field(None, description="Profile for the group", exclude=True)
-    status: Optional[UserStatus] = Field(None, description="Status for the group", exclude=True)
-    updated: Optional[str] = Field(None, description="Updated date for the group", exclude=True)
-    user_id: Optional[str] = Field(None, description="User ID for the group", exclude=True)
-
+    fullname: Optional[str] = Field(
+        None, description="Full name for the group", exclude=True
+    )
+    groups: Optional[List[str]] = Field(
+        None, description="Groups for the group", exclude=True
+    )
+    idp_name: Optional[str] = Field(
+        None, description="IDP name for the group", exclude=True
+    )
+    profile: Optional[Any] = Field(
+        None, description="Profile for the group", exclude=True
+    )
+    status: Optional[UserStatus] = Field(
+        None, description="Status for the group", exclude=True
+    )
+    updated: Optional[str] = Field(
+        None, description="Updated date for the group", exclude=True
+    )
+    user_id: Optional[str] = Field(
+        None, description="User ID for the group", exclude=True
+    )
 
     @property
     def resource_type(self) -> str:
         return "okta:user"
 
     @property
     def resource_id(self) -> str:
@@ -79,18 +98,19 @@
         "", description="Unique Group ID for the group. Usually it's {idp-name}-{name}"
     )
     file_path: str = Field("", description="File path of the group", exclude=True)
     description: Optional[str] = Field("", description="Description of the group")
     extra: Any = Field(None, description=("Extra attributes to store"))
     members: List[UserSimple] = Field([], description="Users in the group")
     identifier: Optional[str] = Field(
-        None, description="Identifier for the group. Usually it's the group name",
+        None,
+        description="Identifier for the group. Usually it's the group name",
         exclude=True,
     )
-    
+
     @classmethod
     def iambic_specific_knowledge(cls) -> set[str]:
         return {"extra", "metadata_commented_dict"}
 
     @property
     def resource_type(self) -> str:
         return "okta:group"
@@ -288,17 +308,15 @@
                 # TODO
                 # upgrade_group_application_assignments
             ]
         )
 
         changes_made = await asyncio.gather(*tasks)
         if any(changes_made):
-            change_details.extend_changes(
-                list(chain.from_iterable(changes_made))
-            )
+            change_details.extend_changes(list(chain.from_iterable(changes_made)))
 
         if ctx.execute:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from typing import TYPE_CHECKING, List, Optional
 
 import okta.models as models
-
 from iambic.core.context import ctx
 from iambic.core.logger import log
 from iambic.core.models import ProposedChange, ProposedChangeType
 from iambic.core.utils import GlobalRetryController
 from iambic.plugins.v0_1_0.okta.models import Group, User
 from iambic.plugins.v0_1_0.okta.utils import generate_user_profile, handle_okta_fn
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.okta.app.models import OktaAppTemplate
 from iambic.plugins.v0_1_0.okta.group.models import OktaGroupTemplate
 from iambic.plugins.v0_1_0.okta.handlers import import_okta_resources, load
 from iambic.plugins.v0_1_0.okta.user.models import OktaUserTemplate
-from okta.client import Client as OktaClient
 
 
 class OktaOrganization(BaseModel):
     idp_name: str
     org_url: str
     api_token: SecretStr
     request_timeout: int = 60
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,15 @@
                     log_params,
                 ),
             ]
         )
 
         changes_made = await asyncio.gather(*tasks)
         if any(changes_made):
-            change_details.extend_changes(
-                list(chain.from_iterable(changes_made))
-            )
+            change_details.extend_changes(list(chain.from_iterable(changes_made)))
 
         if ctx.execute:
             log.debug(
                 "Successfully finished execution for resource",
                 changes_made=bool(change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/request_handler/expire_resources.py` & `iambic_core-0.1.198/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/request_handler/git_apply.py` & `iambic_core-0.1.198/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/iambic/request_handler/git_plan.py` & `iambic_core-0.1.198/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.186/pyproject.toml` & `iambic_core-0.1.198/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.1.186"
+version = "0.1.198"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.1.186/PKG-INFO` & `iambic_core-0.1.198/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.1.186
+Version: 0.1.198
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -51,14 +51,15 @@
 Requires-Dist: types-dateparser (>=1.1.4.5,<2.0.0.0)
 Requires-Dist: types-mock (>=5.0.0.5,<6.0.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
+[![codecov.io](https://codecov.io/github/noqdev/iambic/coverage.svg?branch=main)](https://codecov.io/github/noqdev/iambic?branch=main)
 
 # IAMbic: Cloud IAM as Code
 
 "IAMbic: the Terraform of Cloud IAM"
 
 Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://www.iambic.org](https://www.iambic.org).
 
@@ -73,14 +74,24 @@
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
 ## Getting Started
 
 Dive into IAMbic with our [quick-start guide](http://iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
+## Installing IAMbic and Supported Versions
+
+IAMbic is available on PyPI:
+
+```console
+python -m pip install iambic-core
+```
+
+IAMbic officially supports Python 3.9+.
+
 ### Template Examples
 
 Here are some examples showcasing IAMbic's capabilities:
 
 #### AWS Multi-Account Cloudwatch Role
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
```

