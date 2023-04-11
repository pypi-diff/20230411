# Comparing `tmp/renku-2.3.2.tar.gz` & `tmp/renku-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-2.3.2.tar", max compression
+gzip compressed data, was "renku-2.4.0rc1.tar", max compression
```

## Comparing `renku-2.3.2.tar` & `renku-2.4.0rc1.tar`

### file list

```diff
@@ -1,489 +1,1710 @@
--rw-r--r--   0        0        0      900 2023-03-13 14:44:59.395461 renku-2.3.2/AUTHORS.rst
--rw-r--r--   0        0        0   172627 2023-03-13 14:44:59.399461 renku-2.3.2/CHANGES.rst
--rw-r--r--   0        0        0    11358 2023-03-13 14:44:59.399461 renku-2.3.2/LICENSE
--rw-r--r--   0        0        0    12889 2023-03-13 14:44:59.399461 renku-2.3.2/README.rst
--rw-r--r--   0        0        0    10285 2023-03-13 14:45:53.116555 renku-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     4482 2023-03-13 14:44:59.459467 renku-2.3.2/renku/__init__.py
--rw-r--r--   0        0        0      808 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/__init__.py
--rw-r--r--   0        0        0     2161 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/__init__.py
--rw-r--r--   0        0        0     4755 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/activities.py
--rw-r--r--   0        0        0     6542 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/datasets.py
--rw-r--r--   0        0        0     2088 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/external.py
--rw-r--r--   0        0        0     2801 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/githooks.py
--rw-r--r--   0        0        0     1532 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/migration.py
--rw-r--r--   0        0        0     2348 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/project.py
--rw-r--r--   0        0        0     1519 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/storage.py
--rw-r--r--   0        0        0     4333 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/validate_shacl.py
--rw-r--r--   0        0        0     4913 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/checks/workflow.py
--rw-r--r--   0        0        0     3896 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/clone.py
--rw-r--r--   0        0        0      865 2023-03-13 14:44:59.459467 renku-2.3.2/renku/command/command_builder/__init__.py
--rw-r--r--   0        0        0    16715 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/command.py
--rw-r--r--   0        0        0     1988 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/communication.py
--rw-r--r--   0        0        0     5345 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/database.py
--rw-r--r--   0        0        0     1738 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/lock.py
--rw-r--r--   0        0        0     1518 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/migration.py
--rw-r--r--   0        0        0     7731 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/command_builder/repo.py
--rw-r--r--   0        0        0     4844 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/config.py
--rw-r--r--   0        0        0     5738 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/dataset.py
--rw-r--r--   0        0        0     2742 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/doctor.py
--rw-r--r--   0        0        0      807 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/__init__.py
--rw-r--r--   0        0        0     2697 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/activity.py
--rw-r--r--   0        0        0     5696 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/dataset_files.py
--rw-r--r--   0        0        0     2130 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/dataset_tags.py
--rw-r--r--   0        0        0     3268 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/datasets.py
--rw-r--r--   0        0        0     1244 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/json.py
--rw-r--r--   0        0        0     1387 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/session.py
--rw-r--r--   0        0        0     2801 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/tabulate.py
--rw-r--r--   0        0        0     2760 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/format/workflow.py
--rw-r--r--   0        0        0     1036 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/gc.py
--rw-r--r--   0        0        0     1178 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/githooks.py
--rw-r--r--   0        0        0     9907 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/graph.py
--rw-r--r--   0        0        0     1124 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/group.py
--rw-r--r--   0        0        0     1227 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/init.py
--rw-r--r--   0        0        0     3148 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/log.py
--rw-r--r--   0        0        0     1265 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/login.py
--rw-r--r--   0        0        0     2851 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/mergetool.py
--rw-r--r--   0        0        0     7653 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/migrate.py
--rw-r--r--   0        0        0     9167 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/move.py
--rw-r--r--   0        0        0     1039 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/options.py
--rw-r--r--   0        0        0     1386 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/project.py
--rw-r--r--   0        0        0     4948 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/remove.py
--rw-r--r--   0        0        0     3170 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/rerun.py
--rw-r--r--   0        0        0    11011 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/rollback.py
--rw-r--r--   0        0        0     1624 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/run.py
--rw-r--r--   0        0        0     3412 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/save.py
--rw-r--r--   0        0        0      803 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/__init__.py
--rw-r--r--   0        0        0     5624 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/activity.py
--rw-r--r--   0        0        0     1780 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/agent.py
--rw-r--r--   0        0        0     1271 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/annotation.py
--rw-r--r--   0        0        0     9032 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/calamus.py
--rw-r--r--   0        0        0     3223 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/composite_plan.py
--rw-r--r--   0        0        0     8247 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/dataset.py
--rw-r--r--   0        0        0     1481 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/entity.py
--rw-r--r--   0        0        0     4053 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/parameter.py
--rw-r--r--   0        0        0     3464 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/plan.py
--rw-r--r--   0        0        0     3443 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/project.py
--rw-r--r--   0        0        0     1866 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/schema/workflow_file.py
--rw-r--r--   0        0        0     1602 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/session.py
--rw-r--r--   0        0        0     1060 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/status.py
--rw-r--r--   0        0        0     3968 2023-03-13 14:44:59.463467 renku-2.3.2/renku/command/storage.py
--rw-r--r--   0        0        0     1943 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/template.py
--rw-r--r--   0        0        0     3409 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/update.py
--rw-r--r--   0        0        0     1750 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/util.py
--rw-r--r--   0        0        0     5195 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/version.py
--rw-r--r--   0        0        0      805 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/__init__.py
--rw-r--r--   0        0        0    14016 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/activity_graph.py
--rw-r--r--   0        0        0     1694 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/agent.py
--rw-r--r--   0        0        0     8780 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/composite_plan.py
--rw-r--r--   0        0        0     2175 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/dataset.py
--rw-r--r--   0        0        0     7836 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/graph.py
--rw-r--r--   0        0        0    12534 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/log.py
--rw-r--r--   0        0        0     9414 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/plan.py
--rw-r--r--   0        0        0     3343 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/project.py
--rw-r--r--   0        0        0     5558 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/template.py
--rw-r--r--   0        0        0    14493 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/text_canvas.py
--rw-r--r--   0        0        0     4829 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/view_model/workflow_file.py
--rw-r--r--   0        0        0     4138 2023-03-13 14:44:59.467468 renku-2.3.2/renku/command/workflow.py
--rw-r--r--   0        0        0      781 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/__init__.py
--rw-r--r--   0        0        0     6202 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/config.py
--rw-r--r--   0        0        0     2754 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/constant.py
--rw-r--r--   0        0        0      802 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/__init__.py
--rw-r--r--   0        0        0     2991 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/context.py
--rw-r--r--   0        0        0    53162 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/dataset.py
--rw-r--r--   0        0        0    16948 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/dataset_add.py
--rw-r--r--   0        0        0     9937 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/datasets_provenance.py
--rw-r--r--   0        0        0     3766 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/pointer_file.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/__init__.py
--rw-r--r--   0        0        0    11158 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/api.py
--rw-r--r--   0        0        0     6630 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/azure.py
--rw-r--r--   0        0        0     2315 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/cloud.py
--rw-r--r--   0        0        0    20227 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/dataverse.py
--rw-r--r--   0        0        0     3354 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/dataverse_metadata_templates.py
--rw-r--r--   0        0        0     4891 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/doi.py
--rw-r--r--   0        0        0     5608 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/factory.py
--rw-r--r--   0        0        0     7336 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/git.py
--rw-r--r--   0        0        0    11016 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/local.py
--rw-r--r--   0        0        0     5846 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/models.py
--rw-r--r--   0        0        0    10144 2023-03-13 14:44:59.467468 renku-2.3.2/renku/core/dataset/providers/olos.py
--rw-r--r--   0        0        0    22193 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/providers/renku.py
--rw-r--r--   0        0        0     2598 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/providers/repository.py
--rw-r--r--   0        0        0     5928 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/providers/s3.py
--rw-r--r--   0        0        0     6926 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/providers/web.py
--rw-r--r--   0        0        0    18673 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/providers/zenodo.py
--rw-r--r--   0        0        0     4010 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/request_model.py
--rw-r--r--   0        0        0     5398 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/dataset/tag.py
--rw-r--r--   0        0        0    25560 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/errors.py
--rw-r--r--   0        0        0     1147 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/gc.py
--rw-r--r--   0        0        0     7431 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/git.py
--rw-r--r--   0        0        0     2187 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/githooks.py
--rw-r--r--   0        0        0    16547 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/init.py
--rw-r--r--   0        0        0      799 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/__init__.py
--rw-r--r--   0        0        0     3765 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/activity_gateway.py
--rw-r--r--   0        0        0     1442 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/database_gateway.py
--rw-r--r--   0        0        0     2119 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/dataset_gateway.py
--rw-r--r--   0        0        0     2020 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/plan_gateway.py
--rw-r--r--   0        0        0     1236 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/project_gateway.py
--rw-r--r--   0        0        0     4576 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/storage.py
--rw-r--r--   0        0        0     1806 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/interface/workflow_file_parser.py
--rw-r--r--   0        0        0    10437 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/login.py
--rw-r--r--   0        0        0      788 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/__init__.py
--rw-r--r--   0        0        0     1146 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0003__0_pyld2.py
--rw-r--r--   0        0        0    15350 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0003__1_jsonld.py
--rw-r--r--   0        0        0     9612 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0003__2_initial.py
--rw-r--r--   0        0        0     1146 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0004__0_pyld2.py
--rw-r--r--   0        0        0     5342 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0004__submodules.py
--rw-r--r--   0        0        0     1572 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0005__1_pyld2.py
--rw-r--r--   0        0        0    16157 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0005__2_cwl.py
--rw-r--r--   0        0        0     1039 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0006__dataset_context.py
--rw-r--r--   0        0        0     1454 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0007__source_url.py
--rw-r--r--   0        0        0     1199 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0008__dataset_metadata.py
--rw-r--r--   0        0        0    30449 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0009__new_metadata_storage.py
--rw-r--r--   0        0        0    14102 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/m_0010__metadata_fixes.py
--rw-r--r--   0        0        0    10159 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/migrate.py
--rw-r--r--   0        0        0      794 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/models/__init__.py
--rw-r--r--   0        0        0     5854 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/models/migration.py
--rw-r--r--   0        0        0     3894 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/models/refs.py
--rw-r--r--   0        0        0     5115 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/models/v10.py
--rw-r--r--   0        0        0    11852 2023-03-13 14:44:59.471468 renku-2.3.2/renku/core/migration/models/v3.py
--rw-r--r--   0        0        0     2446 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/migration/models/v7.py
--rw-r--r--   0        0        0     4611 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/migration/models/v8.py
--rw-r--r--   0        0        0    74232 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/migration/models/v9.py
--rw-r--r--   0        0        0     7935 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/migration/utils/__init__.py
--rw-r--r--   0        0        0     8049 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/migration/utils/conversion.py
--rw-r--r--   0        0        0      848 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/__init__.py
--rw-r--r--   0        0        0     1491 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/dataset_provider.py
--rw-r--r--   0        0        0     2991 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/implementations/__init__.py
--rw-r--r--   0        0        0     1814 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/pluginmanager.py
--rw-r--r--   0        0        0     3381 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/provider.py
--rw-r--r--   0        0        0     1863 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/run.py
--rw-r--r--   0        0        0     1478 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/session.py
--rw-r--r--   0        0        0     4374 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/workflow.py
--rw-r--r--   0        0        0     3089 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/plugin/workflow_file_parser.py
--rw-r--r--   0        0        0     3385 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/project.py
--rw-r--r--   0        0        0      804 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/session/__init__.py
--rw-r--r--   0        0        0    11940 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/session/docker.py
--rw-r--r--   0        0        0    19785 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/session/renkulab.py
--rw-r--r--   0        0        0    11878 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/session/session.py
--rw-r--r--   0        0        0     2239 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/session/utils.py
--rw-r--r--   0        0        0    22276 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/storage.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/template/__init__.py
--rw-r--r--   0        0        0    21492 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/template/template.py
--rw-r--r--   0        0        0    14503 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/template/usecase.py
--rw-r--r--   0        0        0      788 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/__init__.py
--rw-r--r--   0        0        0    10319 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/communication.py
--rw-r--r--   0        0        0     6653 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/contexts.py
--rw-r--r--   0        0        0     1332 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/dataset.py
--rw-r--r--   0        0        0     2345 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/datetime8601.py
--rw-r--r--   0        0        0     1408 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/doi.py
--rw-r--r--   0        0        0     1999 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/file_size.py
--rw-r--r--   0        0        0    40329 2023-03-13 14:44:59.475468 renku-2.3.2/renku/core/util/git.py
--rw-r--r--   0        0        0     1281 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/jwt.py
--rw-r--r--   0        0        0     6754 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/metadata.py
--rw-r--r--   0        0        0    10121 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/os.py
--rw-r--r--   0        0        0     7658 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/requests.py
--rw-r--r--   0        0        0     1652 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/shacl.py
--rw-r--r--   0        0        0     6838 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/ssh.py
--rw-r--r--   0        0        0     2194 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/tabulate.py
--rw-r--r--   0        0        0     2261 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/template_vars.py
--rw-r--r--   0        0        0     5373 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/urls.py
--rw-r--r--   0        0        0     1546 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/util.py
--rw-r--r--   0        0        0     1079 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/uuid.py
--rw-r--r--   0        0        0     2873 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/util/yaml.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/__init__.py
--rw-r--r--   0        0        0    22743 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/activity.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/converters/__init__.py
--rw-r--r--   0        0        0    18185 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/converters/cwl.py
--rw-r--r--   0        0        0     5166 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/converters/renku.py
--rw-r--r--   0        0        0    18815 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/execute.py
--rw-r--r--   0        0        0      793 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/model/__init__.py
--rw-r--r--   0        0        0     6554 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/model/concrete_execution_graph.py
--rw-r--r--   0        0        0    37327 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/model/workflow_file.py
--rw-r--r--   0        0        0      799 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/parser/__init__.py
--rw-r--r--   0        0        0    10655 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/parser/renku.py
--rw-r--r--   0        0        0    34230 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/plan.py
--rw-r--r--   0        0        0    33080 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/plan_factory.py
--rw-r--r--   0        0        0      796 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/providers/__init__.py
--rw-r--r--   0        0        0     6023 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/providers/cwltool.py
--rw-r--r--   0        0        0     4295 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/providers/local.py
--rw-r--r--   0        0        0    13417 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/providers/toil.py
--rw-r--r--   0        0        0    13586 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/run.py
--rw-r--r--   0        0        0     1705 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/types.py
--rw-r--r--   0        0        0     7097 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/value_resolution.py
--rw-r--r--   0        0        0     5113 2023-03-13 14:44:59.479469 renku-2.3.2/renku/core/workflow/workflow_file.py
--rw-r--r--   0        0        0       40 2023-03-13 14:44:59.479469 renku-2.3.2/renku/data/__init__.py
--rw-r--r--   0        0        0      114 2023-03-13 14:44:59.479469 renku-2.3.2/renku/data/defaults.ini
--rw-r--r--   0        0        0     3364 2023-03-13 14:44:59.479469 renku-2.3.2/renku/data/gitignore.default
--rwxr-xr-x   0        0        0     4436 2023-03-13 14:44:59.479469 renku-2.3.2/renku/data/pre-commit.sh
--rw-r--r--   0        0        0    48383 2023-03-13 14:44:59.479469 renku-2.3.2/renku/data/shacl_shape.json
--rw-r--r--   0        0        0      803 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/__init__.py
--rw-r--r--   0        0        0    26145 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/dataset.py
--rw-r--r--   0        0        0     1304 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/dataset_provider.py
--rw-r--r--   0        0        0     2790 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/datastructures.py
--rw-r--r--   0        0        0     2576 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/entity.py
--rw-r--r--   0        0        0     1007 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/enums.py
--rw-r--r--   0        0        0     5103 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/git.py
--rw-r--r--   0        0        0     8359 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/project.py
--rw-r--r--   0        0        0    11707 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/project_context.py
--rw-r--r--   0        0        0      866 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/provenance/__init__.py
--rw-r--r--   0        0        0    12812 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/provenance/activity.py
--rw-r--r--   0        0        0     5193 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/provenance/agent.py
--rw-r--r--   0        0        0     1304 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/provenance/annotation.py
--rw-r--r--   0        0        0     1567 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/provenance/parameter.py
--rw-r--r--   0        0        0     6270 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/session.py
--rw-r--r--   0        0        0     1507 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/sort.py
--rw-r--r--   0        0        0    23154 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/template.py
--rw-r--r--   0        0        0      818 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/__init__.py
--rw-r--r--   0        0        0    15954 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/composite_plan.py
--rw-r--r--   0        0        0     1567 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/converters/__init__.py
--rw-r--r--   0        0        0    18161 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/parameter.py
--rw-r--r--   0        0        0    16624 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/plan.py
--rw-r--r--   0        0        0     1678 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/provider.py
--rw-r--r--   0        0        0     4386 2023-03-13 14:44:59.483469 renku-2.3.2/renku/domain_model/workflow/workflow_file.py
--rw-r--r--   0        0        0      804 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/__init__.py
--rw-r--r--   0        0        0    41443 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/database.py
--rw-r--r--   0        0        0      810 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/__init__.py
--rw-r--r--   0        0        0    12135 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/activity_gateway.py
--rw-r--r--   0        0        0     5869 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/database_gateway.py
--rw-r--r--   0        0        0     3400 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/dataset_gateway.py
--rw-r--r--   0        0        0     3164 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/plan_gateway.py
--rw-r--r--   0        0        0     1735 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/gateway/project_gateway.py
--rw-r--r--   0        0        0    17982 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/git_merger.py
--rw-r--r--   0        0        0     4696 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/immutable.py
--rw-r--r--   0        0        0     2418 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/persistent.py
--rw-r--r--   0        0        0    72142 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/repository.py
--rw-r--r--   0        0        0      808 2023-03-13 14:44:59.483469 renku-2.3.2/renku/infrastructure/storage/__init__.py
--rw-r--r--   0        0        0     2246 2023-03-13 14:44:59.487470 renku-2.3.2/renku/infrastructure/storage/factory.py
--rw-r--r--   0        0        0     6760 2023-03-13 14:44:59.487470 renku-2.3.2/renku/infrastructure/storage/rclone.py
--rw-r--r--   0        0        0      913 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      553 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      637 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      523 2023-03-13 14:45:51.692452 renku-2.3.2/renku/templates/.github/dependabot.yml
--rw-r--r--   0        0        0      396 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/.github/workflows/github-project.yml
--rw-r--r--   0        0        0     3940 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/.gitignore
--rw-r--r--   0        0        0       27 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      984 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2087 2023-03-13 14:45:51.692452 renku-2.3.2/renku/templates/R-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/README.md
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/environment.yml
--rw-r--r--   0        0        0      360 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/install.R
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    14286 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/R-minimal.png
--rw-r--r--   0        0        0     4846 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/README.md
--rw-r--r--   0        0        0       27 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2077 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/README.md
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/install.R
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-03-13 14:45:51.684451 renku-2.3.2/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    44589 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/bioconductor.png
--rw-r--r--   0        0        0       27 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       50 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2469 2023-03-13 14:45:51.692452 renku-2.3.2/renku/templates/julia-minimal/Dockerfile
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/Manifest.toml
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/Project.toml
--rw-r--r--   0        0        0     1842 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/README.md
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julia-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    13782 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/julialang.png
--rw-r--r--   0        0        0     1174 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/manifest.yaml
--rw-r--r--   0        0        0       17 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/.dockerignore
--rw-r--r--   0        0        0       77 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/.renkulfsignore
--rw-r--r--   0        0        0     2414 2023-03-13 14:45:51.692452 renku-2.3.2/renku/templates/minimal/Dockerfile
--rw-r--r--   0        0        0     1439 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0       27 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/.dockerignore
--rw-r--r--   0        0        0     5401 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2159 2023-03-13 14:45:51.692452 renku-2.3.2/renku/templates/python-minimal/Dockerfile
--rw-r--r--   0        0        0     1597 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/README.md
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    25599 2023-03-13 14:45:51.688451 renku-2.3.2/renku/templates/python-minimal.png
--rw-r--r--   0        0        0      787 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/__init__.py
--rw-r--r--   0        0        0     1292 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/__init__.py
--rw-r--r--   0        0        0      787 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/graph/__init__.py
--rw-r--r--   0        0        0     2543 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/graph/rdf.py
--rw-r--r--   0        0        0      788 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/__init__.py
--rw-r--r--   0        0        0    16472 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/activity.py
--rw-r--r--   0        0        0     4672 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/dataset.py
--rw-r--r--   0        0        0    10385 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/parameter.py
--rw-r--r--   0        0        0     9251 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/plan.py
--rw-r--r--   0        0        0     3667 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/models/project.py
--rw-r--r--   0        0        0     2543 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/api/util.py
--rw-r--r--   0        0        0     9608 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/__init__.py
--rw-r--r--   0        0        0      946 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/__main__.py
--rw-r--r--   0        0        0     2618 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/clone.py
--rw-r--r--   0        0        0     7637 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/config.py
--rw-r--r--   0        0        0    43546 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/dataset.py
--rw-r--r--   0        0        0     2241 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/doctor.py
--rw-r--r--   0        0        0     1624 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/env.py
--rw-r--r--   0        0        0     7964 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/exception_handler.py
--rw-r--r--   0        0        0     1163 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/gc.py
--rw-r--r--   0        0        0     2562 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/githooks.py
--rw-r--r--   0        0        0     4938 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/graph.py
--rw-r--r--   0        0        0    11132 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/init.py
--rw-r--r--   0        0        0     8605 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/log.py
--rw-r--r--   0        0        0     4869 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/login.py
--rw-r--r--   0        0        0     2523 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/mergetool.py
--rw-r--r--   0        0        0     5713 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/migrate.py
--rw-r--r--   0        0        0     2905 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/move.py
--rw-r--r--   0        0        0     5785 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/project.py
--rw-r--r--   0        0        0     1778 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/remove.py
--rw-r--r--   0        0        0     4251 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/rerun.py
--rw-r--r--   0        0        0     3273 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/rollback.py
--rw-r--r--   0        0        0    26440 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/run.py
--rw-r--r--   0        0        0     3534 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/save.py
--rw-r--r--   0        0        0    11854 2023-03-13 14:44:59.487470 renku-2.3.2/renku/ui/cli/service.py
--rw-r--r--   0        0        0    13686 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/session.py
--rw-r--r--   0        0        0     5513 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/status.py
--rw-r--r--   0        0        0     5628 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/storage.py
--rw-r--r--   0        0        0    13314 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/template.py
--rw-r--r--   0        0        0     6467 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/update.py
--rw-r--r--   0        0        0      792 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/__init__.py
--rw-r--r--   0        0        0     5454 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/callback.py
--rw-r--r--   0        0        0     4092 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/click.py
--rw-r--r--   0        0        0      879 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/color.py
--rw-r--r--   0        0        0    14558 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/curses.py
--rw-r--r--   0        0        0     1411 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/plugins.py
--rw-r--r--   0        0        0     9953 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/utils/terminal.py
--rw-r--r--   0        0        0    47375 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/cli/workflow.py
--rw-r--r--   0        0        0      843 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/.env-example
--rw-r--r--   0        0        0      780 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/__init__.py
--rw-r--r--   0        0        0     1559 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/__init__.py
--rw-r--r--   0        0        0     2941 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/base.py
--rw-r--r--   0        0        0     1192 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/config.py
--rw-r--r--   0        0        0     3339 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/files.py
--rw-r--r--   0        0        0     2359 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/jobs.py
--rw-r--r--   0        0        0      793 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/models/__init__.py
--rw-r--r--   0        0        0     4380 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/models/file.py
--rw-r--r--   0        0        0     2297 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/models/job.py
--rw-r--r--   0        0        0     4067 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/models/project.py
--rw-r--r--   0        0        0     1151 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/models/user.py
--rw-r--r--   0        0        0     2582 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/projects.py
--rw-r--r--   0        0        0      798 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/serializers/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/serializers/file.py
--rw-r--r--   0        0        0     1735 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/serializers/job.py
--rw-r--r--   0        0        0     1836 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/serializers/project.py
--rw-r--r--   0        0        0     1251 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/serializers/user.py
--rw-r--r--   0        0        0     1681 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/cache/users.py
--rw-r--r--   0        0        0     2955 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/config.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/__init__.py
--rw-r--r--   0        0        0      801 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/api/__init__.py
--rw-r--r--   0        0        0     1109 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/api/abstract.py
--rw-r--r--   0        0        0    15661 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/api/mixins.py
--rw-r--r--   0        0        0     2697 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_files_delete_chunks.py
--rw-r--r--   0        0        0     7539 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_files_upload.py
--rw-r--r--   0        0        0     2285 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_list_projects.py
--rw-r--r--   0        0        0     1978 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_list_uploaded.py
--rw-r--r--   0        0        0     4871 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_migrate_project.py
--rw-r--r--   0        0        0     5159 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_migrations_check.py
--rw-r--r--   0        0        0     2396 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/cache_project_clone.py
--rw-r--r--   0        0        0     2692 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/config_set.py
--rw-r--r--   0        0        0     2377 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/config_show.py
--rw-r--r--   0        0        0     5731 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_add_file.py
--rw-r--r--   0        0        0     3964 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_create.py
--rw-r--r--   0        0        0     5398 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_edit.py
--rw-r--r--   0        0        0     2183 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_files_list.py
--rw-r--r--   0        0        0     3381 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_import.py
--rw-r--r--   0        0        0     2111 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_list.py
--rw-r--r--   0        0        0     2685 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_remove.py
--rw-r--r--   0        0        0     3338 2023-03-13 14:44:59.491470 renku-2.3.2/renku/ui/service/controllers/datasets_unlink.py
--rw-r--r--   0        0        0     5418 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/graph_export.py
--rw-r--r--   0        0        0     3953 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/project_edit.py
--rw-r--r--   0        0        0     3204 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/project_lock_status.py
--rw-r--r--   0        0        0     2120 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/project_show.py
--rw-r--r--   0        0        0     7840 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/templates_create_project.py
--rw-r--r--   0        0        0     3155 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/templates_read_manifest.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/utils/__init__.py
--rw-r--r--   0        0        0     1107 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/utils/datasets.py
--rw-r--r--   0        0        0     3254 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/utils/project_clone.py
--rw-r--r--   0        0        0     2685 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/utils/remote_project.py
--rw-r--r--   0        0        0     1665 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/version.py
--rw-r--r--   0        0        0     2494 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/workflow_plans_export.py
--rw-r--r--   0        0        0     2308 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/workflow_plans_list.py
--rw-r--r--   0        0        0     2197 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/controllers/workflow_plans_show.py
--rw-r--r--   0        0        0     6239 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/entrypoint.py
--rw-r--r--   0        0        0    31158 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/errors.py
--rw-r--r--   0        0        0      798 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/gateways/__init__.py
--rw-r--r--   0        0        0     3363 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/gateways/gitlab_api_provider.py
--rw-r--r--   0        0        0      817 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/interfaces/__init__.py
--rw-r--r--   0        0        0     1252 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/interfaces/git_api_provider.py
--rw-r--r--   0        0        0      790 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/__init__.py
--rw-r--r--   0        0        0     3059 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/cleanup.py
--rw-r--r--   0        0        0      780 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/constants.py
--rw-r--r--   0        0        0     1219 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/contexts.py
--rw-r--r--   0        0        0     5268 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/datasets.py
--rw-r--r--   0        0        0     1853 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/delayed_ctrl.py
--rw-r--r--   0        0        0     2689 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/jobs/queues.py
--rw-r--r--   0        0        0     1293 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/logger.py
--rw-r--r--   0        0        0      644 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/logging.yaml
--rw-r--r--   0        0        0     2766 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/scheduler.py
--rw-r--r--   0        0        0      792 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/__init__.py
--rw-r--r--   0        0        0    13215 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/cache.py
--rw-r--r--   0        0        0     4069 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/common.py
--rw-r--r--   0        0        0     2252 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/config.py
--rw-r--r--   0        0        0     8782 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/datasets.py
--rw-r--r--   0        0        0     2219 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/graph.py
--rw-r--r--   0        0        0     5386 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/headers.py
--rw-r--r--   0        0        0     1985 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/jobs.py
--rw-r--r--   0        0        0     4534 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/project.py
--rw-r--r--   0        0        0      935 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/rpc.py
--rw-r--r--   0        0        0     5884 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/templates.py
--rw-r--r--   0        0        0      797 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/v1/__init__.py
--rw-r--r--   0        0        0     4236 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/v1/cache.py
--rw-r--r--   0        0        0     1904 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/v1/templates.py
--rw-r--r--   0        0        0     1170 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/version.py
--rw-r--r--   0        0        0     6931 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/serializers/workflows.py
--rw-r--r--   0        0        0     2210 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/utils/__init__.py
--rw-r--r--   0        0        0     2244 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/utils/callback.py
--rw-r--r--   0        0        0     1347 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/utils/json_encoder.py
--rw-r--r--   0        0        0     1284 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/utils/squash.py
--rw-r--r--   0        0        0     1451 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/utils/timeout.py
--rw-r--r--   0        0        0     1785 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/__init__.py
--rw-r--r--   0        0        0     2462 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/api_versions.py
--rw-r--r--   0        0        0     4795 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/apispec.py
--rw-r--r--   0        0        0     7451 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/cache.py
--rw-r--r--   0        0        0     2981 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/config.py
--rw-r--r--   0        0        0     8211 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/datasets.py
--rw-r--r--   0        0        0     3015 2023-03-13 14:44:59.495471 renku-2.3.2/renku/ui/service/views/decorators.py
--rw-r--r--   0        0        0    14872 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/error_handlers.py
--rw-r--r--   0        0        0     2108 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/graph.py
--rw-r--r--   0        0        0     3291 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/jobs.py
--rw-r--r--   0        0        0     3829 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/project.py
--rw-r--r--   0        0        0     3616 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/templates.py
--rw-r--r--   0        0        0      791 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/v1/__init__.py
--rw-r--r--   0        0        0     3598 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/v1/cache.py
--rw-r--r--   0        0        0     2658 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/v1/templates.py
--rw-r--r--   0        0        0     1702 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/version.py
--rw-r--r--   0        0        0     3897 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/views/workflow_plans.py
--rw-r--r--   0        0        0     2919 2023-03-13 14:44:59.499471 renku-2.3.2/renku/ui/service/worker.py
--rw-r--r--   0        0        0     1522 2023-03-13 14:44:59.499471 renku-2.3.2/renku/version.py
--rw-r--r--   0        0        0    17284 1970-01-01 00:00:00.000000 renku-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-04-11 08:06:10.246300 renku-2.4.0rc1/AUTHORS.rst
+-rw-r--r--   0        0        0   177104 2023-04-11 09:58:52.265747 renku-2.4.0rc1/CHANGES.rst
+-rw-r--r--   0        0        0    11358 2023-03-02 15:15:40.036598 renku-2.4.0rc1/LICENSE
+-rw-r--r--   0        0        0    12889 2023-04-11 08:06:10.249633 renku-2.4.0rc1/README.rst
+-rw-r--r--   0        0        0    10259 2023-04-11 11:09:17.359348 renku-2.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4391 2023-04-11 08:06:19.139735 renku-2.4.0rc1/renku/__init__.py
+-rw-r--r--   0        0        0      784 2023-04-11 08:06:10.259633 renku-2.4.0rc1/renku/command/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-06 07:28:50.614572 renku-2.4.0rc1/renku/command/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      194 2023-02-27 08:58:17.925306 renku-2.4.0rc1/renku/command/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      198 2023-04-11 08:06:12.409658 renku-2.4.0rc1/renku/command/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4070 2023-04-06 07:29:04.865758 renku-2.4.0rc1/renku/command/__pycache__/clone.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2991 2023-02-27 09:00:39.260448 renku-2.4.0rc1/renku/command/__pycache__/clone.cpython-37.pyc
+-rw-r--r--   0        0        0     3028 2023-04-11 08:06:16.539705 renku-2.4.0rc1/renku/command/__pycache__/clone.cpython-38.pyc
+-rw-r--r--   0        0        0     5986 2023-04-06 07:29:17.153455 renku-2.4.0rc1/renku/command/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4007 2023-02-27 09:00:55.083983 renku-2.4.0rc1/renku/command/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     4009 2023-04-11 08:06:23.903122 renku-2.4.0rc1/renku/command/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0    10051 2023-04-06 07:29:09.996187 renku-2.4.0rc1/renku/command/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5283 2023-02-27 09:00:47.173882 renku-2.4.0rc1/renku/command/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0     5240 2023-04-11 08:06:19.746408 renku-2.4.0rc1/renku/command/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     3175 2023-04-06 07:29:17.163456 renku-2.4.0rc1/renku/command/__pycache__/doctor.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2040 2023-02-27 09:00:55.097316 renku-2.4.0rc1/renku/command/__pycache__/doctor.cpython-37.pyc
+-rw-r--r--   0        0        0     2047 2023-04-11 08:43:02.075847 renku-2.4.0rc1/renku/command/__pycache__/doctor.cpython-38.pyc
+-rw-r--r--   0        0        0      694 2023-04-06 07:29:17.166790 renku-2.4.0rc1/renku/command/__pycache__/gc.cpython-311.pyc
+-rwxr-xr-x   0        0        0      498 2023-02-27 09:00:55.103983 renku-2.4.0rc1/renku/command/__pycache__/gc.cpython-37.pyc
+-rw-r--r--   0        0        0      504 2023-04-11 08:06:23.929789 renku-2.4.0rc1/renku/command/__pycache__/gc.cpython-38.pyc
+-rw-r--r--   0        0        0      962 2023-04-06 07:29:17.166790 renku-2.4.0rc1/renku/command/__pycache__/githooks.cpython-311.pyc
+-rwxr-xr-x   0        0        0      690 2023-02-27 09:00:55.103983 renku-2.4.0rc1/renku/command/__pycache__/githooks.cpython-37.pyc
+-rw-r--r--   0        0        0      702 2023-04-11 08:06:23.929789 renku-2.4.0rc1/renku/command/__pycache__/githooks.cpython-38.pyc
+-rw-r--r--   0        0        0    13445 2023-04-06 12:11:00.183341 renku-2.4.0rc1/renku/command/__pycache__/graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8100 2023-02-27 09:00:35.393732 renku-2.4.0rc1/renku/command/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0        0        0     8158 2023-04-11 08:06:14.966354 renku-2.4.0rc1/renku/command/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0     1063 2023-04-06 07:29:17.170123 renku-2.4.0rc1/renku/command/__pycache__/group.cpython-311.pyc
+-rwxr-xr-x   0        0        0      721 2023-02-27 09:00:55.110650 renku-2.4.0rc1/renku/command/__pycache__/group.cpython-37.pyc
+-rw-r--r--   0        0        0      722 2023-04-11 08:06:23.936456 renku-2.4.0rc1/renku/command/__pycache__/group.cpython-38.pyc
+-rw-r--r--   0        0        0     1095 2023-04-06 07:29:17.173457 renku-2.4.0rc1/renku/command/__pycache__/init.cpython-311.pyc
+-rwxr-xr-x   0        0        0      731 2023-02-27 09:00:55.110650 renku-2.4.0rc1/renku/command/__pycache__/init.cpython-37.pyc
+-rw-r--r--   0        0        0      743 2023-04-11 08:06:23.939789 renku-2.4.0rc1/renku/command/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0     4028 2023-04-06 07:29:10.712914 renku-2.4.0rc1/renku/command/__pycache__/log.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2696 2023-02-27 09:00:47.980559 renku-2.4.0rc1/renku/command/__pycache__/log.cpython-37.pyc
+-rw-r--r--   0        0        0     2744 2023-04-11 08:06:20.413082 renku-2.4.0rc1/renku/command/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0        0        0     1231 2023-04-06 07:29:17.176790 renku-2.4.0rc1/renku/command/__pycache__/login.cpython-311.pyc
+-rwxr-xr-x   0        0        0      854 2023-02-27 09:00:55.113983 renku-2.4.0rc1/renku/command/__pycache__/login.cpython-37.pyc
+-rw-r--r--   0        0        0      870 2023-04-11 08:06:23.956456 renku-2.4.0rc1/renku/command/__pycache__/login.cpython-38.pyc
+-rw-r--r--   0        0        0     3994 2023-04-06 07:29:11.743000 renku-2.4.0rc1/renku/command/__pycache__/mergetool.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2183 2023-02-27 09:00:49.003905 renku-2.4.0rc1/renku/command/__pycache__/mergetool.cpython-37.pyc
+-rw-r--r--   0        0        0     2208 2023-04-11 08:06:23.943123 renku-2.4.0rc1/renku/command/__pycache__/mergetool.cpython-38.pyc
+-rw-r--r--   0        0        0     9238 2023-04-06 07:29:14.396556 renku-2.4.0rc1/renku/command/__pycache__/migrate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6122 2023-02-27 09:00:51.497270 renku-2.4.0rc1/renku/command/__pycache__/migrate.cpython-37.pyc
+-rw-r--r--   0        0        0     6214 2023-04-11 08:43:01.189162 renku-2.4.0rc1/renku/command/__pycache__/migrate.cpython-38.pyc
+-rw-r--r--   0        0        0    14316 2023-04-06 07:29:17.183458 renku-2.4.0rc1/renku/command/__pycache__/move.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7697 2023-02-27 09:00:55.123983 renku-2.4.0rc1/renku/command/__pycache__/move.cpython-37.pyc
+-rw-r--r--   0        0        0     7748 2023-04-11 08:06:23.963123 renku-2.4.0rc1/renku/command/__pycache__/move.cpython-38.pyc
+-rw-r--r--   0        0        0      504 2023-04-06 07:28:50.634574 renku-2.4.0rc1/renku/command/__pycache__/options.cpython-311.pyc
+-rwxr-xr-x   0        0        0      420 2023-02-27 08:58:18.021974 renku-2.4.0rc1/renku/command/__pycache__/options.cpython-37.pyc
+-rw-r--r--   0        0        0      426 2023-04-11 08:06:12.422991 renku-2.4.0rc1/renku/command/__pycache__/options.cpython-38.pyc
+-rw-r--r--   0        0        0     1513 2023-04-06 07:29:17.186791 renku-2.4.0rc1/renku/command/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0      885 2023-02-27 09:00:55.137317 renku-2.4.0rc1/renku/command/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0      897 2023-04-11 08:06:23.966457 renku-2.4.0rc1/renku/command/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     7239 2023-04-06 07:29:17.196792 renku-2.4.0rc1/renku/command/__pycache__/remove.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4308 2023-02-27 09:00:55.150650 renku-2.4.0rc1/renku/command/__pycache__/remove.cpython-37.pyc
+-rw-r--r--   0        0        0     4279 2023-04-11 08:06:23.976456 renku-2.4.0rc1/renku/command/__pycache__/remove.cpython-38.pyc
+-rw-r--r--   0        0        0     3914 2023-04-06 07:29:17.203459 renku-2.4.0rc1/renku/command/__pycache__/rerun.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2559 2023-02-27 09:00:55.160650 renku-2.4.0rc1/renku/command/__pycache__/rerun.cpython-37.pyc
+-rw-r--r--   0        0        0     2579 2023-04-11 08:06:23.979790 renku-2.4.0rc1/renku/command/__pycache__/rerun.cpython-38.pyc
+-rw-r--r--   0        0        0    12057 2023-04-06 07:29:17.210126 renku-2.4.0rc1/renku/command/__pycache__/rollback.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6732 2023-02-27 09:00:55.170650 renku-2.4.0rc1/renku/command/__pycache__/rollback.cpython-37.pyc
+-rw-r--r--   0        0        0     6761 2023-04-11 08:06:23.989790 renku-2.4.0rc1/renku/command/__pycache__/rollback.cpython-38.pyc
+-rw-r--r--   0        0        0     1785 2023-04-06 07:28:59.308627 renku-2.4.0rc1/renku/command/__pycache__/run.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1030 2023-02-27 09:00:23.903586 renku-2.4.0rc1/renku/command/__pycache__/run.cpython-37.pyc
+-rw-r--r--   0        0        0     1050 2023-04-11 08:06:13.653005 renku-2.4.0rc1/renku/command/__pycache__/run.cpython-38.pyc
+-rw-r--r--   0        0        0     4038 2023-04-06 07:29:17.213460 renku-2.4.0rc1/renku/command/__pycache__/save.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2576 2023-02-27 09:00:55.177317 renku-2.4.0rc1/renku/command/__pycache__/save.cpython-37.pyc
+-rw-r--r--   0        0        0     2618 2023-04-11 08:06:23.993123 renku-2.4.0rc1/renku/command/__pycache__/save.cpython-38.pyc
+-rw-r--r--   0        0        0     1933 2023-04-06 07:29:17.216794 renku-2.4.0rc1/renku/command/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1278 2023-02-27 09:00:55.187317 renku-2.4.0rc1/renku/command/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0     1325 2023-04-11 08:06:23.996457 renku-2.4.0rc1/renku/command/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0      796 2023-04-06 07:29:02.298876 renku-2.4.0rc1/renku/command/__pycache__/status.cpython-311.pyc
+-rwxr-xr-x   0        0        0      534 2023-02-27 09:00:35.533734 renku-2.4.0rc1/renku/command/__pycache__/status.cpython-37.pyc
+-rw-r--r--   0        0        0      542 2023-04-11 08:06:15.026354 renku-2.4.0rc1/renku/command/__pycache__/status.cpython-38.pyc
+-rw-r--r--   0        0        0     5530 2023-04-06 07:29:17.220127 renku-2.4.0rc1/renku/command/__pycache__/storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3510 2023-02-27 09:00:55.190651 renku-2.4.0rc1/renku/command/__pycache__/storage.cpython-37.pyc
+-rw-r--r--   0        0        0     3508 2023-04-11 08:06:23.999790 renku-2.4.0rc1/renku/command/__pycache__/storage.cpython-38.pyc
+-rw-r--r--   0        0        0     2534 2023-04-06 07:29:17.230128 renku-2.4.0rc1/renku/command/__pycache__/template.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1474 2023-02-27 09:00:55.210651 renku-2.4.0rc1/renku/command/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0        0        0     1508 2023-04-11 08:06:24.009790 renku-2.4.0rc1/renku/command/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0        0        0     1088 2023-04-06 07:29:17.233462 renku-2.4.0rc1/renku/command/__pycache__/update.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2829 2023-02-27 09:00:55.213984 renku-2.4.0rc1/renku/command/__pycache__/update.cpython-37.pyc
+-rw-r--r--   0        0        0      683 2023-04-11 08:06:24.013124 renku-2.4.0rc1/renku/command/__pycache__/update.cpython-38.pyc
+-rw-r--r--   0        0        0     2143 2023-04-06 07:28:50.637908 renku-2.4.0rc1/renku/command/__pycache__/util.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1295 2023-02-27 08:58:18.021974 renku-2.4.0rc1/renku/command/__pycache__/util.cpython-37.pyc
+-rw-r--r--   0        0        0     1312 2023-04-11 08:06:12.426324 renku-2.4.0rc1/renku/command/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0        0        0      766 2023-04-06 07:28:50.637908 renku-2.4.0rc1/renku/command/__pycache__/version.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4782 2023-02-27 08:58:18.021974 renku-2.4.0rc1/renku/command/__pycache__/version.cpython-37.pyc
+-rw-r--r--   0        0        0      582 2023-04-11 08:06:12.426324 renku-2.4.0rc1/renku/command/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0     6838 2023-04-06 07:29:17.236796 renku-2.4.0rc1/renku/command/__pycache__/workflow.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3757 2023-02-27 09:00:55.227318 renku-2.4.0rc1/renku/command/__pycache__/workflow.cpython-37.pyc
+-rw-r--r--   0        0        0     3737 2023-04-11 08:06:24.016457 renku-2.4.0rc1/renku/command/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0        0        0     2096 2023-04-11 08:06:19.139735 renku-2.4.0rc1/renku/command/checks/__init__.py
+-rw-r--r--   0        0        0     1253 2023-04-06 07:29:09.209454 renku-2.4.0rc1/renku/command/checks/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1054 2023-02-27 09:00:45.880532 renku-2.4.0rc1/renku/command/checks/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1028 2023-04-11 08:06:19.439738 renku-2.4.0rc1/renku/command/checks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5778 2023-04-06 07:29:09.209454 renku-2.4.0rc1/renku/command/checks/__pycache__/activities.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3444 2023-02-27 09:00:45.883866 renku-2.4.0rc1/renku/command/checks/__pycache__/activities.cpython-37.pyc
+-rw-r--r--   0        0        0     3491 2023-04-11 08:43:00.379146 renku-2.4.0rc1/renku/command/checks/__pycache__/activities.cpython-38.pyc
+-rw-r--r--   0        0        0    11241 2023-04-06 07:29:09.212788 renku-2.4.0rc1/renku/command/checks/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5631 2023-02-27 09:00:45.887199 renku-2.4.0rc1/renku/command/checks/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0     6897 2023-04-11 08:43:00.379146 renku-2.4.0rc1/renku/command/checks/__pycache__/datasets.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1539 2023-02-27 09:00:45.890532 renku-2.4.0rc1/renku/command/checks/__pycache__/external.cpython-37.pyc
+-rw-r--r--   0        0        0     1547 2023-03-13 14:36:06.943014 renku-2.4.0rc1/renku/command/checks/__pycache__/external.cpython-38.pyc
+-rw-r--r--   0        0        0     3675 2023-04-06 07:29:09.212788 renku-2.4.0rc1/renku/command/checks/__pycache__/githooks.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2121 2023-02-27 09:00:45.893866 renku-2.4.0rc1/renku/command/checks/__pycache__/githooks.cpython-37.pyc
+-rw-r--r--   0        0        0     2152 2023-04-11 08:43:00.382479 renku-2.4.0rc1/renku/command/checks/__pycache__/githooks.cpython-38.pyc
+-rw-r--r--   0        0        0     1149 2023-04-06 07:29:09.219455 renku-2.4.0rc1/renku/command/checks/__pycache__/migration.cpython-311.pyc
+-rwxr-xr-x   0        0        0      910 2023-02-27 09:00:45.900533 renku-2.4.0rc1/renku/command/checks/__pycache__/migration.cpython-37.pyc
+-rw-r--r--   0        0        0      920 2023-04-11 08:43:00.382479 renku-2.4.0rc1/renku/command/checks/__pycache__/migration.cpython-38.pyc
+-rw-r--r--   0        0        0     2204 2023-04-06 07:29:09.219455 renku-2.4.0rc1/renku/command/checks/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1537 2023-02-27 09:00:45.903866 renku-2.4.0rc1/renku/command/checks/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     1553 2023-04-11 08:43:00.385812 renku-2.4.0rc1/renku/command/checks/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     1133 2023-04-06 07:29:09.219455 renku-2.4.0rc1/renku/command/checks/__pycache__/storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0      851 2023-02-27 09:00:45.903866 renku-2.4.0rc1/renku/command/checks/__pycache__/storage.cpython-37.pyc
+-rw-r--r--   0        0        0      877 2023-04-11 08:43:00.385812 renku-2.4.0rc1/renku/command/checks/__pycache__/storage.cpython-38.pyc
+-rw-r--r--   0        0        0     5641 2023-04-06 07:29:09.222789 renku-2.4.0rc1/renku/command/checks/__pycache__/validate_shacl.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3616 2023-02-27 09:00:45.907199 renku-2.4.0rc1/renku/command/checks/__pycache__/validate_shacl.cpython-37.pyc
+-rw-r--r--   0        0        0     3621 2023-04-11 08:43:00.385812 renku-2.4.0rc1/renku/command/checks/__pycache__/validate_shacl.cpython-38.pyc
+-rw-r--r--   0        0        0     5745 2023-04-06 07:29:09.222789 renku-2.4.0rc1/renku/command/checks/__pycache__/workflow.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3540 2023-02-27 09:00:45.907199 renku-2.4.0rc1/renku/command/checks/__pycache__/workflow.cpython-37.pyc
+-rw-r--r--   0        0        0     3558 2023-04-11 08:43:00.389146 renku-2.4.0rc1/renku/command/checks/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0        0        0     4723 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/activities.py
+-rw-r--r--   0        0        0     8186 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/datasets.py
+-rw-r--r--   0        0        0     2769 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/githooks.py
+-rw-r--r--   0        0        0     1500 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/migration.py
+-rw-r--r--   0        0        0     2316 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/project.py
+-rw-r--r--   0        0        0     1487 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/storage.py
+-rw-r--r--   0        0        0     4262 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/validate_shacl.py
+-rw-r--r--   0        0        0     4881 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/checks/workflow.py
+-rw-r--r--   0        0        0     3872 2023-04-11 08:06:10.259633 renku-2.4.0rc1/renku/command/clone.py
+-rw-r--r--   0        0        0      828 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-06 07:28:50.614572 renku-2.4.0rc1/renku/command/command_builder/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      286 2023-02-27 08:58:17.928639 renku-2.4.0rc1/renku/command/command_builder/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      290 2023-04-11 08:09:11.265079 renku-2.4.0rc1/renku/command/command_builder/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22830 2023-04-06 07:28:50.617906 renku-2.4.0rc1/renku/command/command_builder/__pycache__/command.cpython-311.pyc
+-rwxr-xr-x   0        0        0    15297 2023-02-27 08:58:17.931973 renku-2.4.0rc1/renku/command/command_builder/__pycache__/command.cpython-37.pyc
+-rw-r--r--   0        0        0    15354 2023-04-11 08:09:11.268412 renku-2.4.0rc1/renku/command/command_builder/__pycache__/command.cpython-38.pyc
+-rw-r--r--   0        0        0     2477 2023-04-06 07:29:17.466815 renku-2.4.0rc1/renku/command/command_builder/__pycache__/communication.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1749 2023-02-27 09:00:55.817325 renku-2.4.0rc1/renku/command/command_builder/__pycache__/communication.cpython-37.pyc
+-rw-r--r--   0        0        0     1775 2023-04-11 08:06:24.206459 renku-2.4.0rc1/renku/command/command_builder/__pycache__/communication.cpython-38.pyc
+-rw-r--r--   0        0        0     7548 2023-04-06 07:29:09.009438 renku-2.4.0rc1/renku/command/command_builder/__pycache__/database.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4434 2023-02-27 09:00:45.307192 renku-2.4.0rc1/renku/command/command_builder/__pycache__/database.cpython-37.pyc
+-rw-r--r--   0        0        0     4493 2023-04-11 08:06:19.296403 renku-2.4.0rc1/renku/command/command_builder/__pycache__/database.cpython-38.pyc
+-rw-r--r--   0        0        0     2188 2023-04-06 07:29:17.470148 renku-2.4.0rc1/renku/command/command_builder/__pycache__/lock.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1519 2023-02-27 09:00:55.820659 renku-2.4.0rc1/renku/command/command_builder/__pycache__/lock.cpython-37.pyc
+-rw-r--r--   0        0        0     1543 2023-04-11 08:06:24.209792 renku-2.4.0rc1/renku/command/command_builder/__pycache__/lock.cpython-38.pyc
+-rw-r--r--   0        0        0     1720 2023-04-06 07:29:17.473482 renku-2.4.0rc1/renku/command/command_builder/__pycache__/migration.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1254 2023-02-27 09:00:55.823992 renku-2.4.0rc1/renku/command/command_builder/__pycache__/migration.cpython-37.pyc
+-rw-r--r--   0        0        0     1272 2023-04-11 08:06:24.213126 renku-2.4.0rc1/renku/command/command_builder/__pycache__/migration.cpython-38.pyc
+-rw-r--r--   0        0        0     9659 2023-04-06 07:29:09.009438 renku-2.4.0rc1/renku/command/command_builder/__pycache__/repo.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6976 2023-02-27 09:00:45.317192 renku-2.4.0rc1/renku/command/command_builder/__pycache__/repo.cpython-37.pyc
+-rw-r--r--   0        0        0     6761 2023-04-11 08:06:19.299736 renku-2.4.0rc1/renku/command/command_builder/__pycache__/repo.cpython-38.pyc
+-rw-r--r--   0        0        0    16678 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/command.py
+-rw-r--r--   0        0        0     1951 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/communication.py
+-rw-r--r--   0        0        0     5303 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/database.py
+-rw-r--r--   0        0        0     1701 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/lock.py
+-rw-r--r--   0        0        0     1481 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/migration.py
+-rw-r--r--   0        0        0     7694 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/command_builder/repo.py
+-rw-r--r--   0        0        0     4803 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/config.py
+-rw-r--r--   0        0        0     5640 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/dataset.py
+-rw-r--r--   0        0        0     2718 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/doctor.py
+-rw-r--r--   0        0        0      775 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-06 07:28:50.657909 renku-2.4.0rc1/renku/command/format/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      205 2023-02-27 08:58:18.035307 renku-2.4.0rc1/renku/command/format/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      209 2023-04-11 08:09:11.281746 renku-2.4.0rc1/renku/command/format/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3592 2023-04-06 07:29:17.596826 renku-2.4.0rc1/renku/command/format/__pycache__/activity.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2138 2023-02-27 09:00:56.143996 renku-2.4.0rc1/renku/command/format/__pycache__/activity.cpython-37.pyc
+-rw-r--r--   0        0        0     2370 2023-04-11 08:06:24.316460 renku-2.4.0rc1/renku/command/format/__pycache__/activity.cpython-38.pyc
+-rw-r--r--   0        0        0     9055 2023-04-06 07:28:50.661243 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_files.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5045 2023-02-27 08:58:18.038641 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_files.cpython-37.pyc
+-rw-r--r--   0        0        0     5796 2023-04-11 08:09:11.281746 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_files.cpython-38.pyc
+-rw-r--r--   0        0        0     1989 2023-04-06 07:28:50.664577 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1481 2023-02-27 08:58:18.038641 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-37.pyc
+-rw-r--r--   0        0        0     1501 2023-04-11 08:09:11.281746 renku-2.4.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-38.pyc
+-rw-r--r--   0        0        0     3864 2023-04-06 07:28:50.667910 renku-2.4.0rc1/renku/command/format/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2885 2023-02-27 08:58:18.038641 renku-2.4.0rc1/renku/command/format/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0     2885 2023-04-11 08:09:11.281746 renku-2.4.0rc1/renku/command/format/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     1295 2023-04-06 07:28:57.105111 renku-2.4.0rc1/renku/command/format/__pycache__/json.cpython-311.pyc
+-rwxr-xr-x   0        0        0      796 2023-02-27 09:00:23.143576 renku-2.4.0rc1/renku/command/format/__pycache__/json.cpython-37.pyc
+-rw-r--r--   0        0        0      806 2023-04-11 08:09:11.978421 renku-2.4.0rc1/renku/command/format/__pycache__/json.cpython-38.pyc
+-rw-r--r--   0        0        0     1125 2023-04-06 07:28:59.338630 renku-2.4.0rc1/renku/command/format/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0      827 2023-02-27 09:00:23.933586 renku-2.4.0rc1/renku/command/format/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0      843 2023-04-11 08:09:12.271758 renku-2.4.0rc1/renku/command/format/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     3025 2023-04-06 07:28:57.105111 renku-2.4.0rc1/renku/command/format/__pycache__/tabulate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1908 2023-02-27 09:00:23.143576 renku-2.4.0rc1/renku/command/format/__pycache__/tabulate.cpython-37.pyc
+-rw-r--r--   0        0        0     1926 2023-04-11 08:09:11.978421 renku-2.4.0rc1/renku/command/format/__pycache__/tabulate.cpython-38.pyc
+-rw-r--r--   0        0        0     3340 2023-04-06 07:28:57.101777 renku-2.4.0rc1/renku/command/format/__pycache__/workflow.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2410 2023-02-27 09:00:23.140243 renku-2.4.0rc1/renku/command/format/__pycache__/workflow.cpython-37.pyc
+-rw-r--r--   0        0        0     2413 2023-04-11 08:09:11.975088 renku-2.4.0rc1/renku/command/format/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0        0        0     2643 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/activity.py
+-rw-r--r--   0        0        0     6230 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/dataset_files.py
+-rw-r--r--   0        0        0     2098 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/dataset_tags.py
+-rw-r--r--   0        0        0     3236 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/datasets.py
+-rw-r--r--   0        0        0     1212 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/json.py
+-rw-r--r--   0        0        0     1355 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/session.py
+-rw-r--r--   0        0        0     2769 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/tabulate.py
+-rw-r--r--   0        0        0     2728 2023-04-11 08:06:19.143068 renku-2.4.0rc1/renku/command/format/workflow.py
+-rw-r--r--   0        0        0     1012 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/gc.py
+-rw-r--r--   0        0        0     1154 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/githooks.py
+-rw-r--r--   0        0        0     9883 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/graph.py
+-rw-r--r--   0        0        0     1081 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/group.py
+-rw-r--r--   0        0        0     1203 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/init.py
+-rw-r--r--   0        0        0     3124 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/log.py
+-rw-r--r--   0        0        0     1241 2023-04-11 08:06:10.262966 renku-2.4.0rc1/renku/command/login.py
+-rw-r--r--   0        0        0     2822 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/mergetool.py
+-rw-r--r--   0        0        0     7629 2023-04-11 08:42:55.929056 renku-2.4.0rc1/renku/command/migrate.py
+-rw-r--r--   0        0        0     9141 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/move.py
+-rw-r--r--   0        0        0     1015 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/options.py
+-rw-r--r--   0        0        0     1362 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/project.py
+-rw-r--r--   0        0        0     4748 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/remove.py
+-rw-r--r--   0        0        0     3146 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/rerun.py
+-rw-r--r--   0        0        0    10987 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/rollback.py
+-rw-r--r--   0        0        0     1600 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/run.py
+-rw-r--r--   0        0        0     3375 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/save.py
+-rw-r--r--   0        0        0      766 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-06 07:28:50.807922 renku-2.4.0rc1/renku/command/schema/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      196 2023-02-27 08:58:18.071974 renku-2.4.0rc1/renku/command/schema/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      200 2023-04-11 08:09:11.308413 renku-2.4.0rc1/renku/command/schema/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8831 2023-04-06 07:29:02.078858 renku-2.4.0rc1/renku/command/schema/__pycache__/activity.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4938 2023-02-27 09:00:35.393732 renku-2.4.0rc1/renku/command/schema/__pycache__/activity.cpython-37.pyc
+-rw-r--r--   0        0        0     5750 2023-04-11 08:09:13.198436 renku-2.4.0rc1/renku/command/schema/__pycache__/activity.cpython-38.pyc
+-rw-r--r--   0        0        0     2300 2023-04-06 07:28:50.811255 renku-2.4.0rc1/renku/command/schema/__pycache__/agent.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1539 2023-02-27 08:58:18.075308 renku-2.4.0rc1/renku/command/schema/__pycache__/agent.cpython-37.pyc
+-rw-r--r--   0        0        0     1549 2023-04-11 08:09:11.311746 renku-2.4.0rc1/renku/command/schema/__pycache__/agent.cpython-38.pyc
+-rw-r--r--   0        0        0     1351 2023-04-06 07:28:51.157951 renku-2.4.0rc1/renku/command/schema/__pycache__/annotation.cpython-311.pyc
+-rwxr-xr-x   0        0        0      954 2023-02-27 08:58:18.141975 renku-2.4.0rc1/renku/command/schema/__pycache__/annotation.cpython-37.pyc
+-rw-r--r--   0        0        0      966 2023-04-11 08:09:11.355080 renku-2.4.0rc1/renku/command/schema/__pycache__/annotation.cpython-38.pyc
+-rw-r--r--   0        0        0    12294 2023-04-06 07:28:51.141283 renku-2.4.0rc1/renku/command/schema/__pycache__/calamus.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6719 2023-02-27 08:58:18.138642 renku-2.4.0rc1/renku/command/schema/__pycache__/calamus.cpython-37.pyc
+-rw-r--r--   0        0        0     6603 2023-04-11 08:09:11.345080 renku-2.4.0rc1/renku/command/schema/__pycache__/calamus.cpython-38.pyc
+-rw-r--r--   0        0        0     4218 2023-04-06 07:29:02.092193 renku-2.4.0rc1/renku/command/schema/__pycache__/composite_plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1823 2023-02-27 09:00:35.413732 renku-2.4.0rc1/renku/command/schema/__pycache__/composite_plan.cpython-37.pyc
+-rw-r--r--   0        0        0     2663 2023-04-11 08:09:13.205103 renku-2.4.0rc1/renku/command/schema/__pycache__/composite_plan.cpython-38.pyc
+-rw-r--r--   0        0        0    12569 2023-04-06 07:28:50.811255 renku-2.4.0rc1/renku/command/schema/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5967 2023-02-27 08:58:18.075308 renku-2.4.0rc1/renku/command/schema/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0     7579 2023-04-11 08:09:11.311746 renku-2.4.0rc1/renku/command/schema/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1940 2023-04-06 07:28:51.157951 renku-2.4.0rc1/renku/command/schema/__pycache__/entity.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1333 2023-02-27 08:58:18.145309 renku-2.4.0rc1/renku/command/schema/__pycache__/entity.cpython-37.pyc
+-rw-r--r--   0        0        0     1334 2023-04-11 08:09:11.355080 renku-2.4.0rc1/renku/command/schema/__pycache__/entity.cpython-38.pyc
+-rw-r--r--   0        0        0     6722 2023-04-06 07:29:02.082192 renku-2.4.0rc1/renku/command/schema/__pycache__/parameter.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4381 2023-02-27 09:00:35.400399 renku-2.4.0rc1/renku/command/schema/__pycache__/parameter.cpython-37.pyc
+-rw-r--r--   0        0        0     4389 2023-04-11 08:09:13.201769 renku-2.4.0rc1/renku/command/schema/__pycache__/parameter.cpython-38.pyc
+-rw-r--r--   0        0        0     4572 2023-04-06 07:29:02.078858 renku-2.4.0rc1/renku/command/schema/__pycache__/plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1997 2023-02-27 09:00:35.397065 renku-2.4.0rc1/renku/command/schema/__pycache__/plan.cpython-37.pyc
+-rw-r--r--   0        0        0     2812 2023-04-11 08:09:13.198436 renku-2.4.0rc1/renku/command/schema/__pycache__/plan.cpython-38.pyc
+-rw-r--r--   0        0        0     4294 2023-04-06 07:29:02.098860 renku-2.4.0rc1/renku/command/schema/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2105 2023-02-27 09:00:35.427066 renku-2.4.0rc1/renku/command/schema/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     2855 2023-04-11 08:09:13.208436 renku-2.4.0rc1/renku/command/schema/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     2407 2023-04-06 07:29:02.088859 renku-2.4.0rc1/renku/command/schema/__pycache__/workflow_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1693 2023-02-27 09:00:35.413732 renku-2.4.0rc1/renku/command/schema/__pycache__/workflow_file.cpython-37.pyc
+-rw-r--r--   0        0        0     1705 2023-04-11 08:09:13.205103 renku-2.4.0rc1/renku/command/schema/__pycache__/workflow_file.cpython-38.pyc
+-rw-r--r--   0        0        0     5615 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/activity.py
+-rw-r--r--   0        0        0     1744 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/agent.py
+-rw-r--r--   0        0        0     1235 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/annotation.py
+-rw-r--r--   0        0        0     8986 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/calamus.py
+-rw-r--r--   0        0        0     3186 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/composite_plan.py
+-rw-r--r--   0        0        0     8210 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/dataset.py
+-rw-r--r--   0        0        0     1445 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/entity.py
+-rw-r--r--   0        0        0     4016 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/parameter.py
+-rw-r--r--   0        0        0     3427 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/plan.py
+-rw-r--r--   0        0        0     3406 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/project.py
+-rw-r--r--   0        0        0     1829 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/schema/workflow_file.py
+-rw-r--r--   0        0        0     1578 2023-04-11 08:06:10.266300 renku-2.4.0rc1/renku/command/session.py
+-rw-r--r--   0        0        0     1036 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/status.py
+-rw-r--r--   0        0        0     3944 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/storage.py
+-rw-r--r--   0        0        0     1919 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/template.py
+-rw-r--r--   0        0        0     1254 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/update.py
+-rw-r--r--   0        0        0     1726 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/util.py
+-rw-r--r--   0        0        0     1088 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/version.py
+-rw-r--r--   0        0        0      768 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-06 07:28:57.108444 renku-2.4.0rc1/renku/command/view_model/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      202 2023-02-27 09:00:23.143576 renku-2.4.0rc1/renku/command/view_model/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      206 2023-04-11 08:09:11.981754 renku-2.4.0rc1/renku/command/view_model/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    21914 2023-04-06 07:28:57.115111 renku-2.4.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0    13099 2023-02-27 09:00:23.146910 renku-2.4.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-37.pyc
+-rw-r--r--   0        0        0    13160 2023-04-11 08:09:11.985088 renku-2.4.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-38.pyc
+-rw-r--r--   0        0        0     1843 2023-04-06 07:28:57.235121 renku-2.4.0rc1/renku/command/view_model/__pycache__/agent.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1343 2023-02-27 09:00:23.216910 renku-2.4.0rc1/renku/command/view_model/__pycache__/agent.cpython-37.pyc
+-rw-r--r--   0        0        0     1339 2023-04-11 08:09:12.018422 renku-2.4.0rc1/renku/command/view_model/__pycache__/agent.cpython-38.pyc
+-rw-r--r--   0        0        0    13356 2023-04-06 07:28:57.241789 renku-2.4.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7934 2023-02-27 09:00:23.220244 renku-2.4.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-37.pyc
+-rw-r--r--   0        0        0     8192 2023-04-11 08:09:12.021755 renku-2.4.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-38.pyc
+-rw-r--r--   0        0        0     2659 2023-04-06 07:28:59.498643 renku-2.4.0rc1/renku/command/view_model/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1841 2023-02-27 09:00:24.323591 renku-2.4.0rc1/renku/command/view_model/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0     1837 2023-04-11 08:09:12.355092 renku-2.4.0rc1/renku/command/view_model/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0    11907 2023-04-06 07:29:02.102193 renku-2.4.0rc1/renku/command/view_model/__pycache__/graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7477 2023-02-27 09:00:35.433733 renku-2.4.0rc1/renku/command/view_model/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0        0        0     7540 2023-04-11 08:09:13.211769 renku-2.4.0rc1/renku/command/view_model/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0    20058 2023-04-06 07:28:59.235288 renku-2.4.0rc1/renku/command/view_model/__pycache__/log.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11328 2023-02-27 09:00:23.860252 renku-2.4.0rc1/renku/command/view_model/__pycache__/log.cpython-37.pyc
+-rw-r--r--   0        0        0    11232 2023-04-11 08:09:12.248424 renku-2.4.0rc1/renku/command/view_model/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0        0        0    12601 2023-04-06 07:28:57.231788 renku-2.4.0rc1/renku/command/view_model/__pycache__/plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7774 2023-02-27 09:00:23.216910 renku-2.4.0rc1/renku/command/view_model/__pycache__/plan.cpython-37.pyc
+-rw-r--r--   0        0        0     7836 2023-04-11 08:09:12.018422 renku-2.4.0rc1/renku/command/view_model/__pycache__/plan.cpython-38.pyc
+-rw-r--r--   0        0        0     3653 2023-04-06 07:29:17.190125 renku-2.4.0rc1/renku/command/view_model/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2268 2023-02-27 09:00:55.140650 renku-2.4.0rc1/renku/command/view_model/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     2263 2023-04-11 08:06:23.969790 renku-2.4.0rc1/renku/command/view_model/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     6986 2023-04-06 07:29:06.392552 renku-2.4.0rc1/renku/command/view_model/__pycache__/template.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4710 2023-02-27 09:00:46.060535 renku-2.4.0rc1/renku/command/view_model/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0        0        0     4798 2023-04-11 09:50:18.596698 renku-2.4.0rc1/renku/command/view_model/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0        0        0    23022 2023-04-06 07:29:17.983525 renku-2.4.0rc1/renku/command/view_model/__pycache__/text_canvas.cpython-311.pyc
+-rwxr-xr-x   0        0        0    13282 2023-02-27 09:00:57.120675 renku-2.4.0rc1/renku/command/view_model/__pycache__/text_canvas.cpython-37.pyc
+-rw-r--r--   0        0        0    12225 2023-04-11 08:06:24.596464 renku-2.4.0rc1/renku/command/view_model/__pycache__/text_canvas.cpython-38.pyc
+-rw-r--r--   0        0        0     7370 2023-04-06 07:29:17.990192 renku-2.4.0rc1/renku/command/view_model/__pycache__/workflow_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4769 2023-02-27 09:00:57.127342 renku-2.4.0rc1/renku/command/view_model/__pycache__/workflow_file.cpython-37.pyc
+-rw-r--r--   0        0        0     4711 2023-04-11 08:06:24.603130 renku-2.4.0rc1/renku/command/view_model/__pycache__/workflow_file.cpython-38.pyc
+-rw-r--r--   0        0        0    13979 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/activity_graph.py
+-rw-r--r--   0        0        0     1657 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/agent.py
+-rw-r--r--   0        0        0     8768 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/composite_plan.py
+-rw-r--r--   0        0        0     2138 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/dataset.py
+-rw-r--r--   0        0        0     7772 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/graph.py
+-rw-r--r--   0        0        0    12497 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/log.py
+-rw-r--r--   0        0        0     9377 2023-04-11 08:06:19.146401 renku-2.4.0rc1/renku/command/view_model/plan.py
+-rw-r--r--   0        0        0     3306 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/command/view_model/project.py
+-rw-r--r--   0        0        0     5895 2023-04-11 08:43:02.645858 renku-2.4.0rc1/renku/command/view_model/template.py
+-rw-r--r--   0        0        0    14502 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/command/view_model/text_canvas.py
+-rw-r--r--   0        0        0     4792 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/command/view_model/workflow_file.py
+-rw-r--r--   0        0        0     4114 2023-04-11 08:06:10.269633 renku-2.4.0rc1/renku/command/workflow.py
+-rw-r--r--   0        0        0      745 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-06 07:28:50.111198 renku-2.4.0rc1/renku/core/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      165 2023-02-27 08:58:17.881972 renku-2.4.0rc1/renku/core/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      169 2023-04-11 08:09:11.165078 renku-2.4.0rc1/renku/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8506 2023-04-06 07:28:50.117865 renku-2.4.0rc1/renku/core/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4383 2023-02-27 08:58:17.885305 renku-2.4.0rc1/renku/core/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     4404 2023-04-11 08:09:11.165078 renku-2.4.0rc1/renku/core/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     2230 2023-04-06 07:28:50.117865 renku-2.4.0rc1/renku/core/__pycache__/constant.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1704 2023-02-27 08:58:17.885305 renku-2.4.0rc1/renku/core/__pycache__/constant.cpython-37.pyc
+-rw-r--r--   0        0        0     1718 2023-04-11 08:09:11.168411 renku-2.4.0rc1/renku/core/__pycache__/constant.cpython-38.pyc
+-rw-r--r--   0        0        0    49858 2023-04-06 07:28:50.137866 renku-2.4.0rc1/renku/core/__pycache__/errors.cpython-311.pyc
+-rwxr-xr-x   0        0        0    36658 2023-02-27 08:58:17.888639 renku-2.4.0rc1/renku/core/__pycache__/errors.cpython-37.pyc
+-rw-r--r--   0        0        0    33726 2023-04-11 08:09:11.171745 renku-2.4.0rc1/renku/core/__pycache__/errors.cpython-38.pyc
+-rw-r--r--   0        0        0     1033 2023-04-06 07:29:18.200210 renku-2.4.0rc1/renku/core/__pycache__/gc.cpython-311.pyc
+-rwxr-xr-x   0        0        0      736 2023-02-27 09:00:57.660682 renku-2.4.0rc1/renku/core/__pycache__/gc.cpython-37.pyc
+-rw-r--r--   0        0        0      750 2023-04-11 08:06:24.789799 renku-2.4.0rc1/renku/core/__pycache__/gc.cpython-38.pyc
+-rw-r--r--   0        0        0     8894 2023-04-06 07:28:57.251789 renku-2.4.0rc1/renku/core/__pycache__/git.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4805 2023-02-27 09:00:23.223577 renku-2.4.0rc1/renku/core/__pycache__/git.cpython-37.pyc
+-rw-r--r--   0        0        0     4845 2023-04-11 08:09:12.021755 renku-2.4.0rc1/renku/core/__pycache__/git.cpython-38.pyc
+-rw-r--r--   0        0        0     2601 2023-04-06 07:29:09.216122 renku-2.4.0rc1/renku/core/__pycache__/githooks.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1453 2023-02-27 09:00:45.893866 renku-2.4.0rc1/renku/core/__pycache__/githooks.cpython-37.pyc
+-rw-r--r--   0        0        0     1450 2023-04-11 08:06:19.443071 renku-2.4.0rc1/renku/core/__pycache__/githooks.cpython-38.pyc
+-rw-r--r--   0        0        0    19823 2023-04-06 07:29:11.743000 renku-2.4.0rc1/renku/core/__pycache__/init.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11943 2023-02-27 09:00:49.003905 renku-2.4.0rc1/renku/core/__pycache__/init.cpython-37.pyc
+-rw-r--r--   0        0        0    12026 2023-04-11 09:50:19.313374 renku-2.4.0rc1/renku/core/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0    13479 2023-04-06 07:28:51.487978 renku-2.4.0rc1/renku/core/__pycache__/login.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7925 2023-02-27 08:58:18.195309 renku-2.4.0rc1/renku/core/__pycache__/login.cpython-37.pyc
+-rw-r--r--   0        0        0     7763 2023-04-11 08:09:11.428414 renku-2.4.0rc1/renku/core/__pycache__/login.cpython-38.pyc
+-rw-r--r--   0        0        0     3713 2023-04-06 07:29:17.190125 renku-2.4.0rc1/renku/core/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2523 2023-02-27 09:00:55.137317 renku-2.4.0rc1/renku/core/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     2558 2023-04-11 08:06:23.969790 renku-2.4.0rc1/renku/core/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0    31311 2023-04-06 07:28:50.264544 renku-2.4.0rc1/renku/core/__pycache__/storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0    16145 2023-02-27 08:58:17.908639 renku-2.4.0rc1/renku/core/__pycache__/storage.cpython-37.pyc
+-rw-r--r--   0        0        0    16076 2023-04-11 08:09:11.188412 renku-2.4.0rc1/renku/core/__pycache__/storage.cpython-38.pyc
+-rw-r--r--   0        0        0     6170 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/config.py
+-rw-r--r--   0        0        0     2717 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/constant.py
+-rw-r--r--   0        0        0      765 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-06 07:28:50.674577 renku-2.4.0rc1/renku/core/dataset/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      193 2023-02-27 08:58:18.041974 renku-2.4.0rc1/renku/core/dataset/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      197 2023-04-11 08:09:11.285079 renku-2.4.0rc1/renku/core/dataset/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3218 2023-04-06 07:28:59.568649 renku-2.4.0rc1/renku/core/dataset/__pycache__/context.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1993 2023-02-27 09:00:24.413592 renku-2.4.0rc1/renku/core/dataset/__pycache__/context.cpython-37.pyc
+-rw-r--r--   0        0        0     2037 2023-04-11 08:09:12.381759 renku-2.4.0rc1/renku/core/dataset/__pycache__/context.cpython-38.pyc
+-rw-r--r--   0        0        0    72239 2023-04-06 07:28:59.498643 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0    38862 2023-02-27 09:00:24.323591 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0    40647 2023-04-11 09:50:16.296670 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0    28110 2023-04-06 07:28:59.565315 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-311.pyc
+-rwxr-xr-x   0        0        0    12918 2023-02-27 09:00:24.413592 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-37.pyc
+-rw-r--r--   0        0        0    15737 2023-04-11 08:09:12.381759 renku-2.4.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-38.pyc
+-rw-r--r--   0        0        0    12293 2023-04-06 07:28:51.481311 renku-2.4.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7571 2023-02-27 08:58:18.191976 renku-2.4.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-37.pyc
+-rw-r--r--   0        0        0     7463 2023-04-11 08:09:11.428414 renku-2.4.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-38.pyc
+-rw-r--r--   0        0        0     6212 2023-04-06 07:28:59.501977 renku-2.4.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2837 2023-02-27 09:00:24.326924 renku-2.4.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-37.pyc
+-rw-r--r--   0        0        0     3360 2023-04-11 08:09:12.355092 renku-2.4.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-38.pyc
+-rw-r--r--   0        0        0     5256 2023-04-06 07:28:59.501977 renku-2.4.0rc1/renku/core/dataset/__pycache__/request_model.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2686 2023-02-27 09:00:24.330258 renku-2.4.0rc1/renku/core/dataset/__pycache__/request_model.cpython-37.pyc
+-rw-r--r--   0        0        0     2726 2023-04-11 08:09:12.355092 renku-2.4.0rc1/renku/core/dataset/__pycache__/request_model.cpython-38.pyc
+-rw-r--r--   0        0        0     8244 2023-04-06 07:28:59.508644 renku-2.4.0rc1/renku/core/dataset/__pycache__/tag.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5298 2023-02-27 09:00:24.333591 renku-2.4.0rc1/renku/core/dataset/__pycache__/tag.cpython-37.pyc
+-rw-r--r--   0        0        0     5319 2023-04-11 08:09:12.358425 renku-2.4.0rc1/renku/core/dataset/__pycache__/tag.cpython-38.pyc
+-rw-r--r--   0        0        0     2954 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/context.py
+-rw-r--r--   0        0        0    54038 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/dataset.py
+-rw-r--r--   0        0        0    21430 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/dataset_add.py
+-rw-r--r--   0        0        0     9747 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/datasets_provenance.py
+-rw-r--r--   0        0        0     4296 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/pointer_file.py
+-rw-r--r--   0        0        0      760 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/providers/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-06 07:28:50.677911 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      198 2023-02-27 08:58:18.041974 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      202 2023-04-11 08:09:11.285079 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    21559 2023-04-06 07:28:50.687912 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-311.pyc
+-rwxr-xr-x   0        0        0    14454 2023-02-27 08:58:18.045307 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-37.pyc
+-rw-r--r--   0        0        0    15682 2023-04-11 09:50:15.493326 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-38.pyc
+-rw-r--r--   0        0        0     9985 2023-04-06 07:28:50.707913 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6396 2023-02-27 08:58:18.051974 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-37.pyc
+-rw-r--r--   0        0        0     6711 2023-04-11 09:50:15.496660 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1833 2023-02-27 08:58:18.051974 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/cloud.cpython-37.pyc
+-rw-r--r--   0        0        0     1862 2023-04-11 08:06:12.472992 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/cloud.cpython-38.pyc
+-rw-r--r--   0        0        0     2585 2023-04-06 07:28:50.707913 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     1641 2023-04-11 08:06:25.099803 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0    31865 2023-04-06 07:28:51.441308 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-311.pyc
+-rwxr-xr-x   0        0        0    18789 2023-02-27 08:58:18.181976 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-37.pyc
+-rw-r--r--   0        0        0    19319 2023-04-11 09:50:15.576661 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-38.pyc
+-rw-r--r--   0        0        0     2827 2023-04-06 07:28:51.441308 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2782 2023-02-27 08:58:18.181976 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-37.pyc
+-rw-r--r--   0        0        0     2786 2023-04-11 08:09:11.415081 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-38.pyc
+-rw-r--r--   0        0        0     7335 2023-04-06 07:28:51.444641 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5073 2023-02-27 08:58:18.185309 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-37.pyc
+-rw-r--r--   0        0        0     5062 2023-04-11 09:50:15.576661 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-38.pyc
+-rw-r--r--   0        0        0     8360 2023-04-06 07:28:51.451308 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-311.pyc
+-rw-r--r--   0        0        0     5936 2023-04-11 09:50:15.579994 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-38.pyc
+-rw-r--r--   0        0        0     9171 2023-04-06 07:28:50.681245 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5498 2023-02-27 08:58:18.041974 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-37.pyc
+-rw-r--r--   0        0        0     5579 2023-04-11 08:09:11.285079 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-38.pyc
+-rw-r--r--   0        0        0     9812 2023-04-06 07:28:51.454642 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5832 2023-02-27 08:58:18.185309 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-37.pyc
+-rw-r--r--   0        0        0     5949 2023-04-11 09:50:15.579994 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-38.pyc
+-rw-r--r--   0        0        0    14788 2023-04-06 07:28:51.461309 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8830 2023-02-27 08:58:18.188643 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-37.pyc
+-rw-r--r--   0        0        0     8708 2023-04-11 09:50:15.579994 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-38.pyc
+-rw-r--r--   0        0        0     9221 2023-04-06 07:28:50.711247 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5914 2023-02-27 08:58:18.051974 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-37.pyc
+-rw-r--r--   0        0        0     6039 2023-04-11 09:50:15.496660 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0    15562 2023-04-06 07:28:51.464643 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9437 2023-02-27 08:58:18.188643 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-37.pyc
+-rw-r--r--   0        0        0     9537 2023-04-11 09:50:15.583327 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-38.pyc
+-rw-r--r--   0        0        0    29626 2023-04-06 07:28:51.474644 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-311.pyc
+-rwxr-xr-x   0        0        0    17189 2023-02-27 08:58:18.191976 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-37.pyc
+-rw-r--r--   0        0        0    17188 2023-04-11 09:50:15.586661 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-38.pyc
+-rw-r--r--   0        0        0     3422 2023-04-06 07:28:51.447975 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2509 2023-02-27 08:58:18.185309 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-37.pyc
+-rw-r--r--   0        0        0     2531 2023-04-11 08:09:11.418414 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-38.pyc
+-rw-r--r--   0        0        0     9329 2023-04-06 07:28:51.621322 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5831 2023-02-27 09:00:21.696891 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-37.pyc
+-rw-r--r--   0        0        0     6237 2023-04-11 09:50:15.613328 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-38.pyc
+-rw-r--r--   0        0        0     8530 2023-04-06 07:28:51.624656 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5738 2023-02-27 09:00:21.696891 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-37.pyc
+-rw-r--r--   0        0        0     4881 2023-04-11 09:50:15.616661 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-38.pyc
+-rw-r--r--   0        0        0    29173 2023-04-06 07:28:51.631323 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-311.pyc
+-rwxr-xr-x   0        0        0    17850 2023-02-27 09:00:21.703558 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-37.pyc
+-rw-r--r--   0        0        0    17898 2023-04-11 09:50:15.619995 renku-2.4.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-38.pyc
+-rw-r--r--   0        0        0    12028 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/api.py
+-rw-r--r--   0        0        0     6966 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/azure.py
+-rw-r--r--   0        0        0     2225 2023-04-11 08:06:19.149735 renku-2.4.0rc1/renku/core/dataset/providers/common.py
+-rw-r--r--   0        0        0    20652 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/dataverse.py
+-rw-r--r--   0        0        0     3317 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py
+-rw-r--r--   0        0        0     4808 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/doi.py
+-rw-r--r--   0        0        0     5602 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/external.py
+-rw-r--r--   0        0        0     5764 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/dataset/providers/factory.py
+-rw-r--r--   0        0        0     7300 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/git.py
+-rw-r--r--   0        0        0    10567 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/local.py
+-rw-r--r--   0        0        0     5869 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/models.py
+-rw-r--r--   0        0        0    10097 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/olos.py
+-rw-r--r--   0        0        0    22146 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/renku.py
+-rw-r--r--   0        0        0     2553 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/dataset/providers/repository.py
+-rw-r--r--   0        0        0     6392 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/s3.py
+-rw-r--r--   0        0        0     5813 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/web.py
+-rw-r--r--   0        0        0    18624 2023-04-11 09:50:14.239977 renku-2.4.0rc1/renku/core/dataset/providers/zenodo.py
+-rw-r--r--   0        0        0     3973 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/dataset/request_model.py
+-rw-r--r--   0        0        0     5361 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/dataset/tag.py
+-rw-r--r--   0        0        0    25125 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/errors.py
+-rw-r--r--   0        0        0     1115 2023-04-11 08:06:19.153068 renku-2.4.0rc1/renku/core/gc.py
+-rw-r--r--   0        0        0     7394 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/git.py
+-rw-r--r--   0        0        0     2151 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/githooks.py
+-rw-r--r--   0        0        0    16526 2023-04-11 08:43:02.645858 renku-2.4.0rc1/renku/core/init.py
+-rw-r--r--   0        0        0      775 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-06 07:28:50.627907 renku-2.4.0rc1/renku/core/interface/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      192 2023-02-27 08:58:17.935306 renku-2.4.0rc1/renku/core/interface/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      196 2023-04-11 08:06:12.416324 renku-2.4.0rc1/renku/core/interface/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5183 2023-04-06 07:28:57.118445 renku-2.4.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4262 2023-02-27 09:00:23.150243 renku-2.4.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     4258 2023-04-11 08:06:13.319668 renku-2.4.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1484 2023-04-06 07:28:50.627907 renku-2.4.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1221 2023-02-27 08:58:17.935306 renku-2.4.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     1235 2023-04-11 08:06:12.419658 renku-2.4.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2590 2023-04-06 07:28:51.481311 renku-2.4.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2163 2023-02-27 08:58:18.195309 renku-2.4.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     2148 2023-04-11 08:06:12.659660 renku-2.4.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2553 2023-04-06 07:28:57.085109 renku-2.4.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2022 2023-02-27 09:00:23.133576 renku-2.4.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     2046 2023-04-11 08:06:13.306335 renku-2.4.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1164 2023-04-06 07:28:50.627907 renku-2.4.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0      934 2023-02-27 08:58:17.935306 renku-2.4.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0      948 2023-04-11 08:06:12.419658 renku-2.4.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     5884 2023-04-06 07:28:51.427973 renku-2.4.0rc1/renku/core/interface/__pycache__/storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4706 2023-02-27 08:58:18.178642 renku-2.4.0rc1/renku/core/interface/__pycache__/storage.cpython-37.pyc
+-rw-r--r--   0        0        0     4391 2023-04-11 08:09:11.411748 renku-2.4.0rc1/renku/core/interface/__pycache__/storage.cpython-38.pyc
+-rw-r--r--   0        0        0     1897 2023-04-06 07:28:56.778417 renku-2.4.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1561 2023-02-27 09:00:23.096909 renku-2.4.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-37.pyc
+-rw-r--r--   0        0        0     1568 2023-04-11 08:06:13.289668 renku-2.4.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     3741 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/activity_gateway.py
+-rw-r--r--   0        0        0     1418 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/database_gateway.py
+-rw-r--r--   0        0        0     2095 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/dataset_gateway.py
+-rw-r--r--   0        0        0     1996 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/plan_gateway.py
+-rw-r--r--   0        0        0     1212 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/project_gateway.py
+-rw-r--r--   0        0        0     4226 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/interface/storage.py
+-rw-r--r--   0        0        0     1780 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/interface/workflow_file_parser.py
+-rw-r--r--   0        0        0    10400 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/login.py
+-rw-r--r--   0        0        0      764 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/migration/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-06 07:28:51.307963 renku-2.4.0rc1/renku/core/migration/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      181 2023-02-27 09:00:41.403809 renku-2.4.0rc1/renku/core/migration/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      185 2023-04-11 08:06:12.599660 renku-2.4.0rc1/renku/core/migration/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      713 2023-04-06 07:29:19.010278 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__0_pyld2.cpython-311.pyc
+-rwxr-xr-x   0        0        0      611 2023-02-27 09:00:59.497372 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__0_pyld2.cpython-37.pyc
+-rw-r--r--   0        0        0      617 2023-04-11 08:06:25.363139 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__0_pyld2.cpython-38.pyc
+-rw-r--r--   0        0        0    13691 2023-04-06 07:29:19.013612 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__1_jsonld.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7668 2023-02-27 09:00:59.504039 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__1_jsonld.cpython-37.pyc
+-rw-r--r--   0        0        0     7574 2023-04-11 08:06:25.366472 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__1_jsonld.cpython-38.pyc
+-rw-r--r--   0        0        0    13986 2023-04-06 07:29:19.016945 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__2_initial.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6750 2023-02-27 09:00:59.507372 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__2_initial.cpython-37.pyc
+-rw-r--r--   0        0        0     6670 2023-04-11 08:06:25.373139 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0003__2_initial.cpython-38.pyc
+-rw-r--r--   0        0        0      713 2023-04-06 07:29:19.030280 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__0_pyld2.cpython-311.pyc
+-rwxr-xr-x   0        0        0      611 2023-02-27 09:00:59.534039 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__0_pyld2.cpython-37.pyc
+-rw-r--r--   0        0        0      617 2023-04-11 08:06:25.389806 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__0_pyld2.cpython-38.pyc
+-rw-r--r--   0        0        0     6923 2023-04-06 07:29:19.030280 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__submodules.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3585 2023-02-27 09:00:59.540706 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__submodules.cpython-37.pyc
+-rw-r--r--   0        0        0     3581 2023-04-11 08:06:25.393139 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0004__submodules.cpython-38.pyc
+-rw-r--r--   0        0        0     1831 2023-04-06 07:29:19.010278 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__1_pyld2.cpython-311.pyc
+-rwxr-xr-x   0        0        0      987 2023-02-27 09:00:59.500705 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__1_pyld2.cpython-37.pyc
+-rw-r--r--   0        0        0      995 2023-04-11 08:06:25.363139 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__1_pyld2.cpython-38.pyc
+-rw-r--r--   0        0        0    22160 2023-04-06 07:29:19.046948 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__2_cwl.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10323 2023-02-27 09:00:59.560706 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__2_cwl.cpython-37.pyc
+-rw-r--r--   0        0        0    10356 2023-04-11 08:06:25.419806 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0005__2_cwl.cpython-38.pyc
+-rw-r--r--   0        0        0      785 2023-04-06 07:29:19.046948 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0006__dataset_context.cpython-311.pyc
+-rwxr-xr-x   0        0        0      573 2023-02-27 09:00:59.560706 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0006__dataset_context.cpython-37.pyc
+-rw-r--r--   0        0        0      581 2023-04-11 08:06:25.423140 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0006__dataset_context.cpython-38.pyc
+-rw-r--r--   0        0        0     1309 2023-04-06 07:29:19.050282 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0007__source_url.cpython-311.pyc
+-rwxr-xr-x   0        0        0      832 2023-02-27 09:00:59.564040 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0007__source_url.cpython-37.pyc
+-rw-r--r--   0        0        0      836 2023-04-11 08:06:25.426473 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0007__source_url.cpython-38.pyc
+-rw-r--r--   0        0        0     1318 2023-04-06 07:29:19.053615 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0008__dataset_metadata.cpython-311.pyc
+-rwxr-xr-x   0        0        0      895 2023-02-27 09:00:59.567373 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0008__dataset_metadata.cpython-37.pyc
+-rw-r--r--   0        0        0      915 2023-04-11 08:06:25.429807 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0008__dataset_metadata.cpython-38.pyc
+-rw-r--r--   0        0        0    42701 2023-04-06 07:29:19.036947 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0009__new_metadata_storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0    22235 2023-02-27 09:00:59.547373 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0009__new_metadata_storage.cpython-37.pyc
+-rw-r--r--   0        0        0    22343 2023-04-11 08:06:25.406473 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0009__new_metadata_storage.cpython-38.pyc
+-rw-r--r--   0        0        0    19923 2023-04-06 07:29:19.063616 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0010__metadata_fixes.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9976 2023-02-27 09:00:59.584040 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0010__metadata_fixes.cpython-37.pyc
+-rw-r--r--   0        0        0     9963 2023-04-11 08:06:25.439807 renku-2.4.0rc1/renku/core/migration/__pycache__/m_0010__metadata_fixes.cpython-38.pyc
+-rw-r--r--   0        0        0    12808 2023-04-06 07:29:06.382551 renku-2.4.0rc1/renku/core/migration/__pycache__/migrate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8224 2023-02-27 09:00:41.407142 renku-2.4.0rc1/renku/core/migration/__pycache__/migrate.cpython-37.pyc
+-rw-r--r--   0        0        0     8190 2023-04-11 08:06:17.549716 renku-2.4.0rc1/renku/core/migration/__pycache__/migrate.cpython-38.pyc
+-rw-r--r--   0        0        0     1122 2023-04-11 08:06:10.272966 renku-2.4.0rc1/renku/core/migration/m_0003__0_pyld2.py
+-rw-r--r--   0        0        0    15324 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/migration/m_0003__1_jsonld.py
+-rw-r--r--   0        0        0     9570 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0003__2_initial.py
+-rw-r--r--   0        0        0     1122 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0004__0_pyld2.py
+-rw-r--r--   0        0        0     5318 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0004__submodules.py
+-rw-r--r--   0        0        0     1548 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0005__1_pyld2.py
+-rw-r--r--   0        0        0    16122 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0005__2_cwl.py
+-rw-r--r--   0        0        0     1015 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0006__dataset_context.py
+-rw-r--r--   0        0        0     1430 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0007__source_url.py
+-rw-r--r--   0        0        0     1175 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0008__dataset_metadata.py
+-rw-r--r--   0        0        0    30683 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/migration/m_0009__new_metadata_storage.py
+-rw-r--r--   0        0        0    14077 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/m_0010__metadata_fixes.py
+-rw-r--r--   0        0        0    10122 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/migrate.py
+-rw-r--r--   0        0        0      770 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-06 07:29:06.385885 renku-2.4.0rc1/renku/core/migration/models/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      194 2023-02-27 09:00:41.410475 renku-2.4.0rc1/renku/core/migration/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      198 2023-04-11 08:06:17.553050 renku-2.4.0rc1/renku/core/migration/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8580 2023-04-06 07:29:06.385885 renku-2.4.0rc1/renku/core/migration/models/__pycache__/migration.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5334 2023-02-27 09:00:41.413809 renku-2.4.0rc1/renku/core/migration/models/__pycache__/migration.cpython-37.pyc
+-rw-r--r--   0        0        0     5356 2023-04-11 08:06:17.556383 renku-2.4.0rc1/renku/core/migration/models/__pycache__/migration.cpython-38.pyc
+-rw-r--r--   0        0        0     5921 2023-04-06 07:29:10.946267 renku-2.4.0rc1/renku/core/migration/models/__pycache__/refs.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3625 2023-02-27 09:00:48.193895 renku-2.4.0rc1/renku/core/migration/models/__pycache__/refs.cpython-37.pyc
+-rw-r--r--   0        0        0     3655 2023-04-11 08:06:20.539751 renku-2.4.0rc1/renku/core/migration/models/__pycache__/refs.cpython-38.pyc
+-rw-r--r--   0        0        0     5449 2023-04-06 07:29:10.946267 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v10.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3369 2023-02-27 09:00:48.190562 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v10.cpython-37.pyc
+-rw-r--r--   0        0        0     3374 2023-04-11 08:06:20.536417 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v10.cpython-38.pyc
+-rw-r--r--   0        0        0    21899 2023-04-06 07:29:19.020279 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v3.cpython-311.pyc
+-rwxr-xr-x   0        0        0    12834 2023-02-27 09:00:59.607373 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v3.cpython-37.pyc
+-rw-r--r--   0        0        0    12748 2023-04-11 08:06:25.376473 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v3.cpython-38.pyc
+-rw-r--r--   0        0        0     3912 2023-04-06 07:29:19.050282 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v7.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2524 2023-02-27 09:00:59.564040 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v7.cpython-37.pyc
+-rw-r--r--   0        0        0     2560 2023-04-11 08:06:25.426473 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v7.cpython-38.pyc
+-rw-r--r--   0        0        0     7637 2023-04-06 07:29:19.053615 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v8.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4513 2023-02-27 09:00:59.570706 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v8.cpython-37.pyc
+-rw-r--r--   0        0        0     4555 2023-04-11 08:06:25.433140 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v8.cpython-38.pyc
+-rw-r--r--   0        0        0   126157 2023-04-06 07:29:10.942933 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v9.cpython-311.pyc
+-rwxr-xr-x   0        0        0    71741 2023-02-27 09:00:48.197228 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v9.cpython-37.pyc
+-rw-r--r--   0        0        0    70865 2023-04-11 08:06:20.536417 renku-2.4.0rc1/renku/core/migration/models/__pycache__/v9.cpython-38.pyc
+-rw-r--r--   0        0        0     5830 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/migration.py
+-rw-r--r--   0        0        0     3861 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/refs.py
+-rw-r--r--   0        0        0     5091 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/v10.py
+-rw-r--r--   0        0        0    11828 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/v3.py
+-rw-r--r--   0        0        0     2422 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/v7.py
+-rw-r--r--   0        0        0     4587 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/v8.py
+-rw-r--r--   0        0        0    74088 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/migration/models/v9.py
+-rw-r--r--   0        0        0     7865 2023-04-11 08:42:55.939056 renku-2.4.0rc1/renku/core/migration/utils/__init__.py
+-rw-r--r--   0        0        0    11835 2023-04-06 07:28:51.311297 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6644 2023-02-27 09:00:41.417142 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     6569 2023-04-11 08:42:57.112413 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    11665 2023-04-06 07:29:19.040281 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/conversion.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6376 2023-02-27 09:00:59.550706 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/conversion.cpython-37.pyc
+-rw-r--r--   0        0        0     6546 2023-04-11 08:06:25.406473 renku-2.4.0rc1/renku/core/migration/utils/__pycache__/conversion.cpython-38.pyc
+-rw-r--r--   0        0        0     8121 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/migration/utils/conversion.py
+-rw-r--r--   0        0        0      824 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-06 07:28:50.691245 renku-2.4.0rc1/renku/core/plugin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      250 2023-02-27 08:58:18.045307 renku-2.4.0rc1/renku/core/plugin/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      254 2023-04-11 08:06:12.462992 renku-2.4.0rc1/renku/core/plugin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1318 2023-04-06 07:28:50.694579 renku-2.4.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1010 2023-02-27 08:58:18.045307 renku-2.4.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1022 2023-04-11 08:06:12.466325 renku-2.4.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-38.pyc
+-rw-r--r--   0        0        0     1899 2023-04-06 07:28:50.701246 renku-2.4.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1034 2023-02-27 08:58:18.048641 renku-2.4.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-37.pyc
+-rw-r--r--   0        0        0     1040 2023-04-11 08:06:12.466325 renku-2.4.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-38.pyc
+-rw-r--r--   0        0        0     4429 2023-04-06 07:28:54.341548 renku-2.4.0rc1/renku/core/plugin/__pycache__/provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3237 2023-02-27 09:00:22.540235 renku-2.4.0rc1/renku/core/plugin/__pycache__/provider.cpython-37.pyc
+-rw-r--r--   0        0        0     3239 2023-04-11 08:06:12.999664 renku-2.4.0rc1/renku/core/plugin/__pycache__/provider.cpython-38.pyc
+-rw-r--r--   0        0        0     1635 2023-04-06 07:28:59.151948 renku-2.4.0rc1/renku/core/plugin/__pycache__/run.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1434 2023-02-27 09:00:23.780251 renku-2.4.0rc1/renku/core/plugin/__pycache__/run.cpython-37.pyc
+-rw-r--r--   0        0        0     1456 2023-04-11 08:06:13.579671 renku-2.4.0rc1/renku/core/plugin/__pycache__/run.cpython-38.pyc
+-rw-r--r--   0        0        0     1289 2023-04-06 07:28:59.341963 renku-2.4.0rc1/renku/core/plugin/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0      962 2023-02-27 09:00:23.933586 renku-2.4.0rc1/renku/core/plugin/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0      974 2023-04-11 08:06:13.673005 renku-2.4.0rc1/renku/core/plugin/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     5856 2023-04-06 07:28:58.555231 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4235 2023-02-27 09:00:23.556915 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow.cpython-37.pyc
+-rw-r--r--   0        0        0     4174 2023-04-11 08:06:13.509670 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0        0        0     4200 2023-04-06 07:28:57.135113 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2965 2023-02-27 09:00:23.163576 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-37.pyc
+-rw-r--r--   0        0        0     2981 2023-04-11 08:06:13.326335 renku-2.4.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     1467 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/dataset_provider.py
+-rw-r--r--   0        0        0     3046 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/plugin/implementations/__init__.py
+-rw-r--r--   0        0        0     3216 2023-04-06 07:28:50.701246 renku-2.4.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2448 2023-02-27 08:58:18.048641 renku-2.4.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2531 2023-04-11 08:09:11.291746 renku-2.4.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1790 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/pluginmanager.py
+-rw-r--r--   0        0        0     3357 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/provider.py
+-rw-r--r--   0        0        0     1839 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/run.py
+-rw-r--r--   0        0        0     1454 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/session.py
+-rw-r--r--   0        0        0     4195 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/workflow.py
+-rw-r--r--   0        0        0     3065 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/plugin/workflow_file_parser.py
+-rw-r--r--   0        0        0     3355 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/project.py
+-rw-r--r--   0        0        0      780 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/session/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-06 07:28:51.631323 renku-2.4.0rc1/renku/core/session/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      195 2023-02-27 09:00:21.703558 renku-2.4.0rc1/renku/core/session/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      199 2023-04-11 08:06:12.709661 renku-2.4.0rc1/renku/core/session/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    18684 2023-04-06 07:28:51.634657 renku-2.4.0rc1/renku/core/session/__pycache__/docker.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10103 2023-02-27 09:00:21.706891 renku-2.4.0rc1/renku/core/session/__pycache__/docker.cpython-37.pyc
+-rw-r--r--   0        0        0    11338 2023-04-11 08:09:11.471748 renku-2.4.0rc1/renku/core/session/__pycache__/docker.cpython-38.pyc
+-rw-r--r--   0        0        0    26085 2023-04-06 07:28:53.304795 renku-2.4.0rc1/renku/core/session/__pycache__/renkulab.cpython-311.pyc
+-rwxr-xr-x   0        0        0    15296 2023-02-27 09:00:21.920227 renku-2.4.0rc1/renku/core/session/__pycache__/renkulab.cpython-37.pyc
+-rw-r--r--   0        0        0    15766 2023-04-11 09:49:33.399467 renku-2.4.0rc1/renku/core/session/__pycache__/renkulab.cpython-38.pyc
+-rw-r--r--   0        0        0    16650 2023-04-06 07:29:12.783088 renku-2.4.0rc1/renku/core/session/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8748 2023-02-27 09:00:50.210587 renku-2.4.0rc1/renku/core/session/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0     8936 2023-04-11 08:06:21.493095 renku-2.4.0rc1/renku/core/session/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     2293 2023-04-06 07:28:53.308129 renku-2.4.0rc1/renku/core/session/__pycache__/utils.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1420 2023-02-27 09:00:21.923560 renku-2.4.0rc1/renku/core/session/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     1438 2023-04-11 08:06:12.869663 renku-2.4.0rc1/renku/core/session/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13703 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/session/docker.py
+-rw-r--r--   0        0        0    20167 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/core/session/renkulab.py
+-rw-r--r--   0        0        0    11815 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/session/session.py
+-rw-r--r--   0        0        0     2215 2023-04-11 08:06:10.276300 renku-2.4.0rc1/renku/core/session/utils.py
+-rw-r--r--   0        0        0    22082 2023-04-11 08:06:19.156401 renku-2.4.0rc1/renku/core/storage.py
+-rw-r--r--   0        0        0      760 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/core/template/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-06 07:28:59.421970 renku-2.4.0rc1/renku/core/template/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      189 2023-02-27 09:00:46.040534 renku-2.4.0rc1/renku/core/template/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      193 2023-04-11 09:50:16.256669 renku-2.4.0rc1/renku/core/template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    30532 2023-04-06 07:28:59.428637 renku-2.4.0rc1/renku/core/template/__pycache__/template.cpython-311.pyc
+-rwxr-xr-x   0        0        0    17452 2023-02-27 09:00:46.047201 renku-2.4.0rc1/renku/core/template/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0        0        0    17890 2023-04-11 09:50:16.260003 renku-2.4.0rc1/renku/core/template/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0        0        0    18692 2023-04-06 07:29:06.389218 renku-2.4.0rc1/renku/core/template/__pycache__/usecase.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8600 2023-02-27 09:00:46.053868 renku-2.4.0rc1/renku/core/template/__pycache__/usecase.cpython-37.pyc
+-rw-r--r--   0        0        0    10922 2023-04-11 09:50:18.596698 renku-2.4.0rc1/renku/core/template/__pycache__/usecase.cpython-38.pyc
+-rw-r--r--   0        0        0    21581 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/core/template/template.py
+-rw-r--r--   0        0        0    14523 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/core/template/usecase.py
+-rw-r--r--   0        0        0      756 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-06 07:28:50.287879 renku-2.4.0rc1/renku/core/util/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      181 2023-02-27 08:58:17.911972 renku-2.4.0rc1/renku/core/util/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      185 2023-04-11 08:09:11.195078 renku-2.4.0rc1/renku/core/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    16963 2023-04-06 07:28:50.291212 renku-2.4.0rc1/renku/core/util/__pycache__/communication.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11232 2023-02-27 08:58:17.911972 renku-2.4.0rc1/renku/core/util/__pycache__/communication.cpython-37.pyc
+-rw-r--r--   0        0        0    11001 2023-04-11 08:09:11.198412 renku-2.4.0rc1/renku/core/util/__pycache__/communication.cpython-38.pyc
+-rw-r--r--   0        0        0    10257 2023-04-06 07:28:50.611239 renku-2.4.0rc1/renku/core/util/__pycache__/contexts.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6138 2023-02-27 08:58:17.925306 renku-2.4.0rc1/renku/core/util/__pycache__/contexts.cpython-37.pyc
+-rw-r--r--   0        0        0     6209 2023-04-11 08:09:11.265079 renku-2.4.0rc1/renku/core/util/__pycache__/contexts.cpython-38.pyc
+-rwxr-xr-x   0        0        0      669 2023-02-27 08:58:18.185309 renku-2.4.0rc1/renku/core/util/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0      677 2023-04-11 08:06:12.646327 renku-2.4.0rc1/renku/core/util/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     2646 2023-04-06 07:28:51.301296 renku-2.4.0rc1/renku/core/util/__pycache__/datetime8601.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1808 2023-02-27 08:58:18.151975 renku-2.4.0rc1/renku/core/util/__pycache__/datetime8601.cpython-37.pyc
+-rw-r--r--   0        0        0     1792 2023-04-11 08:09:11.381747 renku-2.4.0rc1/renku/core/util/__pycache__/datetime8601.cpython-38.pyc
+-rw-r--r--   0        0        0     1320 2023-04-06 07:28:50.694579 renku-2.4.0rc1/renku/core/util/__pycache__/doi.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-02-27 08:58:18.048641 renku-2.4.0rc1/renku/core/util/__pycache__/doi.cpython-37.pyc
+-rw-r--r--   0        0        0      924 2023-04-11 08:09:11.291746 renku-2.4.0rc1/renku/core/util/__pycache__/doi.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1396 2023-02-27 08:58:17.915306 renku-2.4.0rc1/renku/core/util/__pycache__/file_size.cpython-37.pyc
+-rw-r--r--   0        0        0     1413 2023-04-11 08:06:12.279656 renku-2.4.0rc1/renku/core/util/__pycache__/file_size.cpython-38.pyc
+-rw-r--r--   0        0        0    54972 2023-04-06 07:28:50.304547 renku-2.4.0rc1/renku/core/util/__pycache__/git.cpython-311.pyc
+-rwxr-xr-x   0        0        0    32756 2023-02-27 08:58:17.918639 renku-2.4.0rc1/renku/core/util/__pycache__/git.cpython-37.pyc
+-rw-r--r--   0        0        0    33610 2023-04-11 08:09:11.201745 renku-2.4.0rc1/renku/core/util/__pycache__/git.cpython-38.pyc
+-rw-r--r--   0        0        0     1052 2023-04-06 07:28:53.338131 renku-2.4.0rc1/renku/core/util/__pycache__/jwt.cpython-311.pyc
+-rwxr-xr-x   0        0        0      650 2023-02-27 09:00:21.946894 renku-2.4.0rc1/renku/core/util/__pycache__/jwt.cpython-37.pyc
+-rw-r--r--   0        0        0      660 2023-04-11 08:09:11.621750 renku-2.4.0rc1/renku/core/util/__pycache__/jwt.cpython-38.pyc
+-rw-r--r--   0        0        0     9999 2023-04-06 07:28:51.307963 renku-2.4.0rc1/renku/core/util/__pycache__/metadata.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5054 2023-02-27 08:58:18.151975 renku-2.4.0rc1/renku/core/util/__pycache__/metadata.cpython-37.pyc
+-rw-r--r--   0        0        0     6003 2023-04-11 08:09:11.385081 renku-2.4.0rc1/renku/core/util/__pycache__/metadata.cpython-38.pyc
+-rw-r--r--   0        0        0    19962 2023-04-06 07:28:50.594571 renku-2.4.0rc1/renku/core/util/__pycache__/os.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8663 2023-02-27 08:58:17.921972 renku-2.4.0rc1/renku/core/util/__pycache__/os.cpython-37.pyc
+-rw-r--r--   0        0        0    11040 2023-04-11 08:09:11.258412 renku-2.4.0rc1/renku/core/util/__pycache__/os.cpython-38.pyc
+-rw-r--r--   0        0        0    12498 2023-04-06 07:28:53.311462 renku-2.4.0rc1/renku/core/util/__pycache__/requests.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6827 2023-02-27 09:00:21.926894 renku-2.4.0rc1/renku/core/util/__pycache__/requests.cpython-37.pyc
+-rw-r--r--   0        0        0     6820 2023-04-11 08:09:11.618417 renku-2.4.0rc1/renku/core/util/__pycache__/requests.cpython-38.pyc
+-rw-r--r--   0        0        0     1518 2023-04-06 07:29:02.112194 renku-2.4.0rc1/renku/core/util/__pycache__/shacl.cpython-311.pyc
+-rwxr-xr-x   0        0        0      951 2023-02-27 09:00:35.440399 renku-2.4.0rc1/renku/core/util/__pycache__/shacl.cpython-37.pyc
+-rw-r--r--   0        0        0      955 2023-04-11 08:09:13.211769 renku-2.4.0rc1/renku/core/util/__pycache__/shacl.cpython-38.pyc
+-rw-r--r--   0        0        0     9833 2023-04-06 07:28:53.454808 renku-2.4.0rc1/renku/core/util/__pycache__/ssh.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5693 2023-02-27 09:00:21.990228 renku-2.4.0rc1/renku/core/util/__pycache__/ssh.cpython-37.pyc
+-rw-r--r--   0        0        0     5949 2023-04-11 08:09:11.638417 renku-2.4.0rc1/renku/core/util/__pycache__/ssh.cpython-38.pyc
+-rw-r--r--   0        0        0     2982 2023-04-06 07:28:59.511978 renku-2.4.0rc1/renku/core/util/__pycache__/tabulate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1704 2023-02-27 09:00:24.340258 renku-2.4.0rc1/renku/core/util/__pycache__/tabulate.cpython-37.pyc
+-rw-r--r--   0        0        0     1739 2023-04-11 08:09:12.358425 renku-2.4.0rc1/renku/core/util/__pycache__/tabulate.cpython-38.pyc
+-rwxr-xr-x   0        0        0     2201 2023-02-27 09:00:23.166910 renku-2.4.0rc1/renku/core/util/__pycache__/template_vars.cpython-37.pyc
+-rw-r--r--   0        0        0     2220 2023-04-11 08:06:13.329668 renku-2.4.0rc1/renku/core/util/__pycache__/template_vars.cpython-38.pyc
+-rw-r--r--   0        0        0     8340 2023-04-06 07:28:51.314630 renku-2.4.0rc1/renku/core/util/__pycache__/urls.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4137 2023-02-27 08:58:18.155309 renku-2.4.0rc1/renku/core/util/__pycache__/urls.cpython-37.pyc
+-rw-r--r--   0        0        0     4935 2023-04-11 08:09:11.388414 renku-2.4.0rc1/renku/core/util/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0        0        0     6186 2023-04-06 07:28:51.624656 renku-2.4.0rc1/renku/core/util/__pycache__/util.cpython-311.pyc
+-rwxr-xr-x   0        0        0      861 2023-02-27 08:58:18.038641 renku-2.4.0rc1/renku/core/util/__pycache__/util.cpython-37.pyc
+-rw-r--r--   0        0        0     3643 2023-04-11 08:09:11.461748 renku-2.4.0rc1/renku/core/util/__pycache__/util.cpython-38.pyc
+-rwxr-xr-x   0        0        0      515 2023-02-27 09:00:48.250562 renku-2.4.0rc1/renku/core/util/__pycache__/uuid.cpython-37.pyc
+-rw-r--r--   0        0        0      525 2023-03-13 14:36:07.833026 renku-2.4.0rc1/renku/core/util/__pycache__/uuid.cpython-38.pyc
+-rw-r--r--   0        0        0     4051 2023-04-06 07:28:51.311297 renku-2.4.0rc1/renku/core/util/__pycache__/yaml.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2576 2023-02-27 09:00:22.543568 renku-2.4.0rc1/renku/core/util/__pycache__/yaml.cpython-37.pyc
+-rw-r--r--   0        0        0     2626 2023-04-11 08:09:11.385081 renku-2.4.0rc1/renku/core/util/__pycache__/yaml.cpython-38.pyc
+-rw-r--r--   0        0        0    10282 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/communication.py
+-rw-r--r--   0        0        0     6617 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/contexts.py
+-rw-r--r--   0        0        0     2313 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/datetime8601.py
+-rw-r--r--   0        0        0     1376 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/doi.py
+-rw-r--r--   0        0        0    40487 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/git.py
+-rw-r--r--   0        0        0     1244 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/jwt.py
+-rw-r--r--   0        0        0     7036 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/metadata.py
+-rw-r--r--   0        0        0    12140 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/os.py
+-rw-r--r--   0        0        0     7626 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/requests.py
+-rw-r--r--   0        0        0     1611 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/shacl.py
+-rw-r--r--   0        0        0     6871 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/ssh.py
+-rw-r--r--   0        0        0     2158 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/tabulate.py
+-rw-r--r--   0        0        0     6228 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/urls.py
+-rw-r--r--   0        0        0     3878 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/util.py
+-rw-r--r--   0        0        0     2836 2023-04-11 08:06:19.159735 renku-2.4.0rc1/renku/core/util/yaml.py
+-rw-r--r--   0        0        0      773 2023-04-11 08:06:10.279633 renku-2.4.0rc1/renku/core/workflow/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-06 07:28:53.454808 renku-2.4.0rc1/renku/core/workflow/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      189 2023-02-27 09:00:21.993561 renku-2.4.0rc1/renku/core/workflow/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      193 2023-04-11 08:06:12.906330 renku-2.4.0rc1/renku/core/workflow/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    31736 2023-04-06 07:28:57.261790 renku-2.4.0rc1/renku/core/workflow/__pycache__/activity.cpython-311.pyc
+-rwxr-xr-x   0        0        0    18260 2023-02-27 09:00:23.230244 renku-2.4.0rc1/renku/core/workflow/__pycache__/activity.cpython-37.pyc
+-rw-r--r--   0        0        0    18284 2023-04-11 08:09:12.028421 renku-2.4.0rc1/renku/core/workflow/__pycache__/activity.cpython-38.pyc
+-rw-r--r--   0        0        0    25911 2023-04-06 07:28:59.315295 renku-2.4.0rc1/renku/core/workflow/__pycache__/execute.cpython-311.pyc
+-rwxr-xr-x   0        0        0    14757 2023-02-27 09:00:23.910252 renku-2.4.0rc1/renku/core/workflow/__pycache__/execute.cpython-37.pyc
+-rw-r--r--   0        0        0    14618 2023-04-11 08:06:13.659672 renku-2.4.0rc1/renku/core/workflow/__pycache__/execute.cpython-38.pyc
+-rw-r--r--   0        0        0    46613 2023-04-06 07:28:57.101777 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0    26635 2023-02-27 09:00:23.140243 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan.cpython-37.pyc
+-rw-r--r--   0        0        0    26608 2023-04-11 08:09:11.975088 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan.cpython-38.pyc
+-rw-r--r--   0        0        0    44887 2023-04-06 07:28:57.288459 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-311.pyc
+-rwxr-xr-x   0        0        0    23562 2023-02-27 09:00:23.240244 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-37.pyc
+-rw-r--r--   0        0        0    23749 2023-04-11 08:09:12.035088 renku-2.4.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-38.pyc
+-rw-r--r--   0        0        0    18187 2023-04-06 07:28:57.225121 renku-2.4.0rc1/renku/core/workflow/__pycache__/run.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9834 2023-02-27 09:00:23.213577 renku-2.4.0rc1/renku/core/workflow/__pycache__/run.cpython-37.pyc
+-rw-r--r--   0        0        0     9968 2023-04-11 08:06:13.353002 renku-2.4.0rc1/renku/core/workflow/__pycache__/run.cpython-38.pyc
+-rw-r--r--   0        0        0     2528 2023-04-06 07:28:57.291793 renku-2.4.0rc1/renku/core/workflow/__pycache__/types.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1621 2023-02-27 09:00:23.240244 renku-2.4.0rc1/renku/core/workflow/__pycache__/types.cpython-37.pyc
+-rw-r--r--   0        0        0     1649 2023-04-11 08:06:13.373002 renku-2.4.0rc1/renku/core/workflow/__pycache__/types.cpython-38.pyc
+-rw-r--r--   0        0        0     3708 2023-04-06 07:29:20.027031 renku-2.4.0rc1/renku/core/workflow/__pycache__/update.cpython-311.pyc
+-rw-r--r--   0        0        0     2408 2023-04-11 08:06:25.966479 renku-2.4.0rc1/renku/core/workflow/__pycache__/update.cpython-38.pyc
+-rw-r--r--   0        0        0    13786 2023-04-06 07:28:57.141780 renku-2.4.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6988 2023-02-27 09:00:23.166910 renku-2.4.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-37.pyc
+-rw-r--r--   0        0        0     8679 2023-04-11 08:09:11.991755 renku-2.4.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-38.pyc
+-rw-r--r--   0        0        0     7621 2023-04-06 07:28:59.308627 renku-2.4.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4780 2023-02-27 09:00:23.906919 renku-2.4.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-37.pyc
+-rw-r--r--   0        0        0     4827 2023-04-11 08:06:13.656339 renku-2.4.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-38.pyc
+-rw-r--r--   0        0        0    22713 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/core/workflow/activity.py
+-rw-r--r--   0        0        0      773 2023-04-11 08:06:10.279633 renku-2.4.0rc1/renku/core/workflow/converters/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-06 07:28:53.458141 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      200 2023-02-27 09:00:21.993561 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      204 2023-04-11 08:06:12.906330 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    21208 2023-04-06 07:28:53.468142 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11183 2023-02-27 09:00:21.996895 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-37.pyc
+-rw-r--r--   0        0        0    11072 2023-04-11 08:06:12.909663 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-38.pyc
+-rw-r--r--   0        0        0     7476 2023-04-06 07:28:56.765082 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4685 2023-02-27 09:00:23.090242 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-37.pyc
+-rw-r--r--   0        0        0     4673 2023-04-11 08:06:13.283001 renku-2.4.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-38.pyc
+-rw-r--r--   0        0        0    17930 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/converters/cwl.py
+-rw-r--r--   0        0        0     5142 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/converters/renku.py
+-rw-r--r--   0        0        0    18756 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/execute.py
+-rw-r--r--   0        0        0      769 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/model/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-06 07:28:54.344881 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      191 2023-02-27 09:00:22.543568 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      195 2023-04-11 08:06:13.002998 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8439 2023-04-06 07:28:54.348215 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4821 2023-02-27 09:00:22.543568 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-37.pyc
+-rw-r--r--   0        0        0     4818 2023-04-11 08:06:13.006331 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-38.pyc
+-rw-r--r--   0        0        0    44893 2023-04-06 07:28:56.861757 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0    25926 2023-02-27 09:00:23.103576 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-37.pyc
+-rw-r--r--   0        0        0    25819 2023-04-11 08:06:13.296334 renku-2.4.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-38.pyc
+-rw-r--r--   0        0        0     6530 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/model/concrete_execution_graph.py
+-rw-r--r--   0        0        0    37303 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/model/workflow_file.py
+-rw-r--r--   0        0        0      775 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/parser/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-06 07:28:56.768416 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      198 2023-02-27 09:00:23.090242 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      202 2023-04-11 08:06:13.286334 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    15786 2023-04-06 07:28:56.778417 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8610 2023-02-27 09:00:23.093576 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-37.pyc
+-rw-r--r--   0        0        0     8611 2023-04-11 08:06:13.286334 renku-2.4.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/parser/renku.py
+-rw-r--r--   0        0        0    34209 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/core/workflow/plan.py
+-rw-r--r--   0        0        0    33046 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/core/workflow/plan_factory.py
+-rw-r--r--   0        0        0      772 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/providers/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-06 07:28:57.318462 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      198 2023-02-27 09:00:23.250244 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      202 2023-04-11 08:06:13.379669 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7918 2023-04-06 07:28:57.325129 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4546 2023-02-27 09:00:23.253578 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-37.pyc
+-rw-r--r--   0        0        0     4588 2023-04-11 08:06:13.383002 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-38.pyc
+-rw-r--r--   0        0        0     6829 2023-04-06 07:28:58.558565 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3864 2023-02-27 09:00:23.560248 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-37.pyc
+-rw-r--r--   0        0        0     3875 2023-04-11 08:06:13.513003 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-38.pyc
+-rw-r--r--   0        0        0    21323 2023-04-06 07:28:58.568566 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11195 2023-02-27 09:00:23.566915 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-37.pyc
+-rw-r--r--   0        0        0    11149 2023-04-11 08:06:13.513003 renku-2.4.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-38.pyc
+-rw-r--r--   0        0        0     5999 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/providers/cwltool.py
+-rw-r--r--   0        0        0     4271 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/providers/local.py
+-rw-r--r--   0        0        0    13372 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/providers/toil.py
+-rw-r--r--   0        0        0    13562 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/run.py
+-rw-r--r--   0        0        0     1681 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/types.py
+-rw-r--r--   0        0        0     2869 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/update.py
+-rw-r--r--   0        0        0     8335 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/core/workflow/value_resolution.py
+-rw-r--r--   0        0        0     5089 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/core/workflow/workflow_file.py
+-rw-r--r--   0        0        0      767 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/data/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-06 07:29:20.170376 renku-2.4.0rc1/renku/data/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      187 2023-02-27 09:01:02.207406 renku-2.4.0rc1/renku/data/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      191 2023-04-11 08:06:26.056480 renku-2.4.0rc1/renku/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      114 2023-03-02 15:15:40.049932 renku-2.4.0rc1/renku/data/defaults.ini
+-rw-r--r--   0        0        0     3364 2023-03-02 15:15:40.049932 renku-2.4.0rc1/renku/data/gitignore.default
+-rwxr-xr-x   0        0        0     4372 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/data/pre-commit.sh
+-rw-r--r--   0        0        0    48383 2023-04-11 08:06:10.282966 renku-2.4.0rc1/renku/data/shacl_shape.json
+-rw-r--r--   0        0        0      767 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-06 07:28:50.121198 renku-2.4.0rc1/renku/domain_model/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      195 2023-02-27 08:58:17.885305 renku-2.4.0rc1/renku/domain_model/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      199 2023-04-11 08:09:11.168411 renku-2.4.0rc1/renku/domain_model/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      505 2023-04-06 07:28:50.671244 renku-2.4.0rc1/renku/domain_model/__pycache__/constant.cpython-311.pyc
+-rw-r--r--   0        0        0      377 2023-04-11 08:06:23.969790 renku-2.4.0rc1/renku/domain_model/__pycache__/constant.cpython-38.pyc
+-rw-r--r--   0        0        0    46799 2023-04-06 07:28:51.174619 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0    22941 2023-02-27 08:58:18.151975 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0    26401 2023-04-11 08:09:11.361747 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     1229 2023-04-06 07:28:50.691245 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0      965 2023-02-27 08:58:18.045307 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      977 2023-04-11 08:09:11.288413 renku-2.4.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-38.pyc
+-rw-r--r--   0        0        0     3537 2023-04-06 07:28:57.295127 renku-2.4.0rc1/renku/domain_model/__pycache__/datastructures.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2179 2023-02-27 09:00:23.243577 renku-2.4.0rc1/renku/domain_model/__pycache__/datastructures.cpython-37.pyc
+-rw-r--r--   0        0        0     2195 2023-04-11 08:09:12.038422 renku-2.4.0rc1/renku/domain_model/__pycache__/datastructures.cpython-38.pyc
+-rw-r--r--   0        0        0     4119 2023-04-06 07:28:51.161284 renku-2.4.0rc1/renku/domain_model/__pycache__/entity.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2617 2023-02-27 08:58:18.145309 renku-2.4.0rc1/renku/domain_model/__pycache__/entity.cpython-37.pyc
+-rw-r--r--   0        0        0     2552 2023-04-11 08:09:11.355080 renku-2.4.0rc1/renku/domain_model/__pycache__/entity.cpython-38.pyc
+-rw-r--r--   0        0        0      691 2023-04-06 07:28:50.121198 renku-2.4.0rc1/renku/domain_model/__pycache__/enums.cpython-311.pyc
+-rwxr-xr-x   0        0        0      556 2023-02-27 08:58:17.885305 renku-2.4.0rc1/renku/domain_model/__pycache__/enums.cpython-37.pyc
+-rw-r--r--   0        0        0      564 2023-04-11 08:09:11.168411 renku-2.4.0rc1/renku/domain_model/__pycache__/enums.cpython-38.pyc
+-rw-r--r--   0        0        0     6306 2023-04-06 07:29:12.566403 renku-2.4.0rc1/renku/domain_model/__pycache__/git.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3738 2023-02-27 09:00:49.907250 renku-2.4.0rc1/renku/domain_model/__pycache__/git.cpython-37.pyc
+-rw-r--r--   0        0        0     3772 2023-04-11 08:06:21.386427 renku-2.4.0rc1/renku/domain_model/__pycache__/git.cpython-38.pyc
+-rw-r--r--   0        0        0     9673 2023-04-06 07:28:56.745081 renku-2.4.0rc1/renku/domain_model/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6096 2023-02-27 09:00:23.080242 renku-2.4.0rc1/renku/domain_model/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     6129 2023-04-11 08:09:11.951754 renku-2.4.0rc1/renku/domain_model/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0    19414 2023-04-06 07:28:50.127866 renku-2.4.0rc1/renku/domain_model/__pycache__/project_context.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11819 2023-02-27 08:58:17.888639 renku-2.4.0rc1/renku/domain_model/__pycache__/project_context.cpython-37.pyc
+-rw-r--r--   0        0        0    12047 2023-04-11 08:09:11.168411 renku-2.4.0rc1/renku/domain_model/__pycache__/project_context.cpython-38.pyc
+-rw-r--r--   0        0        0     8261 2023-04-06 07:28:53.301462 renku-2.4.0rc1/renku/domain_model/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6730 2023-02-27 09:00:21.916894 renku-2.4.0rc1/renku/domain_model/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0     7012 2023-04-11 08:09:11.615083 renku-2.4.0rc1/renku/domain_model/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     1597 2023-04-06 07:29:20.370393 renku-2.4.0rc1/renku/domain_model/__pycache__/sort.cpython-311.pyc
+-rwxr-xr-x   0        0        0      923 2023-02-27 09:01:02.647412 renku-2.4.0rc1/renku/domain_model/__pycache__/sort.cpython-37.pyc
+-rw-r--r--   0        0        0      905 2023-04-11 08:06:26.186482 renku-2.4.0rc1/renku/domain_model/__pycache__/sort.cpython-38.pyc
+-rw-r--r--   0        0        0    31738 2023-04-06 07:28:59.435304 renku-2.4.0rc1/renku/domain_model/__pycache__/template.cpython-311.pyc
+-rwxr-xr-x   0        0        0    17777 2023-02-27 09:00:43.270499 renku-2.4.0rc1/renku/domain_model/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0        0        0    18473 2023-04-11 09:50:16.263336 renku-2.4.0rc1/renku/domain_model/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0        0        0    17714 2023-04-11 08:34:51.069714 renku-2.4.0rc1/renku/domain_model/__pycache__/template_BASE_2980914.cpython-38.pyc
+-rw-r--r--   0        0        0    17715 2023-04-11 08:34:51.076381 renku-2.4.0rc1/renku/domain_model/__pycache__/template_LOCAL_2980914.cpython-38.pyc
+-rw-r--r--   0        0        0    18488 2023-04-11 08:34:51.086381 renku-2.4.0rc1/renku/domain_model/__pycache__/template_REMOTE_2980914.cpython-38.pyc
+-rw-r--r--   0        0        0     1092 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/constant.py
+-rw-r--r--   0        0        0    29605 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/dataset.py
+-rw-r--r--   0        0        0     1267 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/dataset_provider.py
+-rw-r--r--   0        0        0     2754 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/datastructures.py
+-rw-r--r--   0        0        0     2499 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/entity.py
+-rw-r--r--   0        0        0      971 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/enums.py
+-rw-r--r--   0        0        0     5059 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/git.py
+-rw-r--r--   0        0        0     8329 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/project.py
+-rw-r--r--   0        0        0    11817 2023-04-11 08:06:19.163068 renku-2.4.0rc1/renku/domain_model/project_context.py
+-rw-r--r--   0        0        0      829 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/provenance/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-06 07:28:51.151284 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      268 2023-02-27 08:58:18.141975 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      272 2023-04-11 08:09:11.348414 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    20304 2023-04-06 07:28:57.125112 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11627 2023-02-27 09:00:23.153576 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-37.pyc
+-rw-r--r--   0        0        0    11893 2023-04-11 08:09:11.988421 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-38.pyc
+-rw-r--r--   0        0        0     8011 2023-04-06 07:28:51.154617 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4939 2023-02-27 08:58:18.141975 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-37.pyc
+-rw-r--r--   0        0        0     4943 2023-04-11 08:09:11.351747 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-38.pyc
+-rw-r--r--   0        0        0     1429 2023-04-06 07:28:51.157951 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1059 2023-02-27 08:58:18.145309 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-37.pyc
+-rw-r--r--   0        0        0     1081 2023-04-11 08:09:11.355080 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-38.pyc
+-rw-r--r--   0        0        0     1829 2023-04-06 07:28:57.128446 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1344 2023-02-27 09:00:23.153576 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-37.pyc
+-rw-r--r--   0        0        0     1352 2023-04-11 08:09:11.988421 renku-2.4.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-38.pyc
+-rw-r--r--   0        0        0    13200 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/provenance/activity.py
+-rw-r--r--   0        0        0     5155 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/provenance/agent.py
+-rw-r--r--   0        0        0     1268 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/provenance/annotation.py
+-rw-r--r--   0        0        0     1530 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/provenance/parameter.py
+-rw-r--r--   0        0        0     6401 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/session.py
+-rw-r--r--   0        0        0     1471 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/sort.py
+-rw-r--r--   0        0        0    23890 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/domain_model/template.py
+-rw-r--r--   0        0        0      782 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/__init__.py
+-rw-r--r--   0        0        0      245 2023-04-06 07:28:54.341548 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      219 2023-02-27 09:00:22.540235 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      223 2023-04-11 08:09:11.701751 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    23682 2023-04-06 07:28:55.614987 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0    13434 2023-02-27 09:00:22.766905 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-37.pyc
+-rw-r--r--   0        0        0    13556 2023-04-11 08:09:11.791752 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-38.pyc
+-rw-r--r--   0        0        0    24869 2023-04-06 07:28:55.624988 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-311.pyc
+-rwxr-xr-x   0        0        0    16054 2023-02-27 09:00:22.773571 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-37.pyc
+-rw-r--r--   0        0        0    15337 2023-04-11 08:09:11.795086 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-38.pyc
+-rw-r--r--   0        0        0    26211 2023-04-06 07:28:55.638322 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0    15277 2023-02-27 09:00:22.776905 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-37.pyc
+-rw-r--r--   0        0        0    15127 2023-04-11 08:09:11.798419 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-38.pyc
+-rw-r--r--   0        0        0     1794 2023-04-06 07:28:54.344881 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1454 2023-02-27 09:00:22.540235 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1472 2023-04-11 08:09:11.701751 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-38.pyc
+-rw-r--r--   0        0        0     6759 2023-04-06 07:28:57.131780 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4623 2023-02-27 09:00:23.156910 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-37.pyc
+-rw-r--r--   0        0        0     4419 2023-04-11 08:09:11.988421 renku-2.4.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-38.pyc
+-rw-r--r--   0        0        0    15917 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/composite_plan.py
+-rw-r--r--   0        0        0     1531 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/converters/__init__.py
+-rw-r--r--   0        0        0     1718 2023-04-06 07:28:56.758415 renku-2.4.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1360 2023-02-27 09:00:23.086909 renku-2.4.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1380 2023-04-11 08:09:11.955088 renku-2.4.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    18124 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/parameter.py
+-rw-r--r--   0        0        0    16602 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/plan.py
+-rw-r--r--   0        0        0     1639 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/provider.py
+-rw-r--r--   0        0        0     4349 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/domain_model/workflow/workflow_file.py
+-rw-r--r--   0        0        0      780 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-06 07:28:50.304547 renku-2.4.0rc1/renku/infrastructure/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      197 2023-02-27 08:58:17.938639 renku-2.4.0rc1/renku/infrastructure/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      201 2023-04-11 08:06:12.289656 renku-2.4.0rc1/renku/infrastructure/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    58092 2023-04-06 08:18:06.624237 renku-2.4.0rc1/renku/infrastructure/__pycache__/database.cpython-311.pyc
+-rwxr-xr-x   0        0        0    34955 2023-02-27 09:00:22.866906 renku-2.4.0rc1/renku/infrastructure/__pycache__/database.cpython-37.pyc
+-rw-r--r--   0        0        0    34840 2023-04-11 09:49:33.589470 renku-2.4.0rc1/renku/infrastructure/__pycache__/database.cpython-38.pyc
+-rw-r--r--   0        0        0    23898 2023-04-06 07:29:10.796254 renku-2.4.0rc1/renku/infrastructure/__pycache__/git_merger.cpython-311.pyc
+-rwxr-xr-x   0        0        0    11914 2023-02-27 09:00:48.060560 renku-2.4.0rc1/renku/infrastructure/__pycache__/git_merger.cpython-37.pyc
+-rw-r--r--   0        0        0    11793 2023-04-11 08:06:20.459750 renku-2.4.0rc1/renku/infrastructure/__pycache__/git_merger.cpython-38.pyc
+-rw-r--r--   0        0        0     7871 2023-04-06 07:28:50.671244 renku-2.4.0rc1/renku/infrastructure/__pycache__/immutable.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4633 2023-02-27 08:58:18.038641 renku-2.4.0rc1/renku/infrastructure/__pycache__/immutable.cpython-37.pyc
+-rw-r--r--   0        0        0     5066 2023-04-11 08:09:11.285079 renku-2.4.0rc1/renku/infrastructure/__pycache__/immutable.cpython-38.pyc
+-rw-r--r--   0        0        0     3050 2023-04-06 07:28:51.317964 renku-2.4.0rc1/renku/infrastructure/__pycache__/persistent.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2224 2023-02-27 08:58:18.155309 renku-2.4.0rc1/renku/infrastructure/__pycache__/persistent.cpython-37.pyc
+-rw-r--r--   0        0        0     2248 2023-04-11 08:06:12.606326 renku-2.4.0rc1/renku/infrastructure/__pycache__/persistent.cpython-38.pyc
+-rw-r--r--   0        0        0   116870 2023-04-06 07:28:50.327882 renku-2.4.0rc1/renku/infrastructure/__pycache__/repository.cpython-311.pyc
+-rwxr-xr-x   0        0        0    66093 2023-02-27 09:49:25.260932 renku-2.4.0rc1/renku/infrastructure/__pycache__/repository.cpython-37.pyc
+-rw-r--r--   0        0        0    67930 2023-04-11 08:09:11.215078 renku-2.4.0rc1/renku/infrastructure/__pycache__/repository.cpython-38.pyc
+-rw-r--r--   0        0        0    40917 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/infrastructure/database.py
+-rw-r--r--   0        0        0      786 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/gateway/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-06 07:28:59.508644 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      211 2023-02-27 09:00:24.333591 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      215 2023-04-11 08:06:13.773007 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    19403 2023-04-06 07:29:02.062190 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/activity_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10627 2023-02-27 09:00:35.377065 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/activity_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0    11001 2023-04-11 08:06:14.959687 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/activity_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     8172 2023-04-06 12:11:00.160008 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/database_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5023 2023-02-27 09:00:35.380399 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/database_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     5057 2023-04-11 08:06:14.959687 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/database_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     5493 2023-04-06 07:28:59.511978 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3096 2023-02-27 09:00:24.336925 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     3248 2023-04-11 08:09:12.358425 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     6100 2023-04-06 07:29:06.242539 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/plan_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3075 2023-02-27 09:00:41.160472 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/plan_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     3678 2023-04-11 08:06:17.343047 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/plan_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1893 2023-04-06 07:29:06.245873 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/project_gateway.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1318 2023-02-27 09:00:41.163806 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/project_gateway.cpython-37.pyc
+-rw-r--r--   0        0        0     1336 2023-04-11 08:06:17.346381 renku-2.4.0rc1/renku/infrastructure/gateway/__pycache__/project_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0    12579 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/gateway/activity_gateway.py
+-rw-r--r--   0        0        0     5845 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/gateway/database_gateway.py
+-rw-r--r--   0        0        0     3743 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/infrastructure/gateway/dataset_gateway.py
+-rw-r--r--   0        0        0     3529 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/gateway/plan_gateway.py
+-rw-r--r--   0        0        0     1711 2023-04-11 08:06:10.286300 renku-2.4.0rc1/renku/infrastructure/gateway/project_gateway.py
+-rw-r--r--   0        0        0    18006 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/infrastructure/git_merger.py
+-rw-r--r--   0        0        0     4969 2023-04-11 08:06:19.166401 renku-2.4.0rc1/renku/infrastructure/immutable.py
+-rw-r--r--   0        0        0     2394 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/infrastructure/persistent.py
+-rw-r--r--   0        0        0    71947 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/infrastructure/repository.py
+-rw-r--r--   0        0        0      784 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/infrastructure/storage/__init__.py
+-rw-r--r--   0        0        0      235 2023-04-06 07:28:51.427973 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      209 2023-02-27 09:00:45.310525 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      213 2023-04-11 08:06:19.296403 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1846 2023-04-06 07:28:51.431307 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1723 2023-02-27 09:00:45.313858 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-37.pyc
+-rw-r--r--   0        0        0     1512 2023-04-11 08:06:19.296403 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-38.pyc
+-rw-r--r--   0        0        0    12022 2023-04-06 07:29:20.767093 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/rclone.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6180 2023-02-27 09:01:03.594091 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/rclone.cpython-37.pyc
+-rw-r--r--   0        0        0     7621 2023-04-11 08:06:26.506486 renku-2.4.0rc1/renku/infrastructure/storage/__pycache__/rclone.cpython-38.pyc
+-rw-r--r--   0        0        0     1989 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/infrastructure/storage/factory.py
+-rw-r--r--   0        0        0     8859 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/infrastructure/storage/rclone.py
+-rw-r--r--   0        0        0      913 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      553 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      637 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      523 2023-03-13 14:14:49.112087 renku-2.4.0rc1/renku/templates/.github/dependabot.yml
+-rw-r--r--   0        0        0      396 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/.github/workflows/github-project.yml
+-rw-r--r--   0        0        0     3940 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/.gitignore
+-rw-r--r--   0        0        0       27 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      984 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2087 2023-03-13 14:14:49.112087 renku-2.4.0rc1/renku/templates/R-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/environment.yml
+-rw-r--r--   0        0        0      360 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    14286 2023-03-13 14:14:49.105420 renku-2.4.0rc1/renku/templates/R-minimal.png
+-rw-r--r--   0        0        0     4846 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/README.md
+-rw-r--r--   0        0        0       27 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2077 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    44589 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/bioconductor.png
+-rw-r--r--   0        0        0       27 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       50 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2469 2023-03-13 14:14:49.112087 renku-2.4.0rc1/renku/templates/julia-minimal/Dockerfile
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/Manifest.toml
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/Project.toml
+-rw-r--r--   0        0        0     1842 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    13782 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/julialang.png
+-rw-r--r--   0        0        0     1174 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/manifest.yaml
+-rw-r--r--   0        0        0       17 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/.dockerignore
+-rw-r--r--   0        0        0       77 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2414 2023-03-13 14:14:49.112087 renku-2.4.0rc1/renku/templates/minimal/Dockerfile
+-rw-r--r--   0        0        0     1439 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0       27 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/.dockerignore
+-rw-r--r--   0        0        0     5401 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2159 2023-03-13 14:14:49.112087 renku-2.4.0rc1/renku/templates/python-minimal/Dockerfile
+-rw-r--r--   0        0        0     1597 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    25599 2023-03-13 14:14:49.108754 renku-2.4.0rc1/renku/templates/python-minimal.png
+-rw-r--r--   0        0        0      763 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-06 07:28:50.631240 renku-2.4.0rc1/renku/ui/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      169 2023-02-27 08:58:18.018640 renku-2.4.0rc1/renku/ui/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      173 2023-04-11 08:06:12.419658 renku-2.4.0rc1/renku/ui/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1268 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-06 07:29:02.068857 renku-2.4.0rc1/renku/ui/api/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      683 2023-02-27 09:00:35.387065 renku-2.4.0rc1/renku/ui/api/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      687 2023-04-11 08:06:14.963020 renku-2.4.0rc1/renku/ui/api/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2857 2023-04-06 07:29:02.278875 renku-2.4.0rc1/renku/ui/api/__pycache__/util.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2047 2023-02-27 09:00:35.517067 renku-2.4.0rc1/renku/ui/api/__pycache__/util.cpython-37.pyc
+-rw-r--r--   0        0        0     2060 2023-04-11 08:06:15.016354 renku-2.4.0rc1/renku/ui/api/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0        0        0      763 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/graph/__init__.py
+-rw-r--r--   0        0        0      204 2023-04-06 07:29:02.068857 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      178 2023-02-27 09:00:35.387065 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      182 2023-04-11 08:06:14.963020 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3219 2023-04-06 07:29:02.072191 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/rdf.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2176 2023-02-27 09:00:35.390399 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/rdf.cpython-37.pyc
+-rw-r--r--   0        0        0     2200 2023-04-11 08:06:14.963020 renku-2.4.0rc1/renku/ui/api/graph/__pycache__/rdf.cpython-38.pyc
+-rw-r--r--   0        0        0     2519 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/graph/rdf.py
+-rw-r--r--   0        0        0      764 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-06 07:29:02.268874 renku-2.4.0rc1/renku/ui/api/models/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      180 2023-02-27 09:00:35.503733 renku-2.4.0rc1/renku/ui/api/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      184 2023-04-11 08:06:15.009687 renku-2.4.0rc1/renku/ui/api/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    25232 2023-04-06 07:29:02.275541 renku-2.4.0rc1/renku/ui/api/models/__pycache__/activity.cpython-311.pyc
+-rwxr-xr-x   0        0        0    16264 2023-02-27 09:00:35.510400 renku-2.4.0rc1/renku/ui/api/models/__pycache__/activity.cpython-37.pyc
+-rw-r--r--   0        0        0    16263 2023-04-11 08:06:15.013021 renku-2.4.0rc1/renku/ui/api/models/__pycache__/activity.cpython-38.pyc
+-rw-r--r--   0        0        0     6237 2023-04-06 07:29:02.288876 renku-2.4.0rc1/renku/ui/api/models/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4453 2023-02-27 09:00:35.527067 renku-2.4.0rc1/renku/ui/api/models/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0     4505 2023-04-11 08:06:15.023021 renku-2.4.0rc1/renku/ui/api/models/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0    15229 2023-04-06 07:29:02.278875 renku-2.4.0rc1/renku/ui/api/models/__pycache__/parameter.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9641 2023-02-27 09:00:35.513734 renku-2.4.0rc1/renku/ui/api/models/__pycache__/parameter.cpython-37.pyc
+-rw-r--r--   0        0        0     9568 2023-04-11 08:06:15.016354 renku-2.4.0rc1/renku/ui/api/models/__pycache__/parameter.cpython-38.pyc
+-rw-r--r--   0        0        0    13448 2023-04-06 07:29:02.282208 renku-2.4.0rc1/renku/ui/api/models/__pycache__/plan.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9075 2023-02-27 09:00:35.520400 renku-2.4.0rc1/renku/ui/api/models/__pycache__/plan.cpython-37.pyc
+-rw-r--r--   0        0        0     8675 2023-04-11 08:06:15.019688 renku-2.4.0rc1/renku/ui/api/models/__pycache__/plan.cpython-38.pyc
+-rw-r--r--   0        0        0     4612 2023-04-06 07:29:02.292209 renku-2.4.0rc1/renku/ui/api/models/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3427 2023-02-27 09:00:35.530401 renku-2.4.0rc1/renku/ui/api/models/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     3455 2023-04-11 08:06:15.023021 renku-2.4.0rc1/renku/ui/api/models/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0    16448 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/activity.py
+-rw-r--r--   0        0        0     4648 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/dataset.py
+-rw-r--r--   0        0        0    10361 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/parameter.py
+-rw-r--r--   0        0        0     9227 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/plan.py
+-rw-r--r--   0        0        0     3643 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/models/project.py
+-rw-r--r--   0        0        0     2519 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/api/util.py
+-rw-r--r--   0        0        0     9319 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/cli/__init__.py
+-rw-r--r--   0        0        0      922 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/cli/__main__.py
+-rw-r--r--   0        0        0    12750 2023-04-06 07:28:50.631240 renku-2.4.0rc1/renku/ui/cli/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     8391 2023-02-27 08:58:18.018640 renku-2.4.0rc1/renku/ui/cli/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     8163 2023-04-11 08:06:12.422991 renku-2.4.0rc1/renku/ui/cli/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-06 08:20:51.194809 renku-2.4.0rc1/renku/ui/cli/__pycache__/__main__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      328 2023-02-27 09:02:40.468652 renku-2.4.0rc1/renku/ui/cli/__pycache__/__main__.cpython-37.pyc
+-rw-r--r--   0        0        0      332 2023-04-03 09:47:23.351495 renku-2.4.0rc1/renku/ui/cli/__pycache__/__main__.cpython-38.pyc
+-rw-r--r--   0        0        0     2765 2023-04-06 07:28:50.637908 renku-2.4.0rc1/renku/ui/cli/__pycache__/clone.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2094 2023-02-27 08:58:18.025307 renku-2.4.0rc1/renku/ui/cli/__pycache__/clone.cpython-37.pyc
+-rw-r--r--   0        0        0     2114 2023-04-11 08:06:12.426324 renku-2.4.0rc1/renku/ui/cli/__pycache__/clone.cpython-38.pyc
+-rw-r--r--   0        0        0     8393 2023-04-06 07:28:50.641241 renku-2.4.0rc1/renku/ui/cli/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6700 2023-02-27 08:58:18.028640 renku-2.4.0rc1/renku/ui/cli/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     6678 2023-04-11 08:06:12.429658 renku-2.4.0rc1/renku/ui/cli/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0    56371 2023-04-06 07:28:50.651242 renku-2.4.0rc1/renku/ui/cli/__pycache__/dataset.cpython-311.pyc
+-rwxr-xr-x   0        0        0    36960 2023-02-27 08:58:18.031974 renku-2.4.0rc1/renku/ui/cli/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0        0        0    36606 2023-04-11 08:09:11.278413 renku-2.4.0rc1/renku/ui/cli/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     2691 2023-04-06 07:28:59.195284 renku-2.4.0rc1/renku/ui/cli/__pycache__/doctor.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1677 2023-02-27 09:00:23.833585 renku-2.4.0rc1/renku/ui/cli/__pycache__/doctor.cpython-37.pyc
+-rw-r--r--   0        0        0     1687 2023-04-11 08:42:57.752426 renku-2.4.0rc1/renku/ui/cli/__pycache__/doctor.cpython-38.pyc
+-rw-r--r--   0        0        0     1568 2023-04-06 07:28:59.195284 renku-2.4.0rc1/renku/ui/cli/__pycache__/env.cpython-311.pyc
+-rwxr-xr-x   0        0        0      943 2023-02-27 09:00:23.836918 renku-2.4.0rc1/renku/ui/cli/__pycache__/env.cpython-37.pyc
+-rw-r--r--   0        0        0      953 2023-04-11 08:06:13.609671 renku-2.4.0rc1/renku/ui/cli/__pycache__/env.cpython-38.pyc
+-rw-r--r--   0        0        0    12453 2023-04-06 07:28:59.198618 renku-2.4.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7790 2023-02-27 09:00:23.836918 renku-2.4.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-37.pyc
+-rw-r--r--   0        0        0     7905 2023-04-11 08:06:13.613005 renku-2.4.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-38.pyc
+-rw-r--r--   0        0        0      871 2023-04-06 07:28:59.218620 renku-2.4.0rc1/renku/ui/cli/__pycache__/gc.cpython-311.pyc
+-rwxr-xr-x   0        0        0      626 2023-02-27 09:00:23.850252 renku-2.4.0rc1/renku/ui/cli/__pycache__/gc.cpython-37.pyc
+-rw-r--r--   0        0        0      634 2023-04-11 08:06:13.619671 renku-2.4.0rc1/renku/ui/cli/__pycache__/gc.cpython-38.pyc
+-rw-r--r--   0        0        0     3221 2023-04-06 07:28:59.221953 renku-2.4.0rc1/renku/ui/cli/__pycache__/githooks.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2143 2023-02-27 09:00:23.850252 renku-2.4.0rc1/renku/ui/cli/__pycache__/githooks.cpython-37.pyc
+-rw-r--r--   0        0        0     2157 2023-04-11 08:06:13.619671 renku-2.4.0rc1/renku/ui/cli/__pycache__/githooks.cpython-38.pyc
+-rw-r--r--   0        0        0     5534 2023-04-06 07:28:59.221953 renku-2.4.0rc1/renku/ui/cli/__pycache__/graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4004 2023-02-27 09:00:23.853585 renku-2.4.0rc1/renku/ui/cli/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0        0        0     4040 2023-04-11 08:06:13.619671 renku-2.4.0rc1/renku/ui/cli/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0    12403 2023-04-06 07:28:59.225287 renku-2.4.0rc1/renku/ui/cli/__pycache__/init.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9590 2023-02-27 09:00:23.853585 renku-2.4.0rc1/renku/ui/cli/__pycache__/init.cpython-37.pyc
+-rw-r--r--   0        0        0     9631 2023-04-11 08:06:13.623005 renku-2.4.0rc1/renku/ui/cli/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0    14269 2023-04-06 07:28:59.228621 renku-2.4.0rc1/renku/ui/cli/__pycache__/log.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7250 2023-02-27 09:00:23.856918 renku-2.4.0rc1/renku/ui/cli/__pycache__/log.cpython-37.pyc
+-rw-r--r--   0        0        0     7303 2023-04-11 08:06:13.626338 renku-2.4.0rc1/renku/ui/cli/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0        0        0     5781 2023-04-06 07:28:59.245289 renku-2.4.0rc1/renku/ui/cli/__pycache__/login.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4265 2023-02-27 09:00:23.870252 renku-2.4.0rc1/renku/ui/cli/__pycache__/login.cpython-37.pyc
+-rw-r--r--   0        0        0     4285 2023-04-11 08:06:13.633005 renku-2.4.0rc1/renku/ui/cli/__pycache__/login.cpython-38.pyc
+-rw-r--r--   0        0        0     3104 2023-04-06 07:28:59.291959 renku-2.4.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2035 2023-02-27 09:00:23.886919 renku-2.4.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-37.pyc
+-rw-r--r--   0        0        0     2055 2023-04-11 08:06:13.646338 renku-2.4.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-38.pyc
+-rw-r--r--   0        0        0     6837 2023-04-06 07:28:59.295293 renku-2.4.0rc1/renku/ui/cli/__pycache__/migrate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4376 2023-02-27 09:00:23.890252 renku-2.4.0rc1/renku/ui/cli/__pycache__/migrate.cpython-37.pyc
+-rw-r--r--   0        0        0     4432 2023-04-11 08:42:57.765759 renku-2.4.0rc1/renku/ui/cli/__pycache__/migrate.cpython-38.pyc
+-rw-r--r--   0        0        0     3054 2023-04-06 07:28:59.295293 renku-2.4.0rc1/renku/ui/cli/__pycache__/move.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2283 2023-02-27 09:00:23.890252 renku-2.4.0rc1/renku/ui/cli/__pycache__/move.cpython-37.pyc
+-rw-r--r--   0        0        0     2303 2023-04-11 08:06:13.646338 renku-2.4.0rc1/renku/ui/cli/__pycache__/move.cpython-38.pyc
+-rw-r--r--   0        0        0     8135 2023-04-06 07:28:59.298627 renku-2.4.0rc1/renku/ui/cli/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3961 2023-02-27 09:00:23.893586 renku-2.4.0rc1/renku/ui/cli/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     4026 2023-04-11 08:09:12.261758 renku-2.4.0rc1/renku/ui/cli/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     1748 2023-04-06 07:28:59.298627 renku-2.4.0rc1/renku/ui/cli/__pycache__/remove.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1262 2023-02-27 09:00:23.896919 renku-2.4.0rc1/renku/ui/cli/__pycache__/remove.cpython-37.pyc
+-rw-r--r--   0        0        0     1272 2023-04-11 08:06:13.649672 renku-2.4.0rc1/renku/ui/cli/__pycache__/remove.cpython-38.pyc
+-rw-r--r--   0        0        0     4672 2023-04-06 07:28:59.301960 renku-2.4.0rc1/renku/ui/cli/__pycache__/rerun.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3454 2023-02-27 09:00:23.896919 renku-2.4.0rc1/renku/ui/cli/__pycache__/rerun.cpython-37.pyc
+-rw-r--r--   0        0        0     3492 2023-04-11 08:06:13.649672 renku-2.4.0rc1/renku/ui/cli/__pycache__/rerun.cpython-38.pyc
+-rw-r--r--   0        0        0     3123 2023-04-06 07:28:59.305294 renku-2.4.0rc1/renku/ui/cli/__pycache__/rollback.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2740 2023-02-27 09:00:23.900252 renku-2.4.0rc1/renku/ui/cli/__pycache__/rollback.cpython-37.pyc
+-rw-r--r--   0        0        0     2750 2023-04-11 08:06:13.653005 renku-2.4.0rc1/renku/ui/cli/__pycache__/rollback.cpython-38.pyc
+-rw-r--r--   0        0        0    27249 2023-04-06 07:28:59.308627 renku-2.4.0rc1/renku/ui/cli/__pycache__/run.cpython-311.pyc
+-rwxr-xr-x   0        0        0    23569 2023-02-27 09:00:23.903586 renku-2.4.0rc1/renku/ui/cli/__pycache__/run.cpython-37.pyc
+-rw-r--r--   0        0        0    23649 2023-04-11 08:09:12.265091 renku-2.4.0rc1/renku/ui/cli/__pycache__/run.cpython-38.pyc
+-rw-r--r--   0        0        0     3770 2023-04-06 07:28:59.331962 renku-2.4.0rc1/renku/ui/cli/__pycache__/save.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2861 2023-02-27 09:00:23.923586 renku-2.4.0rc1/renku/ui/cli/__pycache__/save.cpython-37.pyc
+-rw-r--r--   0        0        0     2883 2023-04-11 08:06:13.666339 renku-2.4.0rc1/renku/ui/cli/__pycache__/save.cpython-38.pyc
+-rw-r--r--   0        0        0    18748 2023-04-06 07:28:59.335296 renku-2.4.0rc1/renku/ui/cli/__pycache__/service.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10161 2023-02-27 09:00:23.926919 renku-2.4.0rc1/renku/ui/cli/__pycache__/service.cpython-37.pyc
+-rw-r--r--   0        0        0    10269 2023-04-11 08:42:57.779093 renku-2.4.0rc1/renku/ui/cli/__pycache__/service.cpython-38.pyc
+-rw-r--r--   0        0        0    16552 2023-04-06 07:28:59.338630 renku-2.4.0rc1/renku/ui/cli/__pycache__/session.cpython-311.pyc
+-rwxr-xr-x   0        0        0    12056 2023-02-27 09:00:23.930253 renku-2.4.0rc1/renku/ui/cli/__pycache__/session.cpython-37.pyc
+-rw-r--r--   0        0        0    12173 2023-04-11 08:09:12.271758 renku-2.4.0rc1/renku/ui/cli/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     6915 2023-04-06 07:28:59.345297 renku-2.4.0rc1/renku/ui/cli/__pycache__/status.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3698 2023-02-27 09:00:23.936920 renku-2.4.0rc1/renku/ui/cli/__pycache__/status.cpython-37.pyc
+-rw-r--r--   0        0        0     3704 2023-04-11 08:06:13.676339 renku-2.4.0rc1/renku/ui/cli/__pycache__/status.cpython-38.pyc
+-rw-r--r--   0        0        0     7891 2023-04-06 07:28:59.348631 renku-2.4.0rc1/renku/ui/cli/__pycache__/storage.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5017 2023-02-27 09:00:23.940253 renku-2.4.0rc1/renku/ui/cli/__pycache__/storage.cpython-37.pyc
+-rw-r--r--   0        0        0     5050 2023-04-11 08:06:13.676339 renku-2.4.0rc1/renku/ui/cli/__pycache__/storage.cpython-38.pyc
+-rw-r--r--   0        0        0    18073 2023-04-06 07:28:59.351964 renku-2.4.0rc1/renku/ui/cli/__pycache__/template.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10839 2023-02-27 09:00:23.943586 renku-2.4.0rc1/renku/ui/cli/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0        0        0    10959 2023-04-11 09:49:33.936140 renku-2.4.0rc1/renku/ui/cli/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0        0        0     7130 2023-04-06 07:28:59.355298 renku-2.4.0rc1/renku/ui/cli/__pycache__/update.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5533 2023-02-27 09:00:23.946920 renku-2.4.0rc1/renku/ui/cli/__pycache__/update.cpython-37.pyc
+-rw-r--r--   0        0        0     5789 2023-04-11 08:06:13.679672 renku-2.4.0rc1/renku/ui/cli/__pycache__/update.cpython-38.pyc
+-rw-r--r--   0        0        0    55844 2023-04-06 07:28:59.361965 renku-2.4.0rc1/renku/ui/cli/__pycache__/workflow.cpython-311.pyc
+-rwxr-xr-x   0        0        0    41076 2023-02-27 09:00:23.950253 renku-2.4.0rc1/renku/ui/cli/__pycache__/workflow.cpython-37.pyc
+-rw-r--r--   0        0        0    42016 2023-04-11 08:09:12.278425 renku-2.4.0rc1/renku/ui/cli/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0        0        0     2594 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/cli/clone.py
+-rw-r--r--   0        0        0     7613 2023-04-11 08:06:10.289633 renku-2.4.0rc1/renku/ui/cli/config.py
+-rw-r--r--   0        0        0    42970 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/dataset.py
+-rw-r--r--   0        0        0     2217 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/cli/doctor.py
+-rw-r--r--   0        0        0     1600 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/env.py
+-rw-r--r--   0        0        0     7931 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/exception_handler.py
+-rw-r--r--   0        0        0     1139 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/gc.py
+-rw-r--r--   0        0        0     2538 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/githooks.py
+-rw-r--r--   0        0        0     4950 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/graph.py
+-rw-r--r--   0        0        0    11113 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/init.py
+-rw-r--r--   0        0        0     8581 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/log.py
+-rw-r--r--   0        0        0     4845 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/login.py
+-rw-r--r--   0        0        0     2499 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/mergetool.py
+-rw-r--r--   0        0        0     5689 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/cli/migrate.py
+-rw-r--r--   0        0        0     2881 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/move.py
+-rw-r--r--   0        0        0     5768 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/project.py
+-rw-r--r--   0        0        0     1754 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/remove.py
+-rw-r--r--   0        0        0     4227 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/rerun.py
+-rw-r--r--   0        0        0     3249 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/rollback.py
+-rw-r--r--   0        0        0    26417 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/run.py
+-rw-r--r--   0        0        0     3510 2023-04-11 08:06:10.292967 renku-2.4.0rc1/renku/ui/cli/save.py
+-rw-r--r--   0        0        0    11830 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/cli/service.py
+-rw-r--r--   0        0        0    13742 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/session.py
+-rw-r--r--   0        0        0     5489 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/status.py
+-rw-r--r--   0        0        0     5604 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/storage.py
+-rw-r--r--   0        0        0    13434 2023-04-11 08:43:02.649191 renku-2.4.0rc1/renku/ui/cli/template.py
+-rw-r--r--   0        0        0     6723 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/update.py
+-rw-r--r--   0        0        0      768 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-06 07:28:50.641241 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      188 2023-02-27 08:58:18.025307 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      192 2023-04-11 08:06:12.426324 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10451 2023-04-06 07:28:59.245289 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5478 2023-02-27 09:00:23.870252 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-37.pyc
+-rw-r--r--   0        0        0     5425 2023-04-11 08:06:13.636338 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-38.pyc
+-rw-r--r--   0        0        0     5836 2023-04-06 07:28:50.644575 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3420 2023-02-27 08:58:18.028640 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-37.pyc
+-rw-r--r--   0        0        0     3426 2023-04-11 08:09:11.275079 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-38.pyc
+-rw-r--r--   0        0        0      325 2023-04-06 07:28:50.641241 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/color.cpython-311.pyc
+-rwxr-xr-x   0        0        0      286 2023-02-27 08:58:18.025307 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/color.cpython-37.pyc
+-rw-r--r--   0        0        0      290 2023-04-11 08:06:12.429658 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/color.cpython-38.pyc
+-rw-r--r--   0        0        0    21688 2023-04-06 07:29:21.417148 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/curses.cpython-311.pyc
+-rwxr-xr-x   0        0        0    10930 2023-02-27 09:01:05.814119 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/curses.cpython-37.pyc
+-rw-r--r--   0        0        0    10994 2023-04-11 08:06:26.943157 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/curses.cpython-38.pyc
+-rw-r--r--   0        0        0     1237 2023-04-06 07:28:59.301960 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1041 2023-02-27 09:00:23.896919 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-37.pyc
+-rw-r--r--   0        0        0      991 2023-04-11 08:06:13.649672 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-38.pyc
+-rw-r--r--   0        0        0    14600 2023-04-06 07:28:59.241955 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7459 2023-02-27 09:00:23.866919 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-37.pyc
+-rw-r--r--   0        0        0     7382 2023-04-11 08:06:13.633005 renku-2.4.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-38.pyc
+-rw-r--r--   0        0        0     5422 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/callback.py
+-rw-r--r--   0        0        0     3982 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/utils/click.py
+-rw-r--r--   0        0        0      855 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/color.py
+-rw-r--r--   0        0        0    14534 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/curses.py
+-rw-r--r--   0        0        0     1387 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/plugins.py
+-rw-r--r--   0        0        0     9929 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/cli/utils/terminal.py
+-rw-r--r--   0        0        0    48023 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/cli/workflow.py
+-rw-r--r--   0        0        0      843 2023-03-02 15:15:40.049932 renku-2.4.0rc1/renku/ui/service/.env-example
+-rw-r--r--   0        0        0      756 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/__init__.py
+-rw-r--r--   0        0        0      200 2023-04-06 07:28:59.198618 renku-2.4.0rc1/renku/ui/service/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      174 2023-02-27 09:00:23.840252 renku-2.4.0rc1/renku/ui/service/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      178 2023-04-11 08:06:13.613005 renku-2.4.0rc1/renku/ui/service/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3362 2023-04-06 07:28:59.201952 renku-2.4.0rc1/renku/ui/service/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1975 2023-02-27 09:00:23.840252 renku-2.4.0rc1/renku/ui/service/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     1981 2023-04-11 08:06:13.613005 renku-2.4.0rc1/renku/ui/service/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     8565 2023-04-06 07:29:21.573828 renku-2.4.0rc1/renku/ui/service/__pycache__/entrypoint.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5020 2023-02-27 09:01:06.120790 renku-2.4.0rc1/renku/ui/service/__pycache__/entrypoint.cpython-37.pyc
+-rw-r--r--   0        0        0     5045 2023-04-11 08:06:27.026491 renku-2.4.0rc1/renku/ui/service/__pycache__/entrypoint.cpython-38.pyc
+-rw-r--r--   0        0        0    45022 2023-04-06 07:29:13.796506 renku-2.4.0rc1/renku/ui/service/__pycache__/errors.cpython-311.pyc
+-rwxr-xr-x   0        0        0    34448 2023-02-27 09:00:51.183933 renku-2.4.0rc1/renku/ui/service/__pycache__/errors.cpython-37.pyc
+-rw-r--r--   0        0        0    31516 2023-04-11 08:06:21.996434 renku-2.4.0rc1/renku/ui/service/__pycache__/errors.cpython-38.pyc
+-rw-r--r--   0        0        0      981 2023-04-06 07:29:14.189872 renku-2.4.0rc1/renku/ui/service/__pycache__/logger.cpython-311.pyc
+-rwxr-xr-x   0        0        0      616 2023-02-27 09:00:51.363935 renku-2.4.0rc1/renku/ui/service/__pycache__/logger.cpython-37.pyc
+-rw-r--r--   0        0        0      622 2023-04-11 08:06:22.136436 renku-2.4.0rc1/renku/ui/service/__pycache__/logger.cpython-38.pyc
+-rw-r--r--   0        0        0     3003 2023-04-06 07:29:22.180546 renku-2.4.0rc1/renku/ui/service/__pycache__/scheduler.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1660 2023-02-27 09:01:06.560795 renku-2.4.0rc1/renku/ui/service/__pycache__/scheduler.cpython-37.pyc
+-rw-r--r--   0        0        0     1672 2023-04-11 08:06:27.113159 renku-2.4.0rc1/renku/ui/service/__pycache__/scheduler.cpython-38.pyc
+-rw-r--r--   0        0        0     4191 2023-04-06 07:29:22.200548 renku-2.4.0rc1/renku/ui/service/__pycache__/worker.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2457 2023-02-27 09:01:06.577462 renku-2.4.0rc1/renku/ui/service/__pycache__/worker.cpython-37.pyc
+-rw-r--r--   0        0        0     2471 2023-04-11 08:06:27.119826 renku-2.4.0rc1/renku/ui/service/__pycache__/worker.cpython-38.pyc
+-rw-r--r--   0        0        0     1535 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/__init__.py
+-rw-r--r--   0        0        0     1431 2023-04-06 07:29:13.833176 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1062 2023-02-27 09:00:51.217267 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1070 2023-04-11 08:06:22.033101 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4358 2023-04-06 07:29:13.836509 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/base.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2793 2023-02-27 09:00:51.220600 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0        0        0     2831 2023-04-11 08:06:22.036434 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0      939 2023-04-06 07:29:14.023192 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0      533 2023-02-27 09:00:51.267267 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0      537 2023-04-11 08:06:22.069768 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     5290 2023-04-06 07:29:13.833176 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/files.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3284 2023-02-27 09:00:51.217267 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/files.cpython-37.pyc
+-rw-r--r--   0        0        0     3282 2023-04-11 08:06:22.033101 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/files.cpython-38.pyc
+-rw-r--r--   0        0        0     2965 2023-04-06 07:29:14.159870 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/jobs.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1765 2023-02-27 09:00:51.343935 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/jobs.cpython-37.pyc
+-rw-r--r--   0        0        0     1785 2023-04-11 08:06:22.123102 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/jobs.cpython-38.pyc
+-rw-r--r--   0        0        0     3472 2023-04-06 07:29:14.179872 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/projects.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2190 2023-02-27 09:00:51.357269 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/projects.cpython-37.pyc
+-rw-r--r--   0        0        0     2220 2023-04-11 08:06:22.133102 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/projects.cpython-38.pyc
+-rw-r--r--   0        0        0     2044 2023-04-06 07:29:14.186539 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/users.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1330 2023-02-27 09:00:51.360602 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/users.cpython-37.pyc
+-rw-r--r--   0        0        0     1356 2023-04-11 08:06:22.133102 renku-2.4.0rc1/renku/ui/service/cache/__pycache__/users.cpython-38.pyc
+-rw-r--r--   0        0        0     2917 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/base.py
+-rw-r--r--   0        0        0     1168 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/config.py
+-rw-r--r--   0        0        0     3315 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/files.py
+-rw-r--r--   0        0        0     2333 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/jobs.py
+-rw-r--r--   0        0        0      769 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/models/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-06 07:29:14.026525 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      200 2023-02-27 09:00:51.270601 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      204 2023-04-11 08:06:22.073101 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5933 2023-04-06 07:29:14.026525 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3793 2023-02-27 09:00:51.270601 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/file.cpython-37.pyc
+-rw-r--r--   0        0        0     3605 2023-04-11 08:06:22.076435 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/file.cpython-38.pyc
+-rw-r--r--   0        0        0     2720 2023-04-06 07:29:14.163204 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/job.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1817 2023-02-27 09:00:51.347268 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/job.cpython-37.pyc
+-rw-r--r--   0        0        0     1839 2023-04-11 08:06:22.123102 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/job.cpython-38.pyc
+-rw-r--r--   0        0        0     5901 2023-04-06 07:29:14.163204 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3776 2023-02-27 09:00:51.347268 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     3825 2023-04-11 08:06:22.123102 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0      952 2023-04-06 07:29:14.029859 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/user.cpython-311.pyc
+-rwxr-xr-x   0        0        0      678 2023-02-27 09:00:51.270601 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/user.cpython-37.pyc
+-rw-r--r--   0        0        0      686 2023-04-11 08:06:22.076435 renku-2.4.0rc1/renku/ui/service/cache/models/__pycache__/user.cpython-38.pyc
+-rw-r--r--   0        0        0     4356 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/models/file.py
+-rw-r--r--   0        0        0     2273 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/models/job.py
+-rw-r--r--   0        0        0     4043 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/models/project.py
+-rw-r--r--   0        0        0     1127 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/models/user.py
+-rw-r--r--   0        0        0     2558 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/projects.py
+-rw-r--r--   0        0        0      774 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/serializers/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-06 07:29:14.029859 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      210 2023-02-27 09:00:51.273934 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      214 2023-04-11 08:06:22.076435 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2288 2023-04-06 07:29:14.029859 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1637 2023-02-27 09:00:51.273934 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/file.cpython-37.pyc
+-rw-r--r--   0        0        0     1615 2023-04-11 08:06:22.079768 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/file.cpython-38.pyc
+-rw-r--r--   0        0        0     2011 2023-04-06 07:29:14.179872 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/job.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1313 2023-02-27 09:00:51.353935 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/job.cpython-37.pyc
+-rw-r--r--   0        0        0     1331 2023-04-11 08:06:22.129769 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/job.cpython-38.pyc
+-rw-r--r--   0        0        0     2217 2023-04-06 07:29:14.183205 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1410 2023-02-27 09:00:51.360602 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     1426 2023-04-11 08:06:22.133102 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     1189 2023-04-06 07:29:14.186539 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/user.cpython-311.pyc
+-rwxr-xr-x   0        0        0      849 2023-02-27 09:00:51.360602 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/user.cpython-37.pyc
+-rw-r--r--   0        0        0      861 2023-04-11 08:06:22.136436 renku-2.4.0rc1/renku/ui/service/cache/serializers/__pycache__/user.cpython-38.pyc
+-rw-r--r--   0        0        0     1821 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/serializers/file.py
+-rw-r--r--   0        0        0     1711 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/serializers/job.py
+-rw-r--r--   0        0        0     1812 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/serializers/project.py
+-rw-r--r--   0        0        0     1227 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/serializers/user.py
+-rw-r--r--   0        0        0     1657 2023-04-11 08:06:10.296300 renku-2.4.0rc1/renku/ui/service/cache/users.py
+-rw-r--r--   0        0        0     2931 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/config.py
+-rw-r--r--   0        0        0      773 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-06 07:29:13.829842 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      198 2023-02-27 09:00:51.213933 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      202 2023-04-11 08:06:22.029768 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3314 2023-04-06 07:29:21.750510 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_delete_chunks.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2304 2023-02-27 09:01:06.187457 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_delete_chunks.cpython-37.pyc
+-rw-r--r--   0        0        0     2324 2023-04-11 08:06:27.056492 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_delete_chunks.cpython-38.pyc
+-rw-r--r--   0        0        0    10557 2023-04-06 07:29:21.760510 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_upload.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5359 2023-02-27 09:01:06.200791 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_upload.cpython-37.pyc
+-rw-r--r--   0        0        0     5377 2023-04-11 08:06:27.066492 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_files_upload.cpython-38.pyc
+-rw-r--r--   0        0        0     3505 2023-04-06 07:29:21.760510 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_projects.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2472 2023-02-27 09:01:06.204124 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_projects.cpython-37.pyc
+-rw-r--r--   0        0        0     2515 2023-04-11 08:06:27.479830 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_projects.cpython-38.pyc
+-rw-r--r--   0        0        0     2835 2023-04-06 07:29:21.763844 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_uploaded.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2037 2023-02-27 09:01:06.204124 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_uploaded.cpython-37.pyc
+-rw-r--r--   0        0        0     2062 2023-04-11 08:06:27.479830 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_list_uploaded.cpython-38.pyc
+-rw-r--r--   0        0        0     5474 2023-04-06 07:29:21.763844 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrate_project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3417 2023-02-27 09:01:06.207457 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrate_project.cpython-37.pyc
+-rw-r--r--   0        0        0     3454 2023-04-11 08:06:27.483163 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrate_project.cpython-38.pyc
+-rw-r--r--   0        0        0     6086 2023-04-06 07:29:21.767178 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3871 2023-02-27 09:01:06.210791 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check.cpython-37.pyc
+-rw-r--r--   0        0        0     3941 2023-04-11 08:43:03.872550 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check.cpython-38.pyc
+-rw-r--r--   0        0        0     3954 2023-04-03 09:33:50.747296 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check_BASE_1830740.cpython-38.pyc
+-rw-r--r--   0        0        0     3634 2023-04-03 09:33:50.750629 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check_LOCAL_1830740.cpython-38.pyc
+-rw-r--r--   0        0        0     4145 2023-04-03 09:33:50.750629 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_migrations_check_REMOTE_1830740.cpython-38.pyc
+-rw-r--r--   0        0        0     2982 2023-04-06 07:29:21.770511 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_project_clone.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2074 2023-02-27 09:01:06.214124 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_project_clone.cpython-37.pyc
+-rw-r--r--   0        0        0     2092 2023-04-11 08:06:27.489830 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/cache_project_clone.cpython-38.pyc
+-rw-r--r--   0        0        0     3483 2023-04-06 07:29:21.827183 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_set.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2249 2023-02-27 09:01:06.257458 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_set.cpython-37.pyc
+-rw-r--r--   0        0        0     2269 2023-04-11 08:06:27.493163 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_set.cpython-38.pyc
+-rw-r--r--   0        0        0     2962 2023-04-06 07:29:21.830516 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_show.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2007 2023-02-27 09:01:06.260791 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_show.cpython-37.pyc
+-rw-r--r--   0        0        0     2025 2023-04-11 08:06:27.496497 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/config_show.cpython-38.pyc
+-rw-r--r--   0        0        0     6809 2023-04-06 07:29:21.833850 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_add_file.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3943 2023-02-27 09:01:06.264125 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_add_file.cpython-37.pyc
+-rw-r--r--   0        0        0     3967 2023-04-11 08:06:27.499830 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_add_file.cpython-38.pyc
+-rw-r--r--   0        0        0     5128 2023-04-06 07:29:21.837184 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_create.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3130 2023-02-27 09:01:06.267458 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_create.cpython-37.pyc
+-rw-r--r--   0        0        0     3172 2023-04-11 08:06:27.516497 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_create.cpython-38.pyc
+-rw-r--r--   0        0        0     6247 2023-04-06 07:29:21.840517 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_edit.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3715 2023-02-27 09:01:06.270791 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_edit.cpython-37.pyc
+-rw-r--r--   0        0        0     3766 2023-04-11 08:06:27.526497 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_edit.cpython-38.pyc
+-rw-r--r--   0        0        0     2776 2023-04-06 07:29:21.843851 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_files_list.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1911 2023-02-27 09:01:06.270791 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_files_list.cpython-37.pyc
+-rw-r--r--   0        0        0     1929 2023-04-11 08:06:27.536497 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_files_list.cpython-38.pyc
+-rw-r--r--   0        0        0     4346 2023-04-06 07:29:21.847185 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_import.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2643 2023-02-27 09:01:06.274125 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_import.cpython-37.pyc
+-rw-r--r--   0        0        0     2665 2023-04-11 08:06:27.549831 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_import.cpython-38.pyc
+-rw-r--r--   0        0        0     2662 2023-04-06 07:29:21.847185 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_list.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1828 2023-02-27 09:01:06.274125 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_list.cpython-37.pyc
+-rw-r--r--   0        0        0     1846 2023-04-11 08:06:27.563164 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_list.cpython-38.pyc
+-rw-r--r--   0        0        0     3427 2023-04-06 07:29:21.847185 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_remove.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2253 2023-02-27 09:01:06.277458 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_remove.cpython-37.pyc
+-rw-r--r--   0        0        0     2275 2023-04-11 08:06:27.573164 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_remove.cpython-38.pyc
+-rw-r--r--   0        0        0     4388 2023-04-06 07:29:21.850518 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_unlink.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2738 2023-02-27 09:01:06.277458 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_unlink.cpython-37.pyc
+-rw-r--r--   0        0        0     2772 2023-04-11 08:06:27.583165 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/datasets_unlink.cpython-38.pyc
+-rw-r--r--   0        0        0     7200 2023-04-06 07:29:21.853852 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/graph_export.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4289 2023-02-27 09:01:06.280792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/graph_export.cpython-37.pyc
+-rw-r--r--   0        0        0     4249 2023-04-11 08:43:03.892550 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/graph_export.cpython-38.pyc
+-rw-r--r--   0        0        0     4451 2023-04-06 07:29:21.867186 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_edit.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2678 2023-02-27 09:01:06.290792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_edit.cpython-37.pyc
+-rw-r--r--   0        0        0     2717 2023-04-11 08:06:27.599831 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_edit.cpython-38.pyc
+-rw-r--r--   0        0        0     4266 2023-04-06 07:29:21.873853 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_lock_status.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2688 2023-02-27 09:01:06.297459 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_lock_status.cpython-37.pyc
+-rw-r--r--   0        0        0     2734 2023-04-11 08:06:27.603165 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_lock_status.cpython-38.pyc
+-rw-r--r--   0        0        0     2652 2023-04-06 07:29:21.877187 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_show.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1829 2023-02-27 09:01:06.300792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_show.cpython-37.pyc
+-rw-r--r--   0        0        0     1846 2023-04-11 08:06:27.606498 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/project_show.cpython-38.pyc
+-rw-r--r--   0        0        0    10668 2023-04-06 07:29:21.880520 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_create_project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6564 2023-02-27 09:01:06.304125 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_create_project.cpython-37.pyc
+-rw-r--r--   0        0        0     6726 2023-04-11 08:06:27.609831 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_create_project.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-04-06 07:29:21.883854 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_read_manifest.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2673 2023-02-27 09:01:06.307458 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_read_manifest.cpython-37.pyc
+-rw-r--r--   0        0        0     2689 2023-04-11 08:06:27.613165 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/templates_read_manifest.cpython-38.pyc
+-rw-r--r--   0        0        0     1465 2023-04-06 07:29:21.890521 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/version.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1111 2023-02-27 09:01:06.310792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/version.cpython-37.pyc
+-rw-r--r--   0        0        0     1127 2023-04-11 08:06:27.616498 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0     2935 2023-04-06 07:29:21.893855 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_export.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2033 2023-02-27 09:01:06.314125 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_export.cpython-37.pyc
+-rw-r--r--   0        0        0     2050 2023-04-11 08:06:27.619831 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_export.cpython-38.pyc
+-rw-r--r--   0        0        0     3019 2023-04-06 07:29:21.913857 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_list.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2021 2023-02-27 09:01:06.330792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_list.cpython-37.pyc
+-rw-r--r--   0        0        0     2039 2023-04-11 08:06:27.629832 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_list.cpython-38.pyc
+-rw-r--r--   0        0        0     2752 2023-04-06 07:29:21.917190 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_show.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1917 2023-02-27 09:01:06.330792 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_show.cpython-37.pyc
+-rw-r--r--   0        0        0     1930 2023-04-11 08:06:27.633165 renku-2.4.0rc1/renku/ui/service/controllers/__pycache__/workflow_plans_show.cpython-38.pyc
+-rw-r--r--   0        0        0      777 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/api/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-06 07:29:21.750510 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      206 2023-02-27 09:01:06.187457 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      210 2023-04-11 08:06:27.059825 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      960 2023-04-06 07:29:21.750510 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/abstract.cpython-311.pyc
+-rwxr-xr-x   0        0        0      802 2023-02-27 09:01:06.187457 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/abstract.cpython-37.pyc
+-rw-r--r--   0        0        0      816 2023-04-11 08:06:27.059825 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/abstract.cpython-38.pyc
+-rw-r--r--   0        0        0    18750 2023-04-06 07:29:21.753843 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/mixins.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9261 2023-02-27 09:01:06.194124 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/mixins.cpython-37.pyc
+-rw-r--r--   0        0        0     9419 2023-04-11 08:06:27.063159 renku-2.4.0rc1/renku/ui/service/controllers/api/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0        0        0     1085 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/api/abstract.py
+-rw-r--r--   0        0        0    15626 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/service/controllers/api/mixins.py
+-rw-r--r--   0        0        0     2647 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py
+-rw-r--r--   0        0        0     7478 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/service/controllers/cache_files_upload.py
+-rw-r--r--   0        0        0     2239 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/cache_list_projects.py
+-rw-r--r--   0        0        0     1927 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/cache_list_uploaded.py
+-rw-r--r--   0        0        0     4823 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/cache_migrate_project.py
+-rw-r--r--   0        0        0     5110 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/controllers/cache_migrations_check.py
+-rw-r--r--   0        0        0     2350 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/cache_project_clone.py
+-rw-r--r--   0        0        0     2649 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/config_set.py
+-rw-r--r--   0        0        0     2333 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/config_show.py
+-rw-r--r--   0        0        0     5682 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_add_file.py
+-rw-r--r--   0        0        0     3916 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_create.py
+-rw-r--r--   0        0        0     5359 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/service/controllers/datasets_edit.py
+-rw-r--r--   0        0        0     2132 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_files_list.py
+-rw-r--r--   0        0        0     3333 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_import.py
+-rw-r--r--   0        0        0     2065 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_list.py
+-rw-r--r--   0        0        0     2637 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_remove.py
+-rw-r--r--   0        0        0     3290 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/datasets_unlink.py
+-rw-r--r--   0        0        0     5373 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/controllers/graph_export.py
+-rw-r--r--   0        0        0     3936 2023-04-11 08:06:19.169735 renku-2.4.0rc1/renku/ui/service/controllers/project_edit.py
+-rw-r--r--   0        0        0     3180 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/project_lock_status.py
+-rw-r--r--   0        0        0     2096 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/project_show.py
+-rw-r--r--   0        0        0     7932 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/templates_create_project.py
+-rw-r--r--   0        0        0     3100 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/templates_read_manifest.py
+-rw-r--r--   0        0        0      773 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/utils/__init__.py
+-rw-r--r--   0        0        0      235 2023-04-06 07:29:13.829842 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      209 2023-02-27 09:00:51.213933 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      213 2023-04-11 08:06:22.029768 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      814 2023-04-06 07:29:21.837184 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0      551 2023-02-27 09:01:06.267458 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0      555 2023-04-11 08:06:27.679832 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     3571 2023-04-06 07:29:13.829842 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/project_clone.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1695 2023-02-27 09:00:51.217267 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/project_clone.cpython-37.pyc
+-rw-r--r--   0        0        0     1747 2023-04-11 08:06:22.029768 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/project_clone.cpython-38.pyc
+-rw-r--r--   0        0        0     3510 2023-04-06 07:29:14.399890 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/remote_project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2084 2023-02-27 09:00:51.500604 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/remote_project.cpython-37.pyc
+-rw-r--r--   0        0        0     2110 2023-04-11 08:06:22.223103 renku-2.4.0rc1/renku/ui/service/controllers/utils/__pycache__/remote_project.cpython-38.pyc
+-rw-r--r--   0        0        0     1083 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/utils/datasets.py
+-rw-r--r--   0        0        0     3230 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/utils/project_clone.py
+-rw-r--r--   0        0        0     2661 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/utils/remote_project.py
+-rw-r--r--   0        0        0     1641 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/version.py
+-rw-r--r--   0        0        0     2441 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_export.py
+-rw-r--r--   0        0        0     2257 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_list.py
+-rw-r--r--   0        0        0     2146 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_show.py
+-rw-r--r--   0        0        0     6150 2023-04-11 08:06:10.299633 renku-2.4.0rc1/renku/ui/service/entrypoint.py
+-rw-r--r--   0        0        0    31379 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/errors.py
+-rw-r--r--   0        0        0      774 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/gateways/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-06 07:29:21.770511 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      201 2023-02-27 09:01:06.214124 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      205 2023-04-11 08:06:27.683166 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4051 2023-04-06 07:29:21.773845 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/gitlab_api_provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2379 2023-02-27 09:01:06.217457 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/gitlab_api_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     2403 2023-04-11 08:43:03.872550 renku-2.4.0rc1/renku/ui/service/gateways/__pycache__/gitlab_api_provider.cpython-38.pyc
+-rw-r--r--   0        0        0     3339 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/gateways/gitlab_api_provider.py
+-rw-r--r--   0        0        0      793 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/interfaces/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-06 07:29:21.767178 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      222 2023-02-27 09:01:06.210791 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      226 2023-04-11 08:06:27.486497 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1257 2023-04-06 07:29:21.767178 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/git_api_provider.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-02-27 09:01:06.210791 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/git_api_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      930 2023-04-11 08:43:03.872550 renku-2.4.0rc1/renku/ui/service/interfaces/__pycache__/git_api_provider.cpython-38.pyc
+-rw-r--r--   0        0        0     1228 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/interfaces/git_api_provider.py
+-rw-r--r--   0        0        0      766 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-06 07:29:14.789923 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      184 2023-02-27 09:00:51.947276 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      188 2023-04-11 08:06:22.363105 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4435 2023-04-06 07:29:14.793256 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/cleanup.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2227 2023-02-27 09:00:51.947276 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/cleanup.cpython-37.pyc
+-rw-r--r--   0        0        0     2209 2023-04-11 08:06:22.363105 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/cleanup.cpython-38.pyc
+-rw-r--r--   0        0        0      206 2023-04-06 07:29:23.090623 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/constants.cpython-311.pyc
+-rwxr-xr-x   0        0        0      180 2023-02-27 09:01:09.174162 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/constants.cpython-37.pyc
+-rw-r--r--   0        0        0      184 2023-04-11 08:06:27.863168 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0        0        0     1023 2023-04-06 07:29:21.757177 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/contexts.cpython-311.pyc
+-rwxr-xr-x   0        0        0      678 2023-02-27 09:01:06.194124 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/contexts.cpython-37.pyc
+-rw-r--r--   0        0        0      671 2023-04-11 08:06:27.063159 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/contexts.cpython-38.pyc
+-rw-r--r--   0        0        0     6872 2023-04-06 07:29:14.796590 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3482 2023-02-27 09:00:51.950610 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0     3453 2023-04-11 08:06:22.363105 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     1845 2023-04-06 07:29:14.939936 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/delayed_ctrl.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1133 2023-02-27 09:00:52.033944 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/delayed_ctrl.cpython-37.pyc
+-rw-r--r--   0        0        0     1147 2023-04-11 08:06:22.469773 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/delayed_ctrl.cpython-38.pyc
+-rw-r--r--   0        0        0     2504 2023-04-06 07:29:21.757177 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/queues.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1898 2023-02-27 09:01:06.197457 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/queues.cpython-37.pyc
+-rw-r--r--   0        0        0     1926 2023-04-11 08:06:27.063159 renku-2.4.0rc1/renku/ui/service/jobs/__pycache__/queues.cpython-38.pyc
+-rw-r--r--   0        0        0     3035 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/cleanup.py
+-rw-r--r--   0        0        0      756 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/constants.py
+-rw-r--r--   0        0        0     1186 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/contexts.py
+-rw-r--r--   0        0        0     5244 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/datasets.py
+-rw-r--r--   0        0        0     1829 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/delayed_ctrl.py
+-rw-r--r--   0        0        0     2665 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/jobs/queues.py
+-rw-r--r--   0        0        0     1269 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/logger.py
+-rw-r--r--   0        0        0      644 2023-03-02 15:15:40.049932 renku-2.4.0rc1/renku/ui/service/logging.yaml
+-rw-r--r--   0        0        0     2742 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/scheduler.py
+-rw-r--r--   0        0        0      768 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-06 07:29:13.796506 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      198 2023-02-27 09:00:51.183933 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      202 2023-04-11 08:06:21.996434 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    18991 2023-04-06 07:29:14.353219 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/cache.cpython-311.pyc
+-rwxr-xr-x   0        0        0    12356 2023-02-27 09:00:51.457270 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/cache.cpython-37.pyc
+-rw-r--r--   0        0        0    12422 2023-04-11 08:43:01.172495 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     6666 2023-04-06 07:29:14.033192 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/common.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4479 2023-02-27 09:00:51.273934 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/common.cpython-37.pyc
+-rw-r--r--   0        0        0     4536 2023-04-11 08:43:01.105827 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     3115 2023-04-06 07:29:21.827183 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2266 2023-02-27 09:01:06.257458 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     2203 2023-04-11 08:06:27.493163 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0    14455 2023-04-06 07:29:16.583407 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9489 2023-02-27 09:00:53.743965 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0     9367 2023-04-11 08:06:23.449784 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     3193 2023-04-06 07:29:21.857185 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2162 2023-02-27 09:01:06.284125 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0        0        0     2194 2023-04-11 08:06:27.596498 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0     8448 2023-04-06 07:29:13.799840 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/headers.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4895 2023-02-27 09:00:51.187266 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/headers.cpython-37.pyc
+-rw-r--r--   0        0        0     4891 2023-04-11 08:06:21.999767 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/headers.cpython-38.pyc
+-rw-r--r--   0        0        0     2924 2023-04-06 07:29:21.860519 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/jobs.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1823 2023-02-27 09:01:06.287458 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/jobs.cpython-37.pyc
+-rw-r--r--   0        0        0     1845 2023-04-11 08:06:28.006503 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/jobs.cpython-38.pyc
+-rw-r--r--   0        0        0     6155 2023-04-06 07:29:21.867186 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4134 2023-02-27 09:01:06.294125 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     4167 2023-04-11 08:06:27.599831 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0      651 2023-04-06 07:29:14.153203 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/rpc.cpython-311.pyc
+-rwxr-xr-x   0        0        0      489 2023-02-27 09:00:51.337268 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/rpc.cpython-37.pyc
+-rw-r--r--   0        0        0      497 2023-04-11 08:06:22.116435 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/rpc.cpython-38.pyc
+-rw-r--r--   0        0        0     8026 2023-04-06 07:29:14.349886 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/templates.cpython-311.pyc
+-rwxr-xr-x   0        0        0     5070 2023-02-27 09:00:51.450603 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/templates.cpython-37.pyc
+-rw-r--r--   0        0        0     5059 2023-04-11 08:06:22.189769 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/templates.cpython-38.pyc
+-rw-r--r--   0        0        0     1208 2023-04-06 07:29:21.890521 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/version.cpython-311.pyc
+-rwxr-xr-x   0        0        0      828 2023-02-27 09:01:06.310792 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/version.cpython-37.pyc
+-rw-r--r--   0        0        0      840 2023-03-02 15:15:52.370080 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0    12418 2023-04-06 07:29:21.897189 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/workflows.cpython-311.pyc
+-rwxr-xr-x   0        0        0     7202 2023-02-27 09:01:06.317459 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/workflows.cpython-37.pyc
+-rw-r--r--   0        0        0     7207 2023-04-11 08:06:27.619831 renku-2.4.0rc1/renku/ui/service/serializers/__pycache__/workflows.cpython-38.pyc
+-rw-r--r--   0        0        0    13180 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/serializers/cache.py
+-rw-r--r--   0        0        0     4045 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/serializers/common.py
+-rw-r--r--   0        0        0     2228 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/config.py
+-rw-r--r--   0        0        0     8754 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/datasets.py
+-rw-r--r--   0        0        0     2195 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/graph.py
+-rw-r--r--   0        0        0     5362 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/headers.py
+-rw-r--r--   0        0        0     1961 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/jobs.py
+-rw-r--r--   0        0        0     4510 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/project.py
+-rw-r--r--   0        0        0      911 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/rpc.py
+-rw-r--r--   0        0        0     5858 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/templates.py
+-rw-r--r--   0        0        0      212 2023-04-11 08:06:03.429555 renku-2.4.0rc1/renku/ui/service/serializers/v0_9/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1695 2023-04-11 08:06:03.439555 renku-2.4.0rc1/renku/ui/service/serializers/v0_9/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0      773 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/v1/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-06 07:29:21.820515 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      206 2023-02-27 09:01:06.250791 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      210 2023-04-11 08:06:28.023169 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4900 2023-04-06 07:29:21.820515 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/cache.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3481 2023-02-27 09:01:06.250791 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/cache.cpython-37.pyc
+-rw-r--r--   0        0        0     3543 2023-04-11 08:06:28.043170 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     2136 2023-04-06 07:29:21.887188 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/templates.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1461 2023-02-27 09:01:06.307458 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/templates.cpython-37.pyc
+-rw-r--r--   0        0        0     1485 2023-04-11 08:06:28.046503 renku-2.4.0rc1/renku/ui/service/serializers/v1/__pycache__/templates.cpython-38.pyc
+-rw-r--r--   0        0        0     4212 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/v1/cache.py
+-rw-r--r--   0        0        0     1880 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/v1/templates.py
+-rw-r--r--   0        0        0      212 2023-04-11 08:06:03.442888 renku-2.4.0rc1/renku/ui/service/serializers/v1_0/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1004 2023-04-11 08:06:03.449555 renku-2.4.0rc1/renku/ui/service/serializers/v1_0/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     1170 2023-03-02 15:15:40.049932 renku-2.4.0rc1/renku/ui/service/serializers/version.py
+-rw-r--r--   0        0        0     6907 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/serializers/workflows.py
+-rw-r--r--   0        0        0     2186 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/utils/__init__.py
+-rw-r--r--   0        0        0     2279 2023-04-06 07:29:11.709664 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1527 2023-02-27 09:00:48.983905 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1547 2023-04-11 08:06:20.943088 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3179 2023-04-06 07:29:11.712998 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/callback.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2325 2023-02-27 09:00:48.983905 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/callback.cpython-37.pyc
+-rw-r--r--   0        0        0     2348 2023-04-11 08:06:20.943088 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/callback.cpython-38.pyc
+-rw-r--r--   0        0        0     1299 2023-04-06 07:29:21.710506 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/json_encoder.cpython-311.pyc
+-rwxr-xr-x   0        0        0      863 2023-02-27 09:01:06.157457 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/json_encoder.cpython-37.pyc
+-rw-r--r--   0        0        0      877 2023-04-11 08:06:27.043158 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/json_encoder.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-06 07:29:14.346552 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/squash.cpython-311.pyc
+-rwxr-xr-x   0        0        0      687 2023-02-27 09:00:51.450603 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/squash.cpython-37.pyc
+-rw-r--r--   0        0        0      691 2023-04-11 08:06:22.189769 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/squash.cpython-38.pyc
+-rw-r--r--   0        0        0     1284 2023-04-06 07:29:23.413983 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/timeout.cpython-311.pyc
+-rwxr-xr-x   0        0        0      812 2023-02-27 09:01:10.017506 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/timeout.cpython-37.pyc
+-rw-r--r--   0        0        0      821 2023-04-11 08:06:28.086504 renku-2.4.0rc1/renku/ui/service/utils/__pycache__/timeout.cpython-38.pyc
+-rw-r--r--   0        0        0     2220 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/utils/callback.py
+-rw-r--r--   0        0        0     1323 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/utils/json_encoder.py
+-rw-r--r--   0        0        0     1260 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/utils/squash.py
+-rw-r--r--   0        0        0     1427 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/utils/timeout.py
+-rw-r--r--   0        0        0     1761 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/__init__.py
+-rw-r--r--   0        0        0     1712 2023-04-06 07:29:14.203207 renku-2.4.0rc1/renku/ui/service/views/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1043 2023-02-27 09:00:51.383936 renku-2.4.0rc1/renku/ui/service/views/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1055 2023-04-11 08:06:22.146436 renku-2.4.0rc1/renku/ui/service/views/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2869 2023-04-06 07:29:15.336635 renku-2.4.0rc1/renku/ui/service/views/__pycache__/api_versions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1842 2023-02-27 09:00:52.593951 renku-2.4.0rc1/renku/ui/service/views/__pycache__/api_versions.cpython-37.pyc
+-rw-r--r--   0        0        0     1891 2023-04-11 08:06:22.623108 renku-2.4.0rc1/renku/ui/service/views/__pycache__/api_versions.cpython-38.pyc
+-rw-r--r--   0        0        0     5761 2023-04-06 07:29:21.710506 renku-2.4.0rc1/renku/ui/service/views/__pycache__/apispec.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4129 2023-02-27 09:01:06.160790 renku-2.4.0rc1/renku/ui/service/views/__pycache__/apispec.cpython-37.pyc
+-rw-r--r--   0        0        0     4134 2023-04-11 08:43:03.862549 renku-2.4.0rc1/renku/ui/service/views/__pycache__/apispec.cpython-38.pyc
+-rw-r--r--   0        0        0     8718 2023-04-06 07:29:21.747176 renku-2.4.0rc1/renku/ui/service/views/__pycache__/cache.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6262 2023-02-27 09:01:06.184124 renku-2.4.0rc1/renku/ui/service/views/__pycache__/cache.cpython-37.pyc
+-rw-r--r--   0        0        0     6274 2023-04-11 08:06:27.056492 renku-2.4.0rc1/renku/ui/service/views/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     3209 2023-04-06 07:29:21.823849 renku-2.4.0rc1/renku/ui/service/views/__pycache__/config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2310 2023-02-27 09:01:06.254124 renku-2.4.0rc1/renku/ui/service/views/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     2319 2023-04-11 08:06:28.219838 renku-2.4.0rc1/renku/ui/service/views/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     9653 2023-04-06 07:29:21.833850 renku-2.4.0rc1/renku/ui/service/views/__pycache__/datasets.cpython-311.pyc
+-rwxr-xr-x   0        0        0     6825 2023-02-27 09:01:06.264125 renku-2.4.0rc1/renku/ui/service/views/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0        0        0     6836 2023-04-11 08:06:28.223172 renku-2.4.0rc1/renku/ui/service/views/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0        0        0     3736 2023-04-06 07:29:14.343219 renku-2.4.0rc1/renku/ui/service/views/__pycache__/decorators.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2540 2023-02-27 09:00:51.443936 renku-2.4.0rc1/renku/ui/service/views/__pycache__/decorators.cpython-37.pyc
+-rw-r--r--   0        0        0     2458 2023-04-11 08:06:22.186436 renku-2.4.0rc1/renku/ui/service/views/__pycache__/decorators.cpython-38.pyc
+-rw-r--r--   0        0        0    21314 2023-04-06 07:29:14.346552 renku-2.4.0rc1/renku/ui/service/views/__pycache__/error_handlers.cpython-311.pyc
+-rwxr-xr-x   0        0        0    13439 2023-02-27 09:00:51.447270 renku-2.4.0rc1/renku/ui/service/views/__pycache__/error_handlers.cpython-37.pyc
+-rw-r--r--   0        0        0    12848 2023-04-11 08:43:01.169162 renku-2.4.0rc1/renku/ui/service/views/__pycache__/error_handlers.cpython-38.pyc
+-rw-r--r--   0        0        0     2059 2023-04-06 07:29:21.853852 renku-2.4.0rc1/renku/ui/service/views/__pycache__/graph.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1525 2023-02-27 09:01:06.280792 renku-2.4.0rc1/renku/ui/service/views/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0        0        0     1535 2023-04-11 08:06:28.246505 renku-2.4.0rc1/renku/ui/service/views/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0     3698 2023-04-06 07:29:21.860519 renku-2.4.0rc1/renku/ui/service/views/__pycache__/jobs.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2401 2023-02-27 09:01:06.287458 renku-2.4.0rc1/renku/ui/service/views/__pycache__/jobs.cpython-37.pyc
+-rw-r--r--   0        0        0     2415 2023-04-11 08:06:28.246505 renku-2.4.0rc1/renku/ui/service/views/__pycache__/jobs.cpython-38.pyc
+-rw-r--r--   0        0        0     4226 2023-04-06 07:29:21.863852 renku-2.4.0rc1/renku/ui/service/views/__pycache__/project.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3043 2023-02-27 09:01:06.290792 renku-2.4.0rc1/renku/ui/service/views/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0        0        0     3059 2023-04-11 08:06:28.249839 renku-2.4.0rc1/renku/ui/service/views/__pycache__/project.cpython-38.pyc
+-rw-r--r--   0        0        0     3809 2023-04-06 07:29:21.877187 renku-2.4.0rc1/renku/ui/service/views/__pycache__/templates.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2846 2023-02-27 09:01:06.300792 renku-2.4.0rc1/renku/ui/service/views/__pycache__/templates.cpython-37.pyc
+-rw-r--r--   0        0        0     2871 2023-04-11 08:06:28.249839 renku-2.4.0rc1/renku/ui/service/views/__pycache__/templates.cpython-38.pyc
+-rw-r--r--   0        0        0     1554 2023-04-06 07:29:21.887188 renku-2.4.0rc1/renku/ui/service/views/__pycache__/version.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1171 2023-02-27 09:01:06.310792 renku-2.4.0rc1/renku/ui/service/views/__pycache__/version.cpython-37.pyc
+-rw-r--r--   0        0        0     1181 2023-03-07 14:12:41.939266 renku-2.4.0rc1/renku/ui/service/views/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0     4261 2023-04-06 07:29:21.893855 renku-2.4.0rc1/renku/ui/service/views/__pycache__/workflow_plans.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3062 2023-02-27 09:01:06.314125 renku-2.4.0rc1/renku/ui/service/views/__pycache__/workflow_plans.cpython-37.pyc
+-rw-r--r--   0        0        0     3094 2023-04-11 08:06:28.256506 renku-2.4.0rc1/renku/ui/service/views/__pycache__/workflow_plans.cpython-38.pyc
+-rw-r--r--   0        0        0     2438 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/api_versions.py
+-rw-r--r--   0        0        0     4771 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/views/apispec.py
+-rw-r--r--   0        0        0     7427 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/cache.py
+-rw-r--r--   0        0        0     2957 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/config.py
+-rw-r--r--   0        0        0     8187 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/datasets.py
+-rw-r--r--   0        0        0     2961 2023-04-11 08:06:10.302967 renku-2.4.0rc1/renku/ui/service/views/decorators.py
+-rw-r--r--   0        0        0    14663 2023-04-11 08:42:55.942389 renku-2.4.0rc1/renku/ui/service/views/error_handlers.py
+-rw-r--r--   0        0        0     2084 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/graph.py
+-rw-r--r--   0        0        0     3267 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/jobs.py
+-rw-r--r--   0        0        0     3805 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/project.py
+-rw-r--r--   0        0        0     3592 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/templates.py
+-rw-r--r--   0        0        0      200 2023-04-11 08:06:03.696225 renku-2.4.0rc1/renku/ui/service/views/v0_9/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1805 2023-04-11 08:06:03.709558 renku-2.4.0rc1/renku/ui/service/views/v0_9/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0      767 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/v1/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-06 07:29:21.817182 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      194 2023-02-27 09:01:06.250791 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      198 2023-04-11 08:06:28.253172 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4010 2023-04-06 07:29:21.817182 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/cache.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2842 2023-02-27 09:01:06.250791 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/cache.cpython-37.pyc
+-rw-r--r--   0        0        0     2856 2023-04-11 08:43:03.882550 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     2748 2023-04-06 07:29:21.883854 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/templates.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2092 2023-02-27 09:01:06.307458 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/templates.cpython-37.pyc
+-rw-r--r--   0        0        0     2110 2023-04-11 08:06:28.253172 renku-2.4.0rc1/renku/ui/service/views/v1/__pycache__/templates.cpython-38.pyc
+-rw-r--r--   0        0        0     3574 2023-04-11 08:42:55.945722 renku-2.4.0rc1/renku/ui/service/views/v1/cache.py
+-rw-r--r--   0        0        0     2634 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/v1/templates.py
+-rw-r--r--   0        0        0      200 2023-04-11 08:06:03.712891 renku-2.4.0rc1/renku/ui/service/views/v1_0/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1705 2023-04-11 08:06:03.722892 renku-2.4.0rc1/renku/ui/service/views/v1_0/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     1702 2023-03-07 14:12:33.875823 renku-2.4.0rc1/renku/ui/service/views/version.py
+-rw-r--r--   0        0        0     3873 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/views/workflow_plans.py
+-rw-r--r--   0        0        0     2890 2023-04-11 08:06:10.306300 renku-2.4.0rc1/renku/ui/service/worker.py
+-rw-r--r--   0        0        0     1485 2023-04-11 08:42:55.945722 renku-2.4.0rc1/renku/version.py
+-rw-r--r--   0        0        0    18611 1970-01-01 00:00:00.000000 renku-2.4.0rc1/setup.py
+-rw-r--r--   0        0        0    17302 1970-01-01 00:00:00.000000 renku-2.4.0rc1/PKG-INFO
```

### Comparing `renku-2.3.2/AUTHORS.rst` & `renku-2.4.0rc1/AUTHORS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+    Copyright 2017-2023 - Swiss Data Science Center (SDSC)
     A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
     Eidgenössische Technische Hochschule Zürich (ETHZ).
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
```

### Comparing `renku-2.3.2/CHANGES.rst` & `renku-2.4.0rc1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+    Copyright 2017-2023 - Swiss Data Science Center (SDSC)
     A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
     Eidgenössische Technische Hochschule Zürich (ETHZ).
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
@@ -14,14 +14,73 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 Changes
 =======
 
+`2.4.0 <https://github.com/SwissDataScienceCenter/renku-python/compare/v2.3.2...v2.4.0>`__ (2023-04-10)
+-------------------------------------------------------------------------------------------------------
+
+Bug Fixes
+~~~~~~~~~
+
+-  **cli:** fix starting local sessions as user without user id 1000
+   (`#3341 <https://github.com/SwissDataScienceCenter/renku-python/issues/3341>`__)
+   (`a345346 <https://github.com/SwissDataScienceCenter/renku-python/commit/a3453463a5c4f61ab01195ec1a6be039fac63489>`__)
+-  **cli:** limit commit message length when there are too many files
+   (`#3375 <https://github.com/SwissDataScienceCenter/renku-python/issues/3375>`__)
+   (`70cf36a <https://github.com/SwissDataScienceCenter/renku-python/commit/70cf36acfbe0b4fd4ed32a3476309661f93c5aa0>`__)
+-  **cli:** start remote sessions from correct branch
+   (`#3382 <https://github.com/SwissDataScienceCenter/renku-python/issues/3382>`__)
+   (`8b4866f <https://github.com/SwissDataScienceCenter/renku-python/commit/8b4866f76075fd3a3c380e1b8a2354b138d97e9d>`__)
+-  **core:** python 3.11 compatibility
+   (`#3386 <https://github.com/SwissDataScienceCenter/renku-python/issues/3386>`__)
+   (`6029ad2 <https://github.com/SwissDataScienceCenter/renku-python/commit/6029ad278e835afa4cdef05a34712e1ed0961374>`__)
+-  **core:** fix issue with v10 dataset migration
+   (`#3359 <https://github.com/SwissDataScienceCenter/renku-python/issues/3359>`__)
+   (`f9da0be <https://github.com/SwissDataScienceCenter/renku-python/commit/f9da0be8585a692c49fbdaa19316b779a965db03>`__)
+-  **service:** fix error message for invalid templates
+   (`#3349 <https://github.com/SwissDataScienceCenter/renku-python/issues/3349>`__)
+   (`6798b1a <https://github.com/SwissDataScienceCenter/renku-python/commit/6798b1a8d646c47918b53764c931c304241284ac>`__)
+
+Features
+~~~~~~~~
+
+-  **cli:** add `--force-build` flag to docker session start
+   (`#3369 <https://github.com/SwissDataScienceCenter/renku-python/issues/3369>`__)
+   (`671d7e4 <https://github.com/SwissDataScienceCenter/renku-python/commit/671d7e46f18c5a6d741522f56fd3bf33887fb8c7>`__)
+-  **cli:** allow setting local port on docker session provider
+   (`#3350 <https://github.com/SwissDataScienceCenter/renku-python/issues/3350>`__)
+   (`5fdac71 <https://github.com/SwissDataScienceCenter/renku-python/commit/5fdac715b26f3ec4d65dd913d6f63416bdabb60e>`__)
+-  **cli:** remove CLI version check
+   (`#3343 <https://github.com/SwissDataScienceCenter/renku-python/issues/3343>`__)
+   (`3dcefb9 <https://github.com/SwissDataScienceCenter/renku-python/commit/3dcefb95974b515d7563ee540a1922206fe89342>`__)
+-  **cli:** support rsync-style syntax using / in `renku dataset add`
+   (`#3362 <https://github.com/SwissDataScienceCenter/renku-python/issues/3362>`__)
+   (`57520c3 <https://github.com/SwissDataScienceCenter/renku-python/commit/57520c3b78b9c16510dedee24ea397e4f073522e>`__)
+-  **core:** add contracts to code to check metadata in `renku.core`
+   (`#3356 <https://github.com/SwissDataScienceCenter/renku-python/issues/3356>`__)
+   (`c8148d8 <https://github.com/SwissDataScienceCenter/renku-python/commit/c8148d80fdf4e6f3a92ebfe201cc96f405b013a0>`__)
+-  **core:** set default sensible flags for `renku update` and `renku graph export``
+   (`#3342 <https://github.com/SwissDataScienceCenter/renku-python/issues/3342>`__)
+   (`8bef1b9 <https://github.com/SwissDataScienceCenter/renku-python/commit/8bef1b9d2dd65bd0b678353363140cdf4a220027>`__)
+-  **dataset:** add external storage backend
+   (`#3323 <https://github.com/SwissDataScienceCenter/renku-python/issues/3323>`__)
+   (`2a461d4 <https://github.com/SwissDataScienceCenter/renku-python/commit/2a461d4908e346c356bffb4dd602088098736d67>`__)
+-  **dataset:** support parallel data download/upload
+   (`#3358 <https://github.com/SwissDataScienceCenter/renku-python/issues/3358>`__)
+   (`3f1e707 <https://github.com/SwissDataScienceCenter/renku-python/commit/3f1e707042214d819c56565b7eed61a472af9702>`__)
+-  **dataset:** store s3 credentials per bucket
+   (`#3339 <https://github.com/SwissDataScienceCenter/renku-python/issues/3339>`__)
+   (`717a780 <https://github.com/SwissDataScienceCenter/renku-python/commit/717a780363746772b077d1494f3be2b36eea0c99>`__)
+-  **template:** allow renaming templates by using aliases
+   (`#3347 <https://github.com/SwissDataScienceCenter/renku-python/issues/3347>`__)
+   (`b582cc5 <https://github.com/SwissDataScienceCenter/renku-python/commit/b582cc5d9ca86218b0c7b9645cd0c03b5e7cae00>`__)
+
 `2.3.2 <https://github.com/SwissDataScienceCenter/renku-python/compare/v2.3.1...v2.3.2>`__ (2023-03-13)
 -------------------------------------------------------------------------------------------------------
 
 Bug Fixes
 ~~~~~~~~~
 
 -  **core:** Fix a bug that caused crashing when migrating to v10 metadata
```

### Comparing `renku-2.3.2/LICENSE` & `renku-2.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/README.rst` & `renku-2.4.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+    Copyright 2017-2023 - Swiss Data Science Center (SDSC)
     A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
     Eidgenössische Technische Hochschule Zürich (ETHZ).
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
```

### Comparing `renku-2.3.2/pyproject.toml` & `renku-2.4.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -16,69 +16,71 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool]
 
 [tool.poetry]
 name = "renku"
-version = "2.3.2" # placeholder, see poetry-dynamic-versioning
+version = "2.4.0rc1" # placeholder, see poetry-dynamic-versioning
 description = "Python SDK and CLI for the Renku platform."
 license = "Apache License 2.0"
 keywords = ["Renku", "CLI"]
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
 ]
 homepage = "https://github.com/swissdatasciencecenter/renku-python"
 documentation = "https://renku-python.rtfd.io/"
 
 authors = ["Swiss Data Science Center <contact@datascience.ch>"]
 include = ["renku/*", "renku/**/*", "CHANGES.rst", "AUTHORS.rst"]
 readme = "README.rst"
 
 [tool.poetry.urls]
 Changelog = "https://github.com/swissdatasciencecenter/renku-python/blob/master/CHANGES.rst"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = "^3.8.1"
 appdirs = "<=1.4.4,>=1.4.3"
 attrs = ">=21.1.0,<22.2.0"
 bashlex = ">=0.16,<0.17"
 calamus = ">=0.3.13,<0.5"
 click = ">=8.0,<8.1.4"
 click-option-group = "<0.6.0,>=0.5.2"
 click-plugins = "==1.1.1"
 coverage = { version = "<6.5,>=4.5.3", extras=["toml"], optional = true }
 cryptography = ">=38.0.0,<40.0.0"
 cwl-utils = ">=0.12,<0.18"
 cwltool = "==3.1.20220628170238"
+deal = ">=4.24.0,<5.0.0"
 deepdiff = "^5.8.0"
 deepmerge = "==1.0.1"
 docker = "<6,>=3.7.2"
 filelock = ">=3.3.0,<3.8.1"
 gitpython = "==3.1.27"
 grandalf = "==0.7"
 humanize = ">=3.0.0,<4.1.0"
-importlib-resources = { version = ">=5.4.0,<5.10.0", python = "<3.9.0" }
+importlib-resources = ">=5.12.0,<5.13.0"
 inject = "<4.4.0,>=4.3.0"
 jinja2 = { version = ">=2.11.3,<3.1.3" }
 networkx = "<2.7,>=2.6.0"
-numpy = ">=1.20.0,<1.22.0"
-packaging = "<22.0,>=21.3"
+numpy = ">=1.24.0,<1.25.0"
+packaging = "<24.0,>=23.0"
 pathspec = "<1.0.0,>=0.8.0"
 patool = "==1.12"
 pluggy = "==1.0.0"
 portalocker = ">=2.2.1,<2.5"
 poetry-dynamic-versioning = "0.21.3"
 psutil = ">=5.4.7,<5.9.2"
 pydantic = "==1.10.2"
@@ -89,15 +91,15 @@
 python-dateutil = "<2.8.3,>=2.6.1"
 python-editor = "==1.0.4"
 python-gitlab = ">=2.10.1,<3.8.2"
 pyyaml = "<6.1.0,>=5.4"
 rdflib = "<7.0,>=6.0.0"
 requests = ">=2.23.0,<2.28.2"
 rich = ">=9.3.0,<12.6.0"
-shellingham = "1.5.0"
+shellingham = "1.5.0.post1"
 tabulate = ">=0.7.7,<0.8.11"
 toil = "==5.7.1"
 tqdm = "<4.62.4,>=4.48.1"
 werkzeug = ">=1.0.0,<2.2.3"
 yagup = ">=0.1.1"
 yaspin = "==2.1.0"
 "zc.relation" = "<1.2,>=1.1"
@@ -117,33 +119,26 @@
 redis = { version = ">=3.5.3,<4.2.0", optional = true }
 rq = { version = "==1.11.0", optional = true }
 rq-scheduler = { version = "==0.11.0", optional = true }
 sentry-sdk = { version = ">=1.5.11,<1.5.12", extras = ["flask"],  optional = true }
 walrus = { version = ">=0.8.2,<0.10.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-black = "==22.10.0"
-flake8 = [
-    { version = ">=6.0.0,<7.0.0", python = ">=3.8.1"},
-    { version = ">=4.0.0,<5.0.0", python = "<3.8.1"}
-]
-Flake8-pyproject = [
-    { version ="==1.2.2", python = ">=3.8.1"},
-    { version ="<1.0.0", python = "<3.8.1"}
-]
+black = "==23.1.0"
+flake8 = ">=6.0.0,<7.0.0"
+Flake8-pyproject = "==1.2.2"
 isort = "<5.10.2,>=5.3.2"
 mypy = ">=0.942,<1.0"
 poetry-lock-package = "^0.5.0"
 pre-commit = "^2.20.0"
 types-PyYAML = "<6.1.0,>=5.4"
 types-python-dateutil = "^2.8.10"
 types-redis = ">=3.5.3,<4.1.0"
 types-requests = "<2.27.2,>=2.23.0"
 types-tabulate = "<0.8.10,>=0.7.7"
-typing-extensions = { version = ">=4.3.0,<5.0.0", python = "<3.8.0" }
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 coverage = { version = "<6.5,>=4.5.3", extras=["toml"] }
 fakeredis = { version = ">=1.4.1,<1.7.2", extras = ["lua"]}
@@ -152,14 +147,15 @@
 pydocstyle = "<6.1.2,>=4.0.1"
 pyte = ">=0.8.0,<0.9.0"
 pytest = ">=4.0.0,<7.1.4"
 pytest-black = "<0.3.13,>=0.3.10"
 pytest-cache = "==1.0"
 pytest-cov = "<3.1.0,>=2.5.1"
 pytest-flake8 = ">=1.0.6,<1.1.1"
+pytest-lazy-fixture = ">=0.6.3,<0.7.0"
 pytest-mock = ">=3.2.0,<3.9.0"
 pytest-pep8 = "==1.0.6"
 pytest-recording = "==0.12.1"
 pytest-timeout = "==2.1.0"
 pytest-xdist = ">=1.34.0,<2.6.0"
 responses = ">=0.22.0,<0.23.0"
 
@@ -237,16 +233,15 @@
 format-jinja = """
     {%- if distance == 0 -%}
         {{ base }}{{"-%s"|format(stage) if stage else ""}}{{".%s"|format(revision) if revision else ""}}{{"+dirty" if dirty else ""}}
     {%- else -%}
         {{ base }}{{"-%s"|format(stage) if stage else ""}}{{".%s"|format(revision) if revision else ""}}.dev{{distance}}+g{{commit}}{{"-dirty" if dirty else ""}}
     {%- endif -%}
 """
-pattern = """
-    (?x)                                                (?# ignore whitespace)
+pattern = """(?x)                                          (?# ignore whitespace)
     ^v(?P<base>\\d+(\\.\\d+)*)                             (?# v1.2.3)
     (-?((?P<stage>[a-zA-Z0-9]+)?\\.?(?P<revision>(pre|post)\\d+)?))?    (?# b0)
     (\\+(?P<tagged_metadata>.+))?$                       (?# e.g., +linux)
 """
 
 [tool.pytest.ini_options]
 addopts = "--flake8 --black --doctest-glob=\"*.rst\" --doctest-modules --cov --cov-report=term-missing --ignore=docs/cheatsheet/"
@@ -256,17 +251,19 @@
 testpaths = ["docs", "tests", "renku", "conftest.py"]
 markers = [
     "integration: mark a test as a integration.",
     "jobs: mark a test as a job test.",
     "migration: mark a test as a migration test.",
     "publish: mark tests that publish datasets to external providers.",
     "redis: mark tests that need a running redis",
+    "remote_repo: used to specify which remote to use in test fixtures.",
     "serial: mark a test that can not be run in parallel",
     "service: mark a test as service test.",
-    "shelled: mark a test as a shelled test.",
+    "shaky: mark an integration test that might fail due to dataset providers' failures.",
+    "shelled: mark a test as a shelled test."
 ]
 filterwarnings = [
     "ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning",
     "ignore:distutils Version classes are deprecated. Use packaging.version instead:DeprecationWarning"
 ]
 
 [tool.mypy]
@@ -298,15 +295,14 @@
     "circus",
     "fakeredis",
     "flaky",
     "grandalf.*",
     "gunicorn.*",
     "humanize",
     "lazy_object_proxy",
-    "lockfile",
     "marshmallow_oneofschema",
     "networkx.*",
     "pathspec",
     "patoolib.*",
     "persistent.*",
     "pexpect",
     "PIL",
```

### Comparing `renku-2.3.2/renku/__init__.py` & `renku-2.4.0rc1/renku/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Renku modules."""
 
-from __future__ import absolute_import, print_function
 
 import importlib
 import importlib.util
 import sys
 import warnings
 
 from renku.version import __template_version__, __version__
```

### Comparing `renku-2.3.2/renku/command/__init__.py` & `renku-2.4.0rc1/renku/ui/service/interfaces/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku commands implementation module."""
+"""Renku service interfaces for IoC adapters/gateways."""
```

### Comparing `renku-2.3.2/renku/command/checks/__init__.py` & `renku-2.4.0rc1/renku/command/checks/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,18 +15,18 @@
 # limitations under the License.
 """Define repository checks for :program:`renku doctor`."""
 
 from .activities import check_activity_dates, check_migrated_activity_ids
 from .datasets import (
     check_dataset_files_outside_datadir,
     check_dataset_old_metadata_location,
+    check_external_files,
     check_invalid_datasets_derivation,
     check_missing_files,
 )
-from .external import check_missing_external_files
 from .githooks import check_git_hooks_installed
 from .migration import check_migration
 from .project import check_project_id_group
 from .storage import check_lfs_info
 from .validate_shacl import check_datasets_structure, check_project_structure
 from .workflow import check_activity_catalog, check_plan_modification_date
 
@@ -40,14 +38,14 @@
     "check_dataset_old_metadata_location",
     "check_datasets_structure",
     "check_git_hooks_installed",
     "check_invalid_datasets_derivation",
     "check_lfs_info",
     "check_migrated_activity_ids",
     "check_migration",
-    "check_missing_external_files",
+    "check_external_files",
     "check_missing_files",
     "check_project_id_group",
     "check_project_structure",
     "check_plan_modification_date",
     "check_activity_dates",
 )
```

### Comparing `renku-2.3.2/renku/command/checks/activities.py` & `renku-2.4.0rc1/renku/command/checks/activities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/checks/datasets.py` & `renku-2.4.0rc1/renku/command/checks/datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -67,14 +65,17 @@
 
     Returns:
         Tuple of whether all dataset files are there and string of found problems.
     """
     missing = defaultdict(list)
 
     for dataset in dataset_gateway.get_all_active_datasets():
+        # NOTE: Datasets with storage backend don't have local copies of files
+        if dataset.storage:
+            continue
         for file_ in dataset.files:
             path = project_context.path / file_.entity.path
             file_exists = path.exists() or (file_.is_external and os.path.lexists(path))
             if not file_exists:
                 missing[dataset.name].append(file_.entity.path)
 
     if not missing:
@@ -160,15 +161,15 @@
             continue
 
         data_dir = dataset.get_datadir()
 
         detected_files = []
 
         for file in dataset.files:
-            if file.is_external:
+            if file.is_external or file.linked:
                 continue
             try:
                 get_safe_relative_path(project_context.path / file.entity.path, project_context.path / data_dir)
             except ValueError:
                 detected_files.append(file)
 
         if not detected_files:
@@ -191,7 +192,54 @@
             + "(use 'renku doctor --fix' to fix them):\n\n\t"
             + "\n\t".join(click.style(file.entity.path, fg="yellow") for file in invalid_files)
             + "\n"
         )
         return False, problems
 
     return True, None
+
+
+@inject.autoparams("dataset_gateway")
+def check_external_files(fix, dataset_gateway: IDatasetGateway, **_):
+    """Find external files.
+
+    Args:
+        fix: Whether to fix found issues.
+        dataset_gateway(IDatasetGateway): The injected dataset gateway.
+        _: keyword arguments.
+
+    Returns:
+        Tuple of whether no external files are found and string of found problems.
+    """
+    from renku.core.dataset.dataset import file_unlink
+
+    external_files = []
+    datasets = defaultdict(list)
+
+    for dataset in dataset_gateway.get_all_active_datasets():
+        for file in dataset.files:
+            if file.is_external:
+                external_files.append(file.entity.path)
+                datasets[dataset.name].append(file)
+
+    if not external_files:
+        return True, None
+
+    external_files_str = "\n\t".join(sorted(external_files))
+
+    if not fix:
+        problems = (
+            f"\n{WARNING}: External files are deprecated in favor of an external dataset backend.\n"
+            "Use 'renku dataset rm' or rerun 'renku doctor' with '--fix' flag to remove them:\n\t"
+            f"{external_files_str}\n"
+        )
+        return False, problems
+
+    communication.info(
+        "The following external files were deleted from the project. You need to add them later manually using a "
+        f"dataset with an external storage backend:\n\t{external_files_str}"
+    )
+
+    for name, files in datasets.items():
+        file_unlink(name=name, yes=True, dataset_files=files)
+
+    return True, None
```

### Comparing `renku-2.3.2/renku/command/checks/githooks.py` & `renku-2.4.0rc1/renku/command/checks/githooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/checks/migration.py` & `renku-2.4.0rc1/renku/command/checks/migration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/checks/project.py` & `renku-2.4.0rc1/renku/command/checks/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/checks/storage.py` & `renku-2.4.0rc1/renku/command/checks/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/checks/validate_shacl.py` & `renku-2.4.0rc1/renku/command/checks/validate_shacl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -47,23 +45,23 @@
     problems = []
 
     for _, result in graph.subject_objects(sh.result):
         path = graph.value(result, sh.resultPath)
         res = graph.value(result, sh.resultMessage)
 
         if res:
-            message = "{0}: {1}".format(path, res)
+            message = f"{path}: {res}"
         else:
             kind = graph.value(result, sh.sourceConstraintComponent)
             focus_node = graph.value(result, sh.focusNode)
 
             if isinstance(focus_node, BNode):
                 focus_node = "<Anonymous>"
 
-            message = "{0}: Type: {1}, Node ID: {2}".format(path, kind, focus_node)
+            message = f"{path}: Type: {kind}, Node ID: {focus_node}"
 
         problems.append(message)
 
     return "\n\t".join(problems)
 
 
 def check_project_structure(**_):
@@ -78,15 +76,15 @@
     data = ProjectSchema().dump(project_context.project)
 
     conform, graph, t = _check_shacl_structure(data)
 
     if conform:
         return True, None
 
-    problems = "{0}Invalid structure of project metadata\n\t{1}".format(WARNING, _shacl_graph_to_string(graph))
+    problems = f"{WARNING}Invalid structure of project metadata\n\t{_shacl_graph_to_string(graph)}"
 
     return False, problems
 
 
 @inject.autoparams("dataset_gateway")
 def check_datasets_structure(dataset_gateway: IDatasetGateway, **_):
     """Validate dataset metadata against SHACL.
```

### Comparing `renku-2.3.2/renku/command/checks/workflow.py` & `renku-2.4.0rc1/renku/command/checks/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/clone.py` & `renku-2.4.0rc1/renku/command/clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/command_builder/__init__.py` & `renku-2.4.0rc1/renku/command/command_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/command_builder/command.py` & `renku-2.4.0rc1/renku/command/command_builder/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/command_builder/communication.py` & `renku-2.4.0rc1/renku/command/command_builder/communication.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/command_builder/database.py` & `renku-2.4.0rc1/renku/command/command_builder/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -78,15 +76,15 @@
 
         try:
             project = project_gateway.get_project()
             minimum_renku_version = Version(project.minimum_renku_version)
             self.project_found = True
         except (KeyError, ImportError, ValueError):
             try:
-                with open(project_context.database_path / "project", "r") as f:
+                with open(project_context.database_path / "project") as f:
                     project = json.load(f)
                     min_version = project.get("minimum_renku_version")
                     if min_version is None:
                         return
                     minimum_renku_version = Version(min_version)
             except (KeyError, OSError, json.JSONDecodeError):
                 # NOTE: We don't check minimum version if there's no project metadata available
```

### Comparing `renku-2.3.2/renku/command/command_builder/lock.py` & `renku-2.4.0rc1/renku/command/command_builder/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/command_builder/migration.py` & `renku-2.4.0rc1/renku/command/command_builder/migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/command_builder/repo.py` & `renku-2.4.0rc1/renku/command/command_builder/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/config.py` & `renku-2.4.0rc1/renku/command/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -35,15 +34,15 @@
         key: The config key.
 
     Returns:
         Tuple of "renku" and the supplied key.
     """
     parts = key.split(".")
     if len(parts) > 1:
-        return "{0}".format(parts[0]), ".".join(parts[1:])
+        return f"{parts[0]}", ".".join(parts[1:])
     return "renku", key
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def _update_multiple_config(
     values: Dict[str, Optional[str]], global_only: bool = False, commit_message: Optional[str] = None
 ):
@@ -94,15 +93,15 @@
     Returns:
         The modified/removed value.
     """
     section, section_key = _split_section_and_key(key)
     if remove:
         value = remove_value(section, section_key, global_only=global_only)
         if value is None:
-            raise errors.ParameterError('Key "{}" not found.'.format(key))
+            raise errors.ParameterError(f'Key "{key}" not found.')
     else:
         set_value(section, section_key, value, global_only=global_only)
         return value
 
 
 def update_config():
     """Command for updating config."""
```

### Comparing `renku-2.3.2/renku/command/dataset.py` & `renku-2.4.0rc1/renku/command/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -14,29 +13,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Repository datasets management."""
 
 from renku.command.command_builder.command import Command
-from renku.core.constant import CONFIG_LOCAL_PATH, DATASET_METADATA_PATHS
+from renku.core.constant import DATASET_METADATA_PATHS
 from renku.core.dataset.dataset import (
     create_dataset,
     edit_dataset,
     export_dataset,
     file_unlink,
     import_dataset,
     list_dataset_files,
     list_datasets,
-    mount_external_storage,
-    pull_external_data,
+    mount_cloud_storage,
+    pull_cloud_storage,
     remove_dataset,
     search_datasets,
     show_dataset,
-    unmount_external_storage,
+    unmount_cloud_storage,
     update_datasets,
 )
 from renku.core.dataset.dataset_add import add_to_dataset
 from renku.core.dataset.tag import add_dataset_tag, list_dataset_tags, remove_dataset_tags
 
 
 def search_datasets_command():
@@ -124,22 +123,22 @@
 
 
 def list_tags_command():
     """Command for listing a dataset's tags."""
     return Command().command(list_dataset_tags).with_database().require_migration()
 
 
-def pull_external_data_command():
-    """Command for pulling/copying data from an external storage."""
-    command = Command().command(pull_external_data).lock_dataset().with_database(write=True)
-    return command.require_migration().with_commit(commit_only=DATASET_METADATA_PATHS + [CONFIG_LOCAL_PATH])
+def pull_cloud_storage_command():
+    """Command for pulling/copying data from a cloud storage."""
+    command = Command().command(pull_cloud_storage).lock_dataset().with_database(write=True)
+    return command.require_migration().with_commit(commit_only=DATASET_METADATA_PATHS)
 
 
-def mount_external_storage_command(unmount: bool):
-    """Command for mounting an external storage."""
-    command = unmount_external_storage if unmount else mount_external_storage
+def mount_cloud_storage_command(unmount: bool):
+    """Command for mounting a cloud storage."""
+    command = unmount_cloud_storage if unmount else mount_cloud_storage
     return Command().command(command).lock_dataset().with_database(write=False).require_migration()
 
 
-def unmount_external_storage_command():
-    """Command for unmounting an external storage."""
-    return Command().command(unmount_external_storage).lock_dataset().with_database(write=False).require_migration()
+def unmount_cloud_storage_command():
+    """Command for unmounting a cloud storage."""
+    return Command().command(unmount_cloud_storage).lock_dataset().with_database(write=False).require_migration()
```

### Comparing `renku-2.3.2/renku/command/doctor.py` & `renku-2.4.0rc1/renku/command/doctor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/command/format/__init__.py` & `renku-2.4.0rc1/renku/infrastructure/storage/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Serializers for different output formats."""
+"""Renku remote storage implementations."""
```

### Comparing `renku-2.3.2/renku/command/format/activity.py` & `renku-2.4.0rc1/renku/command/format/activity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2021 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -33,18 +31,21 @@
         modified_inputs(Set[str]): Set of modified inputs for activities.
 
     Returns:
         String of activities in tabular representation.
     """
     collection = []
     fields = "plan,execution_date,modified_inputs,outputs,command"
-    ActivityDisplay = NamedTuple(
-        "ActivityDisplay",
-        [("plan", str), ("execution_date", datetime), ("modified_inputs", str), ("outputs", str), ("command", str)],
-    )
+
+    class ActivityDisplay(NamedTuple):
+        plan: str
+        execution_date: datetime
+        modified_inputs: str
+        outputs: str
+        command: str
 
     for activity in activities:
         modified_usages = {
             u.entity.path for u in activity.usages if any(are_paths_related(u.entity.path, m) for m in modified_inputs)
         }
         generations = {g.entity.path for g in activity.generations}
         modified_inputs |= generations
```

### Comparing `renku-2.3.2/renku/command/format/dataset_files.py` & `renku-2.4.0rc1/renku/command/format/dataset_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Serializers for dataset list files."""
 
 import re
 from subprocess import PIPE, SubprocessError, run
-from typing import Callable, Dict
+from typing import Callable, Dict, Optional, Union
 
 from renku.domain_model.project_context import project_context
 
 
 def tabular(records, *, columns=None):
     """Format dataset files with a tabular output.
 
@@ -58,87 +56,102 @@
         has_tag(bool): Whether sizes are retrieved for a given tag instead of HEAD commit
     """
     from humanize import naturalsize  # Slow import
 
     repository = project_context.repository
 
     def get_lfs_tracking():
+        if has_tag:
+            return
+
         paths = (r.path for r in records)
         attrs = repository.get_attributes(*paths)
 
         for record in records:
             if attrs.get(str(record.path), {}).get("filter") == "lfs":
                 record.is_lfs = True
             else:
                 record.is_lfs = False
 
-    lfs_files_sizes = {}
+    def naturalize(value) -> str:
+        return naturalsize(value).upper().replace("BYTES", " B")
 
-    try:
-        lfs_run = run(
-            ("git", "lfs", "ls-files", "--name-only", "--size", "--deleted"),
-            stdout=PIPE,
-            cwd=project_context.path,
-            universal_newlines=True,
-        )
-    except SubprocessError:
-        pass
-    else:
-        lfs_output = lfs_run.stdout.split("\n")
-        # Example line format: relative/path/to/file (7.9 MB)
-        pattern = re.compile(r"^(.*?)\s*\((.*)\)")
-
-        for line in lfs_output:
-            match = pattern.search(line)
-            if not match:
-                continue
-            path, size = match.groups()
-            # Fix alignment for bytes
-            if size.endswith(" B"):
-                size = size.replace(" B", "  B")
-            lfs_files_sizes[path] = size
-
-    if has_tag:
-        checksums = [r.entity.checksum for r in records]
-        sizes = repository.get_sizes(*checksums)
-        non_lfs_files_sizes = {
-            r.entity.path: naturalsize(s).upper().replace("BYTES", " B") for r, s in zip(records, sizes)
-        }
-    else:
-        non_lfs_files_sizes = {
-            o.path: o.size for o in repository.head.commit.traverse() if o.path not in lfs_files_sizes
-        }
-        non_lfs_files_sizes = {k: naturalsize(v).upper().replace("BYTES", " B") for k, v in non_lfs_files_sizes.items()}
+    def get_file_sizes():
+        if not any(r for r in records if r.size is None):  # All records already have a size
+            return {}, {}
+
+        lfs_files_sizes = {}
+
+        try:
+            lfs_run = run(
+                ("git", "lfs", "ls-files", "--name-only", "--size", "--deleted"),
+                stdout=PIPE,
+                cwd=project_context.path,
+                text=True,
+            )
+        except SubprocessError:
+            pass
+        else:
+            lfs_output = lfs_run.stdout.split("\n")
+            # Example line format: relative/path/to/file (7.9 MB)
+            pattern = re.compile(r"^(.*?)\s*\((.*)\)")
+
+            for line in lfs_output:
+                match = pattern.search(line)
+                if not match:
+                    continue
+                path, size = match.groups()
+                # Fix alignment for bytes
+                if size.endswith(" B"):
+                    size = size.replace(" B", "  B")
+                lfs_files_sizes[path] = size
 
-        # NOTE: Check .gitattributes file to see if a file is in LFS
-        get_lfs_tracking()
+        non_lfs_files_sizes: Dict[str, Optional[Union[int, str]]]
+        if has_tag:
+            checksums = [r.entity.checksum for r in records]
+            sizes = repository.get_sizes(*checksums)
+            non_lfs_files_sizes = {k.entity.path: naturalize(v) for k, v in zip(records, sizes)}
+        else:
+            non_lfs_files_sizes = {
+                o.path: o.size for o in repository.head.commit.traverse() if o.path not in lfs_files_sizes
+            }
+            non_lfs_files_sizes = {k: naturalize(v) for k, v in non_lfs_files_sizes.items()}
+
+        return lfs_files_sizes, non_lfs_files_sizes
+
+    lfs_files_sizes, non_lfs_files_sizes = get_file_sizes()
+    get_lfs_tracking()
 
     for record in records:
-        size = lfs_files_sizes.get(record.path) or non_lfs_files_sizes.get(record.path)
-        record.size = size
+        size = (
+            lfs_files_sizes.get(record.path) or non_lfs_files_sizes.get(record.path) or None
+            if record.size is None
+            else naturalize(record.size)
+        )
+        record.size = size if size or size == 0 else None
 
         # NOTE: When listing a tag we assume that the file is in LFS if it was in LFS at some point in time
         if has_tag:
             record.is_lfs = lfs_files_sizes.get(record.path) is not None
 
 
-def jsonld(records, **kwargs):
+def jsonld(records, **_):
     """Format dataset files as JSON-LD.
 
     Args:
         records: Filtered collection.
     """
     from renku.command.format.json import dumps
     from renku.command.schema.dataset import DatasetFileSchema
 
     data = [DatasetFileSchema(flattened=True).dump(record) for record in records]
     return dumps(data, indent=2)
 
 
-def json(records, **kwargs):
+def json(records, **_):
     """Format dataset files as JSON.
 
     Args:
         records: Filtered collection.
 
     Returns:
         String of records in JSON representation.
```

### Comparing `renku-2.3.2/renku/command/format/dataset_tags.py` & `renku-2.4.0rc1/renku/command/format/dataset_tags.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/format/datasets.py` & `renku-2.4.0rc1/renku/command/format/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/format/json.py` & `renku-2.4.0rc1/renku/command/format/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/format/session.py` & `renku-2.4.0rc1/renku/command/format/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2021 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/format/tabulate.py` & `renku-2.4.0rc1/renku/command/format/tabulate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/format/workflow.py` & `renku-2.4.0rc1/renku/command/format/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2021 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/gc.py` & `renku-2.4.0rc1/renku/command/gc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/command/githooks.py` & `renku-2.4.0rc1/renku/command/githooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/graph.py` & `renku-2.4.0rc1/renku/command/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/group.py` & `renku-2.4.0rc1/renku/command/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,8 +22,8 @@
 class OptionalGroup(click.Group):
     """Add support for an optional argument."""
 
     def parse_args(self, ctx, args):
         """Check if the first argument is an existing command."""
         if args and args[0] in self.commands:
             args.insert(0, "")
-        super(OptionalGroup, self).parse_args(ctx, args)
+        super().parse_args(ctx, args)
```

### Comparing `renku-2.3.2/renku/command/init.py` & `renku-2.4.0rc1/renku/command/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/command/log.py` & `renku-2.4.0rc1/renku/command/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/login.py` & `renku-2.4.0rc1/renku/command/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/mergetool.py` & `renku-2.4.0rc1/renku/command/mergetool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -65,14 +64,14 @@
     if not with_attributes:
         return
 
     attributes_path = project_context.path / ".gitattributes"
     pattern_string = ".renku/metadata/**    merge=renkumerge\n"
 
     if attributes_path.exists():
-        with open(attributes_path, "r") as f:
+        with open(attributes_path) as f:
             content = f.readlines()
             if pattern_string in content:
                 return
 
     with open(attributes_path, "a") as f:
         f.write(pattern_string)
```

### Comparing `renku-2.3.2/renku/command/migrate.py` & `renku-2.4.0rc1/renku/command/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/move.py` & `renku-2.4.0rc1/renku/command/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -177,15 +176,15 @@
         f"The following move target exist, use '--force' flag to overwrite them:\n\t{existing_str}"
     )
 
 
 def _warn_about_ignored_destinations(destinations):
     ignored = project_context.repository.get_ignored_paths(*destinations)
     if ignored:
-        ignored_str = "\n\t".join((str(Path(p).relative_to(project_context.path)) for p in ignored))
+        ignored_str = "\n\t".join(str(Path(p).relative_to(project_context.path)) for p in ignored)
         communication.warn(f"The following moved path match .gitignore:\n\t{ignored_str}")
 
 
 def _warn_about_git_filters(files):
     """Check if there are any git attributes for files including LFS.
 
     Args:
```

### Comparing `renku-2.3.2/renku/command/options.py` & `renku-2.4.0rc1/renku/command/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/project.py` & `renku-2.4.0rc1/renku/command/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/remove.py` & `renku-2.4.0rc1/renku/command/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -16,34 +15,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Remove a file, a directory, or a symlink."""
 
 import os
 from pathlib import Path
 from subprocess import run
-from typing import List
+from typing import List, Protocol, runtime_checkable
 
 from pydantic import validate_arguments
 
 from renku.command.command_builder import inject
 from renku.command.command_builder.command import Command
 from renku.core import errors
 from renku.core.dataset.datasets_provenance import DatasetsProvenance
 from renku.core.interface.dataset_gateway import IDatasetGateway
 from renku.core.storage import check_external_storage, untrack_paths_from_storage
 from renku.core.util import communication
 from renku.core.util.git import get_git_user
 from renku.core.util.os import delete_dataset_file, expand_directories
 from renku.domain_model.project_context import project_context
 
-try:
-    from typing_extensions import Protocol, runtime_checkable  # NOTE: Required for Python 3.7 compatibility
-except ImportError:
-    from typing import Protocol, runtime_checkable  # type: ignore
-
 
 @runtime_checkable
 class EditCommandCallable(Protocol):
     """Typing Protocol for edit command."""
 
     def __call__(self, filename: str) -> None:
         """The call method."""
@@ -108,15 +102,15 @@
         existing = repository.get_attributes(*tracked)
         if existing:
             communication.warn("There are custom .gitattributes.\n")
             if communication.confirm('Do you want to edit ".gitattributes" now?'):
                 edit_command(filename=str(project_context.path / ".gitattributes"))
 
     # Finally remove the files.
-    files_to_remove = set(str(project_context.path / f) for f in files.values())
+    files_to_remove = {str(project_context.path / f) for f in files.values()}
     final_sources = list(files_to_remove)
     if final_sources:
         run(["git", "rm", "-rf"] + final_sources, check=True)
 
 
 def remove_command():
     """Command to remove a file."""
```

### Comparing `renku-2.3.2/renku/command/rerun.py` & `renku-2.4.0rc1/renku/command/rerun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/rollback.py` & `renku-2.4.0rc1/renku/command/rollback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/run.py` & `renku-2.4.0rc1/renku/command/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/save.py` & `renku-2.4.0rc1/renku/command/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/__init__.py` & `renku-2.4.0rc1/renku/core/workflow/providers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""JSON-LD schemes for core models."""
+"""Renku workflow providers."""
```

### Comparing `renku-2.3.2/renku/command/schema/activity.py` & `renku-2.4.0rc1/renku/command/schema/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -105,27 +103,27 @@
         rdf_type = prov.Activity
         model = Activity
         unknown = EXCLUDE
 
     agents = Nested(prov.wasAssociatedWith, [PersonSchema, SoftwareAgentSchema], many=True)
     annotations = Nested(oa.hasTarget, AnnotationSchema, reverse=True, many=True)
     association = Nested(prov.qualifiedAssociation, AssociationSchema)
-    ended_at_time = fields.DateTime(prov.endedAtTime, add_value_types=True)
+    ended_at_time = fields.DateTime(prov.endedAtTime, format="iso", add_value_types=True)
     generations = Nested(prov.activity, GenerationSchema, reverse=True, many=True, load_default=None)
     id = fields.Id()
     invalidations = Nested(prov.wasInvalidatedBy, EntitySchema, reverse=True, many=True, load_default=None)
     parameters = Nested(
         renku.parameter,
         ParameterValueSchema,
         many=True,
         load_default=None,
     )
     path = fields.String(prov.atLocation)
     project_id = fields.IRI(renku.hasActivity, reverse=True)
-    started_at_time = fields.DateTime(prov.startedAtTime, add_value_types=True)
+    started_at_time = fields.DateTime(prov.startedAtTime, format="iso", add_value_types=True)
     usages = Nested(prov.qualifiedUsage, UsageSchema, many=True)
 
     @pre_dump(pass_many=True)
     def removes_ms(self, objs, many, **kwargs):
         """Remove milliseconds from datetimes.
 
         Note: since DateField uses `strftime` as format, which only supports timezone info without a colon
```

### Comparing `renku-2.3.2/renku/command/schema/agent.py` & `renku-2.4.0rc1/renku/command/schema/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/annotation.py` & `renku-2.4.0rc1/renku/command/schema/annotation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/calamus.py` & `renku-2.4.0rc1/renku/command/schema/calamus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -101,15 +99,15 @@
         if not value:
             return None
         elif isinstance(value, str):
             return value
         elif isinstance(value, dict):
             return super(marshmallow.fields.String, self)._deserialize(value, attr, data, **kwargs)
         else:
-            raise ValueError("Invalid type for field {}: {}".format(self.name, type(value)))
+            raise ValueError(f"Invalid type for field {self.name}: {type(value)}")
 
 
 class StringList(fields.String):
     """A String field that might be a list when deserializing."""
 
     def __init__(self, *args, return_max_value=True, **kwargs):
         """Create an instance."""
```

### Comparing `renku-2.3.2/renku/command/schema/composite_plan.py` & `renku-2.4.0rc1/renku/command/schema/composite_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/dataset.py` & `renku-2.4.0rc1/renku/command/schema/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/entity.py` & `renku-2.4.0rc1/renku/command/schema/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/parameter.py` & `renku-2.4.0rc1/renku/command/schema/parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/plan.py` & `renku-2.4.0rc1/renku/command/schema/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/project.py` & `renku-2.4.0rc1/renku/command/schema/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/schema/workflow_file.py` & `renku-2.4.0rc1/renku/command/schema/workflow_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/session.py` & `renku-2.4.0rc1/renku/command/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/status.py` & `renku-2.4.0rc1/renku/command/status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/storage.py` & `renku-2.4.0rc1/renku/command/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/template.py` & `renku-2.4.0rc1/renku/command/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/command/update.py` & `renku-2.4.0rc1/renku/core/workflow/update.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,57 +11,45 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku ``update`` command."""
+"""Renku workflow update."""
 
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import validate_arguments
 
-from renku.command.command_builder.command import Command
 from renku.core import errors
 from renku.core.errors import ParameterError
 from renku.core.util.os import get_relative_paths
 from renku.core.workflow.activity import (
     get_all_modified_and_deleted_activities_and_entities,
     get_downstream_generating_activities,
     is_activity_valid,
     sort_activities,
 )
 from renku.core.workflow.execute import execute_workflow_graph
 from renku.core.workflow.model.concrete_execution_graph import ExecutionGraph
 from renku.domain_model.project_context import project_context
 
 
-def update_command(skip_metadata_update: bool):
-    """Update existing files by rerunning their outdated workflow."""
-    command = Command().command(_update).require_migration().require_clean()
-    if skip_metadata_update:
-        command = command.with_database(write=False)
-    else:
-        command = command.with_database(write=True).with_commit()
-    return command
-
-
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
-def _update(
+def update(
     update_all: bool,
     dry_run: bool,
     ignore_deleted: bool,
     provider: str,
     config: Optional[str],
     paths: Optional[List[str]] = None,
 ):
-    if not paths and not update_all and not dry_run:
-        raise ParameterError("Either PATHS, --all/-a, or --dry-run/-n should be specified.")
+    """Update stale generated outputs."""
     if paths and update_all:
         raise ParameterError("Cannot use PATHS and --all/-a at the same time.")
 
     paths = paths or []
     paths = get_relative_paths(base=project_context.path, paths=[Path.cwd() / p for p in paths])
 
     modified, _, _ = get_all_modified_and_deleted_activities_and_entities(project_context.repository)
```

### Comparing `renku-2.3.2/renku/command/util.py` & `renku-2.4.0rc1/renku/command/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/command/view_model/__init__.py` & `renku-2.4.0rc1/renku/ui/api/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku commands view models module."""
+"""Renku API Models."""
```

### Comparing `renku-2.3.2/renku/command/view_model/activity_graph.py` & `renku-2.4.0rc1/renku/command/view_model/activity_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/agent.py` & `renku-2.4.0rc1/renku/command/view_model/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/composite_plan.py` & `renku-2.4.0rc1/renku/command/view_model/composite_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -34,15 +32,22 @@
 )
 from renku.domain_model.workflow.plan import AbstractPlan
 
 if TYPE_CHECKING:
     from renku.command.view_model.plan import PlanViewModel
 
 
-ParameterReference = NamedTuple("ParameterReference", [("id", str), ("plan_id", str), ("type", str), ("name", str)])
+class ParameterReference(NamedTuple):
+    """Reference to a workflow parameter."""
+
+    id: str
+    plan_id: str
+    type: str
+    name: str
+
 
 parameter_type_mapping: Dict[type, str] = {
     CommandInput: "Input",
     CommandOutput: "Output",
     CommandParameter: "Parameter",
     ParameterMapping: "Mapping",
 }
```

### Comparing `renku-2.3.2/renku/command/view_model/dataset.py` & `renku-2.4.0rc1/renku/command/view_model/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/graph.py` & `renku-2.4.0rc1/renku/command/view_model/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -137,15 +135,15 @@
         """
         types = collections.defaultdict(set)
         fields = collections.defaultdict(set)
         nodes: Dict[str, str] = {}
 
         def node(x):
             """Return a name of the given node."""
-            return nodes.setdefault(x, "node{0}".format(len(nodes)))
+            return nodes.setdefault(x, f"node{len(nodes)}")
 
         def label(x, g):
             """Generate a label for the node."""
             for labelProp in LABEL_PROPERTIES:
                 label_ = g.value(x, labelProp)
                 if label_:
                     return label_
@@ -155,17 +153,17 @@
             except Exception:
                 return x
 
         def formatliteral(literal, g):
             """Format and escape literal."""
             v = html.escape(literal)
             if literal.datatype:
-                return "&quot;%s&quot;^^%s" % (v, qname(literal.datatype, g))
+                return f"&quot;{v}&quot;^^{qname(literal.datatype, g)}"
             elif literal.language:
-                return "&quot;%s&quot;@%s" % (v, literal.language)
+                return f"&quot;{v}&quot;@{literal.language}"
             return "&quot;%s&quot;" % v
 
         def qname(x, g):
             """Compute qname."""
             try:
                 q = g.compute_qname(x)
                 return q[0] + ":" + q[2]
@@ -208,15 +206,15 @@
                 on = node(o)
                 opstr = '\t%s -> %s [ color=%s, label=< <font point-size="12" ' 'color="#336633">%s</font> > ] ;\n'
                 output.write(opstr % (sn, on, color(p), qname(p, graph)))
             else:
                 fields[sn].add((qname(p, graph), formatliteral(o, graph)))
 
         for u, n in nodes.items():
-            output.write("# %s %s\n" % (u, n))
+            output.write(f"# {u} {n}\n")
             f = [
                 '<tr><td align="left"><b>%s</b></td><td align="left">' "<b>%s</b></td></tr>" % x
                 for x in sorted(types[n])
             ]
             f += ['<tr><td align="left">%s</td><td align="left">%s</td></tr>' % x for x in sorted(fields[n])]
             opstr = (
                 '%s [ shape=none, color=%s label=< <table color="#666666"'
```

### Comparing `renku-2.3.2/renku/command/view_model/log.py` & `renku-2.4.0rc1/renku/command/view_model/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/plan.py` & `renku-2.4.0rc1/renku/command/view_model/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/project.py` & `renku-2.4.0rc1/renku/command/view_model/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/view_model/template.py` & `renku-2.4.0rc1/renku/command/view_model/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -25,58 +23,61 @@
 
 
 class TemplateViewModel:
     """A view model for a ``Template``."""
 
     def __init__(
         self,
+        aliases: List[str],
         description: str,
         icon: Optional[str],
         id: str,
         immutable_files: Optional[List[str]],
         name: str,
+        parameters: List[TemplateParameter],
         reference: Optional[str],
         source: Optional[str],
-        parameters: List[TemplateParameter],
         version: Optional[str],
         versions: List[str],
     ):
+        self.aliases: List[str] = aliases
         self.description: str = description
         self.icon = icon
         self.id: str = id
         self.immutable_files: Optional[List[str]] = immutable_files
         self.name: str = name
-        self.reference = reference
-        self.source = source
         self.parameters: List[TemplateParameterViewModel] = [
             TemplateParameterViewModel.from_template_parameter(p) for p in parameters
         ]
+        self.reference = reference
+        self.source = source
         self.version = version
         self.versions = versions
 
     @classmethod
     def from_template(cls, template: Template) -> "TemplateViewModel":
         """Create view model from ``Template``.
 
         Args:
             template(Template): The input template.
 
         Returns:
             TemplateViewModel: View model for a template.
         """
         return cls(
-            source=template.source,
-            reference=template.reference,
-            version=template.version,
-            id=template.id,
-            name=template.name,
+            aliases=template.aliases,
             description=template.description,
-            parameters=template.parameters,
             icon=template.icon,
+            id=template.id,
             immutable_files=template.immutable_files,
+            name=template.name,
+            parameters=template.parameters,
+            reference=template.reference,
+            source=template.source,
+            version=template.version,
             versions=template.get_all_references(),
         )
 
 
 class TemplateParameterViewModel:
     """A view model for a ``TemplateParameter``."""
 
@@ -113,29 +114,39 @@
         )
 
 
 class TemplateChangeViewModel:
     """A view model for resulting changes from a template set/update."""
 
     def __init__(
-        self, id: str, source: Optional[str], reference: Optional[str], version: Optional[str], file_changes: List[str]
+        self,
+        file_changes: List[str],
+        id: str,
+        old_id: Optional[str],
+        reference: Optional[str],
+        source: Optional[str],
+        version: Optional[str],
     ):
+        self.file_changes = file_changes
         self.id: str = id
-        self.source = source
+        self.old_id: Optional[str] = old_id if old_id != id else ""
         self.reference = reference
+        self.source = source
         self.version = version
-        self.file_changes = file_changes
 
     @classmethod
-    def from_template(cls, template: RenderedTemplate, actions: Dict[str, FileAction]) -> "TemplateChangeViewModel":
+    def from_template(
+        cls, template: RenderedTemplate, actions: Dict[str, FileAction], old_id: Optional[str] = None
+    ) -> "TemplateChangeViewModel":
         """Create view model from ``Template``.
 
         Args:
             template(RenderedTemplate): Input rendered template.
             actions(Dict[str, FileAction]): Mapping of paths to actions taken when rendering the template.
+            old_id(Optional[str]: Current template Id.
 
         Returns:
             TemplateChangeViewModel: View model for the template change.
         """
         actions_mapping: Dict[FileAction, str] = {
             FileAction.APPEND: "Append to",
             FileAction.CREATE: "Initialize",
@@ -149,13 +160,14 @@
 
         file_changes = [
             f"{actions_mapping[action]} {relative_path} ..."
             for relative_path, action in get_sorted_actions(actions=actions).items()
         ]
 
         return cls(
+            file_changes=file_changes,
             id=template.template.id,
-            source=template.template.source,
+            old_id=old_id,
             reference=template.template.reference,
+            source=template.template.source,
             version=template.template.version,
-            file_changes=file_changes,
         )
```

### Comparing `renku-2.3.2/renku/command/view_model/text_canvas.py` & `renku-2.4.0rc1/renku/command/view_model/text_canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -24,15 +22,21 @@
 
 import numpy as np
 from click import style
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
-Point = NamedTuple("Point", [("x", int), ("y", int)])
+
+class Point(NamedTuple):
+    """A point with coordinates for rendering."""
+
+    x: int
+    y: int
+
 
 MAX_NODE_LENGTH = 40
 
 
 class Shape:
     """basic shape class that all shapes inherit from."""
```

### Comparing `renku-2.3.2/renku/command/view_model/workflow_file.py` & `renku-2.4.0rc1/renku/command/view_model/workflow_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/command/workflow.py` & `renku-2.4.0rc1/renku/command/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/__init__.py` & `renku-2.4.0rc1/renku/core/workflow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku core."""
+"""Renku workflow management."""
```

### Comparing `renku-2.3.2/renku/core/config.py` & `renku-2.4.0rc1/renku/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/constant.py` & `renku-2.4.0rc1/renku/core/constant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/dataset/__init__.py` & `renku-2.4.0rc1/renku/core/interface/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku management dataset logic."""
+"""Renku management interfaces."""
```

### Comparing `renku-2.3.2/renku/core/dataset/context.py` & `renku-2.4.0rc1/renku/core/dataset/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/dataset/dataset.py` & `renku-2.4.0rc1/renku/core/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -27,48 +25,57 @@
 from pydantic import validate_arguments
 
 from renku.command.command_builder.command import inject
 from renku.command.view_model.dataset import DatasetFileViewModel, DatasetViewModel
 from renku.core import errors
 from renku.core.config import get_value, remove_value, set_value
 from renku.core.dataset.datasets_provenance import DatasetsProvenance
-from renku.core.dataset.pointer_file import create_external_file, is_external_file_updated, update_external_file
+from renku.core.dataset.pointer_file import (
+    create_external_file,
+    delete_external_file,
+    is_linked_file_updated,
+    update_linked_file,
+)
 from renku.core.dataset.providers.factory import ProviderFactory
 from renku.core.dataset.providers.models import ProviderDataset
 from renku.core.dataset.request_model import ImageRequestModel
 from renku.core.dataset.tag import get_dataset_by_tag, prompt_access_token, prompt_tag_selection
 from renku.core.interface.dataset_gateway import IDatasetGateway
 from renku.core.storage import check_external_storage, pull_paths_from_storage, track_paths_in_storage
 from renku.core.util import communication
 from renku.core.util.datetime8601 import local_now
 from renku.core.util.git import clone_repository, get_cache_directory_for_repository, get_git_user
-from renku.core.util.metadata import is_external_file, prompt_for_credentials, read_credentials, store_credentials
+from renku.core.util.metadata import is_linked_file, prompt_for_credentials, read_credentials, store_credentials
 from renku.core.util.os import (
     create_symlink,
     delete_dataset_file,
     delete_path,
     get_absolute_path,
+    get_file_size,
     get_files,
     get_safe_relative_path,
     hash_file,
     is_path_empty,
     is_subpath,
     unmount_path,
 )
 from renku.core.util.tabulate import tabulate
 from renku.core.util.urls import get_slug
-from renku.core.util.util import NO_VALUE, NoValueType
+from renku.core.util.util import parallel_execute
+from renku.domain_model.constant import NO_VALUE, NON_EXISTING_ENTITY_CHECKSUM, NoValueType
 from renku.domain_model.dataset import Dataset, DatasetDetailsJson, DatasetFile, RemoteEntity, is_dataset_name_valid
+from renku.domain_model.entity import Entity
 from renku.domain_model.enums import ConfigFilter
 from renku.domain_model.project_context import project_context
 from renku.domain_model.provenance.agent import Person
 from renku.domain_model.provenance.annotation import Annotation
 from renku.infrastructure.immutable import DynamicProxy
 
 if TYPE_CHECKING:
+    from renku.core.interface.storage import IStorage
     from renku.infrastructure.repository import Repository
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def search_datasets(name: str) -> List[str]:
     """Get all the datasets whose name starts with the given string.
 
@@ -306,73 +313,87 @@
 
     get_lfs_tracking_and_file_sizes(records, has_tag=bool(tag))
 
     return records
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
-def file_unlink(name: str, include: Optional[List[str]], exclude: Optional[List[str]], yes: bool = False):
+def file_unlink(
+    name: str,
+    include: Optional[List[str]] = None,
+    exclude: Optional[List[str]] = None,
+    yes: bool = False,
+    dataset_files: Optional[List[DatasetFile]] = None,
+):
     """Remove matching files from a dataset.
 
     Args:
         name(str): Dataset name.
-        include(Optional[List[str]]): Include filter for files.
-        exclude(Optional[List[str]]): Exclude filter for files.
+        include(Optional[List[str]]): Include filter for files (Default value = None).
+        exclude(Optional[List[str]]): Exclude filter for files (Default value = None).
         yes(bool): Whether to skip user confirmation or not (Default value = False).
+        dataset_files(Optional[List[DatasetFile]]): Files to remove; ignore include and exclude if passed (Default value
+            = None).
 
     Returns:
         List[DynamicProxy]: List of files that were removed.
     """
     repository = project_context.repository
 
-    if not include and not exclude:
+    if not include and not exclude and not dataset_files:
         raise errors.ParameterError("include or exclude filters not specified.")
 
     datasets_provenance = DatasetsProvenance()
 
     dataset = datasets_provenance.get_by_name(name=name)
 
     if not dataset:
         raise errors.ParameterError("Dataset does not exist.")
 
-    records = filter_dataset_files(names=[name], include=include, exclude=exclude)
-    if not records:
-        raise errors.ParameterError("No records found.")
+    records = []
+    if not dataset_files:
+        records = filter_dataset_files(names=[name], include=include, exclude=exclude)
+        if not records:
+            raise errors.ParameterError("No records found.")
+        dataset_files = [cast(DatasetFile, r) for r in records]
 
     if not yes:
         prompt_text = (
             f'You are about to remove following from "{name}" dataset.'
             + "\n"
-            + "\n".join([str(record.entity.path) for record in records])
+            + "\n".join([str(record.entity.path) for record in dataset_files])
             + "\nDo you wish to continue?"
         )
         communication.confirm(prompt_text, abort=True, warning=True)
 
-    dataset_datadir = dataset.get_datadir()
-    for file in records:
+    for file in dataset_files:
         dataset.unlink_file(file.entity.path)
         path_file = Path(file.entity.path)
-        # INFO: Remove actual dataset file only if it is located within dataset directory
-        if str(path_file.absolute()).startswith(str(dataset_datadir.absolute())):
+
+        if file.is_external or file.linked:
+            try:
+                delete_external_file(file)
+            except errors.InvalidFileOperation as e:
+                communication.warn(f"Cannot delete dataset file {path_file}: {e}.")
+        elif dataset.is_within_datadir(path_file):  # NOTE: Remove dataset file only if it's inside dataset's datadir
+            datadir = dataset.get_datadir()
+
             if not path_file.exists():
-                communication.warn(
-                    f"Dataset file {path_file} could not be found, skipping the removal from {dataset_datadir}."
-                )
+                communication.warn(f"Dataset file {path_file} doesn't exist, skipping the removal from {datadir}.")
                 continue
+
             try:
                 if path_file.is_dir():
                     shutil.rmtree(str(path_file.absolute()), ignore_errors=False, onerror=None)
                 else:
                     path_file.unlink()
             except Exception as err:
-                communication.warn(
-                    f"Dataset file {path_file} could not be removed from {dataset_datadir} because of {err}."
-                )
-            else:
-                repository.add(path_file)
+                communication.warn(f"Dataset file {path_file} could not be removed from {datadir} because of {err}.")
+
+        repository.add(path_file)
 
     datasets_provenance.add_or_update(dataset, creator=get_git_user(repository))
 
     return records
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
@@ -569,15 +590,14 @@
 def update_datasets(
     names: List[str],
     creators: Optional[str],
     include: Optional[List[str]],
     exclude: Optional[List[str]],
     ref: Optional[str],
     delete: bool,
-    no_external: bool,
     no_local: bool,
     no_remote: bool,
     check_data_directory: bool,
     update_all: bool,
     dry_run: bool,
     plain: bool,
     dataset_gateway: IDatasetGateway,
@@ -587,15 +607,14 @@
     Args:
         names(List[str]): Names of datasets to update.
         creators(Optional[str]): Creators to filter dataset files by.
         include(Optional[List[str]]): Include filter for paths to update.
         exclude(Optional[List[str]]): Exclude filter for paths to update.
         ref(Optional[str]): Git reference to use for update.
         delete(bool): Whether to delete files that don't exist on remote anymore.
-        no_external(bool): Whether to exclude external files from the update.
         no_local(bool): Whether to exclude local files from the update.
         no_remote(bool): Whether to exclude remote files from the update.
         check_data_directory(bool): Whether to check the dataset's data directory for new files.
         update_all(bool): Whether to update all datasets.
         dry_run(bool): Whether to return a preview of what would be updated.
         plain(bool): Whether plain output should be produced.
         dataset_gateway(IDatasetGateway): Injected dataset gateway.
@@ -693,37 +712,37 @@
     if not records:
         if must_match_records and not plain:
             raise errors.ParameterError("No files matched the criteria.")
         return imported_dataset_updates_view_models, []
 
     git_files = []
     unique_remotes = set()
-    external_files = []
+    linked_files = []
     local_files = []
 
     for file in records:
         if file.based_on:
             git_files.append(file)
             unique_remotes.add(file.based_on.url)
-        elif file.is_external:
-            external_files.append(file)
+        elif file.linked:
+            linked_files.append(file)
         else:
             local_files.append(file)
 
     if ref and len(unique_remotes) > 1:
         raise errors.ParameterError(
             "Cannot specify a reference with more than one Git repository.\n"
             "Limit list of files to be updated to one repository. See 'renku dataset update -h' for more information."
         )
 
     updated_files: List[DynamicProxy] = []
     deleted_files: List[DynamicProxy] = []
 
-    if external_files and not no_external:
-        updated = update_external_files(external_files, dry_run=dry_run)
+    if linked_files:
+        updated = update_linked_files(linked_files, dry_run=dry_run)
         updated_files.extend(updated)
 
     if git_files and not no_remote:
         updated, deleted = update_dataset_git_files(files=git_files, ref=ref, delete=delete, dry_run=dry_run)
         updated_files.extend(updated)
         deleted_files.extend(deleted)
 
@@ -923,15 +942,15 @@
                 removed = dataset.unlink_file(src, missing_ok=True)
                 if removed:
                     modified_datasets[dataset.name] = dataset
                     new_dataset_file.based_on = removed.based_on
                     new_dataset_file.source = removed.source
 
                     if not to_dataset and (
-                        new_dataset_file.is_external
+                        new_dataset_file.linked
                         or is_subpath(project_context.path / dst, project_context.path / dataset.get_datadir())
                     ):
                         dataset.add_or_update_files(new_dataset_file)
 
                 # NOTE: Update dataset if it contains a destination that is being overwritten
                 modified = dataset.find_file(dst)
                 added = is_subpath(project_context.path / dst, project_context.path / dataset.get_datadir())
@@ -975,15 +994,15 @@
         communication.start_progress(progress_text, len(records))
         check_paths = []
         records_to_check = []
 
         for file in records:
             communication.update_progress(progress_text, 1)
 
-            if file.based_on or file.is_external:
+            if file.based_on or file.linked:
                 continue
 
             if not (project_context.path / file.entity.path).exists():
                 deleted_files.append(file)
                 continue
 
             check_paths.append(file.entity.path)
@@ -1080,15 +1099,15 @@
                     delete_dataset_file(dst, follow_symlinks=True)
                     project_context.repository.add(dst, force=True)
                 deleted_files.append(file)
             elif changed:
                 if not dry_run:
                     # Fetch file if it is tracked by Git LFS
                     pull_paths_from_storage(remote_repository, remote_repository.path / based_on.path)
-                    if is_external_file(path=src, project_path=remote_repository.path):
+                    if is_linked_file(path=src, project_path=remote_repository.path):
                         delete_dataset_file(dst, follow_symlinks=True)
                         create_external_file(target=src.resolve(), path=dst)
                     else:
                         shutil.copy(src, dst)
                     file.based_on = RemoteEntity(
                         checksum=checksum, path=based_on.path, url=based_on.url  # type: ignore
                     )
@@ -1099,36 +1118,36 @@
     if not updated_files and (not delete or not deleted_files):
         # Nothing to commit or update
         return [], deleted_files
 
     return updated_files, deleted_files
 
 
-def update_external_files(records: List[DynamicProxy], dry_run: bool) -> List[DynamicProxy]:
-    """Update files linked to external storage.
+def update_linked_files(records: List[DynamicProxy], dry_run: bool) -> List[DynamicProxy]:
+    """Update files linked to other files in the project.
 
     Args:
         records(List[DynamicProxy]): File records to update.
         dry_run(bool): Whether to return a preview of what would be updated.
     """
     updated_files = []
 
     for file in records:
-        if file.is_external:
+        if file.linked:
             try:
-                updated, checksum = is_external_file_updated(project_path=project_context.path, path=file.entity.path)
+                updated, checksum = is_linked_file_updated(path=file.entity.path)
             except errors.ExternalFileNotFound as e:
                 if not dry_run:
                     raise
                 communication.warn(str(e))
                 continue
 
             if updated:
                 if not dry_run:
-                    update_external_file(path=file.entity.path, checksum=checksum)
+                    update_linked_file(path=file.entity.path, checksum=checksum)
                 updated_files.append(file)
 
     return updated_files
 
 
 @inject.autoparams("dataset_gateway")
 def filter_dataset_files(
@@ -1230,83 +1249,98 @@
     if unused_names:
         unused_names_str = ", ".join(unused_names)
         raise errors.ParameterError(f"These datasets don't exist: {unused_names_str}")
 
     return sorted(records, key=lambda r: r.date_added)
 
 
+def download_file(file: DatasetFile, storage: "IStorage") -> List[DatasetFile]:
+    """Download a dataset file and retrieve its missing metadata (if any).
+
+    Args:
+        file(DatasetFile): Dataset file to download.
+        storage: Dataset's cloud storage (an instance of ``IStorage``).
+
+    Returns:
+         List[DatasetFile]: A list with the updated file if its metadata was missing; an empty list otherwise.
+
+    """
+    if not file.based_on:
+        raise errors.DatasetImportError(f"Dataset file doesn't have a URI: {file.entity.path}")
+
+    path = project_context.path / file.entity.path
+    path.resolve().parent.mkdir(parents=True, exist_ok=True)
+
+    # NOTE: Don't check if destination file exists. ``IStorage.copy`` won't copy a file if it exists and is not
+    # modified.
+
+    communication.start_progress(name=file.entity.path, total=1)
+    try:
+        storage.download(file.based_on.url, path)
+        communication.update_progress(name=file.entity.path, amount=1)
+    finally:
+        communication.finalize_progress(name=file.entity.path)
+
+    # NOTE: File has no missing information
+    if file.has_valid_checksum() and file.has_valid_size():
+        return []
+
+    if not file.has_valid_checksum():
+        md5_hash = hash_file(path, hash_type="md5") or NON_EXISTING_ENTITY_CHECKSUM
+        entity = Entity(path=file.entity.path, checksum=md5_hash)
+        remote_entity = RemoteEntity(checksum=md5_hash, url=file.based_on.url, path=file.based_on.path)
+    else:
+        entity = file.entity
+        remote_entity = file.based_on
+
+    size = file.size if file.has_valid_size() else get_file_size(path)
+
+    return [
+        DatasetFile(
+            entity=entity,
+            based_on=remote_entity,
+            size=size,
+            date_added=file.date_added,
+            date_removed=file.date_removed,
+            source=file.source,
+        )
+    ]
+
+
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
-def pull_external_data(name: str, location: Optional[Path] = None) -> None:
-    """Pull/copy data for an external storage to a dataset's data directory or a specified location.
+def pull_cloud_storage(name: str, location: Optional[Path] = None) -> None:
+    """Pull/copy data for a cloud storage to a dataset's data directory or a specified location.
 
     Args:
         name(str): Name of the dataset
         location(Optional[Path]): A directory to copy data to (Default value = None).
     """
-    datasets_provenance = DatasetsProvenance()
-
-    dataset = datasets_provenance.get_by_name(name=name, strict=True)
-
-    if not dataset.storage:
-        communication.warn(f"Dataset '{name}' doesn't have a storage backend")
-        return
+    dataset, datadir = _get_dataset_with_cloud_storage(name=name)
 
     # NOTE: Try to unmount the path in case it was mounted before
-    unmount_path(project_context.path / dataset.get_datadir())
-
-    create_symlinks = True
-    destination: Union[Path, str]
+    unmount_path(datadir)
 
     if location:
-        destination = get_absolute_path(location)
-    else:
-        stored_location = read_dataset_data_location(dataset=dataset)
-        if stored_location:
-            destination = stored_location
-        else:
-            destination = project_context.path
-            create_symlinks = False
+        if not is_path_empty(datadir):
+            communication.confirm(
+                f"Dataset's data directory will be removed: {dataset.get_datadir()}. Do you want to continue?",
+                abort=True,
+                warning=True,
+            )
+        create_symlink(target=location, symlink_path=datadir, overwrite=True)
 
     provider = ProviderFactory.get_pull_provider(uri=dataset.storage)
     storage = provider.get_storage()
 
-    updated_files = []
-
-    for file in dataset.files:
-        path = Path(destination) / file.entity.path
-        path.parent.mkdir(parents=True, exist_ok=True)
-        # NOTE: Don't check if destination exists. ``IStorage.copy`` won't copy a file if it exists and is not modified.
-
-        if not file.based_on:
-            raise errors.DatasetImportError(f"Dataset file doesn't have a URI: {file.entity.path}")
-
-        with communication.busy(f"Copying {file.entity.path} ..."):
-            storage.download(file.based_on.url, path)
-
-            # NOTE: Make files read-only since we don't support pushing data to the remote storage
-            os.chmod(path, 0o400)
-
-            if not file.based_on.checksum:
-                md5_hash = hash_file(path, hash_type="md5") or ""
-                file.based_on = RemoteEntity(checksum=md5_hash, url=file.based_on.url, path=file.based_on.path)
-
-            new_file = DynamicProxy(file)
-            new_file.dataset = dataset
-            updated_files.append(new_file)
-
-            if create_symlinks:
-                symlink_path = project_context.path / file.entity.path
-                symlink_path.parent.mkdir(parents=True, exist_ok=True)
-                create_symlink(path=path, symlink_path=symlink_path, overwrite=True)
-
-    # NOTE: Store location in metadata in case where we want to mount the external storage in the same location
-    store_dataset_data_location(dataset=dataset, location=location)
+    updated_files = parallel_execute(download_file, dataset.files, rate=5, storage=storage)
 
     if updated_files:
-        _update_datasets_files_metadata(updated_files=updated_files, deleted_files=[], delete=False)
+        dataset.add_or_update_files(updated_files)
+        DatasetsProvenance().add_or_update(dataset, creator=get_git_user(repository=project_context.repository))
+        project_context.database.commit()
 
 
 def store_dataset_data_location(dataset: Dataset, location: Optional[Path]) -> None:
     """Store data location for a dataset in the config file."""
     section = "dataset-locations"
     key = dataset.name
 
@@ -1318,36 +1352,36 @@
 
 def read_dataset_data_location(dataset: Dataset) -> Optional[str]:
     """Read data location for a dataset in the config file."""
     return get_value(section="dataset-locations", key=dataset.name, config_filter=ConfigFilter.LOCAL_ONLY)
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
-def mount_external_storage(name: str, existing: Optional[Path], yes: bool) -> None:
-    """Mount an external storage to a dataset's data directory.
+def mount_cloud_storage(name: str, existing: Optional[Path], yes: bool) -> None:
+    """Mount a cloud storage to a dataset's data directory.
 
     Args:
         name(str): Name of the dataset
-        existing(Optional[Path]): An existing mount point to use instead of actually mounting the external storage.
+        existing(Optional[Path]): An existing mount point to use instead of actually mounting the backend storage.
         yes(bool): Don't prompt when removing non-empty dataset's data directory.
     """
-    dataset, datadir = _get_dataset_with_external_storage(name=name)
+    dataset, datadir = _get_dataset_with_cloud_storage(name=name)
 
     # NOTE: Try to unmount the path in case it was mounted before
     unmount_path(datadir)
 
     if not is_path_empty(datadir) and not yes:
         communication.confirm(
             f"Dataset's data directory will be removed: {dataset.get_datadir()}. Do you want to continue?",
             abort=True,
             warning=True,
         )
 
     if existing:
-        create_symlink(path=existing, symlink_path=datadir, overwrite=True)
+        create_symlink(target=existing, symlink_path=datadir, overwrite=True)
         return
 
     delete_path(datadir)
     datadir.mkdir(parents=True, exist_ok=True)
 
     provider = ProviderFactory.get_mount_provider(uri=dataset.storage)
     credentials = provider.get_credentials()
@@ -1355,25 +1389,25 @@
     storage = provider.get_storage(credentials=credentials)
 
     with communication.busy(f"Mounting {provider.uri}"):
         storage.mount(datadir)
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
-def unmount_external_storage(name: str) -> None:
-    """Mount an external storage to a dataset's data directory.
+def unmount_cloud_storage(name: str) -> None:
+    """Mount a cloud storage to a dataset's data directory.
 
     Args:
         name(str): Name of the dataset
     """
-    _, datadir = _get_dataset_with_external_storage(name=name)
+    _, datadir = _get_dataset_with_cloud_storage(name=name)
     unmount_path(datadir)
 
 
-def _get_dataset_with_external_storage(name: str) -> Tuple[Dataset, Path]:
+def _get_dataset_with_cloud_storage(name: str) -> Tuple[Dataset, Path]:
     datasets_provenance = DatasetsProvenance()
 
     dataset = datasets_provenance.get_by_name(name=name, strict=True)
 
     if not dataset.storage:
         raise errors.ParameterError(f"Dataset '{name}' doesn't have a storage backend")
```

### Comparing `renku-2.3.2/renku/core/dataset/dataset_add.py` & `renku-2.4.0rc1/renku/core/dataset/dataset_add.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,31 +14,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Dataset add business logic."""
 
 import itertools
 import os.path
 import shutil
+import tempfile
 from pathlib import Path
-from typing import Generator, List, Optional, Union, cast
+from typing import Dict, Generator, List, Optional, Tuple, Union, cast
 
+from renku.command.command_builder.command import inject
 from renku.core import errors
 from renku.core.dataset.context import DatasetContext
 from renku.core.dataset.datasets_provenance import DatasetsProvenance
 from renku.core.dataset.pointer_file import create_external_file
 from renku.core.dataset.providers.api import ImporterApi
 from renku.core.dataset.providers.factory import ProviderFactory
+from renku.core.dataset.providers.local import LocalProvider
 from renku.core.dataset.providers.models import DatasetAddAction, DatasetAddMetadata
+from renku.core.interface.dataset_gateway import IDatasetGateway
 from renku.core.interface.storage import IStorage
 from renku.core.storage import check_external_storage, track_paths_in_storage
 from renku.core.util import communication, requests
-from renku.core.util.dataset import check_url
 from renku.core.util.git import get_git_user
-from renku.core.util.os import delete_dataset_file, get_files, get_relative_path, hash_file
-from renku.core.util.urls import is_uri_subfolder
+from renku.core.util.os import get_absolute_path, get_file_size, get_files, get_relative_path, hash_file, is_subpath
+from renku.core.util.urls import check_url, is_uri_subfolder, resolve_uri
+from renku.core.util.util import parallel_execute
+from renku.domain_model.constant import NON_EXISTING_ENTITY_CHECKSUM
 from renku.domain_model.dataset import Dataset, DatasetFile, RemoteEntity
 from renku.domain_model.project_context import project_context
 
 
 def add_to_dataset(
     dataset_name: str,
     urls: List[str],
@@ -67,25 +70,25 @@
 
     try:
         with DatasetContext(name=dataset_name, create=create, datadir=datadir, storage=storage) as dataset:
             destination_path = _create_destination_directory(dataset, destination)
 
             check_external_storage()
 
-            # NOTE: This is not required for external storages
+            # NOTE: This is not required for cloud storages
             if not dataset.storage:
                 _check_available_space(urls, total_size=total_size)
 
             datadir = cast(Path, project_context.path / dataset.get_datadir())
             if create and datadir.exists() and not dataset.storage:
                 # NOTE: Add datadir to paths to add missing files on create
                 for file in get_files(datadir):
                     urls.append(str(file))
 
-            files = _get_files_metadata(
+            files = get_files_metadata(
                 urls=urls,
                 dataset=dataset,
                 importer=importer,
                 destination=destination_path,
                 revision=revision,
                 sources=sources,
                 extract=extract,
@@ -99,33 +102,33 @@
                     raise errors.UsageError("There are no files to create a dataset")
                 else:
                     communication.warn("No new file was added to project")
                     return dataset
 
             # NOTE: All files at this point can be force-added
 
-            move_files_to_dataset(dataset=dataset, files=files)
+            copy_files_to_dataset(dataset=dataset, files=files)
             add_files_to_repository(dataset=dataset, files=files)
             update_dataset_metadata(dataset=dataset, files=files, clear_files_before=clear_files_before)
 
             DatasetsProvenance().add_or_update(dataset, creator=get_git_user(repository=project_context.repository))
     except errors.DatasetNotFound:
         raise errors.DatasetNotFound(
             message="Dataset '{0}' does not exist.\n"
             "Use 'renku dataset create {0}' to create the dataset or retry 'renku dataset add {0}' command "
             "with '--create' option for automatic dataset creation.".format(dataset_name)
         )
     except (FileNotFoundError, errors.GitCommandError) as e:
-        raise errors.ParameterError("Could not find paths/URLs: \n{0}".format("\n".join(urls))) from e
+        raise errors.ParameterError("Could not find paths/URLs: \n{}".format("\n".join(urls))) from e
     else:
         project_context.database.commit()
         return dataset
 
 
-def _get_files_metadata(
+def get_files_metadata(
     *,
     urls: List[str],
     importer: Optional[ImporterApi] = None,
     dataset: Dataset,
     destination: Path,
     extract: bool,
     revision: Optional[str],
@@ -141,42 +144,112 @@
         raise errors.ParameterError("No URL is specified")
     if sources and len(urls) > 1:
         raise errors.ParameterError("Cannot use '--source' with multiple URLs.")
 
     files = []
 
     for url in urls:
-        _, is_git = check_url(url)
+        is_remote, is_git = check_url(url)
 
         if not is_git and sources:
             raise errors.ParameterError("Cannot use '-s/--src/--source' with URLs or local files.")
 
-        provider = ProviderFactory.get_add_provider(uri=url)
+        dataset_add_action = DatasetAddAction.NONE
+
+        if is_remote:
+            provider = ProviderFactory.get_add_provider(uri=url)
+        else:
+            # NOTE: If URI is in the local file system, check to see if it's part of a mounted dataset/provider
+            cloud_dataset, remote_url = get_cloud_dataset_from_path(path=url)
+            if cloud_dataset:
+                url = remote_url
+                provider = ProviderFactory.get_storage_provider(uri=cloud_dataset.storage)
+                # NOTE: Update metadata if destination dataset is the same as source dataset, otherwise copy the file
+                # since it's already in the local filesystem
+                dataset_add_action = DatasetAddAction.COPY
+            else:
+                provider = LocalProvider(uri=url)
 
-        new_files = provider.add(
+        new_files = provider.get_metadata(
             uri=url,
             destination=destination,
             revision=revision,
             sources=sources,
             dataset=dataset,
             extract=extract,
             force=force,
+            dataset_add_action=dataset_add_action,
             **kwargs,
         )
 
         files.extend(new_files)
 
     return files
 
 
+@inject.autoparams("dataset_gateway")
+def has_cloud_storage(dataset_gateway: IDatasetGateway) -> bool:
+    """Return if a project has any dataset with cloud storage with its data directory mounted or pulled."""
+    # NOTE: ``exists`` return False for symlinks if their target doesn't exists, but it's fine here since it means the
+    # dataset's mounted/pulled location doesn't exist.
+    return any(
+        dataset
+        for dataset in dataset_gateway.get_all_active_datasets()
+        if dataset.storage and (project_context.path / dataset.get_datadir()).exists()
+    )
+
+
+@inject.autoparams("dataset_gateway")
+def get_cloud_dataset_from_path(
+    path: Union[Path, str], dataset_gateway: IDatasetGateway, missing_ok: bool = False
+) -> Tuple[Optional[Dataset], Optional[str]]:
+    """Check the path against datasets' storage and return a dataset (if any)."""
+    if not has_cloud_storage():
+        return None, None
+
+    # NOTE: If path is inside the datadir of a dataset with storage backend and the dataset isn't mounted, we should
+    # still add whatever is in the path (because it might have been pulled)
+
+    path = Path(get_absolute_path(path))
+
+    if not missing_ok and not path.exists() and not os.path.lexists(path):
+        return None, None
+
+    for dataset in dataset_gateway.get_all_active_datasets():
+        if not dataset.storage:
+            continue
+
+        datadir = project_context.path / dataset.get_datadir()
+        resolved_path = path.resolve()
+
+        # NOTE: Resolve ``path`` because ``datadir`` is resolved and resolved paths might have be on a different
+        # location (e.g. on macos /tmp resolves to /private/tmp)
+        resolved_relative_path = get_relative_path(resolved_path, base=datadir.resolve())
+
+        if is_subpath(path, base=datadir) or resolved_relative_path is not None:
+            if resolved_relative_path == ".":
+                resolved_relative_path = ""
+            storage_uri = dataset.storage.rstrip("/")
+            remote_url = f"{storage_uri}/{resolved_relative_path}"
+            return dataset, remote_url
+        elif is_subpath(resolved_path, Path(dataset.storage).resolve()):  # NOTE: For local backend storage
+            return dataset, str(resolved_path)
+
+    return None, None
+
+
 def _check_available_space(urls: List[str], total_size: Optional[int] = None):
     """Check that there is enough space available on the device for download."""
     if total_size is None:
         total_size = 0
         for url in urls:
+            is_remote, _ = check_url(url)
+            if not is_remote:
+                continue
+
             try:
                 response = requests.head(url, allow_redirects=True)
                 total_size += int(response.headers.get("content-length", 0))
             except errors.RequestError:
                 pass
     usage = shutil.disk_usage(project_context.path)
 
@@ -188,17 +261,14 @@
         raise errors.OperationError(message)
 
 
 def _create_destination_directory(dataset: Dataset, destination: Optional[Union[Path, str]] = None) -> Path:
     """Create directory for dataset add."""
     dataset_datadir = project_context.path / dataset.get_datadir()
 
-    if dataset_datadir.is_symlink():
-        dataset_datadir.unlink()
-
     # NOTE: Make sure that dataset's data dir exists because we check for existence of a destination later to decide
     # what will be its name
     dataset_datadir.mkdir(parents=True, exist_ok=True)
 
     destination = destination or ""
     relative_path = cast(str, get_relative_path(destination, base=dataset_datadir, strict=True))
     return dataset_datadir / relative_path
@@ -292,105 +362,125 @@
 
     base = dataset.storage.rstrip("/")
     path_within_dataset = get_dataset_file_path_within_dataset(dataset=dataset, entity_path=entity_path)
 
     return f"{base}/{path_within_dataset}"
 
 
-def move_files_to_dataset(dataset: Dataset, files: List[DatasetAddMetadata]):
-    """Copy/Move files into a dataset's directory."""
-
-    def move_file(file: DatasetAddMetadata, storage: Optional[IStorage]) -> bool:
-        if not file.has_action:
-            return False
-
-        if file.action in (
-            DatasetAddAction.COPY,
-            DatasetAddAction.MOVE,
-            DatasetAddAction.SYMLINK,
-            DatasetAddAction.DOWNLOAD,
-        ):
-            # NOTE: Remove existing file if any; required as a safety-net to avoid corrupting external files
-            delete_dataset_file(file.destination, follow_symlinks=True)
+def copy_file(file: DatasetAddMetadata, dataset: Dataset, storage: Optional[IStorage]) -> List[Optional[Path]]:
+    """Copy/move/link a file to dataset's data directory."""
+    if not file.has_action:
+        return []
+
+    # NOTE: If file is in a sub-directory of a dataset's remote storage URI, only update the metadata
+    if file.from_cloud_storage:
+        if dataset.storage and is_uri_subfolder(resolve_uri(dataset.storage), file.url):
+            file.action = DatasetAddAction.METADATA_ONLY
+        else:
+            file.action = DatasetAddAction.DOWNLOAD
+
+    if file.action in (
+        DatasetAddAction.COPY,
+        DatasetAddAction.MOVE,
+        DatasetAddAction.SYMLINK,
+        DatasetAddAction.DOWNLOAD,
+    ):
+        try:
             file.destination.parent.mkdir(parents=True, exist_ok=True)
+        except OSError as e:
+            raise errors.InvalidFileOperation(f"Cannot create destination '{file.destination.parent}': {e}")
 
-        track_in_lfs = True
+    file_to_upload: Union[Path, str] = file.source.resolve()
+    delete_source = False
+    track_in_lfs = True
 
-        # NOTE: If file is in a sub-directory of a dataset's remote storage URI, only update the metadata
-        if file.remote_storage:
-            if dataset.storage and is_uri_subfolder(dataset.storage, file.url):
-                file.action = DatasetAddAction.METADATA_ONLY
+    try:
+        if file.action == DatasetAddAction.DOWNLOAD:
+            # NOTE: Download to a temporary location if dataset has a cloud storage because it's usually mounted as
+            # read-only and download would fail. It's ok not to move it to dataset's data dir since it'll be uploaded.
+            dst: Union[Path, str]
+            if storage:
+                fd, dst = tempfile.mkstemp()
+                os.close(fd)
             else:
-                file.action = DatasetAddAction.DOWNLOAD
+                dst = file.destination
 
-        file_to_upload = file.source.resolve()
+            assert file.provider, f"Storage provider isn't set for {file} with DOWNLOAD action"
+            download_storage = file.provider.get_storage()
+            download_storage.download(file.url, dst)
+            file_to_upload = dst
+        elif file.action == DatasetAddAction.COPY:
+            shutil.copy(file.source, file.destination)
+        elif file.action == DatasetAddAction.MOVE:
+            # NOTE: Set ``delete_source`` in case move fails due to a dataset's read-only mounted data directory
+            delete_source = True
+            shutil.move(file.source, file.destination, copy_function=shutil.copy)  # type: ignore
+            delete_source = False
+            file_to_upload = file.destination
+        elif file.action == DatasetAddAction.SYMLINK:
+            create_external_file(target=file.source, path=file.destination)
+            # NOTE: Don't track symlinks to external files in LFS
+            track_in_lfs = False
+        elif file.metadata_only:
+            # NOTE: Nothing to do when adding file to a dataset with a parent remote storage
+            pass
+        else:
+            raise errors.OperationError(f"Invalid action {file.action}")
+    except OSError as e:
+        # NOTE: It's ok if copying data to a read-only mounted cloud storage fails
+        if "Read-only file system" in str(e) and storage:
+            pass
+        else:
+            dst = get_relative_path(file.destination, project_context.path) or file.destination
+            raise errors.InvalidFileOperation(f"Cannot copy/move '{dst}': {e}")
+
+    if file.size is None:
+        file.size = get_file_size(file_to_upload)
+
+    if storage:
+        # NOTE: Don't track files in a dataset with cloud storage in LFS
+        track_in_lfs = False
+
+        if file.metadata_only:
+            assert file.based_on, f"wasBasedOn isn't set for {file} with METADATA_ONLY action"
+            file_uri = file.based_on.url
+            md5_hash: Optional[str] = file.based_on.checksum
+        else:
+            file_uri = get_upload_uri(dataset=dataset, entity_path=file.entity_path)
+            md5_hash = hash_file(file_to_upload, hash_type="md5")
+
+            # NOTE: If dataset has a storage backend, upload the file to the remote storage.
+            storage.upload(source=file_to_upload, uri=file_uri)
+
+        file.based_on = RemoteEntity(url=file_uri, path=file.entity_path, checksum=md5_hash)
 
-        try:
-            if file.action == DatasetAddAction.COPY:
-                shutil.copy(file.source, file.destination)
-            elif file.action == DatasetAddAction.MOVE:
-                shutil.move(file.source, file.destination, copy_function=shutil.copy)  # type: ignore
-            elif file.action == DatasetAddAction.SYMLINK:
-                create_external_file(target=file.source, path=file.destination)
-                # NOTE: Don't track symlinks to external files in LFS
-                track_in_lfs = False
-            elif file.action == DatasetAddAction.DOWNLOAD:
-                assert file.provider, f"Storage provider isn't set for {file} with DOWNLOAD action"
-                download_storage = file.provider.get_storage()
-                download_storage.download(file.url, file.destination)
-                file_to_upload = file.destination
-            elif file.metadata_only:
-                # NOTE: Nothing to do when adding file to a dataset with a parent remote storage
-                pass
-            else:
-                raise errors.OperationError(f"Invalid action {file.action}")
-        except OSError as e:
-            # NOTE: It's ok if copying data to a read-only mounted cloud storage fails
-            if "Read-only file system" in str(e) and storage:
-                pass
-            else:
-                raise
+    if delete_source:
+        file.source.unlink(missing_ok=True)
 
-        # NOTE: We always copy the files to the dataset's data dir. If dataset has a storage backend, we also upload the
-        # file to the remote storage.
-        if storage:
-            if file.metadata_only:
-                assert file.based_on, f"wasBasedOn isn't set for {file} with METADATA_ONLY action"
-                file_uri = file.based_on.url
-                md5_hash = file.based_on.checksum
-            else:
-                file_uri = get_upload_uri(dataset=dataset, entity_path=file.entity_path)
-                storage.upload(source=file_to_upload, uri=file_uri)
-                md5_hash = hash_file(file_to_upload, hash_type="md5") or ""
+    return [file.destination] if track_in_lfs else []
 
-            file.based_on = RemoteEntity(url=file_uri, path=file.entity_path, checksum=md5_hash)
 
-        return track_in_lfs
+def copy_files_to_dataset(dataset: Dataset, files: List[DatasetAddMetadata]):
+    """Copy/Move files into a dataset's directory."""
 
     dataset_storage = None
     if dataset.storage:
         provider = ProviderFactory.get_storage_provider(uri=dataset.storage)
         dataset_storage = provider.get_storage()
 
-    lfs_files = []
-
-    for dataset_file in files:
-        # TODO: Parallelize copy/download/upload
-        if move_file(file=dataset_file, storage=dataset_storage):
-            lfs_files.append(dataset_file.destination)
+    lfs_files = parallel_execute(copy_file, files, rate=5, dataset=dataset, storage=dataset_storage)
 
     if lfs_files and not dataset.storage:
         track_paths_in_storage(*lfs_files)
 
 
 def add_files_to_repository(dataset: Dataset, files: List[DatasetAddMetadata]):
     """Track files in project's repository."""
     # NOTE: There is nothing to track for remote storages
     if dataset.storage:
-        communication.info("Nothing to add to the project for datasets with a storage backend")
         return
 
     # NOTE: Don't commit files that will be uploaded to a remote storage
     paths_to_commit = [f.get_absolute_commit_path(project_context.path) for f in files]
 
     repository = project_context.repository
 
@@ -401,24 +491,34 @@
     n_staged_changes = len(repository.staged_changes)
     if n_staged_changes == 0:
         communication.warn("No new file was added to project")
 
 
 def update_dataset_metadata(dataset: Dataset, files: List[DatasetAddMetadata], clear_files_before: bool):
     """Add newly-added files to the dataset's metadata."""
-    dataset_files = []
-    repo_paths: List[Union[Path, str]] = [
-        file.entity_path for file in files if (project_context.path / file.entity_path).exists()
-    ]
+    # NOTE: For datasets with cloud storage backend, we use MD5 hash as checksum instead of git hash.
+    if dataset.storage:
+        checksums: Dict[Union[Path, str], Optional[str]] = {
+            f.entity_path: f.based_on.checksum for f in files if f.based_on
+        }
+    else:
+        repo_paths: List[Union[Path, str]] = [
+            file.entity_path for file in files if (project_context.path / file.entity_path).exists()
+        ]
+        checksums = project_context.repository.get_object_hashes(repo_paths)
 
-    checksums = project_context.repository.get_object_hashes(repo_paths)
+    dataset_files = []
 
     for file in files:
         dataset_file = DatasetFile.from_path(
-            path=file.entity_path, source=file.url, based_on=file.based_on, checksum=checksums.get(file.entity_path)
+            path=file.entity_path,
+            source=file.url,
+            based_on=file.based_on,
+            size=file.size,
+            checksum=checksums.get(file.entity_path) or NON_EXISTING_ENTITY_CHECKSUM,
         )
         dataset_files.append(dataset_file)
 
     if clear_files_before:
         dataset.clear_files()
 
     dataset.add_or_update_files(dataset_files)
```

### Comparing `renku-2.3.2/renku/core/dataset/datasets_provenance.py` & `renku-2.4.0rc1/renku/core/dataset/datasets_provenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,27 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Datasets Provenance."""
 
 from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union, overload
+from typing import TYPE_CHECKING, List, Literal, Optional, Union, overload
 from uuid import UUID
 
 from renku.command.command_builder.command import inject
 from renku.core import errors
 from renku.core.interface.dataset_gateway import IDatasetGateway
 from renku.core.util import communication
 
-try:
-    from typing_extensions import Literal  # NOTE: Required for Python 3.7 compatibility
-except ImportError:
-    from typing import Literal  # type: ignore
-
 if TYPE_CHECKING:
     from renku.domain_model.dataset import Dataset, DatasetTag
     from renku.domain_model.provenance.agent import Person
 
 
 class DatasetsProvenance:
     """A set of datasets."""
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/__init__.py` & `renku-2.4.0rc1/renku/ui/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Data registry integration."""
+"""Renku ui modules."""
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/api.py` & `renku-2.4.0rc1/renku/core/dataset/providers/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,20 +14,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """API for providers."""
 
 import abc
 from collections import UserDict
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Protocol, Tuple, Type, Union
 
 from renku.core import errors
 from renku.core.constant import ProviderPriority
 from renku.core.plugin import hookimpl
-from renku.core.util.util import NO_VALUE, NoValueType
+from renku.domain_model.constant import NO_VALUE, NoValueType
 from renku.domain_model.dataset_provider import IDatasetProviderPlugin
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.models import (
         DatasetAddMetadata,
         ProviderDataset,
         ProviderDatasetFile,
@@ -39,15 +39,15 @@
 
 class ProviderApi(IDatasetProviderPlugin):
     """Interface defining provider methods."""
 
     priority: Optional[ProviderPriority] = None
     name: Optional[str] = None
 
-    def __init__(self, uri: Optional[str], **kwargs):
+    def __init__(self, uri: str, **kwargs):
         self._uri: str = uri or ""
 
     def __init_subclass__(cls, **kwargs):
         for required_property in ("priority", "name"):
             if getattr(cls, required_property, None) is None:
                 raise NotImplementedError(f"{required_property} must be set for {cls}")
 
@@ -77,16 +77,16 @@
 
     @staticmethod
     def get_add_parameters() -> List["ProviderParameter"]:
         """Returns parameters that can be set for add."""
         return []
 
     @abc.abstractmethod
-    def add(self, uri: str, destination: Path, **kwargs) -> List["DatasetAddMetadata"]:
-        """Add files from a URI to a dataset."""
+    def get_metadata(self, uri: str, destination: Path, **kwargs) -> List["DatasetAddMetadata"]:
+        """Get metadata of files that will be added to a dataset."""
         raise NotImplementedError
 
 
 class ExportProviderInterface(abc.ABC):
     """Interface defining export providers."""
 
     @staticmethod
@@ -119,23 +119,48 @@
 
     @abc.abstractmethod
     def get_credentials(self) -> "ProviderCredentials":
         """Return an instance of provider's credential class."""
         raise NotImplementedError
 
     @abc.abstractmethod
+    def convert_to_storage_uri(self, uri: str) -> str:
+        """Convert backend-specific URI to a URI that is usable by the IStorage implementation."""
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def get_storage(self, credentials: Optional["ProviderCredentials"] = None) -> "IStorage":
         """Return the storage manager for the provider."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def on_create(self, dataset: "Dataset") -> None:
         """Hook to perform provider-specific actions on a newly-created dataset."""
         raise NotImplementedError
 
+    @staticmethod
+    @abc.abstractmethod
+    def supports_storage(uri: str) -> bool:
+        """Whether or not this provider supports a given URI storage."""
+        raise NotImplementedError
+
+
+class CloudStorageProviderType(Protocol):
+    """Intersection type for ``mypy`` hinting in storage classes."""
+
+    @property
+    def uri(self) -> str:
+        """Return provider's URI."""
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def convert_to_storage_uri(self, uri: str) -> str:
+        """Convert backend-specific URI to a URI that is usable by the IStorage implementation."""
+        raise NotImplementedError
+
 
 class ImporterApi(abc.ABC):
     """Interface defining importer methods."""
 
     def __init__(self, uri: str, original_uri: str):
         self._uri: str = uri
         self._original_uri: str = original_uri
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/azure.py` & `renku-2.4.0rc1/renku/core/dataset/providers/azure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,96 +12,93 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Azure dataset provider."""
 
 import urllib
+from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Tuple, cast
 
-from renku.command.command_builder import inject
 from renku.core import errors
-from renku.core.dataset.providers.api import ProviderApi, ProviderCredentials, ProviderPriority
-from renku.core.dataset.providers.cloud import CloudStorageAddProvider
-from renku.core.dataset.providers.models import ProviderParameter
-from renku.core.interface.storage import IStorage, IStorageFactory
+from renku.core.dataset.providers.api import (
+    AddProviderInterface,
+    ProviderApi,
+    ProviderCredentials,
+    ProviderPriority,
+    StorageProviderInterface,
+)
+from renku.core.dataset.providers.common import get_metadata
+from renku.core.dataset.providers.models import DatasetAddAction
+from renku.core.interface.storage import IStorage
 from renku.core.util.metadata import get_canonical_key, prompt_for_credentials
 from renku.core.util.urls import get_scheme
 from renku.domain_model.project_context import project_context
+from renku.infrastructure.storage.factory import StorageFactory
 
 if TYPE_CHECKING:
+    from renku.core.dataset.providers.models import DatasetAddMetadata
     from renku.domain_model.dataset import Dataset
 
 
-class AzureProvider(ProviderApi, CloudStorageAddProvider):
+class AzureProvider(ProviderApi, StorageProviderInterface, AddProviderInterface):
     """Azure provider."""
 
     priority = ProviderPriority.HIGHEST
     name = "Azure"
 
-    def __init__(self, uri: Optional[str]):
+    def __init__(self, uri: str):
         super().__init__(uri=uri)
 
         account, endpoint, container, _ = parse_azure_uri(uri=self.uri)
 
         self._account: str = account
         self._endpoint: str = endpoint
         self._container = container
 
     @staticmethod
     def supports(uri: str) -> bool:
         """Whether or not this provider supports a given URI."""
         return get_scheme(uri) == "azure"
 
     @staticmethod
-    def get_add_parameters() -> List["ProviderParameter"]:
-        """Returns parameters that can be set for add."""
-        from renku.core.dataset.providers.models import ProviderParameter
-
-        return [
-            ProviderParameter(
-                "storage",
-                flags=["storage"],
-                default=None,
-                help="Uri for the Azure container when creating the dataset at the same time when running 'add'",
-                multiple=False,
-                type=str,
-            ),
-        ]
+    def supports_storage(uri: str) -> bool:
+        """Whether or not this provider supports a given URI storage."""
+        return AzureProvider.supports(uri=uri)
+
+    def get_metadata(
+        self, uri: str, destination: Path, dataset_add_action: DatasetAddAction = DatasetAddAction.NONE, **kwargs
+    ) -> List["DatasetAddMetadata"]:
+        """Get metadata of files that will be added to a dataset."""
+        return get_metadata(provider=self, uri=uri, destination=destination, dataset_add_action=dataset_add_action)
+
+    def convert_to_storage_uri(self, uri: str) -> str:
+        """Convert backend-specific URI to a URI that is usable by the IStorage implementation."""
+        _, _, container, path = parse_azure_uri(uri=uri)
+        return f"azure://{container}/{path}"
 
     def get_credentials(self) -> "AzureCredentials":
         """Return an instance of provider's credential class."""
         return AzureCredentials(provider=self)
 
-    @inject.autoparams("storage_factory")
-    def get_storage(
-        self, storage_factory: "IStorageFactory", credentials: Optional["ProviderCredentials"] = None
-    ) -> "IStorage":
+    def get_storage(self, credentials: Optional["ProviderCredentials"] = None) -> "IStorage":
         """Return the storage manager for the provider."""
         azure_configuration = {
             "type": "azureblob",
-            "endpoint": self.endpoint,
         }
 
-        def create_renku_storage_azure_uri(uri: str) -> str:
-            """Create an Azure URI to work with the Renku storage handler."""
-            _, _, container, path = parse_azure_uri(uri=uri)
-
-            return f"azure://{container}/{path}"
-
         if not credentials:
             credentials = self.get_credentials()
             prompt_for_credentials(credentials)
 
-        return storage_factory.get_storage(
+        return StorageFactory.get_storage(
             storage_scheme="azure",
             provider=self,
             credentials=credentials,
             configuration=azure_configuration,
-            uri_convertor=create_renku_storage_azure_uri,
         )
 
     @property
     def account(self) -> str:
         """Azure account name."""
         return self._account
 
@@ -161,21 +156,30 @@
     """Extract account, endpoint, container, and path within the container from a given URI.
 
     NOTE: We support azure://<account-name>.<endpoint>/<container-name>/<path> or
     azure://<account-name>/<container-name>/<path>.
     """
     parsed_uri = urllib.parse.urlparse(uri)
 
+    if parsed_uri.scheme.lower() != "azure":
+        raise errors.ParameterError(
+            f"Invalid scheme in Azure URI: {uri}.\n"
+            "Valid format is 'azure://<account-name>/<container-name>/<path>' or "
+            "'azure://<account-name>.<endpoint>/<container-name>/<path>'",
+            show_prefix=False,
+        )
+
     account, _, endpoint = parsed_uri.netloc.partition(".")
+    path = parsed_uri.path.strip("/")
+    container, _, path = path.partition("/")
 
-    if parsed_uri.scheme.lower() != "azure" or not account:
+    if not account or not container:
         raise errors.ParameterError(
-            f"Invalid Azure URI: {uri}. Valid format is 'azure://<account-name>.<endpoint>/<container-name>/<path>' or "
-            "azure://<account-name>/<container-name>/<path>"
+            f"Missing account and/or container name in Azure URI: {uri}.\n"
+            "Valid format is 'azure://<account-name>/<container-name>/<path>' or "
+            "'azure://<account-name>.<endpoint>/<container-name>/<path>'",
+            show_prefix=False,
         )
 
     endpoint = endpoint.lower() or "blob.core.windows.net"
 
-    path = parsed_uri.path.strip("/")
-    container, _, path = path.partition("/")
-
     return account, endpoint, container, path.strip("/")
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/cloud.py` & `renku-2.4.0rc1/renku/core/dataset/providers/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Common functionality for cloud storage providers."""
+"""Common functionality for data providers."""
 
 import re
 from pathlib import Path
 from typing import List
 
 from renku.core import errors
-from renku.core.dataset.providers.api import AddProviderInterface, StorageProviderInterface
+from renku.core.dataset.providers.api import StorageProviderInterface
 from renku.core.dataset.providers.models import DatasetAddAction, DatasetAddMetadata
 from renku.domain_model.dataset import RemoteEntity
 from renku.domain_model.project_context import project_context
 
 
-class CloudStorageAddProvider(AddProviderInterface, StorageProviderInterface):
-    """Common AddProviderInterface for cloud providers."""
-
-    def add(self, uri: str, destination: Path, **kwargs) -> List["DatasetAddMetadata"]:
-        """Add files from a URI to a dataset."""
-        if re.search(r"[*?]", uri):
-            raise errors.ParameterError("Wildcards like '*' or '?' are not supported for cloud storage URIs.")
-
-        storage = self.get_storage()
-
-        destination_path_in_repo = Path(destination).relative_to(project_context.repository.path)
-        hashes = storage.get_hashes(uri=uri)
-        return [
-            DatasetAddMetadata(
-                entity_path=destination_path_in_repo / hash.path,
-                url=hash.base_uri,
-                action=DatasetAddAction.REMOTE_STORAGE,
-                based_on=RemoteEntity(checksum=hash.hash if hash.hash else "", url=hash.base_uri, path=hash.path),
-                source=Path(hash.base_uri),
-                destination=destination_path_in_repo,
-                provider=self,
-            )
-            for hash in hashes
-        ]
+def get_metadata(
+    provider: StorageProviderInterface, uri: str, destination: Path, dataset_add_action: DatasetAddAction
+) -> List["DatasetAddMetadata"]:
+    """Add files from a URI to a dataset."""
+    if re.search(r"[*?]", uri):
+        raise errors.ParameterError("Wildcards like '*' or '?' are not supported for cloud storage URIs.")
+
+    storage = provider.get_storage()
+
+    destination_path_in_repo = Path(destination).relative_to(project_context.repository.path)
+    hashes = storage.get_hashes(uri=uri)
+    if dataset_add_action == DatasetAddAction.NONE:
+        dataset_add_action = DatasetAddAction.REMOTE_STORAGE
+    return [
+        DatasetAddMetadata(
+            entity_path=destination_path_in_repo / hash.path,
+            url=hash.uri,
+            action=dataset_add_action,
+            based_on=RemoteEntity(checksum=hash.hash if hash.hash else "", url=hash.uri, path=hash.path),
+            source=Path(hash.uri),
+            destination=destination / hash.path,
+            provider=provider,
+            size=hash.size,
+        )
+        for hash in hashes
+    ]
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/dataverse.py` & `renku-2.4.0rc1/renku/core/dataset/providers/dataverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -39,14 +37,15 @@
     AUTHOR_METADATA_TEMPLATE,
     CONTACT_METADATA_TEMPLATE,
     DATASET_METADATA_TEMPLATE,
 )
 from renku.core.dataset.providers.doi import DOIProvider
 from renku.core.dataset.providers.repository import RepositoryImporter, make_request
 from renku.core.util import communication
+from renku.core.util.datetime8601 import fix_datetime
 from renku.core.util.doi import extract_doi, get_doi_url, is_doi
 from renku.core.util.urls import remove_credentials
 from renku.domain_model.project_context import project_context
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.models import ProviderDataset, ProviderParameter
     from renku.domain_model.dataset import Dataset, DatasetTag
@@ -79,15 +78,15 @@
 
 class DataverseProvider(ProviderApi, ExportProviderInterface, ImportProviderInterface):
     """Dataverse API provider."""
 
     priority = ProviderPriority.HIGH
     name = "Dataverse"
 
-    def __init__(self, uri: Optional[str], is_doi: bool = False):
+    def __init__(self, uri: str, is_doi: bool = False):
         super().__init__(uri=uri)
 
         self.is_doi = is_doi
         self._server_url = None
         self._dataverse_name = None
         self._publish: bool = False
 
@@ -219,15 +218,15 @@
         if not files:
             raise LookupError("no files have been found - deposit is empty or protected")
 
         return [DataverseFileSerializer(**file) for file in files]
 
     def fetch_provider_dataset(self) -> "ProviderDataset":
         """Deserialize a ``Dataset``."""
-        from marshmallow import pre_load
+        from marshmallow import post_load, pre_load
 
         from renku.command.schema.agent import PersonSchema
         from renku.core.dataset.providers.models import ProviderDataset, ProviderDatasetFile, ProviderDatasetSchema
         from renku.domain_model.dataset import Url, generate_default_name
 
         class DataverseDatasetSchema(ProviderDatasetSchema):
             """Schema for Dataverse datasets."""
@@ -250,14 +249,24 @@
                 # Fix license to be a string
                 license = data.get("license")
                 if license and isinstance(license, dict):
                     data["license"] = license.get("url", "")
 
                 return data
 
+            @post_load
+            def fix_timezone(self, obj, **kwargs):
+                """Add timezone to datetime object."""
+                if obj.get("date_modified"):
+                    obj["date_modified"] = fix_datetime(obj["date_modified"])
+                if obj.get("date_published"):
+                    obj["date_published"] = fix_datetime(obj["date_published"])
+
+                return obj
+
         files = self.get_files()
         dataset = ProviderDataset.from_jsonld(data=self._json, schema_class=DataverseDatasetSchema)
         dataset.version = self.version
         dataset.name = generate_default_name(title=dataset.title or "", version=dataset.version)
         dataset.same_as = (
             Url(url_str=get_doi_url(dataset.identifier))
             if is_doi(dataset.identifier)
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/dataverse_metadata_templates.py` & `renku-2.4.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/doi.py` & `renku-2.4.0rc1/renku/core/dataset/providers/doi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,30 +13,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DOI API integration."""
 
 import urllib
 from pathlib import Path
-from typing import Optional
 
 from renku.core import errors
 from renku.core.dataset.providers.api import ImporterApi, ImportProviderInterface, ProviderApi, ProviderPriority
 from renku.core.util.doi import extract_doi, is_doi
 
 DOI_BASE_URL = "https://dx.doi.org"
 
 
 class DOIProvider(ProviderApi, ImportProviderInterface):
     """`doi.org <http://doi.org>`_ registry API provider."""
 
     priority = ProviderPriority.HIGHER
     name = "DOI"
 
-    def __init__(self, uri: Optional[str], headers=None, timeout=3):
+    def __init__(self, uri: str, headers=None, timeout=3):
         super().__init__(uri=uri)
 
         self.timeout = timeout
         self.headers = headers if headers is not None else {"accept": "application/vnd.citationstyles.csl+json"}
 
     @staticmethod
     def supports(uri) -> bool:
@@ -53,15 +50,15 @@
             """Retrieve metadata for given doi."""
             doi = extract_doi(doi)
             url = make_doi_url(doi)
 
             response = requests.get(url, headers=self.headers)
 
             if response.status_code != 200:
-                raise LookupError("record not found. Status: {}".format(response.status_code))
+                raise LookupError(f"record not found. Status: {response.status_code}")
 
             return response
 
         def serialize(response):
             """Serialize HTTP response for DOI."""
             json_data = response.json()
             data = {key.replace("-", "_").lower(): value for key, value in json_data.items()}
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/factory.py` & `renku-2.4.0rc1/renku/core/dataset/providers/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -64,18 +62,20 @@
         return [p for p in ProviderFactory.get_providers() if issubclass(p, StorageProviderInterface)]
 
     @staticmethod
     def get_add_provider(uri):
         """Get an add provider based on uri."""
         for provider in ProviderFactory.get_add_providers():
             try:
-                if provider.supports(uri):  # type: ignore[union-attr]
-                    return provider(uri=uri)  # type: ignore[call-arg]
+                supports = provider.supports(uri)  # type: ignore[union-attr]
             except BaseException as e:
-                communication.warn(f"Couldn't test provider {provider}: {e}")
+                communication.warn(f"Couldn't test add provider {provider.__class__.__name__}: {e}")
+            else:
+                if supports:
+                    return provider(uri=uri)  # type: ignore[call-arg]
 
         raise errors.DatasetProviderNotFound(uri=uri)
 
     @staticmethod
     def get_export_provider(provider_name):
         """Get the export provider with a given name."""
         provider_name = provider_name.lower()
@@ -97,32 +97,36 @@
                 raise errors.DatasetProviderNotFound(message=f"Cannot parse URL '{uri}'")
 
         warning = ""
         import_providers = ProviderFactory.get_import_providers()
 
         for provider in import_providers:
             try:
-                if provider.supports(uri):  # type: ignore[union-attr]
-                    return provider(uri=uri, is_doi=is_doi_)  # type: ignore[call-arg]
+                supports = provider.supports(uri)  # type: ignore[union-attr]
             except BaseException as e:
                 warning += f"Couldn't test provider {provider}: {e}\n"
+            else:
+                if supports:
+                    return provider(uri=uri, is_doi=is_doi_)  # type: ignore[call-arg]
 
         url = uri.split("/")[1].split(".")[0] if is_doi_ else uri  # NOTE: Get DOI provider name if uri is a DOI
         supported_providers = ", ".join(p.name for p in import_providers)  # type: ignore
         message = warning + f"Provider not found: {url}\nHint: Supported providers are: {supported_providers}"
         raise errors.DatasetProviderNotFound(message=message)
 
     @staticmethod
     def get_storage_provider(uri):
         """Get a backend storage provider based on uri."""
         for provider in ProviderFactory.get_storage_providers():
             try:
-                if provider.supports(uri):  # type: ignore[union-attr]
-                    return provider(uri=uri)  # type: ignore[call-arg]
+                supports = provider.supports_storage(uri)  # type: ignore[union-attr]
             except BaseException as e:
                 communication.warn(f"Couldn't test provider {provider}: {e}")
+            else:
+                if supports:
+                    return provider(uri=uri)  # type: ignore[call-arg]
 
         raise errors.DatasetProviderNotFound(uri=uri)
 
     get_create_provider = get_storage_provider
     get_mount_provider = get_storage_provider
     get_pull_provider = get_storage_provider
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/git.py` & `renku-2.4.0rc1/renku/core/dataset/providers/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -23,18 +21,17 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional, Set, Union
 
 from renku.core import errors
 from renku.core.dataset.providers.api import AddProviderInterface, ProviderApi, ProviderPriority
 from renku.core.storage import pull_paths_from_storage
 from renku.core.util import communication
-from renku.core.util.dataset import check_url
 from renku.core.util.git import clone_repository, get_cache_directory_for_repository
 from renku.core.util.os import get_files, is_subpath
-from renku.core.util.urls import remove_credentials
+from renku.core.util.urls import check_url, remove_credentials
 from renku.domain_model.dataset import RemoteEntity
 from renku.domain_model.project_context import project_context
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.models import DatasetAddMetadata, ProviderParameter
 
 
@@ -68,24 +65,24 @@
                 flags=["r", "ref"],
                 default=None,
                 help="Add files from a specific commit/tag/branch.",
                 type=str,
             ),
         ]
 
-    def add(
+    def get_metadata(
         self,
         uri: str,
         destination: Path,
         *,
         sources: Optional[List[Union[Path, str]]] = None,
         revision: Optional[str] = None,
         **kwargs,
     ) -> List["DatasetAddMetadata"]:
-        """Add files from a URI to a dataset."""
+        """Get metadata of files that will be added to a dataset."""
         from renku.core.dataset.providers.models import DatasetAddAction, DatasetAddMetadata
 
         destination_exists = destination.exists()
         destination_is_dir = destination.is_dir()
 
         remote_repository = clone_repository(
             url=uri,
@@ -109,15 +106,15 @@
 
             paths = set()
             for source in sources:
                 # NOTE: Normalized source to resolve .. references (if any). This preserves wildcards.
                 normalized_source = os.path.normpath(source)
                 absolute_source = os.path.join(remote_repository.path, normalized_source)  # type: ignore
                 # NOTE: Path.glob("root/**") does not return correct results (e.g. it include ``root`` in the result)
-                subpaths = set(Path(p) for p in glob.glob(absolute_source))
+                subpaths = {Path(p) for p in glob.glob(absolute_source)}
                 if len(subpaths) == 0:
                     raise errors.ParameterError("No such file or directory", param_hint=str(source))
                 paths |= subpaths
 
             return paths
 
         def should_copy(source_paths: List[Path]) -> bool:
@@ -126,15 +123,15 @@
             source_is_dir = has_multiple_sources or (n_paths == 1 and source_paths[0].is_dir())
 
             if source_is_dir and destination_exists and not destination_is_dir:
                 raise errors.ParameterError(f"Destination is not a directory: '{destination}'")
 
             return has_multiple_sources or (destination_exists and destination_is_dir)
 
-        def get_metadata(src: Path, dst: Path) -> Optional["DatasetAddMetadata"]:
+        def get_file_metadata(src: Path, dst: Path) -> Optional["DatasetAddMetadata"]:
             path_in_src_repo = src.relative_to(remote_repository.path)  # type: ignore
             path_in_dst_repo = dst.relative_to(project_context.path)
 
             already_copied = path_in_dst_repo in new_files  # A path with the same destination is already copied
             new_files[path_in_dst_repo].append(path_in_src_repo)
             if already_copied:
                 return None
@@ -166,15 +163,15 @@
             dst_root = destination / path.name if is_copy else destination
 
             for file in get_files(path):
                 src = file
                 relative_path = file.relative_to(path)
                 dst = dst_root / relative_path
 
-                metadata = get_metadata(src, dst)
+                metadata = get_file_metadata(src, dst)
                 if metadata:
                     results.append(metadata)
 
         duplicates = [v for v in new_files.values() if len(v) > 1]
         if duplicates:
             files = {str(p) for paths in duplicates for p in paths}
             files_str = "/n/t".join(sorted(files))
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/local.py` & `renku-2.4.0rc1/renku/core/dataset/providers/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Local exporter."""
+"""Local provider for local filesystem."""
 
 import os
 import urllib
 import uuid
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional
 
@@ -29,31 +27,31 @@
     ExporterApi,
     ExportProviderInterface,
     ProviderApi,
     ProviderPriority,
 )
 from renku.core.storage import check_external_storage, track_paths_in_storage
 from renku.core.util import communication
-from renku.core.util.dataset import check_url
 from renku.core.util.metadata import is_protected_path
 from renku.core.util.os import get_absolute_path, is_path_empty, is_subpath
+from renku.core.util.urls import check_url
 from renku.domain_model.project_context import project_context
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.models import DatasetAddMetadata, ProviderParameter
     from renku.domain_model.dataset import Dataset, DatasetTag
 
 
-class FilesystemProvider(ProviderApi, AddProviderInterface, ExportProviderInterface):
+class LocalProvider(ProviderApi, AddProviderInterface, ExportProviderInterface):
     """Local filesystem provider."""
 
     priority = ProviderPriority.LOW
     name = "Local"
 
-    def __init__(self, uri: Optional[str]):
+    def __init__(self, uri: str):
         super().__init__(uri=uri)
 
         self._path: Optional[str] = None
 
     @staticmethod
     def supports(uri: str) -> bool:
         """Whether or not this provider supports a given URI."""
@@ -63,17 +61,14 @@
     @staticmethod
     def get_add_parameters() -> List["ProviderParameter"]:
         """Returns parameters that can be set for add."""
         from renku.core.dataset.providers.models import ProviderParameter
 
         return [
             ProviderParameter(
-                "external", flags=["e", "external"], help="Creates a link to external data.", is_flag=True
-            ),
-            ProviderParameter(
                 "copy",
                 flags=["cp", "copy"],
                 help="Copy files to the dataset's data directory. Mutually exclusive with --move and --link.",
                 is_flag=True,
                 default=False,
             ),
             ProviderParameter(
@@ -95,52 +90,52 @@
     @staticmethod
     def get_export_parameters() -> List["ProviderParameter"]:
         """Returns parameters that can be set for export."""
         from renku.core.dataset.providers.models import ProviderParameter
 
         return [ProviderParameter("path", flags=["p", "path"], help="Path to copy data to.", type=str)]
 
-    def add(
+    def get_metadata(
         self,
         uri: str,
         destination: Path,
         *,
-        external: bool = False,
         move: bool = False,
         copy: bool = False,
         link: bool = False,
         force: bool = False,
         **kwargs,
     ) -> List["DatasetAddMetadata"]:
-        """Add files from a URI to a dataset."""
+        """Get metadata of files that will be added to a dataset."""
         from renku.core.dataset.providers.models import DatasetAddAction, DatasetAddMetadata
 
         repository = project_context.repository
 
-        if sum([move, copy, link]) > 1:
+        flags = sum([move, copy, link])
+        if flags > 1:
             raise errors.ParameterError("--move, --copy and --link are mutually exclusive.")
 
-        default_action = DatasetAddAction.COPY
-        prompt_action = True
+        prompt_action = True if flags == 0 else False
 
         if move:
             default_action = DatasetAddAction.MOVE
-            prompt_action = False
         elif link:
             default_action = DatasetAddAction.SYMLINK
-            prompt_action = False
-        elif copy:
-            prompt_action = False
+        else:
+            default_action = DatasetAddAction.COPY
 
+        ends_with_slash = False
         u = urllib.parse.urlparse(uri)
         path = u.path
 
-        action = DatasetAddAction.SYMLINK if external else default_action
+        action = default_action
         source_root = Path(get_absolute_path(path))
-        warnings: List[str] = []
+
+        if source_root.is_dir() and uri.endswith("/"):
+            ends_with_slash = True
 
         def check_recursive_addition(src: Path):
             if is_subpath(destination, src):
                 raise errors.ParameterError(f"Cannot recursively add path containing dataset's data directory: {path}")
 
         def get_destination_root():
             destination_exists = destination.exists()
@@ -152,28 +147,29 @@
             check_recursive_addition(source_root)
 
             if not source_root.exists():
                 raise errors.ParameterError(f"Cannot find source file: {path}")
             if source_root.is_dir() and destination_exists and not destination_is_dir:
                 raise errors.ParameterError(f"Cannot copy directory '{path}' to non-directory '{destination}'")
 
-            return destination / source_root.name if destination_exists and destination_is_dir else destination
+            if destination_exists and destination_is_dir:
+                if ends_with_slash:
+                    return destination
+
+                return destination / source_root.name
+            return destination
 
-        def get_metadata(src: Path) -> DatasetAddMetadata:
-            is_tracked = repository.contains(src)
+        def get_file_metadata(src: Path) -> DatasetAddMetadata:
             in_datadir = is_subpath(src, destination)
 
             relative_path = src.relative_to(source_root)
             dst = destination_root / relative_path
 
-            if is_tracked and external:
-                warnings.append(str(src.relative_to(project_context.path)))
-
-            if not is_tracked and not external and action == DatasetAddAction.SYMLINK:
-                # NOTE: we need to commit src if it is linked to and not external.
+            # NOTE: Add link targets in case they aren't already tracked in the repository
+            if action == DatasetAddAction.SYMLINK:
                 if check_external_storage():
                     track_paths_in_storage(src)
                 repository.add(src)
             source_url = os.path.relpath(src, project_context.path)
             return DatasetAddMetadata(
                 entity_path=Path(source_url) if in_datadir else dst.relative_to(project_context.path),
                 url=os.path.relpath(src, project_context.path),
@@ -189,32 +185,28 @@
             for file in source_root.rglob("*"):
                 if is_protected_path(file):
                     raise errors.ProtectedFiles([file])
 
                 if file.is_dir():
                     check_recursive_addition(file)
                     continue
-                results.append(get_metadata(file))
+                results.append(get_file_metadata(file))
         else:
-            results = [get_metadata(source_root)]
+            results = [get_file_metadata(source_root)]
 
-        if not force and prompt_action and not external:
+        if not force and prompt_action:
             communication.confirm(
                 f"The following files will be copied to {destination.relative_to(project_context.path)} "
                 "(use '--move' or '--link' to move or symlink them instead, '--copy' to not show this warning):\n\t"
                 + "\n\t".join(str(e.source) for e in results)
                 + "\nProceed?",
                 abort=True,
                 warning=True,
             )
 
-        if warnings:
-            message = "\n\t".join(warnings)
-            communication.warn(f"Warning: The following files cannot be added as external:\n\t{message}")
-
         return results
 
     def get_exporter(
         self, dataset: "Dataset", *, tag: Optional["DatasetTag"], path: Optional[str] = None, **kwargs
     ) -> "LocalExporter":
         """Create export manager for given dataset."""
         self._path = path
@@ -222,15 +214,15 @@
 
     def get_importer(self, uri, **kwargs):
         """Get import manager."""
         raise NotImplementedError
 
 
 class LocalExporter(ExporterApi):
-    """Local export manager."""
+    """Local filesystem export manager."""
 
     def __init__(self, dataset: "Dataset", tag: Optional["DatasetTag"], path: Optional[str]):
         super().__init__(dataset)
         self._path: Optional[str] = path
         self._tag: Optional["DatasetTag"] = tag
 
     @staticmethod
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/models.py` & `renku-2.4.0rc1/renku/core/dataset/providers/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -51,28 +51,29 @@
     entity_path: Path  # Entity path relative to the project's root
     url: str
     action: DatasetAddAction
     source: Path
     destination: Path
     provider: Optional["StorageProviderInterface"] = None
     based_on: Optional["RemoteEntity"] = None
+    size: Optional[int] = None
 
     @property
     def has_action(self) -> bool:
         """Returns if file's action is not NONE."""
         return self.action != DatasetAddAction.NONE
 
     @property
     def metadata_only(self) -> bool:
         """Returns if file should be added to a remote storage."""
         return self.action == DatasetAddAction.METADATA_ONLY
 
     @property
-    def remote_storage(self) -> bool:
-        """Returns if file is from a remote storage."""
+    def from_cloud_storage(self) -> bool:
+        """Returns if file is from a cloud storage."""
         return self.action == DatasetAddAction.REMOTE_STORAGE
 
     def get_absolute_commit_path(self, project_path: Path) -> str:
         """Return path of the file in the repository."""
         return os.path.join(project_path, self.entity_path)
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/olos.py` & `renku-2.4.0rc1/renku/core/dataset/providers/olos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -37,15 +35,15 @@
 
 class OLOSProvider(ProviderApi, ExportProviderInterface):
     """Provider for OLOS integration."""
 
     priority = ProviderPriority.HIGH
     name = "OLOS"
 
-    def __init__(self, uri: Optional[str], is_doi: bool = False):
+    def __init__(self, uri: str, is_doi: bool = False):
         super().__init__(uri=uri)
 
         self.is_doi = is_doi
         self._server_url = None
 
     @staticmethod
     def supports(uri):
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/renku.py` & `renku-2.4.0rc1/renku/core/dataset/providers/renku.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -42,15 +40,15 @@
 
 class RenkuProvider(ProviderApi, ImportProviderInterface):
     """Renku API provider."""
 
     priority = ProviderPriority.HIGH
     name = "Renku"
 
-    def __init__(self, uri: Optional[str], **_):
+    def __init__(self, uri: str, **_):
         super().__init__(uri=uri)
 
         self._accept = "application/json"
         self._authorization_header: Optional[Dict[str, str]] = None
         self._gitlab_token: Optional[str] = None
         self._renku_token: Optional[str] = None
         self._tag: Optional[str] = None
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/repository.py` & `renku-2.4.0rc1/renku/core/dataset/providers/repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -58,10 +56,10 @@
 
 def make_request(url, accept: str = "application/json"):
     """Execute network request."""
     from renku.core.util import requests
 
     response = requests.get(url, headers={"Accept": accept})
     if response.status_code != 200:
-        raise LookupError("record not found. Status: {}".format(response.status_code))
+        raise LookupError(f"record not found. Status: {response.status_code}")
 
     return response
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/web.py` & `renku-2.4.0rc1/renku/core/dataset/providers/web.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,28 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Web dataset provider."""
 
-import concurrent.futures
-import os
 import urllib
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Tuple
 from urllib.parse import urlparse
 
 from renku.core import errors
 from renku.core.constant import CACHE
 from renku.core.dataset.providers.api import AddProviderInterface, ProviderApi, ProviderPriority
-from renku.core.util import communication
-from renku.core.util.contexts import wait_for
-from renku.core.util.dataset import check_url
-from renku.core.util.urls import remove_credentials
+from renku.core.util.urls import check_url, remove_credentials
+from renku.core.util.util import parallel_execute
 from renku.domain_model.project_context import project_context
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.models import DatasetAddMetadata
 
 
 class WebProvider(ProviderApi, AddProviderInterface):
@@ -45,25 +39,25 @@
 
     @staticmethod
     def supports(uri: str) -> bool:
         """Whether or not this provider supports a given URI."""
         is_remote, is_git = check_url(uri)
         return is_remote and not is_git
 
-    def add(
+    def get_metadata(
         self,
         uri: str,
         destination: Path,
         *,
         extract: bool = False,
         filename: Optional[str] = None,
         multiple: bool = False,
         **kwargs,
     ) -> List["DatasetAddMetadata"]:
-        """Add files from a URI to a dataset."""
+        """Get metadata of files that will be added to a dataset."""
         dataset = kwargs.get("dataset")
         if dataset and dataset.storage and urlparse(dataset.storage).scheme != urlparse(uri).scheme:
             raise errors.ParameterError(
                 f"The scheme of the url {uri} does not match the defined storage url {dataset.storage}."
             )
 
         return download_file(
@@ -101,36 +95,35 @@
     if "dropbox.com" in url.netloc:
         url = _ensure_dropbox(url)
 
     return urllib.parse.urlunparse(url)
 
 
 def download_file(
-    project_path: Path,
     uri: str,
+    filename: Optional[str] = None,
+    *,
+    project_path: Path,
     destination: Path,
     extract: bool = False,
-    filename: Optional[str] = None,
     multiple: bool = False,
-    delay: float = 0,
 ) -> List["DatasetAddMetadata"]:
     """Download a file from a URI and return its metadata."""
     from renku.core.dataset.providers.models import DatasetAddAction, DatasetAddMetadata
     from renku.core.util import requests
 
     uri = requests.get_redirect_url(uri)  # TODO: Check that this is not duplicate
     uri = _provider_check(uri)
 
     with project_context.with_path(project_path):
         try:
             # NOTE: If execution time was less than the delay, block the request until delay seconds are passed
-            with wait_for(delay):
-                tmp_root, paths = requests.download_file(
-                    base_directory=project_context.metadata_path / CACHE, url=uri, filename=filename, extract=extract
-                )
+            tmp_root, paths = requests.download_file(
+                base_directory=project_context.metadata_path / CACHE, url=uri, filename=filename, extract=extract
+            )
         except errors.RequestError as e:  # pragma nocover
             raise errors.OperationError(f"Cannot download from {uri}") from e
 
         paths = [p for p in paths if not p.is_dir()]
 
         if len(paths) > 1 or multiple:
             if destination.exists() and not destination.is_dir():
@@ -160,41 +153,16 @@
     assert len(urls) == len(names), f"Number of URL and names don't match {len(urls)} != {len(names)}"
 
     if destination.exists() and not destination.is_dir():
         raise errors.ParameterError(f"Destination is not a directory: '{destination}'")
 
     destination.mkdir(parents=True, exist_ok=True)
 
-    listeners = communication.get_listeners()
-
-    def subscribe_communication_listeners(function, **kwargs):
-        try:
-            for communicator in listeners:
-                communication.subscribe(communicator)
-            return function(**kwargs)
-        finally:
-            for communicator in listeners:
-                communication.unsubscribe(communicator)
-
-    files = []
-    n_cpus = os.cpu_count() or 1
-    max_workers = min(n_cpus + 4, 8)
-    with concurrent.futures.ThreadPoolExecutor(max_workers) as executor:
-        futures = {
-            executor.submit(
-                subscribe_communication_listeners,
-                download_file,
-                project_path=project_context.path,
-                uri=url,
-                destination=destination,
-                extract=extract,
-                filename=name,
-                multiple=True,
-                delay=max_workers,  # NOTE: Rate limit to 1 request/second
-            )
-            for url, name in zip(urls, names)
-        }
-
-        for future in concurrent.futures.as_completed(futures):
-            files.extend(future.result())
-
-    return files
+    return parallel_execute(
+        download_file,
+        urls,
+        names,
+        project_path=project_context.path,
+        destination=destination,
+        extract=extract,
+        multiple=True,
+    )
```

### Comparing `renku-2.3.2/renku/core/dataset/providers/zenodo.py` & `renku-2.4.0rc1/renku/core/dataset/providers/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -60,15 +58,15 @@
 
 class ZenodoProvider(ProviderApi, ExportProviderInterface, ImportProviderInterface):
     """Zenodo registry API provider."""
 
     priority = ProviderPriority.HIGH
     name = "Zenodo"
 
-    def __init__(self, uri: Optional[str], is_doi: bool = False):
+    def __init__(self, uri: str, is_doi: bool = False):
         super().__init__(uri=uri)
 
         self.is_doi = is_doi
         self._publish: bool = False
 
     @staticmethod
     def supports(uri):
@@ -517,15 +515,15 @@
 
         try:
             requests.check_response(response=response)
         except errors.RequestError:
             if response.status_code == 400:
                 err_response = response.json()
                 messages = [
-                    '"{0}" failed with "{1}"'.format(err["field"], err["message"]) for err in err_response["errors"]
+                    '"{}" failed with "{}"'.format(err["field"], err["message"]) for err in err_response["errors"]
                 ]
 
                 raise errors.ExportError(
                     "\n" + "\n".join(messages) + "\nSee `renku dataset edit -h` for details on how to edit" " metadata"
                 )
             else:
                 raise errors.ExportError(response.content)
```

### Comparing `renku-2.3.2/renku/core/dataset/request_model.py` & `renku-2.4.0rc1/renku/core/dataset/request_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/dataset/tag.py` & `renku-2.4.0rc1/renku/core/dataset/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/errors.py` & `renku-2.4.0rc1/renku/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -64,15 +62,15 @@
 class ParameterError(RenkuException):
     """Raise in case of invalid parameter."""
 
     def __init__(self, message, param_hint=None, show_prefix: bool = True):
         """Build a custom message."""
         if param_hint:
             if isinstance(param_hint, (tuple, list)):
-                param_hint = " / ".join('"{}"'.format(x) for x in param_hint)
+                param_hint = " / ".join(f'"{x}"' for x in param_hint)
             message = f"Invalid parameter value for {param_hint}: {message}"
         else:
             if show_prefix:
                 message = f"Invalid parameter value - {message}"
 
         super().__init__(message)
 
@@ -115,29 +113,29 @@
 
 
 class DirtyRepository(RenkuException):
     """Raise when trying to work with dirty repository."""
 
     def __init__(self, repository):
         """Build a custom message."""
-        super(DirtyRepository, self).__init__(
+        super().__init__(
             "The repository is dirty. "
             'Please use the "git" command to clean it.'
             "\n\n" + str(repository.status()) + "\n\n"
             "Once you have added the untracked files, "
             'commit them with "git commit".'
         )
 
 
 class DirtyRenkuDirectory(RenkuException):
     """Raise when a directory in the renku repository is dirty."""
 
     def __init__(self, repository):
         """Build a custom message."""
-        super(DirtyRenkuDirectory, self).__init__(
+        super().__init__(
             (
                 "The renku directory {0} contains uncommitted changes.\n"
                 'Please use "git" command to resolve.\n'
                 "Files within {0} directory "
                 "need to be manually committed or removed."
             ).format(RENKU_HOME)
             + "\n\n"
@@ -147,15 +145,15 @@
 
 
 class ProtectedFiles(RenkuException):
     """Raise when trying to work with protected files."""
 
     def __init__(self, ignored: List[Union[Path, str]]):
         """Build a custom message."""
-        super(ProtectedFiles, self).__init__(
+        super().__init__(
             "The following paths are protected as part of renku:"
             "\n\n" + "\n".join("\t" + click.style(str(path), fg="yellow") for path in ignored) + "\n"
             "They cannot be used in renku commands."
         )
 
 
 class MigrationRequired(RenkuException):
@@ -183,44 +181,44 @@
 
 
 class NothingToCommit(RenkuException):
     """Raise when there is nothing to commit."""
 
     def __init__(self):
         """Build a custom message."""
-        super(NothingToCommit, self).__init__("There is nothing to commit.")
+        super().__init__("There is nothing to commit.")
 
 
 class CommitMessageEmpty(RenkuException):
     """Raise invalid commit message."""
 
     def __init__(self):
         """Build a custom message."""
-        super(CommitMessageEmpty, self).__init__("Invalid commit message.")
+        super().__init__("Invalid commit message.")
 
 
 class FailedMerge(RenkuException):
     """Raise when automatic merge failed."""
 
     def __init__(self, repository, branch, merge_args):
         """Build a custom message."""
-        super(FailedMerge, self).__init__(
-            "Failed merge of branch {0} with args {1}".format(branch, ",".join(merge_args))
+        super().__init__(
+            "Failed merge of branch {} with args {}".format(branch, ",".join(merge_args))
             + "The automatic merge failed.\n\n"
             'Please use the "git" command to clean it.'
             "\n\n" + str(repository.status())
         )
 
 
 class UnmodifiedOutputs(RenkuException):
     """Raise when there are unmodified outputs in the repository."""
 
     def __init__(self, repository, unmodified):
         """Build a custom message."""
-        super(UnmodifiedOutputs, self).__init__(
+        super().__init__(
             "There are no detected new outputs or changes.\n"
             "\nIf any of the following files should be considered as outputs,"
             "\nthey need to be removed first in order to be detected "
             "correctly."
             '\n  (use "git rm <file>..." to remove them first)'
             "\n\n" + "\n".join("\t" + click.style(path, fg="green") for path in unmodified) + "\n"
             "\nOnce you have removed the files that should be used as outputs,"
@@ -243,35 +241,35 @@
             "There are not any detected outputs in the repository. This can be due to your command not creating "
             "any new files or due to files that get created already existing before the command was run. In the "
             "latter case, you can remove those files prior to running your command.\nIf you want to track the command"
             "without outputs, use the use --no-output option.\nYou can also use the --output flag to track outputs"
             "manually."
         )
 
-        super(OutputsNotFound, self).__init__(msg)
+        super().__init__(msg)
 
 
 class InvalidInputPath(RenkuException):
     """Raise when input path does not exist or is not in the repository."""
 
 
 class InvalidSuccessCode(RenkuException):
     """Raise when the exit-code is not 0 or redefined."""
 
     def __init__(self, return_code, success_codes=None, message=None):
         """Build a custom message."""
         if message:
             msg = message
         elif not success_codes:
-            msg = "Command returned non-zero exit status {0}.".format(return_code)
+            msg = f"Command returned non-zero exit status {return_code}."
         else:
-            msg = "Command returned {0} exit status, but it expects {1}".format(
-                return_code, ", ".join((str(code) for code in success_codes))
+            msg = "Command returned {} exit status, but it expects {}".format(
+                return_code, ", ".join(str(code) for code in success_codes)
             )
-        super(InvalidSuccessCode, self).__init__(msg)
+        super().__init__(msg)
 
 
 class DatasetNotFound(DatasetException):
     """Raise when dataset is not found."""
 
     def __init__(self, *, name=None, message=None):
         """Build a custom message."""
@@ -342,15 +340,15 @@
             "you could be committing\n"
             "large files directly to the git repository.\n\n"
             "If this is your intention, please repeat the command with "
             "the -S flag (e.g. renku -S run <cmd>), \n"
             'otherwise install LFS with "git lfs install --local".'
         )
 
-        super(ExternalStorageNotInstalled, self).__init__(msg)
+        super().__init__(msg)
 
 
 class ExternalStorageDisabled(RenkuException):
     """Raise when disabled repository storage API is trying to be used."""
 
     def __init__(self):
         """Build a custom message."""
@@ -361,35 +359,35 @@
             "you could be committing\n"
             "large files directly to the git repository.\n\n"
             "If this is your intention, please repeat the command with "
             "the -S flag (e.g. renku -S run <cmd>), \n"
             'otherwise install e.g. git-LFS with "git lfs install --local".'
         )
 
-        super(ExternalStorageDisabled, self).__init__(msg)
+        super().__init__(msg)
 
 
 class UninitializedProject(RenkuException):
     """Raise when a project does not seem to have been initialized yet."""
 
     def __init__(self, repo_path):
         """Build a custom message."""
         msg = "{repo_path} does not seem to be a Renku project.\n" 'Initialize it with "renku init"'.format(
             repo_path=repo_path
         )
-        super(UninitializedProject, self).__init__(msg)
+        super().__init__(msg)
 
 
 class InvalidAccessToken(RenkuException):
     """Raise when access token is incorrect."""
 
     def __init__(self):
         """Build a custom message."""
         msg = "Invalid access token.\n" "Please, update access token."
-        super(InvalidAccessToken, self).__init__(msg)
+        super().__init__(msg)
 
 
 class GitError(RenkuException):
     """Raised when a Git operation fails."""
 
 
 class InvalidGitURL(GitError):
@@ -523,33 +521,33 @@
 
     def __init__(self):
         """Build a custom message."""
         msg = (
             "NodeJs could not be found on this system\n"
             "Please install it, for details see https://nodejs.org/en/download/package-manager/"
         )
-        super(NodeNotFoundError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class SSHNotFoundError(RenkuException):
     """Raised when SSH client is not installed on the system."""
 
     def __init__(self):
         """Build a custom message."""
         msg = "SSH client (ssh) could not be found on this system"
-        super(SSHNotFoundError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class SSHNotSetupError(RenkuException):
     """Raised when SSH client is not installed on the system."""
 
     def __init__(self):
         """Build a custom message."""
         msg = "SSH is not set up correctly, use 'renku session ssh-setup' to set it up."
-        super(SSHNotSetupError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class ObjectNotFoundError(RenkuException):
     """Raised when an object is not found in the storage."""
 
     def __init__(self, filename):
         """Embed exception and build a custom message."""
```

### Comparing `renku-2.3.2/renku/core/gc.py` & `renku-2.4.0rc1/renku/core/gc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/git.py` & `renku-2.4.0rc1/renku/core/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/githooks.py` & `renku-2.4.0rc1/renku/core/githooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/init.py` & `renku-2.4.0rc1/renku/core/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -83,15 +81,15 @@
                         break
 
                 with with_worktree(
                     branch_name=branch_name,
                     commit=repository.head.commit,
                     merge_args=["--no-ff", "-s", "recursive", "-X", "ours", "--allow-unrelated-histories"],
                 ):
-                    communication.warn("Saving current data in branch {0}".format(branch_name))
+                    communication.warn(f"Saving current data in branch {branch_name}")
         except AttributeError:
             communication.echo("Warning! Overwriting non-empty folder.")
         except errors.GitCommandError:
             raise
 
     return branch_name
 
@@ -374,14 +372,15 @@
         metadata["name"] = name
         metadata["__name__"] = name
 
     metadata["__template_version__"] = template_version
 
     template = Template(
         id=metadata["__template_id__"],
+        aliases=[],
         name="",
         description="",
         parameters={},
         icon="",
         ssh_supported=ssh_supported,
         immutable_files=immutable_template_files or [],
         allow_update=automated_template_update,
```

### Comparing `renku-2.3.2/renku/core/interface/__init__.py` & `renku-2.4.0rc1/renku/core/workflow/model/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku management interfaces."""
+"""Renku workflow models."""
```

### Comparing `renku-2.3.2/renku/core/interface/activity_gateway.py` & `renku-2.4.0rc1/renku/core/interface/activity_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/interface/database_gateway.py` & `renku-2.4.0rc1/renku/core/interface/database_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/interface/dataset_gateway.py` & `renku-2.4.0rc1/renku/core/interface/dataset_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/interface/plan_gateway.py` & `renku-2.4.0rc1/renku/core/interface/plan_gateway.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/interface/project_gateway.py` & `renku-2.4.0rc1/renku/core/interface/project_gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/interface/storage.py` & `renku-2.4.0rc1/renku/core/interface/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -16,88 +15,77 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """External storage interface."""
 
 import abc
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 if TYPE_CHECKING:
-    from renku.core.dataset.providers.api import ProviderApi, ProviderCredentials
+    from renku.core.dataset.providers.api import CloudStorageProviderType, ProviderCredentials
 
 
 @dataclass
 class FileHash:
-    """The has for a file at a specific location."""
+    """The hash for a file at a specific location."""
 
-    base_uri: str
+    uri: str
     path: str
-    hash: Optional[str] = None
-    hash_type: Optional[str] = None
-    modified_datetime: Optional[str] = None
-
-    @property
-    def full_uri(self) -> str:
-        """Return the full uri to the file."""
-        return str(Path(self.base_uri) / Path(self.path))
+    size: Optional[int]  # Size in bytes
+    hash: Optional[str]
 
 
 class IStorageFactory(abc.ABC):
-    """Interface to get an external storage."""
+    """Interface to get a cloud storage."""
 
     @staticmethod
     @abc.abstractmethod
     def get_storage(
         storage_scheme: str,
-        provider: "ProviderApi",
+        provider: "CloudStorageProviderType",
         credentials: "ProviderCredentials",
         configuration: Dict[str, str],
-        uri_convertor: Callable[[str], str],
     ) -> "IStorage":
         """Return a storage that handles provider.
 
         Args:
             storage_scheme(str): Storage name.
-            provider(ProviderApi): The backend provider.
+            provider(CloudStorageProviderType): The backend provider.
             credentials(ProviderCredentials): Credentials for the provider.
             configuration(Dict[str, str]): Storage-specific configuration that are passed to the IStorage implementation
-            uri_convertor(Callable[[str], str]): A function that converts backend-specific URI to a URI that is usable
-                by the IStorage implementation.
 
         Returns:
             An instance of IStorage.
         """
         raise NotImplementedError
 
 
 class IStorage(abc.ABC):
     """Interface for the external storage handler."""
 
     def __init__(
         self,
         storage_scheme: str,
-        provider: "ProviderApi",
+        provider: "CloudStorageProviderType",
         credentials: "ProviderCredentials",
         provider_configuration: Dict[str, str],
-        provider_uri_convertor: Callable[[str], str],
     ):
         self._storage_scheme: str = storage_scheme
-        self._provider: "ProviderApi" = provider
+        self._provider: "CloudStorageProviderType" = provider
         self._credentials: "ProviderCredentials" = credentials
         self._provider_configuration: Dict[str, str] = provider_configuration
-        self._provider_uri_convertor: Callable[[str], str] = provider_uri_convertor
 
     @property
     def credentials(self) -> "ProviderCredentials":
         """Return the provider credentials for this storage handler."""
         return self._credentials
 
     @property
-    def provider(self) -> "ProviderApi":
+    def provider(self) -> "CloudStorageProviderType":
         """Return the dataset provider for this storage handler."""
         return self._provider
 
     @property
     def storage_scheme(self) -> str:
         """Storage's URI scheme."""
         return self._storage_scheme
@@ -119,14 +107,19 @@
 
     @abc.abstractmethod
     def get_hashes(self, uri: str, hash_type: str = "md5") -> List[FileHash]:
         """Get the hashes of all files at the uri."""
         raise NotImplementedError
 
     @abc.abstractmethod
+    def is_directory(self, uri: str) -> bool:
+        """Return True if URI points to a directory."""
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def mount(self, path: Union[Path, str]) -> None:
         """Mount the provider's URI to the given path."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def upload(self, source: Union[Path, str], uri: str) -> None:
         """Upload data from ``source`` to ``uri``."""
```

### Comparing `renku-2.3.2/renku/core/interface/workflow_file_parser.py` & `renku-2.4.0rc1/renku/core/interface/workflow_file_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -36,15 +35,15 @@
 
         Returns:
             Tuple[IWorkflowParser, str]: A tuple of the provider itself and the workflow parser name.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def parse(self, path: Union[Path, str]) -> "WorkflowFile":
+    def parse(self, path: Union[Path, str]) -> WorkflowFile:
         """Parse a given workflow file using the provider.
 
         Args:
             path(Union[Path, str]): Path to the workflow file to parse.
 
         Returns:
             WorkflowFile: A ``WorkflowFile`` generated by the provider.
```

### Comparing `renku-2.3.2/renku/core/login.py` & `renku-2.4.0rc1/renku/core/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/migration/__init__.py` & `renku-2.4.0rc1/renku/core/migration/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/m_0003__0_pyld2.py` & `renku-2.4.0rc1/renku/core/migration/m_0003__0_pyld2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0003__1_jsonld.py` & `renku-2.4.0rc1/renku/core/migration/m_0003__1_jsonld.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -188,23 +187,23 @@
 
     if isinstance(files, dict):
         files = list(files.values())
 
     for file_ in files:
         path = Path(file_.get("path"), ".")
         if path.is_absolute():
-            file_["path"] = str(path.relative_to((os.getcwd())))
+            file_["path"] = str(path.relative_to(os.getcwd()))
     data["files"] = files
     return data
 
 
 def _migrate_doi_identifier(data):
     """If the dataset _id is doi, make it a UUID."""
     from renku.core.util.doi import is_doi
-    from renku.core.util.uuid import is_uuid
+    from renku.core.util.util import is_uuid
 
     _id = data.get("_id", "")
     identifier = data.get("identifier", "")
 
     if not is_uuid(_id):
         if not is_uuid(identifier):
             possible_identifier = Path(identifier).name
```

### Comparing `renku-2.3.2/renku/core/migration/m_0003__2_initial.py` & `renku-2.4.0rc1/renku/core/migration/m_0003__2_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -103,15 +102,15 @@
                 expected_path = project_context.path / DATA_DIR / dataset.name / file_.path
                 if expected_path.exists():
                     file_.path = expected_path.relative_to(project_context.path)
 
         dataset.to_yaml(new_path)
 
         Path(old_path).unlink()
-        ref = LinkReference.create(name="datasets/{0}".format(name), force=True)
+        ref = LinkReference.create(name=f"datasets/{name}", force=True)
         ref.set_reference(new_path)
 
     if changed:
         project_path = project_context.metadata_path.joinpath(OLD_METADATA_PATH)
         project = Project.from_yaml(project_path)
         project.version = "3"
         project.to_yaml(project_path)
@@ -128,15 +127,15 @@
         else:
             dataset.name = generate_default_name(dataset.name)
 
         expected_path = get_datasets_path() / dataset.identifier
 
         # migrate the refs
         if not is_using_temporary_datasets_path():
-            ref = LinkReference.create(name="datasets/{0}".format(dataset.name), force=True)
+            ref = LinkReference.create(name=f"datasets/{dataset.name}", force=True)
             ref.set_reference(expected_path / OLD_METADATA_PATH)
 
         if not expected_path.exists():
             old_dataset_path = dataset.path
             if not is_using_temporary_datasets_path():
                 expected_path.parent.mkdir(parents=True, exist_ok=True)
                 shutil.move(old_dataset_path, expected_path)
```

### Comparing `renku-2.3.2/renku/core/migration/m_0004__0_pyld2.py` & `renku-2.4.0rc1/renku/core/migration/m_0004__0_pyld2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0004__submodules.py` & `renku-2.4.0rc1/renku/core/migration/m_0004__submodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0005__1_pyld2.py` & `renku-2.4.0rc1/renku/core/migration/m_0005__1_pyld2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0005__2_cwl.py` & `renku-2.4.0rc1/renku/core/migration/m_0005__2_cwl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -308,15 +307,15 @@
     for a in cmd_line_tool.arguments:
         id_ = CommandArgument.generate_id(base_id, a.position)
         run.arguments.append(CommandArgument(id=id_, position=a.position, value=a.valueFrom))
 
     if not persist:
         return run, None
 
-    step_name = "{0}_{1}.yaml".format(uuid.uuid4().hex, secure_filename("_".join(cmd_line_tool.baseCommand)))
+    step_name = "{}_{}.yaml".format(uuid.uuid4().hex, secure_filename("_".join(cmd_line_tool.baseCommand)))
 
     absolute_path = project_context.metadata_path / OLD_WORKFLOW_PATH / step_name
     path = absolute_path.relative_to(project_context.path)
 
     run.path = path
     process_run = ProcessRun.from_run(run, path, commit=commit)
     process_run.invalidated = _invalidations_from_commit(commit)
@@ -336,15 +335,15 @@
         commit = migration_context.cache.find_previous_commit(path)
     run = Run(path=path, commit=commit)
     rel_path = Path(path).relative_to(project_context.path)
     label = f"{rel_path}@{commit.hexsha}"
     identifier = sha1(label.encode("utf-8")).hexdigest()
     run._id = Run.generate_id(identifier=identifier)
 
-    name = "{0}_migrated.yaml".format(uuid.uuid4().hex)
+    name = f"{uuid.uuid4().hex}_migrated.yaml"
 
     wf_path = project_context.metadata_path / OLD_WORKFLOW_PATH
     run.path = (wf_path / name).relative_to(project_context.path)
 
     for step in workflow.steps:
         if isinstance(step.run, dict):
             continue
```

### Comparing `renku-2.3.2/renku/core/migration/m_0006__dataset_context.py` & `renku-2.4.0rc1/renku/core/migration/m_0006__dataset_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0007__source_url.py` & `renku-2.4.0rc1/renku/core/migration/m_0007__source_url.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0008__dataset_metadata.py` & `renku-2.4.0rc1/renku/core/migration/m_0008__dataset_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/core/migration/m_0009__new_metadata_storage.py` & `renku-2.4.0rc1/renku/core/migration/m_0009__new_metadata_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -24,14 +23,16 @@
 from collections import defaultdict
 from hashlib import sha1
 from itertools import chain
 from pathlib import Path, PurePosixPath
 from typing import TYPE_CHECKING, List, Optional, Union, cast
 from urllib.parse import urlparse
 
+import deal
+
 from renku.command.command_builder import inject
 from renku.core import errors
 from renku.core.dataset.datasets_provenance import DatasetsProvenance
 from renku.core.interface.activity_gateway import IActivityGateway
 from renku.core.interface.database_gateway import IDatabaseGateway
 from renku.core.interface.project_gateway import IProjectGateway
 from renku.core.migration.models import v9 as old_schema
@@ -43,15 +44,16 @@
     read_project_version_from_yaml,
     set_temporary_datasets_path,
     unset_temporary_datasets_path,
 )
 from renku.core.migration.utils.conversion import convert_dataset
 from renku.core.util import communication
 from renku.core.util.yaml import load_yaml
-from renku.domain_model.entity import NON_EXISTING_ENTITY_CHECKSUM, Collection, Entity
+from renku.domain_model.constant import NON_EXISTING_ENTITY_CHECKSUM
+from renku.domain_model.entity import Collection, Entity
 from renku.domain_model.project_context import has_graph_files, project_context
 from renku.domain_model.provenance.activity import Activity, Association, Generation, Usage
 from renku.domain_model.provenance.agent import Person, SoftwareAgent
 from renku.domain_model.provenance.parameter import ParameterValue
 from renku.domain_model.workflow.parameter import (
     DIRECTORY_MIME_TYPE,
     CommandInput,
@@ -344,45 +346,50 @@
     assert len(activities) == len(workflow_run.subprocesses)
     return activities
 
 
 def _process_workflows(
     migration_context: MigrationContext, activity_gateway: IActivityGateway, commit: "Commit", remove: bool
 ):
+    try:
+        deal.disable(warn=False)
+        for file in commit.get_changes(f"{project_context.metadata_path}/workflow/*.yaml"):
+            if file.deleted:
+                continue
+
+            path: str = file.b_path
+
+            if not path.startswith(".renku/workflow") or not path.endswith(".yaml"):
+                continue
+
+            if not (project_context.path / path).exists():
+                communication.warn(f"Workflow file does not exists: '{path}'")
+                continue
+
+            workflow = old_schema.Activity.from_yaml(path=path)
+
+            if isinstance(workflow, old_schema.WorkflowRun):
+                activities = _get_process_runs(workflow)
+            else:
+                activities = [workflow]
+
+            for old_activity in activities:
+                new_activities = _process_run_to_new_activity(
+                    migration_context=migration_context, process_run=old_activity
+                )
+                for new_activity in new_activities:
+                    activity_gateway.add(new_activity)
 
-    for file in commit.get_changes(f"{project_context.metadata_path}/workflow/*.yaml"):
-        if file.deleted:
-            continue
-
-        path: str = file.b_path
-
-        if not path.startswith(".renku/workflow") or not path.endswith(".yaml"):
-            continue
-
-        if not (project_context.path / path).exists():
-            communication.warn(f"Workflow file does not exists: '{path}'")
-            continue
-
-        workflow = old_schema.Activity.from_yaml(path=path)
-
-        if isinstance(workflow, old_schema.WorkflowRun):
-            activities = _get_process_runs(workflow)
-        else:
-            activities = [workflow]
-
-        for old_activity in activities:
-            new_activities = _process_run_to_new_activity(migration_context=migration_context, process_run=old_activity)
-            for new_activity in new_activities:
-                activity_gateway.add(new_activity)
-
-        if remove:
-            try:
-                os.remove(file.b_path)
-            except FileNotFoundError:
-                pass
+            if remove:
+                try:
+                    os.remove(file.b_path)
+                except FileNotFoundError:
+                    pass
+    finally:
+        deal.enable()
 
 
 def _process_run_to_new_activity(
     migration_context: MigrationContext, process_run: old_schema.ProcessRun
 ) -> List[Activity]:
     """Convert a ProcessRun to a new Activity."""
```

### Comparing `renku-2.3.2/renku/core/migration/m_0010__metadata_fixes.py` & `renku-2.4.0rc1/renku/core/migration/m_0010__metadata_fixes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -95,15 +94,15 @@
             nested_update(data, target_key="@renku_data_type", transforms=transformation)
 
             if compressed:
                 with open(path, "wb") as fb, compressor.stream_writer(fb) as compression_writer:
                     with io.TextIOWrapper(compression_writer) as out:
                         json.dump(data, out, ensure_ascii=False)
             else:
-                with open(path, "wt") as ft:
+                with open(path, "w") as ft:
                     json.dump(data, ft, ensure_ascii=False, sort_keys=True, indent=2)
 
 
 def nested_update(data: Dict[str, Any], target_key: str, transforms: List[Tuple[str, str]]) -> None:
     """Update a key's value based on transformations (from, to) in a deeply nested dictionary."""
     for k in list(data.keys()):
         value = data[k]
```

### Comparing `renku-2.3.2/renku/core/migration/migrate.py` & `renku-2.4.0rc1/renku/core/migration/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -217,15 +216,15 @@
     from renku import __version__
 
     if not project_context.dockerfile_path.exists():
         return False, None, None
 
     communication.echo("Updating dockerfile...")
 
-    with open(project_context.dockerfile_path, "r") as f:
+    with open(project_context.dockerfile_path) as f:
         dockerfile_content = f.read()
 
     docker_version = read_renku_version_from_dockerfile()
     if not docker_version:
         if check_only:
             return False, None, None
         raise DockerfileUpdateError(
@@ -269,12 +268,12 @@
     for entry in importlib_resources.files("renku.core.migration").iterdir():
         match = re.search(r"^m_([0-9]{4})__[a-zA-Z0-9_-]*.py$", entry.name)
 
         if match is None:  # migration files match m_0000__[name].py format
             continue
 
         version = int(match.groups()[0])
-        path = "renku.core.migration.{}".format(Path(entry.name).stem)
+        path = f"renku.core.migration.{Path(entry.name).stem}"
         migrations.append((version, path))
 
     migrations = sorted(migrations, key=lambda v: v[1].lower())
     return migrations
```

### Comparing `renku-2.3.2/renku/core/migration/models/__init__.py` & `renku-2.4.0rc1/renku/ui/api/graph/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku migration models."""
+"""Renku Graph API."""
```

### Comparing `renku-2.3.2/renku/core/migration/models/migration.py` & `renku-2.4.0rc1/renku/core/migration/models/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/models/refs.py` & `renku-2.4.0rc1/renku/core/migration/models/refs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -53,15 +52,15 @@
         params = ("--allow-onelevel", name) if no_slashes else (name,)
         return subprocess.run(("git", "check-ref-format") + params).returncode == 0
 
     @name.validator
     def name_validator(self, attribute, value):
         """Validate reference name."""
         if not self.check_ref_format(value):
-            raise errors.ParameterError('The reference name "{0}" is not valid.'.format(value))
+            raise errors.ParameterError(f'The reference name "{value}" is not valid.')
 
     @property
     def path(self):
         """Return full reference path."""
         return self.metadata_path / REFS / self.name
 
     @property
```

### Comparing `renku-2.3.2/renku/core/migration/models/v10.py` & `renku-2.4.0rc1/renku/core/migration/models/v10.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/models/v3.py` & `renku-2.4.0rc1/renku/core/migration/models/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/models/v7.py` & `renku-2.4.0rc1/renku/core/migration/models/v7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/models/v8.py` & `renku-2.4.0rc1/renku/core/migration/models/v8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/migration/models/v9.py` & `renku-2.4.0rc1/renku/core/migration/models/v9.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -394,15 +393,15 @@
             repository = project_context.repository
             self.commit = repository.get_commit(self._label.rsplit("@", maxsplit=1)[-1])
 
         yield self
 
 
 @attr.s(eq=False, order=False)
-class MappedIOStream(object):
+class MappedIOStream:
     """Represents an IO stream (``stdin``, ``stdout``, ``stderr``)."""
 
     _id = attr.ib(default=None, kw_only=True)
     _label = attr.ib(default=None, kw_only=True)
 
     STREAMS = ["stdin", "stdout", "stderr"]
 
@@ -411,19 +410,19 @@
     def default_id(self):
         """Generate an id for a mapped stream."""
         host = "localhost"
         if project_context.has_context():
             host = project_context.remote.host or host
         host = os.environ.get("RENKU_DOMAIN") or host
 
-        return urljoin("https://{host}".format(host=host), posixpath.join("/iostreams", self.stream_type))
+        return urljoin(f"https://{host}", posixpath.join("/iostreams", self.stream_type))
 
     def default_label(self):
         """Set default label."""
-        return 'Stream mapping for stream "{}"'.format(self.stream_type)
+        return f'Stream mapping for stream "{self.stream_type}"'
 
     def __attrs_post_init__(self):
         """Post-init hook."""
         if not self._id:
             self._id = self.default_id()
         if not self._label:
             self._label = self.default_label()
@@ -484,19 +483,19 @@
     @staticmethod
     def generate_id(run_id, position=None):
         """Generate an id for an argument."""
         if position:
             id_ = str(position)
         else:
             id_ = uuid.uuid4().hex
-        return "{}/arguments/{}".format(run_id, id_)
+        return f"{run_id}/arguments/{id_}"
 
     def default_label(self):
         """Set default label."""
-        return 'Command Argument "{}"'.format(self.default_value)
+        return f'Command Argument "{self.default_value}"'
 
     def default_name(self):
         """Create a default name."""
         return _generate_name(base="param", prefix=self.prefix, position=self.position)
 
     def __attrs_post_init__(self):
         """Post-init hook."""
@@ -517,19 +516,19 @@
     @staticmethod
     def generate_id(run_id, position=None):
         """Generate an id for an argument."""
         if position:
             id_ = str(position)
         else:
             id_ = uuid.uuid4().hex
-        return "{}/inputs/{}".format(run_id, id_)
+        return f"{run_id}/inputs/{id_}"
 
     def default_label(self):
         """Set default label."""
-        return 'Command Input "{}"'.format(self.default_value)
+        return f'Command Input "{self.default_value}"'
 
     def default_name(self):
         """Create a default name."""
         return _generate_name(base="input", prefix=self.prefix, position=self.position)
 
     def __attrs_post_init__(self):
         """Post-init hook."""
@@ -552,19 +551,19 @@
     @staticmethod
     def generate_id(run_id, position=None):
         """Generate an id for an argument."""
         if position:
             id_ = str(position)
         else:
             id_ = uuid.uuid4().hex
-        return "{}/outputs/{}".format(run_id, id_)
+        return f"{run_id}/outputs/{id_}"
 
     def default_label(self):
         """Set default label."""
-        return 'Command Output "{}"'.format(self.default_value)
+        return f'Command Output "{self.default_value}"'
 
     def default_name(self):
         """Create a default name."""
         return _generate_name(base="output", prefix=self.prefix, position=self.position)
 
     def __attrs_post_init__(self):
         """Post-init hook."""
@@ -622,15 +621,15 @@
         host = "localhost"
         host = project_context.remote.host or host
         host = os.environ.get("RENKU_DOMAIN") or host
 
         if not identifier:
             identifier = str(uuid.uuid4())
 
-        return urljoin("https://{host}".format(host=host), posixpath.join("/runs", quote(identifier, safe="")))
+        return urljoin(f"https://{host}", posixpath.join("/runs", quote(identifier, safe="")))
 
     def __lt__(self, other):
         """Compares two subprocesses order based on their dependencies."""
         a_inputs = set()
         b_outputs = set()
 
         for i in other.inputs:
@@ -855,15 +854,15 @@
         """Configure calculated properties."""
         if self.commit:
             return self.commit.committed_datetime
 
     @agents.default
     def default_agents(self):
         """Set person agent to be the author of the commit."""
-        renku_agent = SoftwareAgent(label="renku {0}".format(__version__), id=version_url)
+        renku_agent = SoftwareAgent(label=f"renku {__version__}", id=version_url)
         if self.commit:
             return [Person.from_commit(self.commit), renku_agent]
         return [renku_agent]
 
     @influenced.default
     def default_influenced(self):
         """Calculate default values."""
@@ -928,15 +927,15 @@
     def generate_id(cls, commit_hexsha):
         """Calculate action ID."""
         host = "localhost"
         host = project_context.remote.host or host
         host = os.environ.get("RENKU_DOMAIN") or host
 
         return urljoin(
-            "https://{host}".format(host=host),
+            f"https://{host}",
             posixpath.join("/activities", f"commit/{commit_hexsha}"),
         )
 
     @classmethod
     def from_run(cls, run, path, commit=None, subprocess_index=None, update_commits=False):
         """Convert a ``Run`` to a ``ProcessRun``."""
         repository = project_context.repository
@@ -1159,15 +1158,15 @@
         if len(names) == 1:
             return self.name
 
         last_name = names[-1]
         initials = [name[0] for name in names]
         initials.pop()
 
-        return "{0}.{1}".format(".".join(initials), last_name)
+        return "{}.{}".format(".".join(initials), last_name)
 
     @property
     def full_identity(self):
         """Return name, email, and affiliation."""
         return self.get_full_identity(self.email, self.affiliation, self.name)
 
     @staticmethod
@@ -1263,15 +1262,15 @@
     value = str(value)
     if is_doi(value):
         return extract_doi(value)
     return value
 
 
 @attr.s(slots=True)
-class DatasetTag(object):
+class DatasetTag:
     """Represents a Tag of an instance of a dataset."""
 
     name = attr.ib(default=None, kw_only=True, validator=instance_of(str))
 
     description = attr.ib(default=None, kw_only=True, validator=instance_of(str))
 
     commit = attr.ib(default=None, kw_only=True, validator=instance_of(str))
@@ -1405,15 +1404,15 @@
 
         if not self.name:
             self.name = self.filename
 
         parsed_id = urlparse(self._id)
 
         if not parsed_id.scheme:
-            self._id = "file://{}".format(self._id)
+            self._id = f"file://{self._id}"
 
         if not self.url:
             self.url = self.default_url()
 
     def update_commit(self, commit):
         """Set commit and update associated fields."""
         self.commit = commit
@@ -2228,16 +2227,16 @@
     _message = fields.String(rdfs.comment, init_name="message", load_default=None)
     _was_informed_by = fields.List(prov.wasInformedBy, fields.IRI(), init_name="was_informed_by")
     generated = Nested(prov.activity, GenerationSchema, reverse=True, many=True, load_default=None)
     invalidated = Nested(
         prov.wasInvalidatedBy, [OldEntitySchema, OldCollectionSchema], reverse=True, many=True, load_default=None
     )
     influenced = Nested(prov.influenced, OldCollectionSchema, many=True)
-    started_at_time = fields.DateTime(prov.startedAtTime, add_value_types=True)
-    ended_at_time = fields.DateTime(prov.endedAtTime, add_value_types=True)
+    started_at_time = fields.DateTime(prov.startedAtTime, format="iso", add_value_types=True)
+    ended_at_time = fields.DateTime(prov.endedAtTime, format="iso", add_value_types=True)
     agents = Nested(prov.wasAssociatedWith, [OldPersonSchema, OldSoftwareAgentSchema], many=True)
 
     @pre_dump(pass_many=True)
     def removes_ms(self, objs, many, **kwargs):
         """Remove milliseconds from datetimes.
 
         Note: since DateField uses `strftime` as format, which only supports timezone info without a colon
```

### Comparing `renku-2.3.2/renku/core/migration/utils/__init__.py` & `renku-2.4.0rc1/renku/core/migration/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -43,27 +42,27 @@
         id_ = str(uuid.uuid4())
 
     host = "localhost"
     if project_context.has_context():
         host = project_context.remote.host or host
     host = os.environ.get("RENKU_DOMAIN") or host
 
-    return urljoin("https://{host}".format(host=host), posixpath.join("/urls", quote(id_, safe="")))
+    return urljoin(f"https://{host}", posixpath.join("/urls", quote(id_, safe="")))
 
 
 def generate_dataset_tag_id(name, commit):
     """Generate @id field for DatasetTag."""
     host = "localhost"
     if project_context.has_context():
         host = project_context.remote.host or host
     host = os.environ.get("RENKU_DOMAIN") or host
 
-    name = "{0}@{1}".format(name, commit)
+    name = f"{name}@{commit}"
 
-    return urljoin("https://{host}".format(host=host), posixpath.join("/dataset-tags", quote(name, safe="")))
+    return urljoin(f"https://{host}", posixpath.join("/dataset-tags", quote(name, safe="")))
 
 
 def generate_dataset_id(identifier):
     """Generate @id field."""
     # Determine the hostname for the resource URIs.
     # If RENKU_DOMAIN is set, it overrides the host from remote.
     # Default is localhost.
```

### Comparing `renku-2.3.2/renku/core/migration/utils/conversion.py` & `renku-2.4.0rc1/renku/core/migration/utils/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -18,14 +17,15 @@
 """Utility functions for converting metadata."""
 
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 from renku.core.migration.models import v9 as old_datasets
+from renku.core.util.datetime8601 import fix_datetime
 from renku.core.util.git import get_entity_from_revision
 from renku.core.util.urls import get_slug
 from renku.domain_model.dataset import (
     Dataset,
     DatasetFile,
     DatasetTag,
     ImageObject,
@@ -189,18 +189,18 @@
     identifier = _convert_dataset_identifier(dataset.identifier)
     id = Dataset.generate_id(identifier=identifier)
 
     return (
         Dataset(
             creators=[_convert_agent(creator) for creator in dataset.creators],
             dataset_files=convert_dataset_files(dataset.files),
-            date_created=dataset.date_created,
-            date_published=dataset.date_published,
+            date_created=fix_datetime(dataset.date_created),
+            date_published=fix_datetime(dataset.date_published),
             date_removed=None,
-            date_modified=dataset.date_created or dataset.date_published,
+            date_modified=fix_datetime(dataset.date_created or dataset.date_published),
             derived_from=convert_derived_from(dataset.derived_from, dataset.same_as),
             description=dataset.description,
             id=id,
             identifier=identifier,
             images=[_convert_image_object(image, dataset_id=id) for image in (dataset.images or [])],
             in_language=_convert_language(dataset.in_language),
             keywords=dataset.keywords,
```

### Comparing `renku-2.3.2/renku/core/plugin/__init__.py` & `renku-2.4.0rc1/renku/core/migration/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku plugins module."""
-import pluggy
-
-hookimpl = pluggy.HookimplMarker("renku")
+"""Renku migration models."""
```

### Comparing `renku-2.3.2/renku/core/plugin/dataset_provider.py` & `renku-2.4.0rc1/renku/core/plugin/dataset_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/plugin/implementations/__init__.py` & `renku-2.4.0rc1/renku/core/plugin/implementations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -17,16 +16,17 @@
 # limitations under the License.
 """Renku plugin implementations."""
 
 from typing import TYPE_CHECKING, List, Type
 
 from renku.core.dataset.providers.azure import AzureProvider
 from renku.core.dataset.providers.dataverse import DataverseProvider
+from renku.core.dataset.providers.external import ExternalProvider
 from renku.core.dataset.providers.git import GitProvider
-from renku.core.dataset.providers.local import FilesystemProvider
+from renku.core.dataset.providers.local import LocalProvider
 from renku.core.dataset.providers.olos import OLOSProvider
 from renku.core.dataset.providers.renku import RenkuProvider
 from renku.core.dataset.providers.s3 import S3Provider
 from renku.core.dataset.providers.web import WebProvider
 from renku.core.dataset.providers.zenodo import ZenodoProvider
 from renku.core.session.docker import DockerSessionProvider
 from renku.core.session.renkulab import RenkulabSessionProvider
@@ -47,16 +47,17 @@
 
 session_providers: "List[Type[ISessionProvider]]" = [DockerSessionProvider, RenkulabSessionProvider]
 workflow_exporters: "List[Type[IWorkflowConverter]]" = [CWLExporter, RenkuWorkflowFileExporter]
 workflow_providers: "List[Type[IWorkflowProvider]]" = [CWLToolProvider, LocalWorkflowProvider]
 dataset_providers: "List[Type[ProviderApi]]" = [
     AzureProvider,
     DataverseProvider,
+    ExternalProvider,
+    LocalProvider,
     GitProvider,
-    FilesystemProvider,
     OLOSProvider,
     RenkuProvider,
     S3Provider,
     WebProvider,
     ZenodoProvider,
 ]
 workflow_file_parsers: "List[Type[IWorkflowFileParser]]" = [RenkuWorkflowFileParser]
```

### Comparing `renku-2.3.2/renku/core/plugin/pluginmanager.py` & `renku-2.4.0rc1/renku/core/plugin/pluginmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/plugin/provider.py` & `renku-2.4.0rc1/renku/core/plugin/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/plugin/run.py` & `renku-2.4.0rc1/renku/core/plugin/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/plugin/session.py` & `renku-2.4.0rc1/renku/core/plugin/session.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/plugin/workflow.py` & `renku-2.4.0rc1/renku/core/plugin/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -14,28 +13,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Plugin hooks for renku workflow customization."""
 
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Optional, Protocol, Tuple
 
 import pluggy
 
 from renku.core import errors
 from renku.domain_model.workflow.converters import IWorkflowConverter
 from renku.domain_model.workflow.plan import Plan
 
-try:
-    from typing_extensions import Protocol  # NOTE: Required for Python 3.7 compatibility
-except ImportError:
-    from typing import Protocol  # type: ignore
-
-
 hookspec = pluggy.HookspecMarker("renku")
 
 
 @hookspec
 def workflow_format() -> Tuple[IWorkflowConverter, List[str]]:  # type: ignore[empty-body]
     """Plugin Hook for ``workflow export`` call.
```

### Comparing `renku-2.3.2/renku/core/plugin/workflow_file_parser.py` & `renku-2.4.0rc1/renku/core/plugin/workflow_file_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/project.py` & `renku-2.4.0rc1/renku/core/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -21,15 +19,15 @@
 
 from pydantic import validate_arguments
 
 from renku.command.command_builder import inject
 from renku.command.view_model.project import ProjectViewModel
 from renku.core.interface.project_gateway import IProjectGateway
 from renku.core.util.metadata import construct_creator
-from renku.core.util.util import NO_VALUE, NoValueType
+from renku.domain_model.constant import NO_VALUE, NoValueType
 from renku.domain_model.project_context import project_context
 from renku.domain_model.provenance.agent import Person
 
 
 @inject.autoparams()
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def edit_project(
```

### Comparing `renku-2.3.2/renku/core/session/__init__.py` & `renku-2.4.0rc1/renku/infrastructure/gateway/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku interactive session module."""
+"""Renku database gateway implementations."""
```

### Comparing `renku-2.3.2/renku/core/session/docker.py` & `renku-2.4.0rc1/renku/core/session/docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,14 +12,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Docker based interactive session provider."""
 
+import os
+import platform
 import webbrowser
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, cast
 from uuid import uuid4
 
 import docker
 from requests.exceptions import ReadTimeout
@@ -116,15 +117,20 @@
         Returns:
             A reference to ``self``.
         """
         return self
 
     def get_start_parameters(self) -> List["ProviderParameter"]:
         """Returns parameters that can be set for session start."""
-        return []
+        from renku.core.dataset.providers.models import ProviderParameter
+
+        return [
+            ProviderParameter("port", help="Local port to use (random if not specified).", type=int),
+            ProviderParameter("force-build", help="Always build image and don't check if it exists.", is_flag=True),
+        ]
 
     def get_open_parameters(self) -> List["ProviderParameter"]:
         """Returns parameters that can be set for session open."""
         return []
 
     def session_list(self, project_name: str, config: Optional[Dict[str, Any]]) -> List[Session]:
         """Lists all the sessions currently running by the given session provider.
@@ -156,14 +162,15 @@
         **kwargs,
     ) -> Tuple[str, str]:
         """Creates an interactive session.
 
         Returns:
             Tuple[str, str]: Provider message and a possible warning message.
         """
+        show_non_standard_user_warning = True
 
         def session_start_helper(consider_disk_request: bool):
             try:
                 docker_is_running = self.docker_client().ping()
                 if not docker_is_running:
                     raise errors.DockerError(
                         "Could not communicate with the docker instance. Please make sure it is running!"
@@ -209,28 +216,49 @@
                 environment = {
                     "GIT_AUTHOR_NAME": user.name,
                     "GIT_AUTHOR_EMAIL": user.email,
                     "GIT_COMMITTER_EMAIL": user.email,
                     "EMAIL": user.email,
                 }
 
+                additional_options: Dict[str, Any] = {}
+
+                if platform.system() == "Linux" and os.getuid() != 1000:
+                    # NOTE: Current user id is not 1000 like jovyan, need to run docker under that user.
+                    nonlocal show_non_standard_user_warning
+                    if show_non_standard_user_warning:
+                        communication.confirm(
+                            "Your user id is not 1000 and for Jupyter to work the session must be started as root.\n"
+                            "Jupyter itself will run as your user.\n"
+                            "Starting as root has security implications, make sure you trust this Dockerfile.\n"
+                            "Proceed?",
+                            abort=True,
+                        )
+                        show_non_standard_user_warning = False
+
+                    additional_options["user"] = "root"
+                    environment["NB_UID"] = str(os.getuid())
+                    environment["CHOWN_HOME"] = "yes"
+                    environment["CHOWN_HOME_OPTS"] = "-R"
+
                 container = self.docker_client().containers.run(
                     image_name,
                     'jupyter notebook --NotebookApp.ip="0.0.0.0"'
                     f" --NotebookApp.port={DockerSessionProvider.JUPYTER_PORT}"
                     f' --NotebookApp.token="{auth_token}" --NotebookApp.default_url="{default_url}"'
-                    f" --NotebookApp.notebook_dir={work_dir}",
+                    f" --NotebookApp.notebook_dir={work_dir}" + (" --allow-root" if os.getuid() != 1000 else ""),
                     detach=True,
                     labels={"renku_project": project_name, "jupyter_token": auth_token},
-                    ports={f"{DockerSessionProvider.JUPYTER_PORT}/tcp": None},
+                    ports={f"{DockerSessionProvider.JUPYTER_PORT}/tcp": kwargs.get("port")},
                     remove=True,
                     environment=environment,
                     volumes=volumes,
                     working_dir=str(work_dir),
                     **resource_requests,
+                    **additional_options,
                 )
 
                 if not container.ports:
                     container.reload()
 
                 jupyter_urls = DockerSessionProvider._get_jupyter_urls(
                     container.ports, auth_token, jupyter_port=DockerSessionProvider.JUPYTER_PORT
@@ -291,7 +319,11 @@
     def session_url(self, session_name: str) -> Optional[str]:
         """Get the URL of the interactive session."""
         for c in self.docker_client().containers.list():
             if c.short_id == session_name and f"{DockerSessionProvider.JUPYTER_PORT}/tcp" in c.ports:
                 host = c.ports[f"{DockerSessionProvider.JUPYTER_PORT}/tcp"][0]
                 return f'http://{host["HostIp"]}:{host["HostPort"]}/?token={c.labels["jupyter_token"]}'
         return None
+
+    def force_build_image(self, force_build: bool = False, **kwargs) -> bool:
+        """Whether we should force build the image directly or check for an existing image first."""
+        return force_build
```

### Comparing `renku-2.3.2/renku/core/session/renkulab.py` & `renku-2.4.0rc1/renku/core/session/renkulab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -42,16 +41,17 @@
 
 class RenkulabSessionProvider(ISessionProvider):
     """A session provider that uses the notebook service API to launch sessions."""
 
     DEFAULT_TIMEOUT_SECONDS = 300
 
     def __init__(self):
-        self.__renku_url = None
-        self.__notebooks_url = None
+        self.__renku_url: Optional[str] = None
+        self.__notebooks_url: Optional[str] = None
+        self._force_build: bool = False
 
     def _renku_url(self) -> str:
         """Get the URL of the renku instance."""
         if not self.__renku_url:
             renku_url = get_renku_url()
             if not renku_url:
                 raise errors.RenkulabSessionGetUrlError()
@@ -161,21 +161,23 @@
             system_config = SystemSSHConfig()
 
             if not system_config.is_configured:
                 if communication.confirm(
                     "Your system is not set up for SSH connections to Renkulab. Would you like to set it up?"
                 ):
                     ssh_setup()
+                    self._force_build = True
                 else:
                     raise errors.RenkulabSessionError(
                         "Can't run ssh session without setting up Renku SSH support. Run without '--ssh' or "
                         "run 'renku session ssh-setup'."
                     )
 
-            system_config.setup_session_keys()
+            if system_config.setup_session_keys():
+                self._force_build = True
 
     def _cleanup_ssh_connection_configs(
         self, project_name: str, running_sessions: Optional[List[Session]] = None
     ) -> None:
         """Cleanup leftover SSH connections that aren't valid anymore.
 
         Args:
@@ -360,14 +362,15 @@
             server_options["gpu_request"] = int(gpu_request)
         if disk_request:
             server_options["disk_request"] = disk_request
         payload = {
             "image": image_name,
             "commit_sha": session_commit,
             "serverOptions": server_options,
+            "branch": repository.active_branch or "master",
             **self._get_renku_project_name_parts(),
         }
         res = self._send_renku_request(
             "post",
             f"{self._notebooks_url()}/servers",
             headers=self._auth_header(),
             json=payload,
@@ -472,7 +475,11 @@
             "projects",
             project_name_parts["namespace"],
             project_name_parts["project"],
             "sessions/show",
             session_name,
         ]
         return urllib.parse.urljoin(self._renku_url(), "/".join(session_url_parts))
+
+    def force_build_image(self, **kwargs) -> bool:
+        """Whether we should force build the image directly or check for an existing image first."""
+        return self._force_build
```

### Comparing `renku-2.3.2/renku/core/session/session.py` & `renku-2.4.0rc1/renku/core/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -38,17 +37,20 @@
 def _safe_get_provider(provider: str) -> ISessionProvider:
     try:
         return next(p for p in get_supported_session_providers() if p.name == provider)
     except StopIteration:
         raise errors.ParameterError(f"Session provider '{provider}' is not available!")
 
 
-SessionList = NamedTuple(
-    "SessionList", [("sessions", List[Session]), ("all_local", bool), ("warning_messages", List[str])]
-)
+class SessionList(NamedTuple):
+    """Session list return."""
+
+    sessions: List[Session]
+    all_local: bool
+    warning_messages: List[str]
 
 
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def session_list(config_path: Optional[str], provider: Optional[str] = None) -> SessionList:
     """List interactive sessions.
 
     Args:
@@ -124,25 +126,27 @@
     if image_name is None:
         tag = project_context.repository.head.commit.hexsha[:7]
         repo_host = get_image_repository_host()
         image_name = f"{project_name}:{tag}"
         if repo_host:
             image_name = f"{repo_host}/{image_name}"
 
-        if not provider_api.find_image(image_name, config):
-            communication.confirm(
-                f"The container image '{image_name}' does not exist. Would you like to build it using {provider}?",
-                abort=True,
-            )
-            with communication.busy(msg=f"Building image {image_name}"):
-                provider_api.build_image(project_context.dockerfile_path.parent, image_name, config)
-            communication.echo(f"Image {image_name} built successfully.")
-    else:
-        if not provider_api.find_image(image_name, config):
-            raise errors.ParameterError(f"Cannot find the provided container image '{image_name}'!")
+    force_build_image = provider_api.force_build_image(**kwargs)
+
+    if not force_build_image and not provider_api.find_image(image_name, config):
+        communication.confirm(
+            f"The container image '{image_name}' does not exist. Would you like to build it using {provider}?",
+            abort=True,
+        )
+        force_build_image = True
+
+    if force_build_image:
+        with communication.busy(msg=f"Building image {image_name}"):
+            provider_api.build_image(project_context.dockerfile_path.parent, image_name, config)
+        communication.echo(f"Image {image_name} built successfully.")
 
     # set resource settings
     cpu_limit = cpu_request or get_value("interactive", "cpu_request")
 
     if cpu_limit is not None:
         try:
             cpu_limit = float(cpu_limit)
```

### Comparing `renku-2.3.2/renku/core/session/utils.py` & `renku-2.4.0rc1/renku/core/session/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/storage.py` & `renku-2.4.0rc1/renku/core/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -32,17 +30,16 @@
 
 import pathspec
 
 from renku.core import errors
 from renku.core.config import get_value
 from renku.core.constant import RENKU_LFS_IGNORE_PATH, RENKU_PROTECTED_PATHS
 from renku.core.util import communication
-from renku.core.util.file_size import parse_file_size
 from renku.core.util.git import get_in_submodules, run_command
-from renku.core.util.os import expand_directories
+from renku.core.util.os import expand_directories, parse_file_size
 from renku.domain_model.project_context import project_context
 
 if TYPE_CHECKING:
     from renku.domain_model.entity import Entity  # type: ignore
     from renku.infrastructure.repository import Repository
 
 
@@ -97,15 +94,15 @@
             pass
         else:
             return fn(*args, **kwargs)
 
     return wrapper
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def storage_installed():
     """Verify that git-lfs is installed and on system PATH."""
     return bool(which("git-lfs"))
 
 
 def storage_installed_locally():
     """Verify that git-lfs is installed for the project."""
@@ -155,15 +152,15 @@
     """Initialize the external storage for data."""
     try:
         result = run(
             _CMD_STORAGE_INSTALL + (["--force"] if force else []),
             stdout=PIPE,
             stderr=STDOUT,
             cwd=project_context.path,
-            universal_newlines=True,
+            text=True,
         )
 
         if result.returncode != 0:
             raise errors.GitLFSError(f"Error executing 'git lfs install: \n {result.stdout}")
     except (KeyboardInterrupt, OSError) as e:
         raise errors.ParameterError(f"Couldn't run 'git lfs':\n{e}")
 
@@ -347,29 +344,27 @@
             project_dict[project_context.path].append(str(relative_path))
             repositories[project_context.path] = current_repository
 
     for project_path, paths in project_dict.items():
         current_repository = repositories[project_path]
 
         for path in paths:
-            with open(path, "r") as tracked_file:
+            with open(path) as tracked_file:
                 try:
                     header = tracked_file.read(len(_LFS_HEADER))
                     if header == _LFS_HEADER:
                         # file is not pulled
                         continue
                 except UnicodeDecodeError:
                     # likely a binary file, not lfs pointer file
                     pass
             with tempfile.NamedTemporaryFile(mode="w+t", encoding="utf-8", delete=False) as tmp, open(
                 path, "r+t"
             ) as input_file:
-                result = run(
-                    _CMD_STORAGE_CLEAN, cwd=project_path, stdin=input_file, stdout=tmp, universal_newlines=True
-                )
+                result = run(_CMD_STORAGE_CLEAN, cwd=project_path, stdin=input_file, stdout=tmp, text=True)
 
                 if result.returncode != 0:
                     raise errors.GitLFSError(f"Error executing 'git lfs clean: \n {result.stdout}")
 
                 tmp_path = tmp.name
             move(tmp_path, path)
 
@@ -497,23 +492,23 @@
 
     try:
         lfs_output = run(
             command + ignore_pointers,
             stdout=PIPE,
             stderr=STDOUT,
             cwd=project_context.path,
-            universal_newlines=True,
+            text=True,
         )
     except (KeyboardInterrupt, OSError) as e:
         raise errors.GitError(f"Couldn't run 'git lfs migrate info':\n{e}")
 
     if lfs_output.returncode != 0:
         # NOTE: try running without --pointers (old versions of git lfs)
         try:
-            lfs_output = run(command, stdout=PIPE, stderr=STDOUT, cwd=project_context.path, universal_newlines=True)
+            lfs_output = run(command, stdout=PIPE, stderr=STDOUT, cwd=project_context.path, text=True)
         except (KeyboardInterrupt, OSError) as e:
             raise errors.GitError(f"Couldn't run 'git lfs migrate info':\n{e}")
 
         if lfs_output.returncode != 0:
             raise errors.GitLFSError(f"Error executing 'git lfs migrate info: \n {lfs_output.stdout}")
 
     groups = []
@@ -543,22 +538,22 @@
     tempdir = Path(tempfile.mkdtemp())
     map_path = tempdir / "objectmap.csv"
     object_map = [f"--object-map={map_path}"]
 
     command = _CMD_STORAGE_MIGRATE_IMPORT + includes + excludes + object_map
 
     try:
-        lfs_output = run(command, stdout=PIPE, stderr=STDOUT, cwd=project_context.path, universal_newlines=True)
+        lfs_output = run(command, stdout=PIPE, stderr=STDOUT, cwd=project_context.path, text=True)
     except (KeyboardInterrupt, OSError) as e:
         raise errors.GitError(f"Couldn't run 'git lfs migrate import':\n{e}")
 
     if lfs_output.returncode != 0:
         raise errors.GitLFSError(f"Error executing 'git lfs migrate import: \n {lfs_output.stdout}")
 
-    with open(map_path, "r", newline="") as csvfile:
+    with open(map_path, newline="") as csvfile:
         reader = csv.reader(csvfile, delimiter=",")
 
         commit_sha_mapping = [(r[0], r[1]) for r in reader]
 
     os.remove(map_path)
 
     sha_mapping = dict()
```

### Comparing `renku-2.3.2/renku/core/template/__init__.py` & `renku-2.4.0rc1/renku/ui/service/jobs/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku template management."""
+"""Job constants."""
```

### Comparing `renku-2.3.2/renku/core/template/template.py` & `renku-2.4.0rc1/renku/core/template/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -101,15 +99,15 @@
     with open(project_context.template_checksums_path, "w") as checksum_file:
         json.dump(checksums, checksum_file)
 
 
 def read_template_checksum() -> Dict[str, str]:
     """Read templates checksum file for a project."""
     if has_template_checksum():
-        with open(project_context.template_checksums_path, "r") as checksum_file:
+        with open(project_context.template_checksums_path) as checksum_file:
             return json.load(checksum_file)
 
     return {}
 
 
 def has_template_checksum() -> bool:
     """Return if project has a templates checksum file."""
@@ -380,22 +378,22 @@
 
     @classmethod
     def fetch(cls, source: Optional[str], reference: Optional[str]) -> "EmbeddedTemplates":
         """Fetch embedded Renku templates."""
         from renku import __template_version__
 
         template_path = importlib_resources.files("renku") / "templates"
-        with importlib_resources.as_file(template_path) as folder:
-            path = Path(folder)
+        with importlib_resources.as_file(template_path) as templates:
+            path = Path(templates)
 
         return cls(path=path, source="renku", reference=__template_version__, version=__template_version__)
 
     def get_all_references(self, id) -> List[str]:
         """Return all available references for a template id."""
-        template_exists = any(t.id == id for t in self.templates)
+        template_exists = any(id == t.id or id in t.aliases for t in self.templates)
         return [self.reference] if template_exists and self.reference is not None else []
 
     def get_latest_reference_and_version(
         self, id: str, reference: Optional[str], version: Optional[str]
     ) -> Optional[Tuple[Optional[str], str]]:
         """Return latest reference and version number of a template."""
         if version is None:
@@ -409,15 +407,15 @@
             return self.reference, self.version
         else:
             return (self.reference, self.version) if current_version < Version(self.version) else (reference, version)
 
     def get_template(self, id, reference: Optional[str]) -> "Template":
         """Return all available versions for a template id."""
         try:
-            return next(t for t in self.templates if t.id == id)
+            return next(t for t in self.templates if id == t.id or id in t.aliases)
         except StopIteration:
             raise errors.TemplateNotFoundError(f"The template with id '{id}' is not available.")
 
 
 class RepositoryTemplates(TemplatesSource):
     """Represent a local/remote template repository.
 
@@ -492,15 +490,15 @@
         """Return if template id is available at a reference."""
         try:
             content = self.repository.get_content(TEMPLATE_MANIFEST, revision=reference)
             manifest = TemplatesManifest.from_string(content)
         except (errors.FileNotFound, errors.InvalidTemplateError):
             return False
         else:
-            return any(t.id == id for t in manifest.templates)
+            return any(id == t.id or id in t.aliases for t in manifest.templates)
 
     def get_template(self, id, reference: Optional[str]) -> "Template":
         """Return a template at a specific reference."""
         if reference is not None and reference != self.reference:
             try:
                 self.repository.checkout(reference=reference)
             except errors.GitError as e:
@@ -512,12 +510,13 @@
             try:
                 manifest = TemplatesManifest.from_path(self.path / TEMPLATE_MANIFEST)
             except errors.InvalidTemplateError as e:
                 raise errors.InvalidTemplateError(f"Cannot load template's manifest file at '{reference}'.") from e
             else:
                 self.manifest = manifest
 
-        template = next((t for t in self.templates if t.id == id), None)
+        template = next((t for t in self.templates if id == t.id or id in t.aliases), None)
         if template is None:
+            reference = reference or "HEAD"
             raise errors.TemplateNotFoundError(f"The template with id '{id}' is not available at '{reference}'.")
 
         return template
```

### Comparing `renku-2.3.2/renku/core/template/usecase.py` & `renku-2.4.0rc1/renku/core/template/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -225,15 +223,17 @@
         id=template_metadata.id,
         interactive=interactive,
         dry_run=dry_run,
         template_action=TemplateAction.UPDATE,
         input_parameters=None,
     )
 
-    return TemplateChangeViewModel.from_template(template=rendered_template, actions=actions)
+    return TemplateChangeViewModel.from_template(
+        template=rendered_template, actions=actions, old_id=template_metadata.id
+    )
 
 
 @inject.autoparams("project_gateway")
 def _set_or_update_project_from_template(
     templates_source: TemplatesSource,
     reference: str,
     id: str,
@@ -282,20 +282,22 @@
 def select_template(templates_source: TemplatesSource, id: Optional[str] = None) -> Optional[Template]:
     """Select a template from a template source."""
 
     def prompt_to_select_template():
         if not communication.has_prompt():
             raise errors.InvalidTemplateError("Cannot select a template")
 
-        Selection = NamedTuple("Selection", [("index", int), ("id", str)])
+        class Selection(NamedTuple):
+            number: int
+            id: str
 
-        templates = [Selection(index=i, id=t.id) for i, t in enumerate(templates_source.templates, start=1)]
-        tables = tabulate(templates, headers=["index", "id"])
+        templates = [Selection(number=i, id=t.id) for i, t in enumerate(templates_source.templates, start=1)]
+        tables = tabulate(templates, headers=["number", "id"])
 
-        message = f"{tables}\nPlease choose a template by typing its index"
+        message = f"{tables}\nPlease choose a template by typing its number"
 
         template_index = communication.prompt(
             msg=message, type=click.IntRange(1, len(templates_source.templates)), show_default=False, show_choices=False
         )
         return templates_source.templates[template_index - 1]
 
     if id:
```

### Comparing `renku-2.3.2/renku/core/util/__init__.py` & `renku-2.4.0rc1/renku/domain_model/provenance/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku utility methods."""
+"""Define classes used for capturing data provenance.
+
+.. seealso:: https://www.w3.org/TR/prov-o/
+"""
```

### Comparing `renku-2.3.2/renku/core/util/communication.py` & `renku-2.4.0rc1/renku/core/util/communication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/contexts.py` & `renku-2.4.0rc1/renku/core/util/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/dataset.py` & `renku-2.4.0rc1/renku/ui/service/serializers/rpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,22 +10,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Helper utilities for datasets."""
+"""Renku service JSON-RPC serializers."""
+from marshmallow import Schema, fields
 
-import urllib
-from typing import Tuple
 
+class JsonRPCResponse(Schema):
+    """JsonRPC response schema."""
 
-def check_url(url: str) -> Tuple[bool, bool]:
-    """Check if a url is local/remote and if it contains a git repository."""
-    # NOTE: Supported scheme before refactoring were: "", "file", "http", "https", "git+https", "git+ssh"
-    u = urllib.parse.urlparse(url)
-
-    is_remote = u.scheme not in ("", "file") or url.lower().startswith("git@")
-    is_git = is_remote and (u.path.endswith(".git") or u.scheme in ("git+https", "git+ssh") or url.startswith("git@"))
-
-    return is_remote, is_git
+    error = fields.Dict()
```

### Comparing `renku-2.3.2/renku/core/util/datetime8601.py` & `renku-2.4.0rc1/renku/core/util/datetime8601.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/doi.py` & `renku-2.4.0rc1/renku/core/util/doi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/git.py` & `renku-2.4.0rc1/renku/core/util/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -385,15 +383,16 @@
         revision(str, optional): The revision to check at (Default value = None).
         bypass_cache(bool): Whether to ignore cached entries and get information from disk (Default value = False).
         checksum(str, optional): Pre-calculated checksum for performance reasons, will be calculated if not set.
     Returns:
         Entity: The Entity for the given path and revision.
 
     """
-    from renku.domain_model.entity import NON_EXISTING_ENTITY_CHECKSUM, Collection, Entity
+    from renku.domain_model.constant import NON_EXISTING_ENTITY_CHECKSUM
+    from renku.domain_model.entity import Collection, Entity
 
     def get_directory_members(absolute_path: Path) -> List[Entity]:
         """Return first-level files/directories in a directory."""
         members: List[Entity] = []
 
         for member in absolute_path.iterdir():
             if member.name == ".gitkeep":
@@ -487,26 +486,30 @@
         path_to_save = set(paths) - staged_files
         repository.add(*path_to_save)
         saved_paths = [c.b_path for c in repository.staged_changes]
 
         if saved_paths:
             if not message:
                 # Show saved files in message
-                max_len = 100
+                max_line_len = 100
+                max_total_len = 100000
                 message = "Saved changes to: "
                 paths_with_lens = cast(
                     List[Tuple[str, int]],
                     reduce(
                         lambda c, x: c + [(x, c[-1][1] + len(x))],
                         saved_paths,
                         cast(List[Tuple[Optional[str], int]], [(None, len(message))]),
                     )[1:],
                 )
                 # limit first line to max_len characters
-                message += " ".join(p if l < max_len else "\n\t" + p for p, l in paths_with_lens)
+                message += " ".join(p if l < max_line_len else "\n\t" + p for p, l in paths_with_lens)
+
+                if len(message) > max_total_len:
+                    message = message[: max_total_len - 3] + "..."
 
             repository.commit(message)
     except errors.GitCommandError as e:
         raise errors.GitError("Cannot commit changes") from e
     else:
         return saved_paths
 
@@ -883,15 +886,15 @@
     """Return file size for a file inside a git repository."""
     # NOTE: First try to get file size from Git LFS
     try:
         lfs_run = run(
             ("git", "lfs", "ls-files", "--name-only", "--size"),
             stdout=PIPE,
             cwd=repository_path,
-            universal_newlines=True,
+            text=True,
         )
     except SubprocessError:
         pass
     else:
         lfs_output = lfs_run.stdout.split("\n")
         # Example line format: relative/path/to/file (7.9 MB)
         pattern = re.compile(r".*\((.*)\)")
```

### Comparing `renku-2.3.2/renku/core/util/jwt.py` & `renku-2.4.0rc1/renku/core/util/jwt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/metadata.py` & `renku-2.4.0rc1/renku/core/util/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2021 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -24,15 +22,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 from packaging.version import Version
 
 from renku.core import errors
 from renku.core.config import get_value, set_value
-from renku.core.constant import RENKU_HOME, RENKU_PROTECTED_PATHS, RENKU_TMP
+from renku.core.constant import POINTERS, RENKU_HOME, RENKU_PROTECTED_PATHS, RENKU_TMP
 from renku.core.migration.utils import OLD_METADATA_PATH
 from renku.core.util import communication
 from renku.core.util.os import is_subpath
 
 if TYPE_CHECKING:
     from renku.core.dataset.providers.api import ProviderCredentials
     from renku.domain_model.provenance.agent import Person
@@ -84,24 +82,32 @@
         no_email_warning = None
 
     return person, no_email_warning
 
 
 def is_external_file(path: Union[Path, str], project_path: Path):
     """Checks if a path is an external file."""
-    from renku.core.constant import POINTERS, RENKU_HOME
-
     path = project_path / path
     if not path.is_symlink() or not is_subpath(path=path, base=project_path):
         return False
 
     pointer = os.readlink(path)
     return str(os.path.join(RENKU_HOME, POINTERS)) in pointer
 
 
+def is_linked_file(path: Union[Path, str], project_path: Path) -> bool:
+    """Return True if a dataset file is a linked file."""
+    path = project_path / path
+    if not path.is_symlink() or not is_subpath(path=path.resolve(), base=project_path):
+        return False
+
+    pointer = os.readlink(path)
+    return os.path.join(RENKU_HOME, POINTERS) in pointer
+
+
 def read_renku_version_from_dockerfile(path: Optional[Union[Path, str]] = None) -> Optional[Version]:
     """Read RENKU_VERSION from the content of path if a valid version is available."""
     from renku.domain_model.project_context import project_context
 
     path = Path(path) if path else project_context.dockerfile_path
     if not path.exists():
         return None
```

### Comparing `renku-2.3.2/renku/core/util/os.py` & `renku-2.4.0rc1/renku/core/util/os.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -35,19 +33,38 @@
 
 def get_relative_path_to_cwd(path: Union[Path, str]) -> str:
     """Get a relative path to current working directory."""
     absolute_path = os.path.abspath(path)
     return os.path.relpath(absolute_path, os.getcwd())
 
 
+def get_expanded_user_path(path: Union[Path, str]) -> str:
+    """Expand the path if it starts with ``~``."""
+    return "" if not path else os.path.expanduser(path)
+
+
 def get_absolute_path(
-    path: Union[Path, str], base: Optional[Union[Path, str]] = None, resolve_symlinks: bool = False
+    path: Union[Path, str], base: Optional[Union[Path, str]] = None, resolve_symlinks: bool = False, expand: bool = True
 ) -> str:
-    """Return absolute normalized path."""
+    """Return absolute normalized path.
+
+    Args:
+        path(Union[Path, str]): Path to get its absolute.
+        base(Union[Path, str]): Base path to get absolute path from it.
+        resolve_symlinks(bool): Whether to keep or resolve symlinks.
+        expand(bool): Whether to expand ``~`` or not (Default value = True)
+
+    Returns:
+        str: Absolute path.
+    """
+    if expand:
+        path = get_expanded_user_path(path)
     if base is not None:
+        if expand:
+            base = get_expanded_user_path(base)
         base = Path(base).resolve() if resolve_symlinks else os.path.abspath(base)
         path = os.path.join(base, path)
 
     if resolve_symlinks:
         return os.path.realpath(path)
     else:
         # NOTE: Do not use os.path.realpath or Path.resolve() because they resolve symlinks
@@ -64,15 +81,15 @@
         absolute_path = base / path
         return absolute_path.resolve().relative_to(base)
     except ValueError:
         raise ValueError(f"Path '{path}' is not with base directory '{base}'")
 
 
 def get_relative_path(path: Union[Path, str], base: Union[Path, str], strict: bool = False) -> Optional[str]:
-    """Return a relative path to the base if path is within base with/without resolving symlinks."""
+    """Return a relative path to the base if path is within base without resolving symlinks."""
     try:
         absolute_path = get_absolute_path(path=path, base=base)
         return str(Path(absolute_path).relative_to(base))
     except ValueError:
         if strict:
             raise errors.ParameterError(f"File {path} is not within path {base}")
 
@@ -133,28 +150,28 @@
 
     :ref path: target path
     """
     subpaths = Path(path).glob("*")
     return not any(subpaths)
 
 
-def create_symlink(path: Union[Path, str], symlink_path: Union[Path, str], overwrite: bool = True) -> None:
-    """Create a symlink that points from symlink_path to path."""
+def create_symlink(target: Union[Path, str], symlink_path: Union[Path, str], overwrite: bool = True) -> None:
+    """Create a symlink that points from symlink_path to target."""
     # NOTE: Don't resolve symlink path
     absolute_symlink_path = get_absolute_path(symlink_path)
-    absolute_path = get_absolute_path(path, resolve_symlinks=True)
+    absolute_path = get_absolute_path(target, resolve_symlinks=True)
 
     Path(absolute_symlink_path).parent.mkdir(parents=True, exist_ok=True)
 
     try:
         if overwrite:
             delete_path(absolute_symlink_path)
         os.symlink(absolute_path, absolute_symlink_path)
     except OSError:
-        raise errors.InvalidFileOperation(f"Cannot create symlink from '{symlink_path}' to '{path}'")
+        raise errors.InvalidFileOperation(f"Cannot create symlink from '{symlink_path}' to '{target}'")
 
 
 def delete_path(path: Union[Path, str]) -> None:
     """Delete a file/directory/symlink."""
     try:
         os.remove(path)
     except FileNotFoundError:
@@ -164,15 +181,15 @@
 
 
 def unmount_path(path: Union[Path, str]) -> None:
     """Unmount the given path and ignore all errors."""
 
     def execute_command(*command: str) -> bool:
         try:
-            subprocess.run(command, check=True, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            subprocess.run(command, check=True, text=True, capture_output=True)
         except (subprocess.CalledProcessError, FileNotFoundError):
             return False
         else:
             return True
 
     path = str(path)
 
@@ -191,14 +208,23 @@
 
 
 def is_ascii(data):
     """Check if provided string contains only ascii characters."""
     return len(data) == len(data.encode())
 
 
+def get_file_size(path: Union[Path, str], follow_symlinks: bool = True) -> Optional[int]:
+    """Return size of a file in bytes."""
+    path = Path(path).resolve() if follow_symlinks else Path(path)
+    try:
+        return path.stat().st_size
+    except OSError:
+        return None
+
+
 def normalize_to_ascii(input_string, sep="-"):
     """Convert a string to only contain ASCII characters, with non-ASCII substring replaced with ``sep``."""
     replace_all = [sep, "_", "."]
     for replacement in replace_all:
         input_string = input_string.replace(replacement, " ")
 
     return (
@@ -309,7 +335,53 @@
             if path_.is_dir():
                 for expanded in path_.rglob("*"):
                     processed_paths.add(str(expanded))
                     yield str(expanded)
             else:
                 processed_paths.add(matched_path)
                 yield matched_path
+
+
+UNITS = {
+    "b": 1,
+    "kb": 1000,
+    "mb": 1000**2,
+    "gb": 1000**3,
+    "tb": 1000**4,
+    "m": 1000**2,
+    "g": 1000**3,
+    "t": 1000**4,
+    "p": 1000**5,
+    "e": 1000**6,
+    "z": 1000**7,
+    "y": 1000**8,
+    "ki": 1024,
+    "mi": 1024**2,
+    "gi": 1024**3,
+    "ti": 1024**4,
+    "pi": 1024**5,
+    "ei": 1024**6,
+    "zi": 1024**7,
+    "yi": 1024**8,
+}
+
+
+def parse_file_size(size_str):
+    """Parse a human readable file size to bytes."""
+    res = re.search(r"([0-9.]+)([a-zA-Z]{1,2})", size_str)
+    if not res or res.group(2).lower() not in UNITS:
+        raise ValueError(
+            "Supplied file size does not contain a unit. " "Valid units are: {}".format(", ".join(UNITS.keys()))
+        )
+
+    value = float(res.group(1))
+    unit = UNITS[res.group(2).lower()]
+
+    return int(value * unit)
+
+
+def bytes_to_unit(size_in_bytes, unit: str) -> Optional[float]:
+    """Return size in the provided unit."""
+    unit = unit.lower()
+    if unit not in UNITS:
+        raise ValueError(f"Invalid unit '{unit}'. Valid units are: [{', '.join(UNITS)}]")
+    return None if size_in_bytes is None else size_in_bytes / UNITS[unit]
```

### Comparing `renku-2.3.2/renku/core/util/requests.py` & `renku-2.4.0rc1/renku/core/util/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/shacl.py` & `renku-2.4.0rc1/renku/core/util/shacl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -30,15 +28,15 @@
 def validate_graph(graph, shacl_path=None, format="nquads"):
     """Validate the current graph with a SHACL schema.
 
     Uses default schema if not supplied.
     """
     shacl: Union[str, bytes]
     if shacl_path:
-        with open(shacl_path, "r", encoding="utf-8") as f:
+        with open(shacl_path, encoding="utf-8") as f:
             shacl = f.read()
     else:
         shacl = importlib_resources.files("renku.data").joinpath("shacl_shape.json").read_bytes()
 
     return validate(
         graph,
         shacl_graph=shacl,
```

### Comparing `renku-2.3.2/renku/core/util/ssh.py` & `renku-2.4.0rc1/renku/core/util/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -26,19 +24,24 @@
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
 
 from renku.core import errors
 from renku.core.session.utils import get_renku_url
 from renku.core.util import communication
 from renku.domain_model.project_context import project_context
 
-SSHKeyPair = NamedTuple("SSHKeyPair", [("private_key", str), ("public_key", str)])
+
+class SSHKeyPair(NamedTuple):
+    """A public/private key pair for SSH."""
+
+    private_key: str
+    public_key: str
 
 
 def generate_ssh_keys() -> SSHKeyPair:
-    """Generate an SSH keypair.
+    """Generate an SSH key pair.
 
     Returns:
         Private Public key pair.
     """
     key = Ed25519PrivateKey.generate()
 
     private_key = key.private_bytes(
@@ -126,34 +129,35 @@
             project_name(str): The name of the project, without the owner name.
             session_name(str): The name of the session to setup a connection to.
         Returns:
             The path to the SSH connection file.
         """
         return self.renku_ssh_root / f"00-{project_name}-{session_name}.conf"
 
-    def setup_session_keys(self):
+    def setup_session_keys(self) -> bool:
         """Add a users key to a project."""
         project_context.ssh_authorized_keys_path.parent.mkdir(parents=True, exist_ok=True)
         project_context.ssh_authorized_keys_path.touch(mode=0o600, exist_ok=True)
 
         if not self.public_key_string:
             raise errors.SSHNotSetupError()
 
         if self.public_key_string in project_context.ssh_authorized_keys_path.read_text():
-            return
+            return False
 
         communication.info("Adding SSH public key to project.")
         with project_context.ssh_authorized_keys_path.open("at") as f:
             f.writelines(self.public_key_string)
 
         project_context.repository.add(project_context.ssh_authorized_keys_path)
         project_context.repository.commit("Add SSH public key.")
         communication.info(
             "Added public key. Changes need to be pushed and remote image built for changes to take effect."
         )
+        return True
 
     def setup_session_config(self, project_name: str, session_name: str) -> str:
         """Setup local SSH config for connecting to a session.
 
         Args:
             project_name(str): The name of the project, without the owner name.
             session_name(str): The name of the session to setup a connection to.
```

### Comparing `renku-2.3.2/renku/core/util/tabulate.py` & `renku-2.4.0rc1/renku/core/util/tabulate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/util/template_vars.py` & `renku-2.4.0rc1/renku/domain_model/provenance/parameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,40 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Template variable utility methods."""
-
-import datetime
-from string import Formatter
-from typing import Any, Iterable, Mapping, Tuple, Union
-
-from renku.core.errors import ParameterError
-from renku.domain_model.workflow.parameter import CommandParameterBase
-
+"""Classes for tracking parameter values in provenance."""
 
-class TemplateVariableFormatter(Formatter):
-    """Template variable formatter for `CommandParameterBase`."""
+from typing import Any
+from uuid import uuid4
 
-    RESERVED_KEYS = ["iter_index"]
+from renku.domain_model.workflow.plan import Plan
 
-    def __init__(self):
-        super(TemplateVariableFormatter, self).__init__()
 
-    def apply(self, param: str, parameters: Mapping[str, Any] = {}) -> str:
-        """Renders the parameter template into its final value."""
-        try:
-            return super().vformat(param, args=[datetime.datetime.now()], kwargs=parameters)
-        except KeyError as e:
-            raise ParameterError(f"Could not resolve the variable {str(e)}")
+class ParameterValue:
+    """Value for a parameter in provenance."""
 
-    def get_value(self, key, args, kwargs):
-        """Ignore some special keys when formatting the variable."""
-        if key in self.RESERVED_KEYS:
-            return key
-        return super().get_value(key, args, kwargs)
+    def __init__(self, *, id: str, parameter_id: str, value: Any):
+        self.id = id
+        self.parameter_id: str = parameter_id
+        self.value: Any = value
 
     @staticmethod
-    def to_map(parameters: Iterable[Union[CommandParameterBase, Tuple[str, str]]]) -> Mapping[str, str]:
-        """Converts a list of `CommandParameterBase` into parameter name-value dictionary."""
-        return dict(
-            map(
-                lambda x: (x.name, x.actual_value) if isinstance(x, CommandParameterBase) else (x[1], str(x[0])),
-                parameters,
-            )
-        )
+    def generate_id(activity_id: str) -> str:
+        """Generate a default id."""
+        return f"{activity_id}/parameter-value/{uuid4().hex}"
+
+    def apply_value_to_parameter(self, plan: Plan) -> None:
+        """Apply the current value as actual_value on the plan's parameter."""
+        parameter = plan.get_field_by_id(self.parameter_id)
+        parameter.actual_value = self.value
```

### Comparing `renku-2.3.2/renku/core/util/urls.py` & `renku-2.4.0rc1/renku/core/util/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,15 +15,16 @@
 # limitations under the License.
 """Helper utilities for handling URLs."""
 
 import os
 import re
 import unicodedata
 import urllib
-from typing import List, Optional
+from pathlib import Path
+from typing import List, Optional, Tuple
 from urllib.parse import ParseResult, urlparse
 
 from renku.core import errors
 from renku.core.config import get_value
 from renku.core.util.git import get_remote, parse_git_url
 from renku.core.util.os import is_subpath
 from renku.domain_model.project_context import project_context
@@ -138,7 +137,33 @@
     if parsed_uri.scheme != parsed_subfolder_uri.scheme:
         # INFO: catch s3://test vs http://test
         return False
     if parsed_uri.netloc != parsed_subfolder_uri.netloc:
         # INFO: catch s3://test1 vs s3://test2
         return False
     return is_subpath(parsed_subfolder_uri_path, parsed_uri_path)
+
+
+def resolve_uri(uri: str) -> str:
+    """Resolve path part of a URI if it's a local URI."""
+    scheme = get_scheme(uri)
+
+    if scheme not in ("file", ""):
+        return uri
+
+    path = get_path(uri)
+    path = str(Path(path).resolve())
+
+    return f"{scheme}://{path}" if scheme else path
+
+
+def check_url(url: str) -> Tuple[bool, bool]:
+    """Check if a url is local/remote and if it contains a git repository."""
+    # NOTE: Supported scheme before refactoring were: "", "file", "http", "https", "git+https", "git+ssh"
+    u = urllib.parse.urlparse(url)
+    scheme = u.scheme.lower()
+    starts_with_git = url.lower().startswith("git@")
+
+    is_remote = scheme not in ("", "file") or starts_with_git
+    is_git = is_remote and (u.path.lower().endswith(".git") or scheme in ("git+https", "git+ssh") or starts_with_git)
+
+    return is_remote, is_git
```

### Comparing `renku-2.3.2/renku/core/util/util.py` & `renku-2.4.0rc1/renku/domain_model/provenance/annotation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""General utility functions."""
-
-from typing import Any, NewType, Optional
-
-from packaging.version import Version
-
+"""Represent an annotation for a workflow."""
 
-def to_string(value: Optional[Any], strip: bool = False) -> str:
-    """Return a string representation of value and return an empty string for None."""
-    return "" if value is None else str(value).strip() if strip else str(value)
+import copy
+from uuid import uuid4
 
 
-def to_semantic_version(value: str) -> Optional[Version]:
-    """Convert value to SemVer."""
-    try:
-        return Version(value)
-    except ValueError:
-        return None
+class Annotation:
+    """Represents a custom annotation for a research object."""
 
+    def __init__(self, *, id: str, body=None, source=None):
+        self.id = id
+        self.body = body
+        self.source = source
 
-NoValueType = NewType("NoValueType", object)
-"""Type to represent a value not being set in cases where ``None`` is a valid value."""
+    def copy(self):
+        """Return a copy of this annotation."""
+        return copy.deepcopy(self)
 
-NO_VALUE = NoValueType(object())
-"""Sentinel to represent a value not being set in cases where ``None`` is a valid value."""
+    @staticmethod
+    def generate_id():
+        """Generate an id for an annotation."""
+        return f"/annotations/{uuid4().hex}"
```

### Comparing `renku-2.3.2/renku/core/util/uuid.py` & `renku-2.4.0rc1/renku/command/format/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2019-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Helper utilities for handling UUIDs."""
-import uuid
-
-
-def is_uuid(value):
-    """Check if value is UUID4.
-
-    Copied from https://stackoverflow.com/questions/19989481/
-    """
-    try:
-        uuid_obj = uuid.UUID(value, version=4)
-    except ValueError:
-        return False
-
-    return str(uuid_obj) == value
+"""Serializers for different output formats."""
```

### Comparing `renku-2.3.2/renku/core/util/yaml.py` & `renku-2.4.0rc1/renku/core/util/yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/core/workflow/__init__.py` & `renku-2.4.0rc1/renku/command/view_model/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku workflow management."""
+"""Renku commands view models module."""
```

### Comparing `renku-2.3.2/renku/core/workflow/activity.py` & `renku-2.4.0rc1/renku/core/workflow/activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -181,15 +180,15 @@
                     graph.add_edge(a, b)
                 overridden_activities[a].add(path)
             elif comparison > 0:
                 if not networkx.has_path(graph, b, a):
                     graph.add_edge(b, a)
                 overridden_activities[b].add(path)
             else:
-                raise ValueError(f"Cannot create an order between activities that generate '{path}': {a.id} and {b.id}")
+                raise ValueError(f"Cannot create an order between activities that generate '{path}': {a} and {b}")
 
     def remove_overridden_activities():
         to_be_removed = set()
         to_be_processed = set(overridden_activities.keys())
 
         while len(to_be_processed) > 0:
             activity = to_be_processed.pop()
```

### Comparing `renku-2.3.2/renku/core/workflow/converters/__init__.py` & `renku-2.4.0rc1/renku/command/schema/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku workflow converters."""
+"""JSON-LD schemes for core models."""
```

### Comparing `renku-2.3.2/renku/core/workflow/converters/cwl.py` & `renku-2.4.0rc1/renku/core/workflow/converters/cwl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -38,26 +37,26 @@
 
 
 class CommandLineTool(cwl.CommandLineTool):
     """CommandLineTool that supports empty outputs."""
 
     def get_dict(self):
         """Set outputs to empty if not set."""
-        d = super(CommandLineTool, self).get_dict()  # type: ignore[misc]
+        d = super().get_dict()  # type: ignore[misc]
         if "outputs" not in d:
             d["outputs"] = []
         return d
 
 
 class WorkflowStep(cwl.WorkflowStep):
     """WorkflowStep that supports empty outputs."""
 
     def get_dict(self):
         """Set out to empty if not set."""
-        d = super(WorkflowStep, self).get_dict()  # type: ignore[misc]
+        d = super().get_dict()  # type: ignore[misc]
         if "out" not in d:
             d["out"] = []
         return d
 
 
 def _get_argument_type(value):
     """Get the type of a command line argument."""
@@ -184,48 +183,46 @@
             cycles = [list(map(lambda x: x.name, cycle)) for cycle in cycles]
             raise errors.GraphCycleError(cycles)
 
         import networkx as nx
 
         for i, wf in enumerate(nx.topological_sort(graph.workflow_graph)):
             step_clitool = CWLExporter._convert_step(workflow=wf, basedir=basedir, resolve_paths=resolve_paths)
-            step = WorkflowStep(in_=[], out=[], run=step_clitool, id="step_{}".format(i))
+            step = WorkflowStep(in_=[], out=[], run=step_clitool, id=f"step_{i}")
 
             for input in wf.inputs:
                 input_path = input.actual_value
 
                 sanitized_id = CWLExporter._sanitize_id(input.id)
                 if input_path in inputs:
                     # already used as top-level input elsewhere, reuse
                     step.in_.append(cwl.WorkflowStepInput(sanitized_id, source=inputs[input_path]))
                 elif input_path in outputs:
                     # output of a previous step, refer to it
                     consumed_outputs.add(outputs[input_path][0])
                     step.in_.append(
-                        cwl.WorkflowStepInput(
-                            sanitized_id, source="{}/{}".format(outputs[input_path][1], outputs[input_path][0])
-                        )
+                        cwl.WorkflowStepInput(sanitized_id, source=f"{outputs[input_path][1]}/{outputs[input_path][0]}")
                     )
                 else:
                     # input isn't output and doesn't exist yet, add new
-                    inputs[input_path] = "input_{}".format(input_index)
+                    inputs[input_path] = f"input_{input_index}"
                     step.in_.append(cwl.WorkflowStepInput(sanitized_id, source=inputs[input_path]))
                     input_index += 1
 
             for parameter in wf.parameters:
-                argument_id = "argument_{}".format(argument_index)
+                argument_id = f"argument_{argument_index}"
                 arguments[argument_id] = parameter.actual_value
                 step.in_.append(cwl.WorkflowStepInput(CWLExporter._sanitize_id(parameter.id), source=argument_id))
                 argument_index += 1
 
             for output in wf.outputs:
                 sanitized_id = CWLExporter._sanitize_id(output.id)
 
                 if output.mapped_to:
-                    sanitized_id = "output_{}".format(output.mapped_to.stream_type)
+                    sanitized_id = f"output_{output.mapped_to.stream_type}"
                 outputs[output.actual_value] = (sanitized_id, step.id)
                 step.out.append(cwl.WorkflowStepOutput(sanitized_id))
 
             steps.append(step)
 
         workflow_object = cwl.Workflow([], [], steps, id=str(uuid4()), requirements=[], hints=[], cwlVersion="v1.0")
 
@@ -249,17 +246,15 @@
         for id_, value in arguments.items():
             value, type_ = _get_argument_type(value)
             workflow_object.inputs.append(cwl.WorkflowInputParameter(id=id_, type=type_, default=value))
 
         for index, (path, (id_, step_id)) in enumerate(outputs.items(), 1):
             type_ = "Directory" if os.path.isdir(path) else "File"
             workflow_object.outputs.append(
-                cwl.WorkflowOutputParameter(
-                    id="output_{}".format(index), outputSource="{}/{}".format(step_id, id_), type=type_
-                )
+                cwl.WorkflowOutputParameter(id=f"output_{index}", outputSource=f"{step_id}/{id_}", type=type_)
             )
 
         return workflow_object
 
     @staticmethod
     def _convert_step(workflow: Plan, basedir: Path, resolve_paths: bool) -> CommandLineTool:
         """Converts a single workflow step to a CWL CommandLineTool."""
@@ -314,23 +309,23 @@
             if arg:
                 tool_object.inputs.append(arg)
 
         for input_ in inputs:
             tool_input = CWLExporter._convert_input(input_, basedir, resolve_paths=resolve_paths)
 
             workdir_req.listing.append(
-                cwl.Dirent(entry="$(inputs.{})".format(tool_input.id), entryname=input_.actual_value, writable=False)
+                cwl.Dirent(entry=f"$(inputs.{tool_input.id})", entryname=input_.actual_value, writable=False)
             )
 
             environment_variables.append(
                 cwl.EnvironmentDef(f"{RENKU_ENV_PREFIX}{input_.name}", str(input_.actual_value))
             )
             tool_object.inputs.append(tool_input)
             if input_.mapped_to:
-                tool_object.stdin = "$(inputs.{}.path)".format(tool_input.id)
+                tool_object.stdin = f"$(inputs.{tool_input.id}.path)"
                 jsrequirement = True
 
         for parameter in workflow.parameters:
             environment_variables.append(
                 cwl.EnvironmentDef(f"{RENKU_ENV_PREFIX}{parameter.name}", str(parameter.actual_value))
             )
             tool_object.inputs.append(CWLExporter._convert_parameter(parameter))
@@ -428,15 +423,15 @@
 
     @staticmethod
     def _convert_output(output: CommandOutput):
         """Converts an output to a CWL output."""
         if output.mapped_to:
             return (
                 cwl.CommandOutputParameter(
-                    id="output_{}".format(output.mapped_to.stream_type),
+                    id=f"output_{output.mapped_to.stream_type}",
                     type=output.mapped_to.stream_type,
                     streamable=False,
                 ),
                 None,
             )
 
         type_ = (
@@ -456,23 +451,23 @@
                 separate = False
 
                 if prefix.endswith(" "):
                     prefix = prefix[:-1]
                     separate = True
 
             arg = cwl.CommandInputParameter(
-                id="{}_arg".format(sanitized_id),
+                id=f"{sanitized_id}_arg",
                 type="string",
                 inputBinding=cwl.CommandLineBinding(position=output.position, prefix=prefix, separate=separate),
                 default=output.actual_value,
             )
             outp = cwl.CommandOutputParameter(
                 id=sanitized_id,
                 type=type_,
-                outputBinding=cwl.CommandOutputBinding(glob="$(inputs.{})".format(arg.id)),
+                outputBinding=cwl.CommandOutputBinding(glob=f"$(inputs.{arg.id})"),
             )
             return outp, arg
 
         return (
             cwl.CommandOutputParameter(
                 id=sanitized_id, type=type_, outputBinding=cwl.CommandOutputBinding(glob=output.actual_value)
             ),
```

### Comparing `renku-2.3.2/renku/core/workflow/converters/renku.py` & `renku-2.4.0rc1/renku/core/workflow/converters/renku.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/execute.py` & `renku-2.4.0rc1/renku/core/workflow/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -239,15 +238,15 @@
             iter_params["indexed"].update(
                 [(f"{param_name}.{ik}", iv) for ik, iv in inner_iter_params["indexed"].items()]
             )
             for tag, param in inner_iter_params["tagged"].items():
                 if tag in iter_params["tagged"]:
                     iter_params["tagged"][tag].update([(f"{param_name}.{ik}", iv) for ik, iv in param.items()])
                 else:
-                    iter_params["tagged"][tag] = dict([(f"{param_name}.{ik}", iv) for ik, iv in param.items()])
+                    iter_params["tagged"][tag] = {f"{param_name}.{ik}": iv for ik, iv in param.items()}
             params[param_name] = inner_params
         else:
             params[param_name] = param_value
     return iter_params, params
 
 
 def _validate_iterate_parameters(
@@ -342,16 +341,15 @@
     for tag in iter_params["tagged"].values():
         columns.extend(tag.keys())
         tagged_values.append(zip(*tag.values()))
 
     def _flatten(values):
         for i in values:
             if isinstance(i, (list, tuple)):
-                for k in i:
-                    yield k
+                yield from i
             else:
                 yield i
 
     for i, values in enumerate(itertools.product(*iter_params["params"].values(), *tagged_values)):
         plan_params = copy.deepcopy(workflow_params)
         iteration_values = {}
         for k, v in iter_params["indexed"].items():
```

### Comparing `renku-2.3.2/renku/core/workflow/model/__init__.py` & `renku-2.4.0rc1/renku/command/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku workflow models."""
+"""Renku commands implementation module."""
```

### Comparing `renku-2.3.2/renku/core/workflow/model/concrete_execution_graph.py` & `renku-2.4.0rc1/renku/core/workflow/model/concrete_execution_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/model/workflow_file.py` & `renku-2.4.0rc1/renku/core/workflow/model/workflow_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/parser/__init__.py` & `renku-2.4.0rc1/renku/core/dataset/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku workflow file parsers."""
+"""Renku management dataset logic."""
```

### Comparing `renku-2.3.2/renku/core/workflow/parser/renku.py` & `renku-2.4.0rc1/renku/core/workflow/parser/renku.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/plan.py` & `renku-2.4.0rc1/renku/core/workflow/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -32,17 +31,17 @@
 from renku.core.interface.activity_gateway import IActivityGateway
 from renku.core.interface.plan_gateway import IPlanGateway
 from renku.core.interface.project_gateway import IProjectGateway
 from renku.core.plugin.workflow_file_parser import read_workflow_file
 from renku.core.util import communication
 from renku.core.util.git import get_git_user
 from renku.core.util.os import are_paths_related, get_relative_paths
-from renku.core.util.util import NO_VALUE, NoValueType
 from renku.core.workflow.model.concrete_execution_graph import ExecutionGraph
 from renku.core.workflow.value_resolution import CompositePlanValueResolver, ValueResolver
+from renku.domain_model.constant import NO_VALUE, NoValueType
 from renku.domain_model.project_context import project_context
 from renku.domain_model.provenance.activity import Activity
 from renku.domain_model.provenance.agent import Person
 from renku.domain_model.provenance.annotation import Annotation
 from renku.domain_model.workflow.composite_plan import CompositePlan
 from renku.domain_model.workflow.plan import AbstractPlan, Plan
 from renku.infrastructure.immutable import DynamicProxy
@@ -191,15 +190,14 @@
             plan_chain = list(get_derivative_chain(workflow))
             relevant_activities = [a for p in plan_chain for a in activity_map.get(p.id, [])]
             touches_files_cache: Dict[str, bool] = {}
             duration_cache: Dict[str, Optional[timedelta]] = {}
             touches_existing_files = _check_workflow_touches_existing_files(workflow, touches_files_cache, activity_map)
 
             if isinstance(workflow, Plan):
-
                 num_executions = 0
                 last_execution: Optional[datetime] = None
 
                 for activity in relevant_activities:
                     num_executions += 1
 
                     if last_execution is None or last_execution < activity.ended_at_time:
@@ -791,18 +789,18 @@
 
     Adds information about last execution, number of executions and whether the plan was used to create files
     currently existing in the project.
     """
 
     all_activities = activity_gateway.get_all_activities()
     activity_map = _reverse_activity_plan_map(list(all_activities))
-    latest_plan_chains: Set[Tuple[AbstractPlan]] = set(
+    latest_plan_chains: Set[Tuple[AbstractPlan]] = {
         cast(Tuple[AbstractPlan], tuple(get_derivative_chain(p)))
         for p in plan_gateway.get_newest_plans_by_names().values()
-    )
+    }
 
     result: Dict[str, Union[Plan, CompositePlan]] = {}
     touches_file_cache: Dict[str, bool] = {}
     duration_cache: Dict[str, Optional[timedelta]] = {}
 
     # check which plans where involved in using/creating existing files
     for plan_chain in latest_plan_chains:
```

### Comparing `renku-2.3.2/renku/core/workflow/plan_factory.py` & `renku-2.4.0rc1/renku/core/workflow/plan_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -172,15 +171,14 @@
         """Yield command input parameters."""
         position = 0
         prefix: Optional[str] = None
 
         output_streams = {getattr(self, stream_name) for stream_name in ("stdout", "stderr")}
 
         for index, argument in enumerate(arguments):
-
             if prefix:
                 if argument.startswith("-"):
                     position += 1
                     self.add_command_parameter(default_value=prefix, position=position)
                     prefix = None
 
             if argument.startswith("--"):
@@ -302,15 +300,15 @@
                 parameter_candidates[str(input_path)] = parameter
             parameter_candidates[str(input_path)] = parameter
 
         for candidate_path, name in candidates:
             candidate = self._resolve_existing_subpath(self.working_dir / candidate_path)
 
             if candidate is None:
-                raise errors.UsageError('Path "{0}" does not exist inside the current project.'.format(candidate_path))
+                raise errors.UsageError(f'Path "{candidate_path}" does not exist inside the current project.')
 
             glob = str(candidate.relative_to(self.working_dir))
 
             if glob in input_candidates:
                 input = input_candidates[glob]
 
                 self.add_command_output_from_input(input, name=name)
```

### Comparing `renku-2.3.2/renku/core/workflow/providers/__init__.py` & `renku-2.4.0rc1/renku/ui/cli/utils/color.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku workflow providers."""
+"""Terminal Color definitions."""
+
+YELLOW = "yellow"
+MAGENTA = "magenta"
+GREEN = "green"
+RED = "red"
+BLUE = "blue"
```

### Comparing `renku-2.3.2/renku/core/workflow/providers/cwltool.py` & `renku-2.4.0rc1/renku/core/workflow/providers/cwltool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/providers/local.py` & `renku-2.4.0rc1/renku/core/workflow/providers/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/providers/toil.py` & `renku-2.4.0rc1/renku/core/workflow/providers/toil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -46,15 +45,15 @@
 from renku.domain_model.workflow.provider import IWorkflowProvider
 
 
 class AbstractToilJob(Job):
     """Toil job implementation for a renku ``Plan``."""
 
     def __init__(self, workflow: Plan, *args, **kwargs):
-        super(AbstractToilJob, self).__init__(unitName=workflow.name, displayName=workflow.name, *args, **kwargs)
+        super().__init__(unitName=workflow.name, displayName=workflow.name, *args, **kwargs)
         self.workflow: Plan = workflow
         self._input_files: Dict[str, FileID] = {}
         self._parents_promise: List[Promise] = []
         self._environment = os.environ.copy()
 
     @abstractmethod
     def _execute(self, command_line: List[str], mapped_std: Dict[str, str]) -> int:
```

### Comparing `renku-2.3.2/renku/core/workflow/run.py` & `renku-2.4.0rc1/renku/core/workflow/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/types.py` & `renku-2.4.0rc1/renku/core/workflow/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/core/workflow/value_resolution.py` & `renku-2.4.0rc1/renku/core/workflow/value_resolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,25 +12,61 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Resolution of ``Workflow`` execution values precedence."""
 
+import datetime
 from abc import ABC, abstractmethod
 from itertools import chain
-from typing import Any, Dict, Optional, Set
+from string import Formatter
+from typing import Any, Dict, Iterable, Mapping, Optional, Set, Tuple, Union
 
 from renku.core import errors
-from renku.core.util.template_vars import TemplateVariableFormatter
 from renku.domain_model.workflow.composite_plan import CompositePlan
-from renku.domain_model.workflow.parameter import ParameterMapping
+from renku.domain_model.workflow.parameter import CommandParameterBase, ParameterMapping
 from renku.domain_model.workflow.plan import AbstractPlan, Plan
 
 
+class TemplateVariableFormatter(Formatter):
+    """Template variable formatter for `CommandParameterBase`."""
+
+    RESERVED_KEYS = ["iter_index"]
+
+    def __init__(self):
+        super().__init__()
+
+    def apply(self, param: str, parameters: Optional[Mapping[str, Any]] = None) -> str:
+        """Renders the parameter template into its final value."""
+        if parameters is None:
+            parameters = {}
+
+        try:
+            return super().vformat(param, args=[datetime.datetime.now()], kwargs=parameters)
+        except KeyError as e:
+            raise errors.ParameterError(f"Could not resolve the variable {str(e)}")
+
+    def get_value(self, key, args, kwargs):
+        """Ignore some special keys when formatting the variable."""
+        if key in self.RESERVED_KEYS:
+            return key
+        return super().get_value(key, args, kwargs)
+
+    @staticmethod
+    def to_map(parameters: Iterable[Union[CommandParameterBase, Tuple[str, str]]]) -> Mapping[str, str]:
+        """Converts a list of `CommandParameterBase` into parameter name-value dictionary."""
+        return dict(
+            map(
+                lambda x: (x.name, x.actual_value) if isinstance(x, CommandParameterBase) else (x[1], str(x[0])),
+                parameters,
+            )
+        )
+
+
 class ValueResolver(ABC):
     """Value resolution class for an ``AbstractPlan``."""
 
     def __init__(self, plan: AbstractPlan, values: Optional[Dict[str, Any]]):
         self._values = values
         self.missing_parameters: Set[str] = set()
         self._plan = plan
@@ -63,15 +98,15 @@
 class PlanValueResolver(ValueResolver):
     """Value resolution class for a ``Plan``.
 
     Applies values and default_values to a workflow.
     """
 
     def __init__(self, plan: Plan, values: Dict[str, Any]):
-        super(PlanValueResolver, self).__init__(plan, values)
+        super().__init__(plan, values)
 
     def apply(self) -> AbstractPlan:
         """Applies values and default_values to a ``Plan``.
 
         Returns:
             A Plan with values applied.
         """
@@ -108,15 +143,15 @@
     - Default value on a mapping to the parameter
     - Value passed to a mapping to the parameter
     - Value passed to the parameter
     - Value propagated to a parameter from the source of a ParameterLink
     """
 
     def __init__(self, plan: CompositePlan, values: Optional[Dict[str, Any]] = None):
-        super(CompositePlanValueResolver, self).__init__(plan, values)
+        super().__init__(plan, values)
 
     def apply(self) -> AbstractPlan:
         """Applies values and default_values to a ``CompositePlan``.
 
         Returns:
             A ``CompositePlan`` with values applied.
         """
```

### Comparing `renku-2.3.2/renku/core/workflow/workflow_file.py` & `renku-2.4.0rc1/renku/core/workflow/workflow_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/data/gitignore.default` & `renku-2.4.0rc1/renku/data/gitignore.default`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/data/pre-commit.sh` & `renku-2.4.0rc1/renku/data/pre-commit.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env bash
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -92,30 +90,30 @@
   if [ "$CHECK_DATADIR" = "true" ]; then
     ALL_FILES=( "${MODIFIED_FILES[@]}" "${ADDED_FILES[@]}")
     ARGS=()
     for file in "${ALL_FILES[@]}"; do
       ARGS+=("-I" "$file")
     done
     IFS=$'\n' read -r -d '' -a DATASET_FILES \
-      <<< "$(renku dataset update -n --no-external --no-remote -c --plain "${ARGS[@]}")"
+      <<< "$(renku dataset update -n --no-remote -c --plain "${ARGS[@]}")"
 
     if [ ${#DATASET_FILES[@]} -ne 0 ]; then
       echo "Files in datasets data directory that aren't up to date:"
       echo
       for entry in "${DATASET_FILES[@]}"; do
         read -r change path dataset <<< "$entry"
 
         if [ "$change" = "f" ]; then
           echo "$path ($dataset) modified"
         elif [ "$change" = "r" ]; then
           echo "$path ($dataset) removed"
         fi
       done
       echo
-      echo 'Run "renku dataset update -c --all --no-remote --no-external" to update the datasets.'
+      echo 'Run "renku dataset update -c --all --no-remote" to update the datasets.'
       echo
       echo 'To disable this check, run "renku config set check_datadir_files false".'
       exit 1
     fi
   fi
 fi
```

### Comparing `renku-2.3.2/renku/data/shacl_shape.json` & `renku-2.4.0rc1/renku/data/shacl_shape.json`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/domain_model/__init__.py` & `renku-2.4.0rc1/renku/core/plugin/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2017-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Model objects used in Python SDK."""
+"""Renku plugins module."""
+import pluggy
+
+hookimpl = pluggy.HookimplMarker("renku")
```

### Comparing `renku-2.3.2/renku/domain_model/dataset.py` & `renku-2.4.0rc1/renku/domain_model/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -22,22 +20,24 @@
 import posixpath
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional, Union, cast
 from urllib.parse import quote, urlparse
 from uuid import uuid4
 
+import deal
 import marshmallow
 
 from renku.core import errors
 from renku.core.util.datetime8601 import fix_datetime, local_now, parse_date
 from renku.core.util.git import get_entity_from_revision
-from renku.core.util.metadata import is_external_file
+from renku.core.util.metadata import is_linked_file
+from renku.core.util.os import get_absolute_path
 from renku.core.util.urls import get_path, get_slug
-from renku.core.util.util import NO_VALUE
+from renku.domain_model.constant import NO_VALUE, NON_EXISTING_ENTITY_CHECKSUM
 from renku.domain_model.project_context import project_context
 from renku.infrastructure.immutable import Immutable, Slots
 from renku.infrastructure.persistent import Persistent
 
 if TYPE_CHECKING:
     from renku.domain_model.entity import Entity
     from renku.domain_model.provenance.agent import Person
@@ -198,18 +198,18 @@
 
 
 class RemoteEntity(Slots):
     """Reference to an Entity in a remote repository."""
 
     __slots__ = ("checksum", "id", "path", "url")
 
-    def __init__(self, *, checksum: str, id: Optional[str] = None, path: Union[Path, str], url: str):
+    def __init__(self, *, checksum: Optional[str], id: Optional[str] = None, path: Union[Path, str], url: str):
         super().__init__()
-        self.checksum: str = checksum
-        self.id: str = id or RemoteEntity.generate_id(checksum=checksum, path=path, url=url)
+        self.checksum: str = checksum or NON_EXISTING_ENTITY_CHECKSUM
+        self.id: str = id or RemoteEntity.generate_id(checksum=self.checksum, path=path, url=url)
         self.path: str = str(path)
         self.url: str = url
 
     @staticmethod
     def generate_id(checksum: str, path: Union[Path, str], url: str) -> str:
         """Generate an id."""
         parsed_url = urlparse(url)
@@ -227,64 +227,71 @@
     def __hash__(self):
         return hash((self.checksum, self.path, self.url))
 
 
 class DatasetFile(Slots):
     """A file in a dataset."""
 
-    __slots__ = ("based_on", "date_added", "date_removed", "entity", "id", "is_external", "source")
+    __slots__ = ("based_on", "date_added", "date_removed", "entity", "id", "is_external", "source", "linked", "size")
 
+    @deal.ensure(lambda self, *_, result, **kwargs: self.date_removed is None or self.date_removed >= self.date_added)
     def __init__(
         self,
         *,
         entity: "Entity",
         based_on: Optional[RemoteEntity] = None,
         date_added: Optional[datetime] = None,
         date_removed: Optional[datetime] = None,
         id: Optional[str] = None,
         is_external: Optional[bool] = False,
+        linked: Optional[bool] = False,
         source: Optional[Union[Path, str]] = None,
+        size: Optional[int] = None,
     ):
         from renku.domain_model.entity import Entity
 
         assert entity is None or isinstance(entity, Entity), f"Invalid entity type: '{entity}'"
 
         super().__init__()
 
         self.based_on: Optional[RemoteEntity] = based_on
         self.date_added: datetime = fix_datetime(date_added) or local_now()
         self.date_removed: Optional[datetime] = fix_datetime(date_removed)
         self.entity: "Entity" = entity
         self.id: str = id or DatasetFile.generate_id()
         self.is_external: bool = is_external or False
+        self.linked: bool = linked or False
         self.source: Optional[str] = str(source)
+        self.size: Optional[int] = size
 
     @classmethod
     def from_path(
         cls,
         path: Union[str, Path],
         source=None,
         based_on: Optional[RemoteEntity] = None,
         checksum: Optional[str] = None,
+        size: Optional[int] = None,
     ) -> "DatasetFile":
         """Return an instance from a path."""
-        from renku.domain_model.entity import NON_EXISTING_ENTITY_CHECKSUM, Entity
+        from renku.domain_model.entity import Entity
 
         # NOTE: Data is added from an external storage and isn't pulled yet
         if based_on and not (project_context.path / path).exists():
             checksum = based_on.checksum if based_on.checksum else NON_EXISTING_ENTITY_CHECKSUM
             id = Entity.generate_id(checksum=checksum, path=path)
             entity = Entity(id=id, checksum=checksum, path=path)
         else:
             entity = get_entity_from_revision(
                 repository=project_context.repository, path=path, bypass_cache=True, checksum=checksum
             )
 
-        is_external = is_external_file(path=path, project_path=project_context.path)
-        return cls(entity=entity, is_external=is_external, source=source, based_on=based_on)
+        is_external = False
+        linked = is_linked_file(path=path, project_path=project_context.path)
+        return cls(entity=entity, is_external=is_external, source=source, based_on=based_on, linked=linked, size=size)
 
     @staticmethod
     def generate_id():
         """Generate an identifier for DatasetFile.
 
         NOTE: ID should not rely on Entity properties because the same Entity can be added and removed multiple times.
         So, it should be marked by different DatasetFiles.
@@ -295,14 +302,25 @@
     def from_dataset_file(cls, other: "DatasetFile") -> "DatasetFile":
         """Return a copy with a different id."""
         self = other.copy()
         self.id = DatasetFile.generate_id()
 
         return self
 
+    def __repr__(self) -> str:
+        return f"<DatasetFile {self.entity.path}>"
+
+    def correct_linked_attribute(self):
+        """Replace ``is_external`` attribute with ``linked`` for linked dataset files."""
+        if self.is_external and is_linked_file(self.entity.path, project_path=project_context.path):
+            self.linked = True
+            self.is_external = False
+        elif not hasattr(self, "linked"):
+            self.linked = False
+
     def copy(self) -> "DatasetFile":
         """Return a clone of this object."""
         return copy.copy(self)
 
     def is_equal_to(self, other: "DatasetFile"):
         """Compare content.
 
@@ -310,34 +328,63 @@
         """
         return (
             self.based_on == other.based_on
             and self.date_added == other.date_added
             and self.date_removed == other.date_removed
             and self.entity == other.entity
             and self.is_external == other.is_external
+            and self.linked == other.linked
             and self.source == other.source
         )
 
+    @deal.ensure(lambda self, *_, result, **kwargs: self.date_removed >= self.date_added)
     def remove(self, date: Optional[datetime] = None):
         """Create a new instance and mark it as removed."""
         date_removed = fix_datetime(date) or local_now()
         self.date_removed = date_removed
 
     def is_removed(self) -> bool:
         """Return true if dataset is removed and should not be accessed."""
         return self.date_removed is not None
 
+    def has_valid_checksum(self) -> bool:
+        """Return if file has a valid checksum."""
+        return (
+            bool(self.entity.checksum)
+            and self.entity.checksum != NON_EXISTING_ENTITY_CHECKSUM
+            and (
+                self.based_on is None
+                or self.based_on.checksum != NON_EXISTING_ENTITY_CHECKSUM
+                or bool(self.based_on.checksum)
+            )
+        )
+
+    def has_valid_size(self) -> bool:
+        """Return if file has a valid size."""
+        return self.size is not None
+
 
 class Dataset(Persistent):
     """Represent a dataset."""
 
     date_modified: Optional[datetime] = None  # type: ignore
     storage: Optional[str] = None
     datadir: Optional[str] = None
 
+    @deal.ensure(
+        lambda self, *_, result, **kwargs: (self.date_created is not None and self.date_published is None)
+        or (self.date_created is None and self.date_published is not None)
+    )
+    @deal.ensure(
+        lambda self, *_, result, **kwargs: (self.date_created is not None and self.date_modified >= self.date_created)
+        or (self.date_published is not None and self.date_modified >= self.date_published)
+    )
+    @deal.ensure(
+        lambda self, *_, result, **kwargs: self.date_removed is None or self.date_removed >= self.date_modified
+    )
     def __init__(
         self,
         *,
         annotations: Optional[List["Annotation"]] = None,
         creators: Optional[List["Person"]] = None,
         datadir: Optional[Path] = None,
         dataset_files: Optional[List[DatasetFile]] = None,
@@ -401,14 +448,25 @@
         self.title: Optional[str] = title
         self.version: Optional[str] = version
         self.annotations: List["Annotation"] = annotations or []
 
         if datadir:
             self.datadir: Optional[str] = str(datadir)
 
+        self.correct_linked_files()
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+        self.correct_linked_files()
+
+    def correct_linked_files(self):
+        """Fix linked dataset files."""
+        for file in self.dataset_files:
+            file.correct_linked_attribute()
+
     @staticmethod
     def generate_id(identifier: str) -> str:
         """Generate an identifier for Dataset."""
         return f"/datasets/{identifier}"
 
     @staticmethod
     def _validate_name(name):
@@ -441,15 +499,15 @@
 
     @property
     def keywords_csv(self):
         """Comma-separated list of keywords associated with dataset."""
         return ", ".join(self.keywords)
 
     def get_datadir(self) -> Path:
-        """Return dataset's data directory."""
+        """Return dataset's data directory relative to project's root."""
         if self.datadir:
             return Path(self.datadir)
 
         return Path(os.path.join(project_context.datadir, self.name))
 
     def __repr__(self) -> str:
         return f"<Dataset {self.identifier} {self.name}>"
@@ -483,14 +541,23 @@
             f"Replacing identifier of dataset '{self.name}:{self.identifier}' "
             f"that is derived from {self.derived_from.url_id}"
         )
 
         self._assign_new_identifier(identifier)
         # NOTE: Do not unset `same_as` because it can be set for imported datasets
 
+    @deal.ensure(
+        lambda self, *_, result, **kwargs: (self.date_created is not None and self.date_published is None)
+        or (self.date_created is None and self.date_published is not None)
+    )
+    @deal.ensure(
+        lambda self, *_, result, **kwargs: (self.date_created is not None and self.date_modified >= self.date_created)
+        or (self.date_published is not None and self.date_modified >= self.date_published)
+    )
+    @deal.ensure(lambda self, *_, result, **kwargs: self.derived_from is not None)
     def derive_from(
         self,
         dataset: "Dataset",
         creator: Optional["Person"],
         identifier: Optional[str] = None,
         date_created: Optional[datetime] = None,
     ):
@@ -515,14 +582,15 @@
         identifier = identifier or uuid4().hex
         self.initial_identifier = identifier
         self.identifier = identifier
         self.id = Dataset.generate_id(identifier)
         # NOTE: We also need to re-assign the _p_oid since identifier has changed
         self.reassign_oid()
 
+    @deal.ensure(lambda self, *_, result, **kwargs: self.date_removed >= self.date_modified)
     def remove(self, date: Optional[datetime] = None):
         """Mark the dataset as removed."""
         self.date_removed = fix_datetime(date) or local_now()
 
     def is_removed(self) -> bool:
         """Return true if dataset is removed."""
         return self.date_removed is not None
@@ -604,24 +672,30 @@
                 raise errors.InvalidFileOperation(f"File cannot be found: {path}")
             return None
 
         file.remove()
 
         return file
 
+    def is_within_datadir(self, path: Union[Path, str]) -> bool:
+        """Return True if a given path is inside dataset's data directory."""
+        datadir = get_absolute_path(self.get_datadir())
+        absolute_path = get_absolute_path(path)
+        return os.path.commonpath([absolute_path, datadir]) == datadir
+
     def add_or_update_files(self, files: Union[DatasetFile, List[DatasetFile]]):
         """Add new files or update existing files."""
         assert not self.immutable, f"Dataset is immutable {self}"
 
         if isinstance(files, DatasetFile):
             files = [files]
 
         new_files = []
 
-        for file in files:
+        for file in cast(List[DatasetFile], files):
             existing_file = self.find_file(file.entity.path)
             if not existing_file:
                 new_files.append(file)
             elif file.entity.checksum != existing_file.entity.checksum or file.date_added != existing_file.date_added:
                 self.dataset_files.remove(existing_file)
                 new_files.append(file)
```

### Comparing `renku-2.3.2/renku/domain_model/dataset_provider.py` & `renku-2.4.0rc1/renku/domain_model/dataset_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/datastructures.py` & `renku-2.4.0rc1/renku/domain_model/datastructures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/entity.py` & `renku-2.4.0rc1/renku/domain_model/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -20,16 +18,14 @@
 import os.path
 from pathlib import Path
 from typing import List, Optional, Sequence, Union
 from urllib.parse import quote
 
 from renku.infrastructure.immutable import Immutable
 
-NON_EXISTING_ENTITY_CHECKSUM = "0" * 40
-
 
 class Entity(Immutable):
     """Represent a file."""
 
     __slots__ = ("checksum", "path")
 
     path: str
```

### Comparing `renku-2.3.2/renku/domain_model/enums.py` & `renku-2.4.0rc1/renku/domain_model/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2020- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/git.py` & `renku-2.4.0rc1/renku/domain_model/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -76,15 +74,15 @@
     """Remove the .git extension from the repo name."""
     if repo_name is not None and repo_name.endswith(".git"):
         return repo_name[: -len(".git")]
     return repo_name
 
 
 @attr.s()
-class GitURL(object):
+class GitURL:
     """Parser for common Git URLs."""
 
     # Initial value
     href = attr.ib()
     path = attr.ib(default=None)
     scheme = attr.ib(default="ssh")
     hostname = attr.ib(default="localhost")
```

### Comparing `renku-2.3.2/renku/domain_model/project.py` & `renku-2.4.0rc1/renku/domain_model/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -24,15 +22,15 @@
 
 import persistent
 
 from renku.core import errors
 from renku.core.util.datetime8601 import fix_datetime, local_now, parse_date
 from renku.core.util.git import get_git_user
 from renku.core.util.os import normalize_to_ascii
-from renku.core.util.util import NO_VALUE
+from renku.domain_model.constant import NO_VALUE
 from renku.domain_model.provenance.agent import Person
 from renku.domain_model.provenance.annotation import Annotation
 from renku.version import __minimum_project_version__
 
 if TYPE_CHECKING:
     from renku.domain_model.project_context import ProjectContext, ProjectRemote
     from renku.infrastructure.repository import Repository
```

### Comparing `renku-2.3.2/renku/domain_model/project_context.py` & `renku-2.4.0rc1/renku/domain_model/project_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -218,17 +216,17 @@
     def _top(self) -> "ProjectProperties":
         """Return current context."""
         if self._context_stack:
             return self._context_stack[-1]
 
         raise errors.ProjectContextError("No project context was pushed")
 
-    def has_context(self) -> bool:
-        """Return if at least one context is pushed."""
-        return bool(self._context_stack)
+    def has_context(self, path: Optional[Union[Path, str]] = None) -> bool:
+        """Return if at least one context which is equal to path (if not None) is pushed."""
+        return True if self._context_stack and (path is None or self.path == Path(path).resolve()) else False
 
     def clear(self) -> None:
         """Remove all contexts and reset the state without committing intermediate changes.
 
         NOTE: This method should be used only in tests.
         """
         while self._context_stack:
```

### Comparing `renku-2.3.2/renku/domain_model/provenance/__init__.py` & `renku-2.4.0rc1/renku/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define classes used for capturing data provenance.
-
-.. seealso:: https://www.w3.org/TR/prov-o/
-"""
+"""Renku core."""
```

### Comparing `renku-2.3.2/renku/domain_model/provenance/activity.py` & `renku-2.4.0rc1/renku/domain_model/provenance/activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -18,14 +16,15 @@
 """Represent an execution of a Plan."""
 
 from datetime import datetime
 from itertools import chain
 from typing import Dict, List, Optional, Union, cast
 from uuid import uuid4
 
+import deal
 from werkzeug.utils import cached_property
 
 from renku.command.command_builder import inject
 from renku.core.interface.project_gateway import IProjectGateway
 from renku.core.util.datetime8601 import local_now
 from renku.core.util.git import get_entity_from_revision, get_git_user
 from renku.domain_model.entity import Collection, Entity
@@ -94,14 +93,15 @@
 
 class Activity(Persistent):
     """Represent an activity in the repository."""
 
     invalidated_at: Optional[datetime] = None
     hidden_usages: List[HiddenUsage] = list()
 
+    @deal.ensure(lambda self, *_, result, **kwargs: self.ended_at_time >= self.started_at_time)
     def __init__(
         self,
         *,
         agents: List[Union[Person, SoftwareAgent]],
         annotations: Optional[List[Annotation]] = None,
         association: Association,
         ended_at_time: datetime,
@@ -132,14 +132,16 @@
         if not self.id.startswith("/activities/"):
             self.id = f"/activities/{self.id}"
 
         # TODO: _was_informed_by = attr.ib(kw_only=True)
         # TODO: influenced = attr.ib(kw_only=True)
 
     @classmethod
+    @deal.post(lambda activity: activity is None or activity.ended_at_time >= activity.started_at_time)
+    # NOTE: check for none due to bug in deal thinking inner function return value is actual return
     @inject.autoparams("project_gateway")
     def from_plan(
         cls,
         plan: Plan,
         repository: "Repository",
         project_gateway: IProjectGateway,
         started_at_time: datetime,
@@ -270,18 +272,19 @@
         elif self.started_at_time < other.started_at_time:
             return -1
         elif self.started_at_time > other.started_at_time:
             return 1
 
         return 0
 
-    def delete(self, when: datetime = local_now()):
+    @deal.ensure(lambda self, *_, result, **kwargs: self.invalidated_at >= self.ended_at_time)
+    def delete(self, when: Optional[datetime] = None):
         """Mark the activity as deleted."""
         self.unfreeze()
-        self.invalidated_at = when
+        self.invalidated_at = when or local_now()
         self.freeze()
 
 
 class ActivityCollection(Persistent):
     """Represent a list of activities."""
 
     def __init__(self, *, activities: List[Activity], id: Optional[str] = None):
```

### Comparing `renku-2.3.2/renku/domain_model/provenance/agent.py` & `renku-2.4.0rc1/renku/domain_model/provenance/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -157,13 +155,13 @@
         if len(names) == 1:
             return self.name
 
         last_name = names[-1]
         initials = [name[0] for name in names]
         initials.pop()
 
-        return "{0}.{1}".format(".".join(initials), last_name)
+        return "{}.{}".format(".".join(initials), last_name)
 
     @property
     def full_identity(self):
         """Return name, email, and affiliation."""
         return self.get_full_identity(self.email, self.affiliation, self.name)
```

### Comparing `renku-2.3.2/renku/domain_model/provenance/annotation.py` & `renku-2.4.0rc1/renku/ui/service/utils/squash.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Represent an annotation for a workflow."""
+"""Utilities for renku service controllers."""
+import collections.abc
 
-import copy
-from uuid import uuid4
 
+def squash(data, parent_key="", sep="."):
+    """Squash deeply nested dictionary."""
+    items = []
+    for k, v in data.items():
+        k = str(k)
+        if k[0] == "_":
+            k = k[1:]
+
+        new_key = parent_key + sep + k if parent_key else k
+        if isinstance(v, collections.abc.MutableMapping):
+            items.extend(squash(v, new_key, sep=sep).items())
+        else:
+            items.append((new_key, v))
 
-class Annotation:
-    """Represents a custom annotation for a research object."""
-
-    def __init__(self, *, id: str, body=None, source=None):
-        self.id = id
-        self.body = body
-        self.source = source
-
-    def copy(self):
-        """Return a copy of this annotation."""
-        return copy.deepcopy(self)
-
-    @staticmethod
-    def generate_id():
-        """Generate an id for an annotation."""
-        return f"/annotations/{uuid4().hex}"
+    return dict(items)
```

### Comparing `renku-2.3.2/renku/domain_model/provenance/parameter.py` & `renku-2.4.0rc1/renku/ui/service/cache/models/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Classes for tracking parameter values in provenance."""
+"""Renku service cache user related models."""
+from walrus import Model, TextField
 
-from typing import Any
-from uuid import uuid4
+from renku.ui.service.cache.base import BaseCache
 
-from renku.domain_model.workflow.plan import Plan
 
+class User(Model):
+    """User cache model."""
 
-class ParameterValue:
-    """Value for a parameter in provenance."""
+    __database__ = BaseCache.model_db
+    __namespace__ = BaseCache.namespace
 
-    def __init__(self, *, id: str, parameter_id: str, value: Any):
-        self.id = id
-        self.parameter_id: str = parameter_id
-        self.value: Any = value
-
-    @staticmethod
-    def generate_id(activity_id: str) -> str:
-        """Generate a default id."""
-        return f"{activity_id}/parameter-value/{uuid4().hex}"
-
-    def apply_value_to_parameter(self, plan: Plan) -> None:
-        """Apply the current value as actual_value on the plan's parameter."""
-        parameter = plan.get_field_by_id(self.parameter_id)
-        parameter.actual_value = self.value
+    user_id = TextField(primary_key=True, index=True)
+    fullname = TextField()
+    email = TextField()
+    token = TextField()
```

### Comparing `renku-2.3.2/renku/domain_model/session.py` & `renku-2.4.0rc1/renku/domain_model/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -76,29 +74,29 @@
 
         Returns:
             bool: True if the given container images is available locally.
         """
         pass
 
     @abstractmethod
-    def session_provider(self) -> "ISessionProvider":
+    def session_provider(self) -> ISessionProvider:
         """Supported session provider.
 
         Returns:
             a reference to ``self``.
         """
         pass
 
     @abstractmethod
-    def get_start_parameters(self) -> List["ProviderParameter"]:
+    def get_start_parameters(self) -> List[ProviderParameter]:
         """Returns parameters that can be set for session start."""
         pass
 
     @abstractmethod
-    def get_open_parameters(self) -> List["ProviderParameter"]:
+    def get_open_parameters(self) -> List[ProviderParameter]:
         """Returns parameters that can be set for session open."""
         pass
 
     @abstractmethod
     def session_list(self, project_name: str, config: Optional[Dict[str, Any]]) -> List[Session]:
         """Lists all the sessions currently running by the given session provider.
 
@@ -180,7 +178,11 @@
         """Perform any required checks on the state of the repository prior to starting a session.
 
         The expectation is that this method will abort the
         session start if the checks are not successful or will take corrective actions to
         make sure that the session launches successfully. By default this method does not do any checks.
         """
         return None
+
+    def force_build_image(self, **kwargs) -> bool:
+        """Whether we should force build the image directly or check for an existing image first."""
+        return False
```

### Comparing `renku-2.3.2/renku/domain_model/sort.py` & `renku-2.4.0rc1/renku/domain_model/sort.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/template.py` & `renku-2.4.0rc1/renku/domain_model/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -27,14 +25,15 @@
 
 import jinja2
 import yaml
 
 from renku.core import errors
 from renku.core.constant import RENKU_HOME
 from renku.core.util.os import get_safe_relative_path, hash_file
+from renku.core.util.util import to_string
 
 if TYPE_CHECKING:
     from renku.domain_model.project import Project
 
 TEMPLATE_MANIFEST = "manifest.yaml"
 
 
@@ -127,14 +126,15 @@
     @property
     def templates(self) -> List["Template"]:
         """Return list of available templates info in the manifest."""
         if self._templates is None:
             self._templates = [
                 Template(
                     id=cast(str, t.get("id") or t.get("folder")),
+                    aliases=t.get("aliases", []),
                     name=cast(str, t.get("name")),
                     description=cast(str, t.get("description")),
                     parameters=cast(Dict[str, Dict[str, Any]], t.get("variables") or t.get("parameters")),
                     icon=cast(str, t.get("icon")),
                     ssh_supported=t.get("ssh_supported", False),
                     immutable_files=t.get("immutable_template_files", []),
                     allow_update=t.get("allow_template_update", True),
@@ -158,25 +158,36 @@
         warnings = []
 
         if not self._content:
             raise errors.InvalidTemplateError("Cannot find any valid template in manifest file")
         elif not isinstance(self._content, list):
             raise errors.InvalidTemplateError(f"Invalid manifest content type: '{type(self._content).__name__}'")
 
+        existing_ids: Set[str] = set()
+
         # NOTE: First check if required fields exists for creating Template instances
         for template_entry in self._content:
             if not isinstance(template_entry, dict):
                 raise errors.InvalidTemplateError(f"Invalid template type: '{type(template_entry).__name__}'")
 
             id = template_entry.get("id") or template_entry.get("folder")
             if not id:
                 raise errors.InvalidTemplateError(f"Template doesn't have an id: '{template_entry}'")
             if not template_entry.get("id"):
                 warnings.append(f"Template '{id}' should use 'id' attribute instead of 'folder'.")
 
+            # NOTE: Check for duplicate IDs and aliases
+            aliases = {id}
+            aliases.update(template_entry.get("aliases", []))
+            duplicates = existing_ids.intersection(aliases)
+            if duplicates:
+                duplicates_str = ", ".join(sorted(f"'{d}'" for d in duplicates))
+                raise errors.InvalidTemplateError(f"Found duplicate IDs or aliases: {duplicates_str}")
+            existing_ids.update(aliases)
+
             parameters = template_entry.get("variables")
             if parameters:
                 if not isinstance(parameters, dict):
                     raise errors.InvalidTemplateError(
                         f"Invalid template variable type on template '{id}': '{type(parameters).__name__}', "
                         "should be 'dict'."
                     )
@@ -206,14 +217,15 @@
         self,
         id: str,
         name: str,
         description: str,
         parameters: Dict[str, Dict[str, Any]],
         icon: str,
         ssh_supported: bool,
+        aliases: List[str],
         immutable_files: List[str],
         allow_update: bool,
         source: Optional[str],
         reference: Optional[str],
         version: Optional[str],
         path: Optional[Path],
         templates_source: Optional[TemplatesSource],
@@ -223,23 +235,27 @@
         self.reference = reference
         self.version = version
         self.id: str = id
         self.name: str = name
         self.description: str = description
         self.icon = icon
         self.ssh_supported = ssh_supported
+        self.aliases: List[str] = aliases
         self.immutable_files: List[str] = immutable_files or []
         self.allow_update: bool = allow_update
         parameters = parameters or {}
         self.parameters: List[TemplateParameter] = [
             TemplateParameter.from_dict(name=k, value=v) for k, v in parameters.items()
         ]
 
         self._templates_source: Optional[TemplatesSource] = templates_source
 
+    def __repr__(self) -> str:
+        return f"<Template {self.id}@{self.version}>"
+
     @property
     def templates_source(self) -> Optional[TemplatesSource]:
         """Return template's source."""
         return self._templates_source
 
     @templates_source.setter
     def templates_source(self, templates_source: TemplatesSource):
@@ -292,17 +308,15 @@
             if raise_errors:
                 raise errors.InvalidTemplateError(issue)
             issues.append(issue)
 
         existing_prohibited_paths: Set[str] = set()
 
         for pattern in self.PROHIBITED_PATHS:
-            matches = set(
-                m for m in self.path.glob(pattern) if str(m.relative_to(self.path)) not in self.REQUIRED_FILES
-            )
+            matches = {m for m in self.path.glob(pattern) if str(m.relative_to(self.path)) not in self.REQUIRED_FILES}
             if matches:
                 existing_prohibited_paths.update(str(m.relative_to(self.path)) for m in matches)
 
         if existing_prohibited_paths:
             prohibited_paths_str = "\n\t\t\t".join(p for p in existing_prohibited_paths)
             issue = f"These paths are not allowed in a template:\n\t\t\t{prohibited_paths_str}"
             if raise_errors:
@@ -530,15 +544,16 @@
             # NOTE: Ignore Project.automated_update since it's default is False and won't allow any update at all
 
             immutable_files = project.template_metadata.immutable_template_files or []
 
         # NOTE: Always set __renku_version__ to the value read from the Dockerfile (if available) since setting/updating
         # the template doesn't change project's metadata version and shouldn't update the Renku version either
         renku_version = metadata.get("__renku_version__")
-        metadata["__renku_version__"] = str(read_renku_version_from_dockerfile()) or renku_version or __version__
+        dockerfile_version = to_string(read_renku_version_from_dockerfile())
+        metadata["__renku_version__"] = dockerfile_version or renku_version or __version__
 
         return cls(metadata=metadata, immutable_files=immutable_files)
 
     @property
     def source(self):
         """Template source."""
         return self.metadata.get("__template_source__")
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/__init__.py` & `renku-2.4.0rc1/renku/domain_model/workflow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/composite_plan.py` & `renku-2.4.0rc1/renku/domain_model/workflow/composite_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/converters/__init__.py` & `renku-2.4.0rc1/renku/domain_model/workflow/converters/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/parameter.py` & `renku-2.4.0rc1/renku/domain_model/workflow/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/plan.py` & `renku-2.4.0rc1/renku/domain_model/workflow/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -158,15 +156,15 @@
 
         NOTE: Don't call this function for deleting plans since it doesn't delete the whole plan derivatives chain. Use
         renku.core.workflow.plan::remove_plan instead.
         """
         when = when or local_now()
 
         self.unfreeze()
-        self.date_removed = when
+        self.date_removed = when or local_now()
         self.freeze()
 
 
 class Plan(AbstractPlan):
     """Represent a `renku run` execution template."""
 
     annotations: List[Annotation] = list()
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/provider.py` & `renku-2.4.0rc1/renku/domain_model/workflow/provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -36,14 +34,14 @@
 
         Returns:
             Tuple[IWorkflowProvider,str]: A tuple of the provider itself and the workflow executor backends name.
         """
         pass
 
     @abstractmethod
-    def workflow_execute(self, dag: "nx.DiGraph", basedir: Path, config: Dict[str, Any]):
+    def workflow_execute(self, dag: nx.DiGraph, basedir: Path, config: Dict[str, Any]):
         """Executes a given ``AbstractPlan`` using the provider.
 
         Returns:
             A list of output paths that were generated by this workflow.
         """
         pass
```

### Comparing `renku-2.3.2/renku/domain_model/workflow/workflow_file.py` & `renku-2.4.0rc1/renku/domain_model/workflow/workflow_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `renku-2.3.2/renku/infrastructure/__init__.py` & `renku-2.4.0rc1/renku/core/template/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku metadata storage/retrieval."""
+"""Renku template management."""
```

### Comparing `renku-2.3.2/renku/infrastructure/database.py` & `renku-2.4.0rc1/renku/infrastructure/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -24,14 +23,15 @@
 import json
 from enum import Enum
 from pathlib import Path
 from types import BuiltinFunctionType, FunctionType
 from typing import Any, Dict, List, Optional, Union, cast
 from uuid import uuid4
 
+import deal
 import persistent
 import zstandard as zstd
 from BTrees.Length import Length
 from BTrees.OOBTree import BTree, OOBucket, OOSet, OOTreeSet
 from persistent import GHOST, UPTODATE
 from persistent.interfaces import IPickleCache
 from zc.relation.catalog import Catalog
@@ -64,15 +64,15 @@
         module_name(str): The module name to check.
         type_name(str): The type within the module to check.
 
     Raises:
         TypeError: If the type is now allowed in the database.
     """
 
-    if module_name not in ["BTrees", "builtins", "datetime", "persistent", "renku", "zc", "zope"]:
+    if module_name not in ["BTrees", "builtins", "datetime", "persistent", "renku", "zc", "zope", "deal"]:
         raise TypeError(f"Objects of type '{type_name}' are not allowed")
 
 
 def get_type_name(object) -> Optional[str]:
     """Return fully-qualified object's type name.
 
     Args:
@@ -362,24 +362,25 @@
             path(str): Path of the database object.
             absolute(bool): Whether the path is absolute or a filename inside the database (Default value = False).
             override_type(Optional[str]): load object as a different type than what is set inside `renku_data_type`
                 (Default value = None).
         Returns:
             persistent.Persistent: The object.
         """
+        deal.disable(warn=False)
         data = self._storage.load(filename=path, absolute=absolute)
         if override_type is not None:
             if "@renku_data_type" not in data:
                 raise errors.IncompatibleParametersError("Cannot override type on found data.")
 
             data["@renku_data_type"] = override_type
         object = self._reader.deserialize(data)
         object._p_changed = 0
         object._p_serial = PERSISTED
-
+        deal.enable()
         return object
 
     def get_by_id(self, id: str) -> persistent.Persistent:
         """Return an object by its id.
 
         Args:
             id(str): The id to look up.
@@ -438,19 +439,21 @@
 
     def setstate(self, object: persistent.Persistent):
         """Load the state for a ghost object.
 
         Args:
             object(persistent.Persistent): The object to set the state on.
         """
+        deal.disable(warn=False)
         data = self._storage.load(filename=self._get_filename_from_oid(object._p_oid))
         self._reader.set_ghost_state(object, data)
         object._p_serial = PERSISTED
         if isinstance(object, Persistent):
             object.freeze()
+        deal.enable()
 
     def commit(self):
         """Commit modified and new objects."""
         while self._objects_to_commit:
             _, object = self._objects_to_commit.popitem()
             if object._p_changed or object._p_serial == NEW:
                 self._store_object(object)
@@ -577,15 +580,15 @@
         self[oid] = object
 
 
 class Index(persistent.Persistent):
     """Database index."""
 
     def __init__(self, *, name: str, object_type, attribute: Optional[str], key_type=None):
-        """Create an index where keys are extracted using `attribute` from an object or a key.
+        """Create an index where keys are extracted using ``attribute`` from an object or a key.
 
         Args:
             name (str): Index's name.
             object_type: Type of objects that the index points to.
             attribute (Optional[str], optional): Name of an attribute to be used to automatically generate a key
                 (e.g. `entity.path`).
             key_type: Type of keys. If not None then a key must be provided when updating the index
@@ -631,14 +634,17 @@
     def __setstate__(self, data):
         self._name = data.pop("name")
         self._object_type = get_class(data.pop("object_type"))
         self._key_type = get_class(data.pop("key_type"))
         self._attribute = data.pop("attribute")
         self._entries = data.pop("entries")
 
+    def __iter__(self):
+        return self._entries.__iter__()
+
     @property
     def name(self) -> str:
         """Return Index's name."""
         return self._name
 
     @property
     def object_type(self) -> type:
@@ -790,15 +796,15 @@
                 self.path.mkdir(parents=True, exist_ok=True)
 
         if compress:
             with open(path, "wb") as fb, self.zstd_compressor.stream_writer(fb) as compressor:
                 with io.TextIOWrapper(compressor) as out:
                     json.dump(data, out, ensure_ascii=False)
         else:
-            with open(path, "wt") as ft:
+            with open(path, "w") as ft:
                 json.dump(data, ft, ensure_ascii=False, sort_keys=True, indent=2)
 
     def load(self, filename: str, absolute: bool = False):
         """Load data for object with object id oid.
 
         Args:
             filename(str): The file name of the data to load.
@@ -860,95 +866,85 @@
             data = {"@renku_data_value": data}
 
         data["@renku_data_type"] = get_type_name(object)
         data["@renku_oid"] = object._p_oid
 
         return data
 
-    def _serialize_helper(self, object):
+    def _serialize_helper(self, obj):
         # TODO: Raise an error if an unsupported object is being serialized
-        if object is None:
+        if obj is None:
             return None
-        elif isinstance(object, (int, float, str, bool)):
-            return object
-        elif isinstance(object, list):
-            return [self._serialize_helper(value) for value in object]
-        elif isinstance(object, set):
+        elif isinstance(obj, (int, float, str, bool)):
+            return obj
+        elif isinstance(obj, list):
+            return [self._serialize_helper(value) for value in obj]
+        elif isinstance(obj, set):
             return {
                 "@renku_data_type": SET_TYPE,
-                "@renku_data_value": [self._serialize_helper(value) for value in object],
+                "@renku_data_value": [self._serialize_helper(value) for value in obj],
             }
-        elif isinstance(object, frozenset):
+        elif isinstance(obj, frozenset):
             return {
                 "@renku_data_type": FROZEN_SET_TYPE,
-                "@renku_data_value": [self._serialize_helper(value) for value in object],
+                "@renku_data_value": [self._serialize_helper(value) for value in obj],
             }
-        elif isinstance(object, dict):
+        elif isinstance(obj, dict):
             result = dict()
-            items = sorted(object.items(), key=lambda x: x[0])
+            items = sorted(obj.items(), key=lambda x: x[0])
             for key, value in items:
                 result[key] = self._serialize_helper(value)
             return result
-        elif isinstance(object, Index):
+        elif isinstance(obj, Index):
             # NOTE: Index objects are not stored as references and are included in their parent object (i.e. root)
-            state = object.__getstate__()
+            state = obj.__getstate__()
             state = self._serialize_helper(state)
-            return {"@renku_data_type": get_type_name(object), "@renku_oid": object._p_oid, **state}
-        elif isinstance(object, (OOTreeSet, Length, OOSet)):
-            state = object.__getstate__()
+            return {"@renku_data_type": get_type_name(obj), "@renku_oid": obj._p_oid, **state}
+        elif isinstance(obj, (OOTreeSet, Length, OOSet)):
+            state = obj.__getstate__()
             state = self._serialize_helper(state)
-            return {"@renku_data_type": get_type_name(object), "@renku_data_value": state}
-        elif isinstance(object, persistent.Persistent):
-            if not object._p_oid:
-                object._p_oid = Database.generate_oid(object)
-            if object._p_state not in [GHOST, UPTODATE] or (object._p_state == UPTODATE and object._p_serial == NEW):
-                self._database.register(object)
-            return {"@renku_data_type": get_type_name(object), "@renku_oid": object._p_oid, "@renku_reference": True}
-        elif isinstance(object, datetime.datetime):
-            value = object.isoformat()
-        elif isinstance(object, tuple):
-            value = tuple(self._serialize_helper(value) for value in object)
-        elif isinstance(object, (InterfaceClass)):
+            return {"@renku_data_type": get_type_name(obj), "@renku_data_value": state}
+        elif isinstance(obj, persistent.Persistent):
+            if not obj._p_oid:
+                obj._p_oid = Database.generate_oid(obj)
+            if obj._p_state not in [GHOST, UPTODATE] or (obj._p_state == UPTODATE and obj._p_serial == NEW):
+                self._database.register(obj)
+            return {"@renku_data_type": get_type_name(obj), "@renku_oid": obj._p_oid, "@renku_reference": True}
+        elif isinstance(obj, datetime.datetime):
+            value = obj.isoformat()
+        elif isinstance(obj, tuple):
+            value = tuple(self._serialize_helper(value) for value in obj)
+        elif isinstance(obj, (InterfaceClass)):
             # NOTE: Zope interfaces are weird, they're a class with type InterfaceClass, but need to be deserialized
             # as the class (without instantiation)
-            return {"@renku_data_type": TYPE_TYPE, "@renku_data_value": f"{object.__module__}.{object.__name__}"}
-        elif isinstance(object, type):
+            return {"@renku_data_type": TYPE_TYPE, "@renku_data_value": f"{obj.__module__}.{obj.__name__}"}
+        elif isinstance(obj, type):
             # NOTE: We're storing a type, not an instance
-            return {"@renku_data_type": TYPE_TYPE, "@renku_data_value": get_type_name(object)}
-        elif isinstance(object, (FunctionType, BuiltinFunctionType)):
-            name = object.__name__
-            module = getattr(object, "__module__", None)
+            return {"@renku_data_type": TYPE_TYPE, "@renku_data_value": get_type_name(obj)}
+        elif isinstance(obj, (FunctionType, BuiltinFunctionType)):
+            name = obj.__name__
+            module = getattr(obj, "__module__", None)
             return {"@renku_data_type": FUNCTION_TYPE, "@renku_data_value": f"{module}.{name}"}
-        elif hasattr(object, "__getstate__"):
-            if id(object) in self._serialization_cache:
-                # NOTE: We already serialized this -> circular/repeat reference.
-                return {"@renku_data_type": REFERENCE_TYPE, "@renku_data_value": self._serialization_cache[id(object)]}
-
-            # NOTE: The reference used for circular reference is just the position in the serialization cache,
-            # as the order is deterministic. So the order in which objects are encoutered is their id for referencing.
-            self._serialization_cache[id(object)] = len(self._serialization_cache)
-
-            value = object.__getstate__().copy()
-            value = {k: v for k, v in value.items() if not k.startswith("_v_")}
-            value = self._serialize_helper(value)
-            assert not isinstance(value, dict) or "id" in value, f"Invalid object state: {value} for {object}"
         else:
-            if id(object) in self._serialization_cache:
+            if id(obj) in self._serialization_cache:
                 # NOTE: We already serialized this -> circular/repeat reference
-                return {"@renku_data_type": REFERENCE_TYPE, "@renku_data_value": self._serialization_cache[id(object)]}
+                return {"@renku_data_type": REFERENCE_TYPE, "@renku_data_value": self._serialization_cache[id(obj)]}
 
             # NOTE: The reference used for circular reference is just the position in the serialization cache,
             # as the order is deterministic So the order in which objects are encoutered is their id for referencing.
-            self._serialization_cache[id(object)] = len(self._serialization_cache)
-
-            value = object.__dict__.copy()
+            self._serialization_cache[id(obj)] = len(self._serialization_cache)
+            if hasattr(obj, "__getstate__"):
+                # NOTE: On Python 3.11+ this just returns __dict__ if __getstate__ isn't implemented.
+                value = obj.__getstate__().copy()
+            else:
+                value = obj.__dict__.copy()
             value = {k: v for k, v in value.items() if not k.startswith("_v_")}
             value = self._serialize_helper(value)
 
-        return {"@renku_data_type": get_type_name(object), "@renku_data_value": value}
+        return {"@renku_data_type": get_type_name(obj), "@renku_data_value": value}
 
 
 class ObjectReader:
     """Deserialize objects loaded from storage."""
 
     def __init__(self, database: Database):
         self._classes: Dict[str, type] = {}
@@ -1027,15 +1023,15 @@
             if object_type in (TYPE_TYPE, FUNCTION_TYPE):
                 # NOTE: if we stored a type (not instance), return the type
                 return self._get_class(data["@renku_data_value"])
             elif object_type == REFERENCE_TYPE:
                 # NOTE: we had a circular reference, we return the (not yet finalized) class here
                 return self._deserialization_cache[data["@renku_data_value"]]
             elif object_type == SET_TYPE:
-                return set([self._deserialize_helper(value) for value in data["@renku_data_value"]])
+                return {self._deserialize_helper(value) for value in data["@renku_data_value"]}
             elif object_type == FROZEN_SET_TYPE:
                 return frozenset([self._deserialize_helper(value) for value in data["@renku_data_value"]])
 
             cls = self._get_class(object_type)
 
             if cls is None:
                 raise TypeError(f"Couldn't find class '{object_type}'")
@@ -1093,16 +1089,19 @@
 
                 data = self._deserialize_helper(data)
                 assert isinstance(data, dict)
 
                 if "id" in data and data["id"] in self._normal_object_cache:
                     return self._normal_object_cache[data["id"]]
 
-                for name, value in data.items():
-                    object.__setattr__(new_object, name, value)
+                if hasattr(new_object, "__setstate__"):
+                    new_object.__setstate__(data)
+                else:
+                    for name, value in data.items():
+                        object.__setattr__(new_object, name, value)
 
                 if issubclass(cls, Immutable):
                     new_object = cls.make_instance(new_object)
 
                 if "id" in data and isinstance(data["id"], str) and data["id"].startswith("/"):
                     self._normal_object_cache[data["id"]] = new_object
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/__init__.py` & `renku-2.4.0rc1/renku/core/util/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku database gateway implementations."""
+"""Renku utility methods."""
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/activity_gateway.py` & `renku-2.4.0rc1/renku/infrastructure/gateway/activity_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -17,14 +16,15 @@
 # limitations under the License.
 """Renku activity database gateway implementation."""
 
 import itertools
 from pathlib import Path
 from typing import List, Optional, Set, Tuple, Union
 
+import deal
 from persistent.list import PersistentList
 
 from renku.command.command_builder.command import inject
 from renku.core import errors
 from renku.core.interface.activity_gateway import IActivityGateway
 from renku.core.interface.plan_gateway import IPlanGateway
 from renku.core.util.os import are_paths_related
@@ -137,14 +137,21 @@
         return upstream_chains
 
     def get_all_activities(self, include_deleted: bool = False) -> List[Activity]:
         """Get all activities in the project."""
         database = project_context.database
         return [a for a in database["activities"].values() if not a.deleted or include_deleted]
 
+    @deal.pre(lambda _: _.activity.started_at_time is not None)
+    @deal.pre(lambda _: _.activity.ended_at_time is not None)
+    @deal.pre(lambda _: _.activity.started_at_time >= project_context.project.date_created)
+    @deal.pre(
+        lambda _: _.activity.invalidated_at is None or _.activity.invalidated_at >= project_context.project.date_created
+    )
+    @deal.pre(lambda _: _.activity.started_at_time >= _.activity.association.plan.date_created)
     def add(self, activity: Activity) -> None:
         """Add an ``Activity`` to storage."""
 
         database = project_context.database
 
         database["activities"].add(activity)
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/database_gateway.py` & `renku-2.4.0rc1/renku/infrastructure/gateway/database_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/dataset_gateway.py` & `renku-2.4.0rc1/renku/infrastructure/gateway/dataset_gateway.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -15,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Renku dataset gateway interface."""
 
 from typing import List, Optional
 
+import deal
 from persistent.list import PersistentList
 
 from renku.core.interface.dataset_gateway import IDatasetGateway
 from renku.domain_model.dataset import Dataset, DatasetTag
 from renku.domain_model.project_context import project_context
 
 
@@ -47,14 +47,15 @@
         """Return the provenance for all datasets."""
         return list(project_context.database["datasets-provenance-tails"].values())
 
     def get_all_tags(self, dataset: Dataset) -> List[DatasetTag]:
         """Return the list of all tags for a dataset."""
         return list(project_context.database["datasets-tags"].get(dataset.name, []))
 
+    @deal.pre(lambda _: _.tag.date_created is None or _.tag.date_created >= project_context.project.date_created)
     def add_tag(self, dataset: Dataset, tag: DatasetTag):
         """Add a tag from a dataset."""
         tags: PersistentList = project_context.database["datasets-tags"].get(dataset.name)
         if not tags:
             tags = PersistentList()
             project_context.database["datasets-tags"].add(tags, key=dataset.name)
 
@@ -66,14 +67,18 @@
         """Remove a tag from a dataset."""
         tags: PersistentList = project_context.database["datasets-tags"].get(dataset.name)
         for t in tags:
             if t.name == tag.name:
                 tags.remove(t)
                 break
 
+    # NOTE: Enable this again once we properly deal with `date_created` on imported Renku datasets
+    # @deal.pre(
+    #     lambda _: _.dataset.date_created is None or _.dataset.date_created >= project_context.project.date_created
+    # )
     def add_or_remove(self, dataset: Dataset) -> None:
         """Add or remove a dataset."""
         database = project_context.database
 
         if dataset.date_removed:
             database["datasets"].pop(dataset.name, None)
             database["datasets-tags"].pop(dataset.name, None)
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/plan_gateway.py` & `renku-2.4.0rc1/renku/ui/api/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku plan database gateway implementation."""
+r"""Renku API utilities."""
 
-from typing import Dict, List, Optional, cast
+from functools import wraps
+from typing import TYPE_CHECKING, Optional
 
-from renku.core import errors
-from renku.core.interface.plan_gateway import IPlanGateway
 from renku.domain_model.project_context import project_context
-from renku.domain_model.workflow.plan import AbstractPlan
 
+if TYPE_CHECKING:
+    from renku.infrastructure.gateway.activity_gateway import ActivityGateway
+    from renku.infrastructure.gateway.plan_gateway import PlanGateway
 
-class PlanGateway(IPlanGateway):
-    """Gateway for plan database operations."""
 
-    def get_by_id(self, id: Optional[str]) -> Optional[AbstractPlan]:
-        """Get a plan by id."""
-        return project_context.database["plans"].get(id)
-
-    def get_by_name(self, name: str) -> Optional[AbstractPlan]:
-        """Get a plan by name."""
-        return project_context.database["plans-by-name"].get(name)
-
-    def get_by_name_or_id(self, name_or_id: str) -> AbstractPlan:
-        """Get a plan by name or id."""
-        workflow = self.get_by_id(name_or_id) or self.get_by_name(name_or_id)
-
-        if not workflow:
-            raise errors.WorkflowNotFoundError(name_or_id)
-        return workflow
-
-    def list_by_name(self, starts_with: str, ends_with: Optional[str] = None) -> List[str]:
-        """Search plans by name."""
-        return [
-            name
-            for name in project_context.database["plans-by-name"].keys(min=starts_with, max=ends_with)
-            if not cast(AbstractPlan, self.get_by_name(name)).deleted
-        ]
-
-    def get_newest_plans_by_names(self, include_deleted: bool = False) -> Dict[str, AbstractPlan]:
-        """Return a mapping of all plan names to their newest plans."""
-        database = project_context.database
-        if include_deleted:
-            return dict(database["plans-by-name"])
-        return {k: v for k, v in database["plans-by-name"].items() if not v.deleted}
-
-    def get_all_plans(self) -> List[AbstractPlan]:
-        """Get all plans in project."""
-        return list(project_context.database["plans"].values())
-
-    def add(self, plan: AbstractPlan) -> None:
-        """Add a plan to the database."""
-        database = project_context.database
-
-        if database["plans"].get(plan.id) is not None:
-            return
-
-        database["plans"].add(plan)
-
-        if plan.derived_from is not None:
-            derived_from = self.get_by_id(plan.derived_from)
-
-            if derived_from is not None:
-                database["plans-by-name"].pop(derived_from.name, None)
-        database["plans-by-name"].add(plan)
+def ensure_project_context(fn):
+    """Check existence of a project context.
+
+    Args:
+        fn: The function to wrap.
+
+    Returns:
+        The function with the current project injected.
+    """
+
+    def get_current_project():
+        """Return current project context if any or a new project object.
+
+        Returns:
+            The current project context or None.
+        """
+        from renku.ui.api import Project
+
+        return Project._project_contexts.top if Project._project_contexts.top else None
+
+    @wraps(fn)
+    def wrapper(*args, **kwargs):
+        from renku.ui.api import Project
+
+        project = get_current_project() or Project()
+        return fn(*args, **kwargs, project=project)
+
+    return wrapper
+
+
+@ensure_project_context
+def get_activity_gateway(project) -> Optional["ActivityGateway"]:
+    """Return an instance of ActivityGateway when inside a Renku project."""
+    from renku.infrastructure.gateway.activity_gateway import ActivityGateway
+
+    try:
+        _ = project_context.repository
+    except ValueError:
+        return None
+
+    return ActivityGateway()
+
+
+@ensure_project_context
+def get_plan_gateway(project) -> Optional["PlanGateway"]:
+    """Return an instance of PlanGateway when inside a Renku project."""
+    from renku.infrastructure.gateway.plan_gateway import PlanGateway
+
+    try:
+        _ = project_context.repository
+    except ValueError:
+        return None
+
+    return PlanGateway()
```

### Comparing `renku-2.3.2/renku/infrastructure/gateway/project_gateway.py` & `renku-2.4.0rc1/renku/infrastructure/gateway/project_gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/infrastructure/git_merger.py` & `renku-2.4.0rc1/renku/infrastructure/git_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -37,17 +36,22 @@
 from renku.domain_model.project import Project
 from renku.domain_model.project_context import project_context
 from renku.domain_model.workflow.plan import AbstractPlan
 from renku.infrastructure.database import Database, Index
 from renku.infrastructure.repository import Repository
 from renku.version import __version__
 
-RemoteEntry = NamedTuple(
-    "RemoteEntry", [("reference", str), ("database", Database), ("path", Path), ("repository", Repository)]
-)
+
+class RemoteEntry(NamedTuple):
+    """Reference to an entry in a database on a separate branch."""
+
+    reference: str
+    database: Database
+    path: Path
+    repository: Repository
 
 
 class GitMerger:
     """Git metadata merger."""
 
     def merge(self, local: Path, remote: Path, base: Path) -> None:
         """Merge two renku metadata entries together."""
@@ -293,15 +297,14 @@
                     existing = set(base.keywords) - removed
                     local.keywords = list(added | existing)
                 elif remote.keywords != base.keywords:
                     local.keywords = remote.keywords
 
             # NOTE: Merge description
             if local.description != remote.description:
-
                 if base is None or (local.description != base.description and remote.description != base.description):
                     local.description = communication.prompt(
                         f"Project description was modified in local and remote branch.\n"
                         f"local: {local.description}\nremote: {remote.description}\nEnter merged description: ",
                         default=local.description,
                     )
                 elif remote.description != base.description:
```

### Comparing `renku-2.3.2/renku/infrastructure/immutable.py` & `renku-2.4.0rc1/renku/infrastructure/immutable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -15,51 +14,61 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Slots and Immutable classes."""
 
 import threading
 import weakref
+from typing import Tuple, cast
 
 
 class Slots:
     """An immutable class.
 
     Subclasses are supposed to use __slots__ to define their members.
     """
 
     __slots__ = ("__weakref__",)
-    __all_slots__ = None
+    __all_slots__: Tuple[str, ...] = tuple()
+
+    def __new__(cls, *args, **kwargs):
+        """Create and return an empty instance of the class."""
+        if not cls.__all_slots__:
+            cls.__all_slots__ = cast(Tuple[str, ...], cls._get_all_slots())
+
+        return object.__new__(cls)
 
     def __init__(self, **kwargs):
-        if not self.__class__.__all_slots__:
-            self.__class__.__all_slots__ = self._get_all_slots()
         for key, value in kwargs.items():
             object.__setattr__(self, key, value)
 
     @classmethod
     def make_instance(cls, **kwargs):
         """Instantiate from the given parameters."""
         return cls(**kwargs)
 
     def __getstate__(self):
-        if not self.__class__.__all_slots__:
-            self.__class__.__all_slots__ = self._get_all_slots()
         return {name: getattr(self, name, None) for name in self.__class__.__all_slots__ if name != "__weakref__"}
 
     def __setstate__(self, state):
+        new_attributes = set(self.__all_slots__) - set(state)
+        for name in new_attributes:
+            if name != "__weakref__":
+                object.__setattr__(self, name, None)
+
         for name, value in state.items():
-            setattr(self, name, value)
+            object.__setattr__(self, name, value)
 
-    def _get_all_slots(self):
+    @classmethod
+    def _get_all_slots(cls):
         all_slots = set()
-        for cls in self.__class__.mro():
-            if not hasattr(cls, "__slots__"):
+        for klass in cls.mro():
+            if not hasattr(klass, "__slots__"):
                 continue
-            slots = {cls.__slots__} if isinstance(cls.__slots__, str) else set(cls.__slots__)
+            slots = {klass.__slots__} if isinstance(klass.__slots__, str) else set(klass.__slots__)
             all_slots.update(slots)
         return tuple(all_slots)
 
 
 class Immutable(Slots):
     """An immutable class that its instances can be cached and reused.
```

### Comparing `renku-2.3.2/renku/infrastructure/persistent.py` & `renku-2.4.0rc1/renku/infrastructure/persistent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/infrastructure/repository.py` & `renku-2.4.0rc1/renku/infrastructure/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -32,14 +30,15 @@
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
+    Literal,
     NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
@@ -49,19 +48,14 @@
 )
 
 import git
 
 from renku.core import errors
 from renku.core.util.os import delete_dataset_file, get_absolute_path
 
-try:
-    from typing_extensions import Literal  # NOTE: Required for Python 3.7 compatibility
-except ImportError:
-    from typing import Literal  # type: ignore
-
 NULL_TREE = git.NULL_TREE
 _MARKER = object()
 GIT_IGNORE = ".gitignore"
 
 
 def git_unicode_unescape(s: Optional[str], encoding: str = "utf-8") -> str:
     """Undoes git/GitPython unicode encoding."""
@@ -138,15 +132,15 @@
     def remotes(self) -> "RemoteManager":
         """Return all remotes."""
         if self._repository is None:
             raise errors.ParameterError("Repository not set.")
         return RemoteManager(self._repository)
 
     @property  # type: ignore
-    @lru_cache()
+    @lru_cache
     def submodules(self) -> "SubmoduleManager":
         """Return a list of submodules."""
         if self._repository is None:
             raise errors.ParameterError("Repository not set.")
         return SubmoduleManager(self._repository)
 
     @property
@@ -975,15 +969,15 @@
             return result[0]
         return None
 
     @staticmethod
     def hash_string(content: str) -> str:
         """Calculate the object-hash for a blob with specified content."""
         content_bytes = content.encode("utf-8")
-        data = f"blob {len(content_bytes)}\0".encode("utf-8") + content_bytes
+        data = f"blob {len(content_bytes)}\0".encode() + content_bytes
         return hashlib.sha1(data).hexdigest()  # nosec
 
 
 class Repository(BaseRepository):
     """Abstract Base repository."""
 
     def __init__(
@@ -1189,15 +1183,14 @@
             return self._get_submodule(submodule)
 
     def __iter__(self):
         if self._repository is None:
             raise errors.ParameterError("Repository not set.")
 
         for s in self._repository.submodules:
-
             yield self._get_submodule(s)
 
     def __len__(self) -> int:
         if self._repository is None:
             raise errors.ParameterError("Repository not set.")
 
         return len(self._repository.submodules)
```

### Comparing `renku-2.3.2/renku/infrastructure/storage/__init__.py` & `renku-2.4.0rc1/renku/ui/service/views/v1/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku remote storage implementations."""
+"""Renku service v1.0 views."""
```

### Comparing `renku-2.3.2/renku/infrastructure/storage/factory.py` & `renku-2.4.0rc1/renku/infrastructure/storage/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,48 +12,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Storage factory implementation."""
 
-from typing import TYPE_CHECKING, Callable, Dict
+from typing import TYPE_CHECKING, Dict
 
 from renku.core.interface.storage import IStorage, IStorageFactory
 
 if TYPE_CHECKING:
-    from renku.core.dataset.providers.api import ProviderApi, ProviderCredentials
+    from renku.core.dataset.providers.api import CloudStorageProviderType, ProviderCredentials
 
 
 class StorageFactory(IStorageFactory):
     """Return an external storage."""
 
     @staticmethod
     def get_storage(
         storage_scheme: str,
-        provider: "ProviderApi",
+        provider: "CloudStorageProviderType",
         credentials: "ProviderCredentials",
         configuration: Dict[str, str],
-        uri_convertor: Callable[[str], str],
     ) -> "IStorage":
         """Return a storage that handles provider.
 
         Args:
             storage_scheme(str): Storage name.
-            provider(ProviderApi): The backend provider.
+            provider(CloudStorageProviderType): The backend provider.
             credentials(ProviderCredentials): Credentials for the provider.
             configuration(Dict[str, str]): Storage-specific configuration that are passed to the IStorage implementation
-            uri_convertor(Callable[[str], str]): A function that converts backend-specific URI to a URI that is usable
-                by the IStorage implementation.
 
         Returns:
             An instance of IStorage.
         """
         from .rclone import RCloneStorage
 
         return RCloneStorage(
             storage_scheme=storage_scheme,
             provider=provider,
             credentials=credentials,
             provider_configuration=configuration,
-            provider_uri_convertor=uri_convertor,
         )
```

### Comparing `renku-2.3.2/renku/infrastructure/storage/rclone.py` & `renku-2.4.0rc1/renku/core/dataset/providers/external.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,178 +1,151 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Base storage handler."""
+"""External dataset provider."""
+
+from __future__ import annotations
 
-import json
-import os
-import subprocess
+import urllib
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import TYPE_CHECKING, List, Optional, Tuple, cast
 
 from renku.core import errors
-from renku.core.interface.storage import FileHash, IStorage
-from renku.core.util.util import NO_VALUE
+from renku.core.dataset.providers.api import (
+    AddProviderInterface,
+    ProviderApi,
+    ProviderCredentials,
+    ProviderPriority,
+    StorageProviderInterface,
+)
+from renku.core.dataset.providers.common import get_metadata
+from renku.core.dataset.providers.models import DatasetAddAction
+from renku.core.interface.storage import IStorage
+from renku.core.util.os import get_absolute_path
+from renku.core.util.urls import get_scheme
+from renku.domain_model.project_context import project_context
+from renku.infrastructure.storage.factory import StorageFactory
+
+if TYPE_CHECKING:
+    from renku.core.dataset.providers.models import DatasetAddMetadata
+    from renku.domain_model.dataset import Dataset
+
+
+class ExternalProvider(ProviderApi, StorageProviderInterface, AddProviderInterface):
+    """External provider for remote filesystem."""
+
+    priority = ProviderPriority.HIGHEST
+    name = "External"
+
+    def __init__(self, uri: str):
+        super().__init__(uri=get_uri_absolute_path(uri).rstrip("/"))
+
+    @staticmethod
+    def supports(uri: str) -> bool:
+        """External doesn't support any URI for addition. It's only for storage backends."""
+        return False
+
+    @staticmethod
+    def supports_storage(uri: str) -> bool:
+        """Whether or not this provider supports a given URI storage."""
+        return get_scheme(uri) in ("file", "")
+
+    @property
+    def path(self) -> str:
+        """Return External path."""
+        return self.uri
+
+    def get_metadata(
+        self, uri: str, destination: Path, dataset_add_action: DatasetAddAction = DatasetAddAction.NONE, **_
+    ) -> List["DatasetAddMetadata"]:
+        """Get metadata of files that will be added to a dataset."""
+        files = get_metadata(provider=self, uri=uri, destination=destination, dataset_add_action=dataset_add_action)
+        for file in files:
+            if file.url and not file.url.startswith("file:"):
+                file.url = f"file://{file.url}"
+                if file.based_on:
+                    file.based_on.url = file.url
+        return files
+
+    def convert_to_storage_uri(self, uri: str) -> str:
+        """Convert backend-specific URI to a URI that is usable by the IStorage implementation."""
+        return f"file://{get_uri_absolute_path(uri=uri)}"
+
+    def get_credentials(self) -> "ExternalCredentials":
+        """Return an instance of provider's credential class."""
+        return ExternalCredentials(provider=self)
+
+    def get_storage(self, credentials: Optional["ProviderCredentials"] = None) -> "IStorage":
+        """Return the storage manager for the provider."""
+        external_configuration = {
+            "type": "local",
+        }
+
+        if not credentials:
+            credentials = self.get_credentials()
+
+        return StorageFactory.get_storage(
+            storage_scheme="file",
+            provider=self,
+            credentials=credentials,
+            configuration=external_configuration,
+        )
+
+    def on_create(self, dataset: "Dataset") -> None:
+        """Hook to perform provider-specific actions when creating a dataset."""
+        storage = self.get_storage(credentials=None)
+
+        # NOTE: The underlying rclone tool cannot tell if a directory within a External bucket exists or not
+        if not storage.exists(self.uri):
+            raise errors.ParameterError(f"External path '{self.path}' doesn't exists.")
+
+        project_context.repository.add_ignored_pattern(pattern=str(dataset.get_datadir()))
+
+
+class ExternalCredentials(ProviderCredentials):
+    """External-specific credentials."""
+
+    def __init__(self, provider: ExternalProvider):
+        super().__init__(provider=provider)
+
+    @staticmethod
+    def get_credentials_names() -> Tuple[str, ...]:
+        """Return a tuple of the required credentials for a provider."""
+        return tuple()
+
+    @property
+    def provider(self) -> ExternalProvider:
+        """Return the associated provider instance."""
+        return cast(ExternalProvider, self._provider)
 
+    def get_credentials_section_name(self) -> str:
+        """Get section name for storing credentials.
 
-class RCloneStorage(IStorage):
-    """External storage implementation that uses RClone."""
-
-    def download(self, uri: str, destination: Union[Path, str]) -> None:
-        """Download data from ``uri`` to ``destination``."""
-        self.run_command_with_uri("copyto", uri, destination)
-
-    def exists(self, uri: str) -> bool:
-        """Checks if a remote storage URI exists."""
-        try:
-            self.run_command_with_uri("lsf", uri=uri, max_depth=1)
-        except errors.StorageObjectNotFound:
-            return False
-        else:
-            return True
-
-    def get_hashes(self, uri: str, hash_type: str = "md5") -> List[FileHash]:
-        """Download hashes with rclone and parse them.
-
-        Returns a tuple containing a list of parsed hashes.
-
-        Arguments:
-            uri(str): Provider uri.
-            hash_type(str): Type of hash to get from rclone (Default value = `md5`).
-
-        Example:
-            hashes_raw json::
-
-                [
-                    {
-                        "Path":"resources/hg19.window.masker.bed.gz.tbi","Name":"hg19.window.masker.bed.gz.tbi",
-                        "Size":578288,"MimeType":"application/x-gzip","ModTime":"2022-02-07T18:45:52.000000000Z",
-                        "IsDir":false,"Hashes":{"md5":"e93ac5364e7799bbd866628d66c7b773"},"Tier":"STANDARD"
-                    }
-                ]
+        NOTE: This methods should be overridden by subclasses to allow multiple credentials per providers if needed.
         """
-        hashes_raw = self.run_command_with_uri("lsjson", uri, hash=True, R=True, files_only=True)
-        # TODO: Handle JSON load errors
-        hashes = json.loads(hashes_raw)
-        if not hashes:
-            raise errors.ParameterError(f"Cannot find URI: {uri}")
-
-        output = []
-        for hash in hashes:
-            hash_content = hash.get("Hashes", {}).get(hash_type)
-            output.append(
-                FileHash(
-                    base_uri=uri,
-                    path=hash["Path"],
-                    hash=hash_content,
-                    hash_type=hash_type if hash_content else None,
-                    modified_datetime=hash.get("ModTime"),
-                )
-            )
-        return output
-
-    def mount(self, path: Union[Path, str]) -> None:
-        """Mount the provider's URI to the given path."""
-        self.run_command_with_uri("mount", self.provider.uri, str(path), daemon=True, read_only=True, no_modtime=True)
-
-    def get_configurations(self) -> Dict[str, str]:
-        """Get required configurations for rclone to access the storage."""
-        configurations = {}
-        for name, value in self.credentials.items():
-            if value is not NO_VALUE:
-                name = get_rclone_env_var_name(self.storage_scheme, name)
-                configurations[name] = value
-
-        for name, value in self._provider_configuration.items():
-            name = get_rclone_env_var_name(self.storage_scheme, name)
-            configurations[name] = value
-
-        return configurations
-
-    def run_command_with_uri(self, command: str, uri: str, *args, **kwargs) -> Any:
-        """Run a RClone command by converting a given URI."""
-        uri = self._provider_uri_convertor(uri)
-
-        return self.run_command(command, uri, *args, **kwargs)
-
-    def run_command(self, command: str, *args, **kwargs) -> Any:
-        """Run a RClone command with storage-specific configuration."""
-        return run_rclone_command(command, *args, **kwargs, env=self.get_configurations())
-
-    def upload(self, source: Union[Path, str], uri: str) -> None:
-        """Upload data from ``source`` to ``uri``."""
-        uri = self._provider_uri_convertor(uri)
-
-        self.run_command("copyto", source, uri)
-
-
-def run_rclone_command(command: str, *args: Any, env=None, **kwargs) -> str:
-    """Execute an RClone command."""
-    os_env = os.environ.copy()
-    if env:
-        os_env.update(env)
-
-    full_command = ("rclone", command, *transform_kwargs(**kwargs), *transform_args(*args))
-    try:
-        result = subprocess.run(full_command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=os_env)
-    except FileNotFoundError:
-        raise errors.RCloneException("RClone is not installed. See https://rclone.org/install/")
-
-    # See https://rclone.org/docs/#list-of-exit-codes for rclone exit codes
-    if result.returncode == 0:
-        return result.stdout
-
-    all_outputs = result.stdout + result.stderr
-    if result.returncode in (3, 4):
-        raise errors.StorageObjectNotFound(all_outputs)
-    elif (
-        "AccessDenied" in all_outputs
-        or "no authentication method configured" in all_outputs
-        or "Need account+key" in all_outputs
-    ):
-        raise errors.AuthenticationError(f"Authentication failed when accessing the cloud storage: {all_outputs}")
-    else:
-        raise errors.RCloneException(f"Remote storage operation failed: {all_outputs}")
-
-
-def transform_args(*args) -> List[str]:
-    """Transforms args to command line args."""
-    return [str(a) for a in args]
-
-
-def transform_kwargs(**kwargs) -> List[str]:
-    """Transforms kwargs to command line args."""
-
-    def transform_kwarg(key: str, value: Any) -> List[str]:
-        if value in (False, None):
-            return []
-        else:
-            name = f"-{key}" if len(key) == 1 else f"--{key.replace('_', '-')}"
-            return [name] if value is True else [name, f"{value}"]
-
-    all_args = []
-    for key, value in kwargs.items():
-        args = transform_kwarg(key, value)
-        all_args.extend(args)
-
-    return all_args
-
-
-def get_rclone_env_var_name(provider_name, name) -> str:
-    """Get name of an RClone env var config."""
-    # See https://rclone.org/docs/#config-file
-    name = name.replace(" ", "_").replace("-", "_")
-    return f"RCLONE_CONFIG_{provider_name}_{name}".upper()
+        return self.provider.uri
+
+
+def get_uri_absolute_path(uri: str) -> str:
+    """Return absolute path to the external directory without resolving symlinks.
+
+    Support formats are ``file://<path>``, file:<path> or just ``<path>``.
+
+    Args:
+        uri(str): URI to get path from.
+
+    Returns:
+        str: Expanded/non-expanded URI's absolute path.
+    """
+    return get_absolute_path(urllib.parse.urlparse(uri).path, expand=True)
```

### Comparing `renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md` & `renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/config.yml` & `renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md` & `renku-2.4.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/.github/dependabot.yml` & `renku-2.4.0rc1/renku/templates/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/.gitignore` & `renku-2.4.0rc1/renku/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal/.gitignore` & `renku-2.4.0rc1/renku/templates/R-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal/.renkulfsignore` & `renku-2.4.0rc1/renku/templates/R-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal/Dockerfile` & `renku-2.4.0rc1/renku/templates/R-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal/README.md` & `renku-2.4.0rc1/renku/templates/R-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal/workflows/my-workflow.yaml` & `renku-2.4.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/R-minimal.png` & `renku-2.4.0rc1/renku/templates/R-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/README.md` & `renku-2.4.0rc1/renku/templates/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioc-minimal/.gitignore` & `renku-2.4.0rc1/renku/templates/bioc-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioc-minimal/.renkulfsignore` & `renku-2.4.0rc1/renku/templates/bioc-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioc-minimal/Dockerfile` & `renku-2.4.0rc1/renku/templates/bioc-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioc-minimal/README.md` & `renku-2.4.0rc1/renku/templates/bioc-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioc-minimal/workflows/my-workflow.yaml` & `renku-2.4.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/bioconductor.png` & `renku-2.4.0rc1/renku/templates/bioconductor.png`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julia-minimal/.gitignore` & `renku-2.4.0rc1/renku/templates/julia-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julia-minimal/.renkulfsignore` & `renku-2.4.0rc1/renku/templates/julia-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julia-minimal/Dockerfile` & `renku-2.4.0rc1/renku/templates/julia-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julia-minimal/README.md` & `renku-2.4.0rc1/renku/templates/julia-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julia-minimal/workflows/my-workflow.yaml` & `renku-2.4.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/julialang.png` & `renku-2.4.0rc1/renku/templates/julialang.png`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/manifest.yaml` & `renku-2.4.0rc1/renku/templates/manifest.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/minimal/.renkulfsignore` & `renku-2.4.0rc1/renku/templates/minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/minimal/Dockerfile` & `renku-2.4.0rc1/renku/templates/minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/minimal/workflows/my-workflow.yaml` & `renku-2.4.0rc1/renku/templates/minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal/.gitignore` & `renku-2.4.0rc1/renku/templates/python-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal/.renkulfsignore` & `renku-2.4.0rc1/renku/templates/python-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal/Dockerfile` & `renku-2.4.0rc1/renku/templates/python-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal/README.md` & `renku-2.4.0rc1/renku/templates/python-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal/workflows/my-workflow.yaml` & `renku-2.4.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/templates/python-minimal.png` & `renku-2.4.0rc1/renku/templates/python-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/ui/__init__.py` & `renku-2.4.0rc1/renku/ui/service/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022- Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku ui modules."""
+"""Renku service."""
```

### Comparing `renku-2.3.2/renku/ui/api/__init__.py` & `renku-2.4.0rc1/renku/ui/api/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/graph/__init__.py` & `renku-2.4.0rc1/renku/data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku Graph API."""
+"""Data files for the Renku package."""
```

### Comparing `renku-2.3.2/renku/ui/api/graph/rdf.py` & `renku-2.4.0rc1/renku/ui/api/graph/rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/models/__init__.py` & `renku-2.4.0rc1/renku/ui/service/jobs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku API Models."""
+"""Renku service jobs."""
```

### Comparing `renku-2.3.2/renku/ui/api/models/activity.py` & `renku-2.4.0rc1/renku/ui/api/models/activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/models/dataset.py` & `renku-2.4.0rc1/renku/ui/api/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/models/parameter.py` & `renku-2.4.0rc1/renku/ui/api/models/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/models/plan.py` & `renku-2.4.0rc1/renku/ui/api/models/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/models/project.py` & `renku-2.4.0rc1/renku/ui/api/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/api/util.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_list_projects.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,60 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-r"""Renku API utilities."""
+"""Renku service cache list cached projects controller."""
+import itertools
 
-from functools import wraps
-from typing import TYPE_CHECKING, Optional
-
-from renku.domain_model.project_context import project_context
-
-if TYPE_CHECKING:
-    from renku.infrastructure.gateway.activity_gateway import ActivityGateway
-    from renku.infrastructure.gateway.plan_gateway import PlanGateway
-
-
-def ensure_project_context(fn):
-    """Check existence of a project context.
-
-    Args:
-        fn: The function to wrap.
-
-    Returns:
-        The function with the current project injected.
-    """
-
-    def get_current_project():
-        """Return current project context if any or a new project object.
-
-        Returns:
-            The current project context or None.
-        """
-        from renku.ui.api import Project
-
-        return Project._project_contexts.top if Project._project_contexts.top else None
-
-    @wraps(fn)
-    def wrapper(*args, **kwargs):
-        from renku.ui.api import Project
-
-        project = get_current_project() or Project()
-        return fn(*args, **kwargs, project=project)
-
-    return wrapper
-
-
-@ensure_project_context
-def get_activity_gateway(project) -> Optional["ActivityGateway"]:
-    """Return an instance of ActivityGateway when inside a Renku project."""
-    from renku.infrastructure.gateway.activity_gateway import ActivityGateway
-
-    try:
-        _ = project_context.repository
-    except ValueError:
-        return None
-
-    return ActivityGateway()
-
-
-@ensure_project_context
-def get_plan_gateway(project) -> Optional["PlanGateway"]:
-    """Return an instance of PlanGateway when inside a Renku project."""
-    from renku.infrastructure.gateway.plan_gateway import PlanGateway
-
-    try:
-        _ = project_context.repository
-    except ValueError:
-        return None
-
-    return PlanGateway()
+from renku.ui.service.controllers.api.abstract import ServiceCtrl
+from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
+from renku.ui.service.serializers.cache import ProjectListResponseRPC
+from renku.ui.service.views import result_response
+
+
+class ListProjectsCtrl(ServiceCtrl, RenkuOperationMixin):
+    """Controller for listing cached projects endpoint."""
+
+    RESPONSE_SERIALIZER = ProjectListResponseRPC()
+
+    def __init__(self, cache, user_data):
+        """Construct controller."""
+        self.ctx = {}
+        super().__init__(cache, user_data, {})
+
+    @property
+    def context(self):
+        """Controller operation context."""
+        return self.ctx
+
+    def list_projects(self):
+        """List locally cache projects."""
+        projects = [project for project in self.cache.get_projects(self.user) if project.abs_path.exists()]
+
+        result = {
+            "projects": [
+                max(g, key=lambda p: p.created_at) for _, g in itertools.groupby(projects, lambda p: p.git_url)
+            ]
+        }
+
+        return result
+
+    def renku_op(self):
+        """Renku operation for the controller."""
+        # NOTE: We leave it empty since it does not execute renku operation.
+        pass
+
+    def to_response(self):
+        """Execute controller flow and serialize to service response."""
+        return result_response(ListProjectsCtrl.RESPONSE_SERIALIZER, self.list_projects())
```

### Comparing `renku-2.3.2/renku/ui/cli/__init__.py` & `renku-2.4.0rc1/renku/ui/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -85,15 +84,15 @@
 
 import click
 import yaml
 from click_plugins import with_plugins
 
 from renku.command.options import option_external_storage_requested
 from renku.command.util import WARNING
-from renku.command.version import check_version, print_version
+from renku.command.version import print_version
 from renku.core import errors
 from renku.core.constant import DATABASE_PATH
 from renku.core.util.git import get_git_path
 from renku.domain_model.project_context import project_context
 from renku.ui.cli.clone import clone
 from renku.ui.cli.config import config
 from renku.ui.cli.dataset import dataset
@@ -214,23 +213,14 @@
     is_eager=True,
     help=print_global_config_path.__doc__,
 )
 @click.option(
     "--path", show_default=True, metavar="<path>", default=get_git_path, help="Location of a Renku repository."
 )
 @option_external_storage_requested
-@click.option(
-    "--disable-version-check",
-    envvar="RENKU_DISABLE_VERSION_CHECK",
-    is_flag=True,
-    default=False,
-    callback=check_version,
-    expose_value=False,
-    help="Do not periodically check PyPI for a new version of renku.",
-)
 @click.pass_context
 def cli(ctx, path, external_storage_requested):
     """Check common Renku commands used in various situations."""
     from renku.domain_model.project_context import project_context
 
     path = Path(path)
```

### Comparing `renku-2.3.2/renku/ui/cli/__main__.py` & `renku-2.4.0rc1/renku/ui/cli/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/clone.py` & `renku-2.4.0rc1/renku/ui/cli/clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/config.py` & `renku-2.4.0rc1/renku/ui/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/dataset.py` & `renku-2.4.0rc1/renku/ui/cli/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -134,14 +133,22 @@
    :description: Add data from <url> to a dataset. <url> can be a local
                  file path, an http(s) address or a Git git+http or git+ssh repository.
    :target: rp,ui
 
 This will copy the contents of ``data-url`` to the dataset and add it
 to the dataset metadata.
 
+.. note::
+
+   If the URL refers to a local directory, data is added differently depending
+   on if there is a trailing slash (``/``) or not. If the URL ends in a slash,
+   files inside the directory are added to the target directory. If it does
+   not end in a slash, then the directory itself will be added inside the
+   target directory.
+
 You can create a dataset when you add data to it for the first time by passing
 ``--create`` flag to add command:
 
 .. code-block:: console
 
     $ renku dataset add --create new-dataset http://data-url
 
@@ -206,27 +213,14 @@
                  location the data is copied to.
    :target: rp
 
 To add a specific version of files, use ``--ref`` option for selecting a
 branch, commit, or tag. The value passed to this option must be a valid
 reference in the remote Git repository.
 
-Adding external data to the dataset:
-
-Sometimes you might want to add data to your dataset without copying the
-actual files to your repository. This is useful for example when external data
-is too large to store locally. The external data must exist (i.e. be mounted)
-on your filesystem. Renku creates a symbolic to your data and you can use this
-symbolic link in renku commands as a normal file. To add an external file pass
-``--external`` or ``-e`` when adding local data to a dataset:
-
-.. code-block:: console
-
-    $ renku dataset add my-dataset -e /path/to/external/file
-
 Updating a dataset:
 
 After adding files from a remote Git repository or importing a dataset from a
 provider like Dataverse or Zenodo, you can check for updates in those files by
 using ``renku dataset update --all`` command. For Git repositories, this command
 checks all remote files and copies over new content if there is any. It does
 not delete files from the local dataset if they are deleted from the remote Git
@@ -257,22 +251,14 @@
 .. code-block:: console
 
     $ renku dataset update -I '*.csv' my-dataset
 
 Note that putting glob patterns in quotes is needed to tell Unix shell not
 to expand them.
 
-External data are also updated automatically. Since they require a checksum
-calculation which can take a long time when data is large, you can exclude them
-from an update by passing ``--no-external`` flag to the update command:
-
-.. code-block:: console
-
-    $ renku dataset update --all --no-external
-
 You can use ``--dry-run`` flag to get a preview of what files/datasets will be
 updated by an update operation.
 
 Tagging a dataset:
 
 A dataset can be tagged with an arbitrary tag to refer to the dataset at that
 point in time. A tag can be added like this:
@@ -528,15 +514,15 @@
 import click
 from lazy_object_proxy import Proxy
 
 import renku.ui.cli.utils.color as color
 from renku.command.format.dataset_files import DATASET_FILES_COLUMNS, DATASET_FILES_FORMATS
 from renku.command.format.dataset_tags import DATASET_TAGS_FORMATS
 from renku.command.format.datasets import DATASETS_COLUMNS, DATASETS_FORMATS
-from renku.core.util.util import NO_VALUE, NoValueType
+from renku.domain_model.constant import NO_VALUE, NoValueType
 
 
 def _complete_datasets(ctx, param, incomplete):
     from renku.command.dataset import search_datasets_command
 
     try:
         result = search_datasets_command().build().execute(name=incomplete)
@@ -554,15 +540,15 @@
 @click.option(
     "--format", type=click.Choice(list(DATASETS_FORMATS.keys())), default="tabular", help="Choose an output format."
 )
 @click.option(
     "-c",
     "--columns",
     type=click.STRING,
-    default="id,name,title,version,datadir",
+    default="id,name,title,version,datadir,storage",
     metavar="<columns>",
     help="Comma-separated list of column to display: {}.".format(", ".join(DATASETS_COLUMNS.keys())),
     show_default=True,
 )
 def list_dataset(format, columns):
     """List datasets."""
     from renku.command.dataset import list_datasets_command
@@ -743,19 +729,17 @@
             custom_metadata=custom_metadata,
             custom_metadata_source=metadata_source,
         )
     ).output
 
     if not updated:
         click.echo(
-            (
-                "Nothing to update. "
-                "Check available fields with `renku dataset edit --help`\n\n"
-                'Hint: `renku dataset edit --title "new title"`'
-            )
+            "Nothing to update. "
+            "Check available fields with `renku dataset edit --help`\n\n"
+            'Hint: `renku dataset edit --title "new title"`'
         )
     else:
         click.echo("Successfully updated: {}.".format(", ".join(updated.keys())))
         if no_email_warnings:
             click.echo(
                 ClickCallback.WARNING + "No email or wrong format for: " + ", ".join(cast(List[str], no_email_warnings))
             )
@@ -812,14 +796,15 @@
 @dataset.command()
 @click.argument("name", shell_complete=_complete_datasets)
 @click.argument("urls", type=click.Path(), nargs=-1)
 @click.option("-f", "--force", is_flag=True, help="Allow adding otherwise ignored files.")
 @click.option("-o", "--overwrite", is_flag=True, help="Overwrite existing files.")
 @click.option("-c", "--create", is_flag=True, help="Create dataset if it does not exist.")
 @click.option("-d", "--destination", default="", help="Destination directory within the dataset path")
+@click.option("--storage", default=None, type=click.STRING, help="URI of the cloud storage backend.")
 @click.option(
     "--datadir",
     default=None,
     type=click.Path(),
     help="Dataset's data directory (defaults to 'data/<dataset name>').",
 )
 @add_provider_options()
@@ -867,15 +852,15 @@
     default="tabular",
     help="Choose an output format.",
 )
 @click.option(
     "-c",
     "--columns",
     type=click.STRING,
-    default="dataset_name,added,size,path,lfs",
+    default="dataset_name,path,size,added,lfs",
     metavar="<columns>",
     help="Comma-separated list of column to display: {}.".format(", ".join(DATASET_FILES_COLUMNS.keys())),
     show_default=True,
 )
 def ls_files(names, tag, creators, include, exclude, format, columns):
     """List files in dataset."""
     from renku.command.dataset import list_files_command
@@ -902,19 +887,17 @@
     """Remove matching files from a dataset."""
     from renku.command.dataset import file_unlink_command
     from renku.core import errors
     from renku.ui.cli.utils.callback import ClickCallback
 
     if not include and not exclude:
         raise errors.ParameterError(
-            (
-                "include or exclude filters not found.\n"
-                "Check available filters with 'renku dataset unlink --help'\n"
-                "Hint: 'renku dataset unlink my-dataset -I path'"
-            )
+            "include or exclude filters not found.\n"
+            "Check available filters with 'renku dataset unlink --help'\n"
+            "Hint: 'renku dataset unlink my-dataset -I path'"
         )
 
     communicator = ClickCallback()
     file_unlink_command().with_communicator(communicator).build().execute(
         name=name, include=include, exclude=exclude, yes=yes
     )
     click.secho("OK", fg=color.GREEN)
@@ -1121,15 +1104,14 @@
         .execute(
             names=list(names),
             creators=creators,
             include=include,
             exclude=exclude,
             ref=ref,
             delete=delete,
-            no_external=no_external,
             no_local=no_local,
             no_remote=no_remote,
             check_data_directory=check_data_directory,
             update_all=update_all,
             dry_run=dry_run,
             plain=plain,
         )
@@ -1190,46 +1172,46 @@
     "--location",
     default=None,
     type=click.Path(exists=False, file_okay=False, writable=True),
     help="A directory to copy data to, instead of the dataset's data directory.",
 )
 def pull(name, location):
     """Pull data from a cloud storage."""
-    from renku.command.dataset import pull_external_data_command
+    from renku.command.dataset import pull_cloud_storage_command
     from renku.ui.cli.utils.callback import ClickCallback
 
     communicator = ClickCallback()
-    pull_external_data_command().with_communicator(communicator).build().execute(name=name, location=location)
+    pull_cloud_storage_command().with_communicator(communicator).build().execute(name=name, location=location)
 
 
 @dataset.command(hidden=True)
 @click.argument("name", shell_complete=_complete_datasets)
 @click.option(
     "-e",
     "--existing",
     default=None,
     type=click.Path(exists=True, file_okay=False),
     help="Use an existing mount point instead of mounting the remote storage.",
 )
-@click.option("-u", "--unmount", is_flag=True, help="Unmount dataset's external storage.")
+@click.option("-u", "--unmount", is_flag=True, help="Unmount dataset's backend storage.")
 @click.option("-y", "--yes", is_flag=True, help="No prompt when removing non-empty dataset's data directory.")
 def mount(name, existing, unmount, yes):
     """Mount a cloud storage in the dataset's data directory."""
-    from renku.command.dataset import mount_external_storage_command
+    from renku.command.dataset import mount_cloud_storage_command
     from renku.ui.cli.utils.callback import ClickCallback
 
-    command = mount_external_storage_command(unmount=unmount).with_communicator(ClickCallback()).build()
+    command = mount_cloud_storage_command(unmount=unmount).with_communicator(ClickCallback()).build()
 
     if unmount:
         command.execute(name=name)
     else:
         command.execute(name=name, existing=existing, yes=yes)
 
 
 @dataset.command(hidden=True)
 @click.argument("name", shell_complete=_complete_datasets)
 def unmount(name):
-    """Unmount an external storage in the dataset's data directory."""
-    from renku.command.dataset import unmount_external_storage_command
+    """Unmount a backend storage in the dataset's data directory."""
+    from renku.command.dataset import unmount_cloud_storage_command
     from renku.ui.cli.utils.callback import ClickCallback
 
-    unmount_external_storage_command().with_communicator(ClickCallback()).build().execute(name=name)
+    unmount_cloud_storage_command().with_communicator(ClickCallback()).build().execute(name=name)
```

### Comparing `renku-2.3.2/renku/ui/cli/doctor.py` & `renku-2.4.0rc1/renku/ui/cli/doctor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/env.py` & `renku-2.4.0rc1/renku/ui/cli/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/exception_handler.py` & `renku-2.4.0rc1/renku/ui/cli/exception_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -150,15 +149,15 @@
                 from renku.core.util.git import get_git_repository
 
                 user = get_git_repository().get_user()
 
                 scope.user = {"name": user.name, "email": user.email}
 
             event_id = capture_exception()
-            click.echo(_BUG + "Recorded in Sentry with ID: {0}\n".format(event_id), err=True)
+            click.echo(_BUG + f"Recorded in Sentry with ID: {event_id}\n", err=True)
             raise
 
     def _handle_github(self):
         """Handle exception and submit it as GitHub issue."""
         value = click.prompt(
             _BUG
             + click.style('1. Open an issue by typing "open";\n', fg=color.GREEN)
```

### Comparing `renku-2.3.2/renku/ui/cli/gc.py` & `renku-2.4.0rc1/renku/ui/cli/gc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/githooks.py` & `renku-2.4.0rc1/renku/ui/cli/githooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/graph.py` & `renku-2.4.0rc1/renku/ui/cli/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -58,17 +57,18 @@
 
             [... many more lines ...]
 
         }
     ]
 
 If you want the Knowledge Graph data for the whole project, you can use
-``renku graph export --full``. Alternatively, you can get data for a single
-commit by using ``renku graph export --revision <git commit sha>`` or by
-specifying a range of commits like ``renku graph export --revision sha1..sha2``.
+``renku graph export --full`` (``--full`` is the default). Alternatively,
+you can get data for a single commit by using ``renku graph export
+--revision <git commit sha>`` or by specifying a range of commits like
+``renku graph export --revision sha1..sha2``.
 
 ``renku graph export`` currently supports various formats for export, such as
 ``json-ld``, ``rdf``, ``nt`` (for triples) and ``dot`` (for GraphViz graphs),
 which can be specified using the ``--format`` option. For instance,
 
 .. code-block:: console
 
@@ -108,18 +108,18 @@
     type=CaseInsensitiveChoice(list(GRAPH_FORMATS.keys())),
     default="json-ld",
     help="Choose an output format.",
 )
 @click.option(
     "--revision",
     type=str,
-    default="HEAD",
+    default=None,
     help="Limit graph to changes done in revision (or range of revisions like 'A..B').",
 )
-@click.option("-f", "--full", is_flag=True, help="Generate full graph for project. Overrides --revision.")
+@click.option("-f", "--full", is_flag=True, help="Generate full graph for project (default). Overrides --revision.")
 @click.option("--strict", is_flag=True, default=False, help="Validate triples before output.")
 @click.option(
     "--no-indent", is_flag=True, default=False, help="Format without indentation/pretty-printing (only for JSON-LD)."
 )
 def export(format, revision, full, strict, no_indent):
     r"""Export Renku graph metadata for project."""
     from renku.command.graph import export_graph_command
```

### Comparing `renku-2.3.2/renku/ui/cli/init.py` & `renku-2.4.0rc1/renku/ui/cli/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -64,20 +63,20 @@
     $ renku init --template-ref master --template-source \
     https://github.com/SwissDataScienceCenter/renku-project-template
 
     Fetching template from
     https://github.com/SwissDataScienceCenter/renku-project-template@master
     ... OK
 
-    INDEX ID             DESCRIPTION                PARAMETERS
+    NUMBER ID             DESCRIPTION                PARAMETERS
     ----- -------------- -------------------------- ----------------------
     1     python-minimal Basic Python Project:[...] description: proj[...]
     2     R-minimal      Basic R Project: The [...] description: proj[...]
 
-    Please choose a template by typing the index:
+    Please choose a template by typing the number:
 
 Provide parameters
 ~~~~~~~~~~~~~~~~~~
 
 Some templates require parameters to properly initialize a new project. You
 can check them by listing the templates ``renku template ls --verbose``.
 
@@ -129,25 +128,25 @@
 ``README.rst`` will never be overwritten. ``.gitignore`` will be appended to
 to prevent files accidentally getting committed. Files that are not present
 in the template will be left untouched by the command.
 
 .. code-block:: console
 
     $ echo "# Example\nThis is a README." > README.md
-    $ echo "FROM python:3.7-alpine" > Dockerfile
+    $ echo "FROM python:3.10-alpine" > Dockerfile
     $ renku init
 
-    INDEX  ID              PARAMETERS
+    NUMBER  ID              PARAMETERS
     -------  --------------  ------------
         1  python-minimal  description
         2  R-minimal       description
         3  bioc-minimal    description
         4  julia-minimal   description
         5  minimal
-    Please choose a template by typing the index: 1
+    Please choose a template by typing the number: 1
     The template requires a value for "description": Test Project
     Initializing Git repository...
     Warning: The following files exist in the directory and will be overwritten:
             Dockerfile
     Proceed? [y/N]: y
     Initializing new Renku repository...
     Initializing file .dockerignore ...
```

### Comparing `renku-2.3.2/renku/ui/cli/log.py` & `renku-2.4.0rc1/renku/ui/cli/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/login.py` & `renku-2.4.0rc1/renku/ui/cli/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/mergetool.py` & `renku-2.4.0rc1/renku/ui/cli/mergetool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/migrate.py` & `renku-2.4.0rc1/renku/ui/cli/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/move.py` & `renku-2.4.0rc1/renku/ui/cli/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/project.py` & `renku-2.4.0rc1/renku/ui/cli/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -34,15 +33,15 @@
 
 import json
 from pathlib import Path
 
 import click
 
 import renku.ui.cli.utils.color as color
-from renku.core.util.util import NO_VALUE
+from renku.domain_model.constant import NO_VALUE
 from renku.ui.cli.utils.callback import ClickCallback
 
 
 @click.group()
 def project():
     """Project commands."""
```

### Comparing `renku-2.3.2/renku/ui/cli/remove.py` & `renku-2.4.0rc1/renku/ui/cli/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/rerun.py` & `renku-2.4.0rc1/renku/ui/cli/rerun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/rollback.py` & `renku-2.4.0rc1/renku/ui/cli/rollback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/run.py` & `renku-2.4.0rc1/renku/ui/cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -226,14 +225,15 @@
 Sometimes the list of inputs and outputs are not known before execution of the
 program. For example, a program might accept a date range as input and access
 all files within that range during its execution.
 
 To address this issue, the program can dump a mapping of input and output files
 that it is accessing in ``inputs.yml`` and ``outputs.yml``. This YAML file
 should be of the format
+
 .. code-block:: YAML
 
    name1: path1
    name2: path2
 
 where name is the user-defined name of the input/output and path is the path.
 When the program is finished, Renku will look for existence of these two files
```

### Comparing `renku-2.3.2/renku/ui/cli/save.py` & `renku-2.4.0rc1/renku/ui/cli/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/service.py` & `renku-2.4.0rc1/renku/ui/cli/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2021 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/session.py` & `renku-2.4.0rc1/renku/ui/cli/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -51,16 +50,18 @@
 and check their sessions locally without going to a Renku deployment and launching
 a session there, or in the case where they simply have no access to a Renku deployment.
 
 .. code-block:: console
 
     $ renku session start -p docker
 
-The command first looks for a local image to use. If a local image isn't found, it searches the remote Renku deployment
-(if any) and pulls the image if it exists. Finally, it prompts the user to build the image locally if no image is found.
+The command first looks for a local image to use. If a local image isn't found, it
+searches the remote Renku deployment (if any) and pulls the image if it exists.
+Finally, it prompts the user to build the image locally if no image is found. You
+can force the image to always be built by using the ``--force-build`` flag.
 
 Renkulab provider
 ~~~~~~~~~~~~~~~~~
 
 The ``renkulab`` provider will launch a regular interactive session
 in the Renku deployment that hosts the current project. If the project has not
 been uploaded/created in a Renku deployment then this provider will not be able
```

### Comparing `renku-2.3.2/renku/ui/cli/status.py` & `renku-2.4.0rc1/renku/ui/cli/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/storage.py` & `renku-2.4.0rc1/renku/ui/cli/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/template.py` & `renku-2.4.0rc1/renku/ui/cli/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -331,14 +330,15 @@
                 click.echo(print_name("    Type: ") + print_value(p.type))
             if p.possible_values:
                 click.echo(print_name("    Possible values: ") + print_value(p.possible_values))
             if p.default is not None:
                 click.echo(print_name("    Default value: ") + print_value(p.default))
 
     click.echo(print_name("Id: ") + print_value(template.id))
+    click.echo(print_name("Id aliases: ") + print_value(template.aliases))
     click.echo(print_name("Name: ") + print_value(template.name))
     click.echo(print_name("Source: ") + print_value(template.source))
     click.echo(print_name("Reference: ") + print_value(to_string(template.reference)))
     click.echo(print_name("Version: ") + print_value(template.version))
     click.echo(print_name("Description: ") + print_value(template.description))
     click.echo(print_name("Parameters:"))
     print_template_parameters()
@@ -366,12 +366,13 @@
     """Print detailed template info."""
     from renku.core.util.util import to_string
 
     print_name = functools.partial(click.style, bold=True, fg="magenta")
     print_value = functools.partial(click.style, bold=True)
 
     click.echo(print_name("Id: ") + print_value(changes.id))
+    click.echo(print_name("Old Id: ") + print_value(changes.old_id))
     click.echo(print_name("Source: ") + print_value(changes.source))
     click.echo(print_name("New reference: ") + print_value(to_string(changes.reference)))
     click.echo(print_name("New version: ") + print_value(to_string(changes.version)))
     click.echo(print_name("File changes:"))
     click.echo("  " + "\n  ".join(changes.file_changes))
```

### Comparing `renku-2.3.2/renku/ui/cli/update.py` & `renku-2.4.0rc1/renku/ui/cli/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -91,16 +90,16 @@
 command is run. If this is the case then you can pass the ``--skip-metadata-update``
 flag to ``renku update``.
 
 .. cheatsheet::
    :group: Running
    :command: $ renku update [--all] [<path>...]
    :description: Update outdated output files created by renku run. With
-                 <path>'s: Only recreate these files. With --all: Update
-                 all outdated output files.
+                 <path>'s: Only recreate these files. With --all (default):
+                 Update all outdated output files.
    :target: rp
 
 Pre-update checks
 ~~~~~~~~~~~~~~~~~
 
 In the next example, files ``A`` or ``B`` are modified, hence the majority
 of dependent files must be recreated.
@@ -156,21 +155,22 @@
 downstream dependencies that aren't deleted.
 
 """
 
 import click
 from lazy_object_proxy import Proxy
 
+from renku.command.util import WARNING
 from renku.core import errors
 from renku.ui.cli.utils.callback import ClickCallback
 from renku.ui.cli.utils.plugins import available_workflow_providers
 
 
 @click.command()
-@click.option("--all", "-a", "update_all", is_flag=True, default=False, help="Update all outdated files.")
+@click.option("--all", "-a", "update_all", is_flag=True, default=False, help="Update all outdated files (default).")
 @click.option("--dry-run", "-n", is_flag=True, default=False, help="Show a preview of plans that will be executed.")
 @click.argument("paths", type=click.Path(exists=True, dir_okay=True), nargs=-1)
 @click.option(
     "provider",
     "-p",
     "--provider",
     default="toil",
@@ -186,14 +186,18 @@
 def update(update_all, dry_run, paths, provider, config, ignore_deleted, skip_metadata_update):
     """Update existing files by rerunning their outdated workflow."""
     from renku.command.format.activity import tabulate_activities
     from renku.command.update import update_command
 
     communicator = ClickCallback()
 
+    if not paths and not update_all and not dry_run:
+        message = f"{WARNING}Updating all outputs could trigger expensive computations. Are you sure?"
+        communicator.confirm(message, default=True, abort=True)
+
     try:
         result = (
             update_command(skip_metadata_update=skip_metadata_update)
             .with_communicator(communicator)
             .build()
             .execute(
                 update_all=update_all,
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/__init__.py` & `renku-2.4.0rc1/renku/ui/cli/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/callback.py` & `renku-2.4.0rc1/renku/ui/cli/utils/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -71,15 +70,15 @@
     def confirm(self, msg, abort=False, warning=False, default=False):
         """Get confirmation for an action."""
         return False
 
     def start_progress(self, name, total, **kwargs):
         """Start a new tqdm progressbar."""
         if name in self._progress_bars:
-            raise ValueError("Name {} is already a registered progressbar.".format(name))
+            raise ValueError(f"Name {name} is already a registered progressbar.")
 
         if "type" not in kwargs:
             kwargs["type"] = "download"
 
         if kwargs["type"] not in self._progress_types:
             self._progress_bars[name] = None
         elif kwargs["type"] == "download":
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/click.py` & `renku-2.4.0rc1/renku/ui/cli/utils/click.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -31,15 +30,15 @@
     Based on https://github.com/pallets/click/issues/569.
     """
 
     def convert(self, value, param, ctx):
         """Convert value to its choice value."""
         if value is None:
             return None
-        return super(CaseInsensitiveChoice, self).convert(value.lower(), param, ctx)
+        return super().convert(value.lower(), param, ctx)
 
 
 class MutuallyExclusiveOption(click.Option):
     """Custom option class to allow specifying mutually exclusive options in click commands."""
 
     def __init__(self, *args, **kwargs):
         mutually_exclusive = sorted(kwargs.pop("mutually_exclusive", []))
@@ -47,33 +46,32 @@
         self.mutually_exclusive_names = []
 
         for mutex in mutually_exclusive:
             if type(mutex) == tuple:
                 self.mutually_exclusive.add(mutex[0])
                 self.mutually_exclusive_names.append(mutex[1])
             else:
-
                 self.mutually_exclusive.add(mutex)
                 self.mutually_exclusive_names.append(mutex)
 
         _help = kwargs.get("help", "")
         if self.mutually_exclusive:
             ex_str = ", ".join(self.mutually_exclusive_names)
             kwargs["help"] = f"{_help} NOTE: This argument is mutually exclusive with arguments: [{ex_str}]."
-        super(MutuallyExclusiveOption, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         """Handles the parse result for the option."""
         if self.mutually_exclusive.intersection(opts) and self.name in opts:
             raise click.UsageError(
                 "Illegal usage: `{}` is mutually exclusive with "
                 "arguments `{}`.".format(self.name, ", ".join(sorted(self.mutually_exclusive_names)))
             )
 
-        return super(MutuallyExclusiveOption, self).handle_parse_result(ctx, opts, args)
+        return super().handle_parse_result(ctx, opts, args)
 
 
 def create_options(providers, parameter_function: str):
     """Create options for a group of providers."""
 
     def wrapper(f):
         from click_option_group import optgroup
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/color.py` & `renku-2.4.0rc1/renku/ui/service/cache/serializers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Terminal Color definitions."""
-
-YELLOW = "yellow"
-MAGENTA = "magenta"
-GREEN = "green"
-RED = "red"
-BLUE = "blue"
+"""Renku service cache serializers."""
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/curses.py` & `renku-2.4.0rc1/renku/ui/cli/utils/curses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/plugins.py` & `renku-2.4.0rc1/renku/ui/cli/utils/plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/utils/terminal.py` & `renku-2.4.0rc1/renku/ui/cli/utils/terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/cli/workflow.py` & `renku-2.4.0rc1/renku/ui/cli/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2018-2022- Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -126,26 +125,52 @@
 
 .. code-block:: console
 
     $ renku workflow execute --provider cwltool --set input-1=file.txt my-run
 
 Parameters can be set using the ``--set`` keyword or by specifying them in a
 values YAML file and passing that using ``--values``. In case of passing a file,
-the YAML should follow the this structure:
+for a composite workflow like:
+
+.. code-block:: console
+
+    $ renku run --name train -- python train.py --lr=0.1 --gamma=0.5 --output=result.csv
+    $ renku run --name eval -- python eval.py --image=graph.png --data=result.csv
+    $ renku workflow compose --map learning_rate=train.lr --map graph=eval.image
+
+the YAML file could look like:
 
 .. code-block:: yaml
 
+    # composite (mapped) parameters
     learning_rate: 0.9
-    dataset_input: dataset.csv
-    chart_output: chart.png
-    my-workflow:
-        lr: 0.8
-        lookup-table: lookup.xml
-        my-other-workflow:
-            language: en
+    graph: overview.png
+    train: # child workflow name
+        # child workflow parameters
+        gamma: 1.0
+
+Which would rerun the two steps but with ``lr`` set to ``0.9``, ``gamma`` set to ``1.0``
+and the output saved under ``overview.png``.
+
+Note that this would be the same as using:
+
+.. code-block:: yaml
+
+    train:
+        lr: 0.9
+        gamma: 1.0
+    eval:
+        image: overview.png
+
+For a regular (non-composite) workflow it is enough to just specify key-value pairs like:
+
+.. code-block:: yaml
+
+    lr: 0.9
+    gamma: 1.0
 
 In addition to being passed on the command line and being available to
 ``renku.ui.api.*`` classes in Python scripts, parameters are also set as
 environment variables when executing the command, in the form of
 ``RENKU_ENV_<parameter name>``.
 
 Provider specific settings can be passed as file using the ``--config`` parameter.
@@ -727,15 +752,15 @@
 from lazy_object_proxy import Proxy
 
 import renku.ui.cli.utils.color as color
 from renku.command.format.workflow import WORKFLOW_COLUMNS, WORKFLOW_FORMATS, WORKFLOW_VISUALIZE_FORMATS
 from renku.command.util import ERROR
 from renku.command.view_model.activity_graph import ACTIVITY_GRAPH_COLUMNS
 from renku.core import errors
-from renku.core.util.util import NO_VALUE
+from renku.domain_model.constant import NO_VALUE
 from renku.ui.cli.utils.callback import ClickCallback
 from renku.ui.cli.utils.plugins import available_workflow_providers, get_supported_formats
 from renku.ui.cli.utils.terminal import print_workflow_file, show_text_with_pager
 
 
 def _complete_workflows(ctx, param, incomplete):
     from renku.command.workflow import search_workflows_command
@@ -1183,17 +1208,15 @@
             values=values,
             set_params=set_params,
         )
     )
 
     if result.output:
         click.echo(
-            "Unchanged files:\n\n\t{0}".format(
-                "\n\t".join(click.style(path, fg=color.YELLOW) for path in result.output)
-            )
+            "Unchanged files:\n\n\t{}".format("\n\t".join(click.style(path, fg=color.YELLOW) for path in result.output))
         )
 
 
 @workflow.command()
 @click.option(
     "--from",
     "sources",
```

### Comparing `renku-2.3.2/renku/ui/service/.env-example` & `renku-2.4.0rc1/renku/ui/service/.env-example`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/ui/service/__init__.py` & `renku-2.4.0rc1/renku/ui/service/gateways/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,8 +10,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service."""
+"""Renku service adapters/gateways."""
```

### Comparing `renku-2.3.2/renku/ui/service/cache/__init__.py` & `renku-2.4.0rc1/renku/ui/service/cache/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/base.py` & `renku-2.4.0rc1/renku/ui/service/cache/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/config.py` & `renku-2.4.0rc1/renku/ui/service/cache/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/files.py` & `renku-2.4.0rc1/renku/ui/service/cache/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/jobs.py` & `renku-2.4.0rc1/renku/ui/service/cache/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -56,15 +55,15 @@
             return
 
         return job_obj
 
     @staticmethod
     def get_jobs(user):
         """Get all user jobs."""
-        return Job.query((Job.user_id == user.user_id))
+        return Job.query(Job.user_id == user.user_id)
 
     @staticmethod
     def invalidate_job(user, job_id):
         """Remove users job record."""
         job_obj = JobManagementCache.get_job(user, job_id)
 
         if job_obj:
```

### Comparing `renku-2.3.2/renku/ui/service/cache/models/__init__.py` & `renku-2.4.0rc1/renku/core/workflow/parser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service cache models."""
+"""Renku workflow file parsers."""
```

### Comparing `renku-2.3.2/renku/ui/service/cache/models/file.py` & `renku-2.4.0rc1/renku/ui/service/cache/models/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/models/job.py` & `renku-2.4.0rc1/renku/ui/service/cache/models/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/models/project.py` & `renku-2.4.0rc1/renku/ui/service/cache/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/models/user.py` & `renku-2.4.0rc1/renku/ui/service/controllers/api/abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,23 +10,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service cache user related models."""
-from walrus import Model, TextField
+"""Renku service controller module interfaces."""
 
-from renku.ui.service.cache.base import BaseCache
+from abc import ABC
 
 
-class User(Model):
-    """User cache model."""
+class ServiceCtrl(ABC):
+    """Interface for Renku service controllers."""
 
-    __database__ = BaseCache.model_db
-    __namespace__ = BaseCache.namespace
+    def renku_op(self):
+        """Renku operation for the controller."""
+        pass
 
-    user_id = TextField(primary_key=True, index=True)
-    fullname = TextField()
-    email = TextField()
-    token = TextField()
+    def to_response(self):
+        """Execute controller flow and serialize to service response."""
+        pass
```

### Comparing `renku-2.3.2/renku/ui/service/cache/projects.py` & `renku-2.4.0rc1/renku/ui/service/cache/projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/serializers/__init__.py` & `renku-2.4.0rc1/renku/ui/service/serializers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,8 +10,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service cache serializers."""
+"""Renku service serializers."""
```

### Comparing `renku-2.3.2/renku/ui/service/cache/serializers/file.py` & `renku-2.4.0rc1/renku/ui/service/cache/serializers/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/serializers/job.py` & `renku-2.4.0rc1/renku/ui/service/cache/serializers/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/serializers/project.py` & `renku-2.4.0rc1/renku/ui/service/cache/serializers/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/serializers/user.py` & `renku-2.4.0rc1/renku/ui/service/cache/serializers/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/cache/users.py` & `renku-2.4.0rc1/renku/ui/service/cache/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/config.py` & `renku-2.4.0rc1/renku/ui/service/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/__init__.py` & `renku-2.4.0rc1/renku/ui/service/controllers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/api/__init__.py` & `renku-2.4.0rc1/renku/ui/service/controllers/utils/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service controllers api."""
+"""Utilities for renku service dataset controllers."""
+
+
+def set_url_for_uploaded_images(images, cache, user):
+    """Set proper url/path for uploaded or relative dataset images."""
+    for img in images:
+        if img.get("file_id"):
+            file = cache.get_file(user, img.pop("file_id"))
+            img["content_url"] = str(file.abs_path)
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/api/abstract.py` & `renku-2.4.0rc1/renku/command/update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023- Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service controller module interfaces."""
+"""Renku ``update`` command."""
 
-from abc import ABC
+from renku.command.command_builder.command import Command
 
 
-class ServiceCtrl(ABC):
-    """Interface for Renku service controllers."""
+def update_command(skip_metadata_update: bool):
+    """Update existing files by rerunning their outdated workflow."""
+    from renku.core.workflow.update import update
 
-    def renku_op(self):
-        """Renku operation for the controller."""
-        pass
-
-    def to_response(self):
-        """Execute controller flow and serialize to service response."""
-        pass
+    command = Command().command(update).require_migration().require_clean()
+    if skip_metadata_update:
+        command = command.with_database(write=False)
+    else:
+        command = command.with_database(write=True).with_commit()
+    return command
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/api/mixins.py` & `renku-2.4.0rc1/renku/ui/service/controllers/api/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -46,15 +45,15 @@
 from renku.ui.service.serializers.common import DelayedResponseRPC
 
 PROJECT_FETCH_TIME = 30
 
 
 def local_identity(method):
     """Ensure identity on local execution."""
-    # noqa
+
     @wraps(method)
     def _impl(self, *method_args, **method_kwargs):
         """Implementation of method wrapper."""
         if not hasattr(self, "user") and not isinstance(getattr(self, "user", None), User):
             raise UserAnonymousError()
 
         return method(self, *method_args, **method_kwargs)
@@ -155,15 +154,14 @@
             return self.local()
 
         elif "git_url" in self.context and "user_id" not in self.user_data:
             # NOTE: Anonymous session support.
             return self.remote()
 
         elif "git_url" in self.context and "user_id" in self.user_data:
-
             try:
                 project = Project.get(
                     (Project.user_id == self.user_data["user_id"]) & (Project.git_url == self.context["git_url"])
                 )
             except ValueError:
                 from renku.ui.service.controllers.cache_project_clone import ProjectCloneCtrl
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_files_delete_chunks.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -31,15 +30,15 @@
 
     REQUEST_SERIALIZER = FileChunksDeleteRequest()
     RESPONSE_SERIALIZER = FileChunksDeleteResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct list uploaded files controller."""
         self.ctx = DeleteFileChunksCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(DeleteFileChunksCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def delete_chunks(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_files_upload.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_files_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -20,15 +19,15 @@
 import shutil
 from pathlib import Path
 
 import patoolib
 from patoolib.util import PatoolError
 
 from renku.core.errors import RenkuException
-from renku.core.util.file_size import bytes_to_unit
+from renku.core.util.os import bytes_to_unit
 from renku.ui.service.config import CACHE_UPLOADS_PATH, MAX_CONTENT_LENGTH, SUPPORTED_ARCHIVES
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
 from renku.ui.service.errors import IntermittentFileExistsError, UserUploadTooLargeError
 from renku.ui.service.serializers.cache import FileUploadRequest, FileUploadResponseRPC, extract_file
 from renku.ui.service.views import result_response
 
@@ -47,15 +46,15 @@
             "file_name": self.file.filename,
             "content_type": self.file.content_type,
             "is_archive": self.file.content_type in SUPPORTED_ARCHIVES,
         }
         args = {**flask_request.args, **flask_request.form}
         self.response_builder.update(UploadFilesCtrl.REQUEST_SERIALIZER.load(args))
 
-        super(UploadFilesCtrl, self).__init__(cache, user_data, {})
+        super().__init__(cache, user_data, {})
 
     @property
     def context(self):
         """Controller operation context."""
         return self.response_builder
 
     @property
@@ -145,15 +144,15 @@
 
         return self.postprocess_file(file_path)
 
     def postprocess_file(self, file_path):
         """Postprocessing of uploaded file."""
         files = []
         if self.response_builder["unpack_archive"] and self.response_builder["is_archive"]:
-            unpack_dir = "{0}.unpacked".format(file_path.name)
+            unpack_dir = f"{file_path.name}.unpacked"
             temp_dir = file_path.parent / Path(unpack_dir)
             if temp_dir.exists():
                 shutil.rmtree(temp_dir)
             temp_dir.mkdir(exist_ok=True)
 
             try:
                 patoolib.extract_archive(str(file_path), outdir=str(temp_dir))
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_list_projects.py` & `renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,51 +10,43 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service cache list cached projects controller."""
-import itertools
+"""Renku service plans list controller."""
 
+from renku.command.command_builder.command import Command
+from renku.core.workflow.plan import get_plans_with_metadata
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
-from renku.ui.service.serializers.cache import ProjectListResponseRPC
+from renku.ui.service.serializers.workflows import WorkflowPlansListRequest, WorkflowPlansListResponseRPC
 from renku.ui.service.views import result_response
 
 
-class ListProjectsCtrl(ServiceCtrl, RenkuOperationMixin):
-    """Controller for listing cached projects endpoint."""
+class WorkflowPlansListCtrl(ServiceCtrl, RenkuOperationMixin):
+    """Controller for plans list endpoint."""
 
-    RESPONSE_SERIALIZER = ProjectListResponseRPC()
+    REQUEST_SERIALIZER = WorkflowPlansListRequest()
+    RESPONSE_SERIALIZER = WorkflowPlansListResponseRPC()
 
-    def __init__(self, cache, user_data):
-        """Construct controller."""
-        self.ctx = {}
-        super(ListProjectsCtrl, self).__init__(cache, user_data, {})
+    def __init__(self, cache, user_data, request_data):
+        """Construct a plans list controller."""
+        self.ctx = WorkflowPlansListCtrl.REQUEST_SERIALIZER.load(request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
-    def list_projects(self):
-        """List locally cache projects."""
-        projects = [project for project in self.cache.get_projects(self.user) if project.abs_path.exists()]
-
-        result = {
-            "projects": [
-                max(g, key=lambda p: p.created_at) for _, g in itertools.groupby(projects, lambda p: p.git_url)
-            ]
-        }
-
-        return result
-
     def renku_op(self):
         """Renku operation for the controller."""
-        # NOTE: We leave it empty since it does not execute renku operation.
-        pass
+        plan_list_command = Command().command(get_plans_with_metadata).with_database().require_migration()
+        result = plan_list_command.build().execute()
+        return result.output
 
     def to_response(self):
         """Execute controller flow and serialize to service response."""
-        return result_response(ListProjectsCtrl.RESPONSE_SERIALIZER, self.list_projects())
+        self.ctx["plans"] = self.execute_op()
+        return result_response(WorkflowPlansListCtrl.RESPONSE_SERIALIZER, self.ctx)
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_list_uploaded.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_list_uploaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -26,15 +25,15 @@
     """Controller for listing uploaded files endpoint."""
 
     RESPONSE_SERIALIZER = FileListResponseRPC()
 
     def __init__(self, cache, user_data):
         """Construct list uploaded files controller."""
         self.ctx = {}
-        super(ListUploadedFilesCtrl, self).__init__(cache, user_data, {})
+        super().__init__(cache, user_data, {})
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_migrate_project.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_migrate_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -77,15 +76,15 @@
 
         self.force_template_update = self.ctx.get("force_template_update", False)
         self.skip_template_update = self.ctx.get("skip_template_update", False)
         self.skip_docker_update = self.ctx.get("skip_docker_update", False)
         self.skip_migrations = self.ctx.get("skip_migrations", False)
         self.commit_message = f"{MESSAGE_PREFIX} migrate to latest version for renku {__version__}"
 
-        super(MigrateProjectCtrl, self).__init__(
+        super().__init__(
             cache,
             user_data,
             request_data,
             migrate_project=migrate_project,
             skip_lock=skip_lock,
             clone_depth=PROJECT_CLONE_NO_DEPTH,
         )
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_migrations_check.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_migrations_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -38,15 +37,15 @@
     REQUEST_SERIALIZER = ProjectMigrationCheckRequest()
     RESPONSE_SERIALIZER = ProjectMigrationCheckResponseRPC()
 
     def __init__(self, cache, user_data, request_data, git_api_provider: IGitAPIProvider):
         """Construct migration check controller."""
         self.ctx = MigrationsCheckCtrl.REQUEST_SERIALIZER.load(request_data)
         self.git_api_provider = git_api_provider
-        super(MigrationsCheckCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def _fast_op_without_cache(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/cache_project_clone.py` & `renku-2.4.0rc1/renku/ui/service/controllers/cache_project_clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -31,15 +30,15 @@
     REQUEST_SERIALIZER = RepositoryCloneRequest()
     RESPONSE_SERIALIZER = ProjectCloneResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct controller."""
         self.request_data = ProjectCloneCtrl.REQUEST_SERIALIZER.load(request_data)
         self.ctx = ProjectCloneContext().load({**user_data, **self.request_data}, unknown=EXCLUDE)
-        super(ProjectCloneCtrl, self).__init__(cache, user_data, self.request_data)
+        super().__init__(cache, user_data, self.request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def project_clone(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/config_set.py` & `renku-2.4.0rc1/renku/ui/service/controllers/config_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -33,15 +32,15 @@
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct controller."""
         self.ctx = SetConfigCtrl.REQUEST_SERIALIZER.load(request_data)
         config_keys = ", ".join(request_data["config"].keys())
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} config set {config_keys}"
 
-        super(SetConfigCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/config_show.py` & `renku-2.4.0rc1/renku/ui/service/controllers/config_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -29,15 +28,15 @@
 
     REQUEST_SERIALIZER = ConfigShowRequest()
     RESPONSE_SERIALIZER = ConfigShowResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct controller."""
         self.ctx = ShowConfigCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(ShowConfigCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_add_file.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_add_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -40,15 +39,15 @@
     RESPONSE_SERIALIZER = DatasetAddResponseRPC()
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct a datasets add controller."""
         self.ctx = DatasetsAddFileCtrl.REQUEST_SERIALIZER.load(request_data)
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} dataset add {self.ctx['name']}"
 
-        super(DatasetsAddFileCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def prepare_paths(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_create.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -35,15 +34,15 @@
     RESPONSE_SERIALIZER = DatasetCreateResponseRPC()
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct a datasets create controller."""
         self.ctx = DatasetsCreateCtrl.REQUEST_SERIALIZER.load(request_data)
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} dataset create {self.ctx['name']}"
 
-        super(DatasetsCreateCtrl, self).__init__(cache, user_data, request_data, migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_edit.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -17,15 +16,15 @@
 # limitations under the License.
 """Renku service datasets edit controller."""
 from typing import Dict, List, Union, cast
 
 from renku.command.dataset import edit_dataset_command
 from renku.core.dataset.request_model import ImageRequestModel
 from renku.core.util.metadata import construct_creators
-from renku.core.util.util import NO_VALUE, NoValueType
+from renku.domain_model.constant import NO_VALUE, NoValueType
 from renku.domain_model.provenance.agent import Person
 from renku.ui.service.cache.models.job import Job
 from renku.ui.service.config import CACHE_UPLOADS_PATH, MESSAGE_PREFIX
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOpSyncMixin
 from renku.ui.service.controllers.utils.datasets import set_url_for_uploaded_images
 from renku.ui.service.serializers.datasets import DatasetEditRequest, DatasetEditResponseRPC
@@ -39,15 +38,15 @@
     RESPONSE_SERIALIZER = DatasetEditResponseRPC()
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct a datasets edit list controller."""
         self.ctx = cast(Dict, DatasetsEditCtrl.REQUEST_SERIALIZER.load(request_data))
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} dataset edit {self.ctx['name']}"
 
-        super(DatasetsEditCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_files_list.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,42 +10,41 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service datasets files controller."""
+"""Renku service datasets list controller."""
 
-from renku.command.dataset import list_files_command
+from renku.command.dataset import list_datasets_command
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
-from renku.ui.service.serializers.datasets import DatasetFilesListRequest, DatasetFilesListResponseRPC
+from renku.ui.service.serializers.datasets import DatasetListRequest, DatasetListResponseRPC
 from renku.ui.service.views import result_response
 
 
-class DatasetsFilesListCtrl(ServiceCtrl, RenkuOperationMixin):
-    """Controller for datasets files list endpoint."""
+class DatasetsListCtrl(ServiceCtrl, RenkuOperationMixin):
+    """Controller for datasets list endpoint."""
 
-    REQUEST_SERIALIZER = DatasetFilesListRequest()
-    RESPONSE_SERIALIZER = DatasetFilesListResponseRPC()
+    REQUEST_SERIALIZER = DatasetListRequest()
+    RESPONSE_SERIALIZER = DatasetListResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
-        """Construct a datasets files list controller."""
-        self.ctx = DatasetsFilesListCtrl.REQUEST_SERIALIZER.load(request_data)
-
-        super(DatasetsFilesListCtrl, self).__init__(cache, user_data, request_data)
+        """Construct a datasets list controller."""
+        self.ctx = DatasetsListCtrl.REQUEST_SERIALIZER.load(request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
         """Renku operation for the controller."""
-        result = list_files_command().build().execute(datasets=[self.ctx["name"]])
+        result = list_datasets_command().build().execute()
         return result.output
 
     def to_response(self):
         """Execute controller flow and serialize to service response."""
-        self.ctx["files"] = self.execute_op()
-        return result_response(DatasetsFilesListCtrl.RESPONSE_SERIALIZER, self.ctx)
+        self.ctx["datasets"] = self.execute_op()
+        return result_response(DatasetsListCtrl.RESPONSE_SERIALIZER, self.ctx)
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_import.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -35,15 +34,15 @@
     RESPONSE_SERIALIZER = DatasetImportResponseRPC()
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct a datasets import controller."""
         self.ctx = DatasetsImportCtrl.REQUEST_SERIALIZER.load(request_data)
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} dataset import of {self.ctx['dataset_uri']}"
 
-        super(DatasetsImportCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_list.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_files_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,41 +10,42 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service datasets list controller."""
+"""Renku service datasets files controller."""
 
-from renku.command.dataset import list_datasets_command
+from renku.command.dataset import list_files_command
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
-from renku.ui.service.serializers.datasets import DatasetListRequest, DatasetListResponseRPC
+from renku.ui.service.serializers.datasets import DatasetFilesListRequest, DatasetFilesListResponseRPC
 from renku.ui.service.views import result_response
 
 
-class DatasetsListCtrl(ServiceCtrl, RenkuOperationMixin):
-    """Controller for datasets list endpoint."""
+class DatasetsFilesListCtrl(ServiceCtrl, RenkuOperationMixin):
+    """Controller for datasets files list endpoint."""
 
-    REQUEST_SERIALIZER = DatasetListRequest()
-    RESPONSE_SERIALIZER = DatasetListResponseRPC()
+    REQUEST_SERIALIZER = DatasetFilesListRequest()
+    RESPONSE_SERIALIZER = DatasetFilesListResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
-        """Construct a datasets list controller."""
-        self.ctx = DatasetsListCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(DatasetsListCtrl, self).__init__(cache, user_data, request_data)
+        """Construct a datasets files list controller."""
+        self.ctx = DatasetsFilesListCtrl.REQUEST_SERIALIZER.load(request_data)
+
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
         """Renku operation for the controller."""
-        result = list_datasets_command().build().execute()
+        result = list_files_command().build().execute(datasets=[self.ctx["name"]])
         return result.output
 
     def to_response(self):
         """Execute controller flow and serialize to service response."""
-        self.ctx["datasets"] = self.execute_op()
-        return result_response(DatasetsListCtrl.RESPONSE_SERIALIZER, self.ctx)
+        self.ctx["files"] = self.execute_op()
+        return result_response(DatasetsFilesListCtrl.RESPONSE_SERIALIZER, self.ctx)
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_remove.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -32,15 +31,15 @@
     RESPONSE_SERIALIZER = DatasetRemoveResponseRPC()
 
     def __init__(self, cache, user_data, request_data, migrate_project=False):
         """Construct a datasets remove controller."""
         self.ctx = DatasetsRemoveCtrl.REQUEST_SERIALIZER.load(request_data)
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} dataset remove {self.ctx['name']}"
 
-        super(DatasetsRemoveCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/datasets_unlink.py` & `renku-2.4.0rc1/renku/ui/service/controllers/datasets_unlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -42,15 +41,15 @@
             filters = f"-I {self.include} -X {self.exclude}"
         elif not self.include and self.exclude:
             filters = f"-X {self.exclude}"
         else:
             filters = f"-I {self.include}"
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} unlink dataset {self.ctx['name']} {filters}"
 
-        super(DatasetsUnlinkCtrl, self).__init__(cache, user_data, request_data, migrate_project=migrate_project)
+        super().__init__(cache, user_data, request_data, migrate_project=migrate_project)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/graph_export.py` & `renku-2.4.0rc1/renku/ui/service/controllers/graph_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -41,15 +40,15 @@
 
     REQUEST_SERIALIZER = GraphExportRequest()
     RESPONSE_SERIALIZER = GraphExportResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct a datasets list controller."""
         self.ctx = GraphExportCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(GraphExportCtrl, self).__init__(cache, user_data, request_data, clone_depth=PROJECT_CLONE_NO_DEPTH)
+        super().__init__(cache, user_data, request_data, clone_depth=PROJECT_CLONE_NO_DEPTH)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/project_edit.py` & `renku-2.4.0rc1/renku/ui/service/controllers/project_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -15,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Renku service project edit controller."""
 from typing import Dict, cast
 
 from renku.command.project import edit_project_command
-from renku.core.util.util import NO_VALUE
+from renku.domain_model.constant import NO_VALUE
 from renku.ui.service.cache.models.job import Job
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOpSyncMixin
 from renku.ui.service.serializers.project import ProjectEditRequest, ProjectEditResponseRPC
 from renku.ui.service.views import result_response
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/project_lock_status.py` & `renku-2.4.0rc1/renku/ui/service/controllers/project_lock_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2021 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/project_show.py` & `renku-2.4.0rc1/renku/ui/service/controllers/project_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/templates_create_project.py` & `renku-2.4.0rc1/renku/ui/service/controllers/templates_create_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -26,15 +25,15 @@
 from renku.core.template.template import fetch_templates_source
 from renku.core.util.contexts import renku_project_context
 from renku.domain_model.template import Template
 from renku.infrastructure.repository import Repository
 from renku.ui.service.config import MESSAGE_PREFIX
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
-from renku.ui.service.errors import UserProjectCreationError
+from renku.ui.service.errors import UserProjectCreationError, UserTemplateInvalidError
 from renku.ui.service.serializers.templates import ProjectTemplateRequest, ProjectTemplateResponseRPC
 from renku.ui.service.utils import new_repo_push
 from renku.ui.service.views import result_response
 from renku.version import __version__, is_release
 
 
 class TemplatesCreateProjectCtrl(ServiceCtrl, RenkuOperationMixin):
@@ -46,15 +45,15 @@
     def __init__(self, cache, user_data, request_data):
         """Construct a templates read manifest controller."""
         self.ctx = cast(
             Dict[str, Any],
             TemplatesCreateProjectCtrl.REQUEST_SERIALIZER.load({**user_data, **request_data}, unknown=EXCLUDE),
         )
         self.ctx["commit_message"] = f"{MESSAGE_PREFIX} init {self.ctx['project_name']}"
-        super(TemplatesCreateProjectCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
         self.template: Optional[Template] = None
 
     @property
     def context(self):
         """Controller context."""
         return self.ctx
@@ -113,24 +112,26 @@
 
     def setup_template(self):
         """Reads template manifest."""
         templates_source = fetch_templates_source(source=self.ctx["git_url"], reference=self.ctx["ref"])
         identifier = self.ctx["identifier"]
         try:
             self.template = templates_source.get_template(id=identifier, reference=None)
-        except (errors.InvalidTemplateError, errors.TemplateNotFoundError) as e:
+        except errors.TemplateNotFoundError as e:
             raise UserProjectCreationError(
                 error_message=f"the template '{identifier}' does not exist in the target template's repository"
             ) from e
+        except errors.InvalidTemplateError as e:
+            raise UserTemplateInvalidError(error_message=f"the template '{identifier}' is invalid") from e
 
         repository = Repository(templates_source.path)
         self.template_version = repository.head.commit.hexsha
 
         # Verify missing parameters
-        template_parameters = set(p.name for p in self.template.parameters)
+        template_parameters = {p.name for p in self.template.parameters}
         provided_parameters = {p["key"]: p["value"] for p in self.ctx["parameters"]}
         missing_keys = list(template_parameters - provided_parameters.keys())
         if len(missing_keys) > 0:
             raise UserProjectCreationError(error_message=f"the template requires a value for '${missing_keys[0]}'")
 
         return provided_parameters
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/templates_read_manifest.py` & `renku-2.4.0rc1/renku/ui/service/controllers/templates_read_manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -36,15 +35,15 @@
 
     REQUEST_SERIALIZER = ManifestTemplatesRequest()
     RESPONSE_SERIALIZER = ManifestTemplatesResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct a templates read manifest controller."""
         self.ctx = TemplatesReadManifestCtrl.REQUEST_SERIALIZER.load({**user_data, **request_data}, unknown=EXCLUDE)
-        super(TemplatesReadManifestCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller context."""
         return self.ctx
 
     def template_manifest(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/utils/__init__.py` & `renku-2.4.0rc1/renku/ui/service/controllers/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/utils/project_clone.py` & `renku-2.4.0rc1/renku/ui/service/controllers/utils/project_clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/utils/remote_project.py` & `renku-2.4.0rc1/renku/ui/service/controllers/utils/remote_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/version.py` & `renku-2.4.0rc1/renku/ui/service/controllers/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/workflow_plans_export.py` & `renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -29,15 +28,15 @@
 
     REQUEST_SERIALIZER = WorkflowPlansExportRequest()
     RESPONSE_SERIALIZER = WorkflowPlansExportResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
         """Construct a workflow plan show controller."""
         self.ctx = WorkflowPlansExportCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(WorkflowPlansExportCtrl, self).__init__(cache, user_data, request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
```

### Comparing `renku-2.3.2/renku/ui/service/controllers/workflow_plans_list.py` & `renku-2.4.0rc1/renku/ui/service/controllers/workflow_plans_show.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,43 +10,41 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service plans list controller."""
+"""Renku service plans show controller."""
 
-from renku.command.command_builder.command import Command
-from renku.core.workflow.plan import get_plans_with_metadata
+from renku.command.workflow import show_workflow_command
 from renku.ui.service.controllers.api.abstract import ServiceCtrl
 from renku.ui.service.controllers.api.mixins import RenkuOperationMixin
-from renku.ui.service.serializers.workflows import WorkflowPlansListRequest, WorkflowPlansListResponseRPC
+from renku.ui.service.serializers.workflows import WorkflowPlansShowRequest, WorkflowPlansShowResponseRPC
 from renku.ui.service.views import result_response
 
 
-class WorkflowPlansListCtrl(ServiceCtrl, RenkuOperationMixin):
-    """Controller for plans list endpoint."""
+class WorkflowPlansShowCtrl(ServiceCtrl, RenkuOperationMixin):
+    """Controller for plan show endpoint."""
 
-    REQUEST_SERIALIZER = WorkflowPlansListRequest()
-    RESPONSE_SERIALIZER = WorkflowPlansListResponseRPC()
+    REQUEST_SERIALIZER = WorkflowPlansShowRequest()
+    RESPONSE_SERIALIZER = WorkflowPlansShowResponseRPC()
 
     def __init__(self, cache, user_data, request_data):
-        """Construct a plans list controller."""
-        self.ctx = WorkflowPlansListCtrl.REQUEST_SERIALIZER.load(request_data)
-        super(WorkflowPlansListCtrl, self).__init__(cache, user_data, request_data)
+        """Construct a workflow plan show controller."""
+        self.ctx = WorkflowPlansShowCtrl.REQUEST_SERIALIZER.load(request_data)
+        super().__init__(cache, user_data, request_data)
 
     @property
     def context(self):
         """Controller operation context."""
         return self.ctx
 
     def renku_op(self):
         """Renku operation for the controller."""
-        plan_list_command = Command().command(get_plans_with_metadata).with_database().require_migration()
-        result = plan_list_command.build().execute()
+        result = show_workflow_command().build().execute(name_or_id_or_path=self.ctx["plan_id"], with_metadata=True)
         return result.output
 
     def to_response(self):
         """Execute controller flow and serialize to service response."""
-        self.ctx["plans"] = self.execute_op()
-        return result_response(WorkflowPlansListCtrl.RESPONSE_SERIALIZER, self.ctx)
+        result = self.execute_op()
+        return result_response(WorkflowPlansShowCtrl.RESPONSE_SERIALIZER, result)
```

### Comparing `renku-2.3.2/renku/ui/service/entrypoint.py` & `renku-2.4.0rc1/renku/ui/service/entrypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -85,15 +84,15 @@
         return jsonify({"service_version": renku.__version__, "spec_url": url_for("apispec.openapi")})
 
     @app.route("/health")
     def health():
         """Service health check."""
         import renku
 
-        return "renku repository service version {}\n".format(renku.__version__)
+        return f"renku repository service version {renku.__version__}\n"
 
     if custom_exceptions:
         register_exceptions(app)
 
     return app
 
 
@@ -159,19 +158,15 @@
 
 app = create_app()
 
 
 @app.after_request
 def after_request(response):
     """After request handler."""
-    service_log.info(
-        "{0} {1} {2} {3} {4}".format(
-            request.remote_addr, request.method, request.scheme, request.full_path, response.status
-        )
-    )
+    service_log.info(f"{request.remote_addr} {request.method} {request.scheme} {request.full_path} {response.status}")
 
     return response
 
 
 if __name__ == "__main__":
     if len(JWT_TOKEN_SECRET) < 32:
         raise InvalidTokenError("web token must be greater or equal to 32 bytes")
```

### Comparing `renku-2.3.2/renku/ui/service/errors.py` & `renku-2.4.0rc1/renku/ui/service/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -258,19 +257,23 @@
         )
 
 
 class UserTemplateInvalidError(ServiceError):
     """The provided URL doesn't lead to a valid template repository."""
 
     code = SVC_ERROR_USER + 101
-    userMessage = "The target repository is not a valid Renku template repository."
-    devMessage = "Target repository is not a valid template."
+    userMessage = "The target repository is not a valid Renku template repository: {error_message}"
+    devMessage = "Target repository is not a valid template.: {error_message}"
 
-    def __init__(self, exception=None):
-        super().__init__(exception=exception)
+    def __init__(self, exception=None, error_message=ERROR_NOT_AVAILABLE):
+        super().__init__(
+            userMessage=self.userMessage.format(error_message=error_message),
+            devMessage=self.devMessage.format(error_message=error_message),
+            exception=exception,
+        )
 
 
 class UserProjectCreationError(ServiceError):
     """Error when creating a new project from a Renku template.
 
     One (or more) project field is wrong.
     """
```

### Comparing `renku-2.3.2/renku/ui/service/gateways/__init__.py` & `renku-2.4.0rc1/renku/ui/service/cache/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,8 +10,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service adapters/gateways."""
+"""Renku service cache models."""
```

### Comparing `renku-2.3.2/renku/ui/service/gateways/gitlab_api_provider.py` & `renku-2.4.0rc1/renku/ui/service/gateways/gitlab_api_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/interfaces/__init__.py` & `renku-2.4.0rc1/renku/ui/service/serializers/v1/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -11,8 +10,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service interfaces for IoC adapters/gateways."""
+"""Renku service v1.0 serializers."""
```

### Comparing `renku-2.3.2/renku/ui/service/interfaces/git_api_provider.py` & `renku-2.4.0rc1/renku/ui/service/interfaces/git_api_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/__init__.py` & `renku-2.4.0rc1/renku/core/workflow/converters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service jobs."""
+"""Renku workflow converters."""
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/cleanup.py` & `renku-2.4.0rc1/renku/ui/service/jobs/cleanup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/constants.py` & `renku-2.4.0rc1/renku/core/session/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Job constants."""
+"""Renku interactive session module."""
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/contexts.py` & `renku-2.4.0rc1/renku/ui/service/jobs/contexts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -27,11 +26,11 @@
 @contextlib.contextmanager
 def enqueue_retry(queue, retry=3):
     """Ensure job gets queued."""
     count = 0
     while count < retry:
         try:
             yield WorkerQueues.get(queue)
-        except (OSError, IOError, BusyLoadingError):
+        except (OSError, BusyLoadingError):
             time.sleep(2**count)
             count += 1
         break
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/datasets.py` & `renku-2.4.0rc1/renku/ui/service/jobs/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/delayed_ctrl.py` & `renku-2.4.0rc1/renku/ui/service/jobs/delayed_ctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/jobs/queues.py` & `renku-2.4.0rc1/renku/ui/service/jobs/queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/logger.py` & `renku-2.4.0rc1/renku/ui/service/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/logging.yaml` & `renku-2.4.0rc1/renku/ui/service/logging.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/ui/service/scheduler.py` & `renku-2.4.0rc1/renku/ui/service/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/__init__.py` & `renku-2.4.0rc1/renku/domain_model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service serializers."""
+"""Model objects used in Python SDK."""
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/cache.py` & `renku-2.4.0rc1/renku/ui/service/serializers/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -46,15 +45,15 @@
     """
     files = request.files
     if "file" not in files:
         raise ValidationError("missing key: file")
 
     file = files["file"]
     if file and not file.filename:
-        raise ValidationError("wrong filename: {0}".format(file.filename))
+        raise ValidationError(f"wrong filename: {file.filename}")
 
     if file:
         file.filename = secure_filename(file.filename)
         return file
 
 
 class FileUploadRequest(ArchiveSchema):
@@ -178,15 +177,15 @@
 
         return data
 
     def format_url(self, data):
         """Format url with auth."""
         git_url = urlparse(data["git_url"])
 
-        url = "oauth2:{0}@{1}".format(data["token"], git_url.netloc)
+        url = "oauth2:{}@{}".format(data["token"], git_url.netloc)
         return git_url._replace(netloc=url).geturl()
 
     @post_load
     def finalize_data(self, data, **kwargs):
         """Finalize data."""
         data["url_with_auth"] = self.format_url(data)
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/common.py` & `renku-2.4.0rc1/renku/ui/service/serializers/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/config.py` & `renku-2.4.0rc1/renku/ui/service/serializers/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/datasets.py` & `renku-2.4.0rc1/renku/ui/service/serializers/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -113,15 +112,15 @@
     client_extras = fields.String()
 
     @post_load()
     def check_files(self, data, **kwargs):
         """Check serialized file list."""
         for _file in data["files"]:
             if "file_id" in _file and "file_path" in _file:
-                raise ValidationError(("invalid reference found:" "use either `file_id` or `file_path`"))
+                raise ValidationError("invalid reference found: use either `file_id` or `file_path`")
 
         return data
 
 
 class DatasetAddResponse(DatasetNameSchema, RenkuSyncSchema):
     """Response schema for a dataset add file view."""
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/graph.py` & `renku-2.4.0rc1/renku/ui/service/serializers/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/headers.py` & `renku-2.4.0rc1/renku/ui/service/serializers/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/jobs.py` & `renku-2.4.0rc1/renku/ui/service/serializers/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/project.py` & `renku-2.4.0rc1/renku/ui/service/serializers/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/rpc.py` & `renku-2.4.0rc1/renku/ui/service/serializers/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
@@ -11,15 +9,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service JSON-RPC serializers."""
+"""Renku service version controller."""
 from marshmallow import Schema, fields
 
 
-class JsonRPCResponse(Schema):
-    """JsonRPC response schema."""
+class VersionResponse(Schema):
+    """Version response schema."""
+
+    latest_version = fields.String()
+    supported_project_version = fields.Number()
+    minimum_api_version = fields.String()
+    maximum_api_version = fields.String()
+
+
+class VersionResponseRPC(Schema):
+    """Version response RPC schema."""
 
-    error = fields.Dict()
+    result = fields.Nested(VersionResponse)
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/templates.py` & `renku-2.4.0rc1/renku/ui/service/serializers/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -86,15 +85,15 @@
 
         project_slug = f"{data['project_namespace']}/{project_name_stripped}"
         data["new_project_url"] = new_project_url
         data["project_name_stripped"] = project_name_stripped
         data["project_slug"] = project_slug
 
         new_project_url_parsed = urlparse(new_project_url)
-        url = "oauth2:{0}@{1}".format(data["token"], new_project_url_parsed.netloc)
+        url = "oauth2:{}@{}".format(data["token"], new_project_url_parsed.netloc)
         data["new_project_url_with_auth"] = new_project_url_parsed._replace(netloc=url).geturl()
 
         return data
 
 
 class ManifestTemplateSchema(Schema):
     """Manifest template schema."""
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/v1/__init__.py` & `renku-2.4.0rc1/renku/ui/service/controllers/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service v1.0 serializers."""
+"""Renku service controllers api."""
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/v1/cache.py` & `renku-2.4.0rc1/renku/ui/service/serializers/v1/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/v1/templates.py` & `renku-2.4.0rc1/renku/ui/service/serializers/v1/templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/serializers/workflows.py` & `renku-2.4.0rc1/renku/ui/service/serializers/workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/utils/__init__.py` & `renku-2.4.0rc1/renku/ui/service/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/utils/callback.py` & `renku-2.4.0rc1/renku/ui/service/utils/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+# Copyright 2017-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `renku-2.3.2/renku/ui/service/utils/json_encoder.py` & `renku-2.4.0rc1/renku/ui/service/utils/json_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/utils/timeout.py` & `renku-2.4.0rc1/renku/ui/service/utils/timeout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/__init__.py` & `renku-2.4.0rc1/renku/ui/service/views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/api_versions.py` & `renku-2.4.0rc1/renku/ui/service/views/api_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/apispec.py` & `renku-2.4.0rc1/renku/ui/service/views/apispec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/cache.py` & `renku-2.4.0rc1/renku/ui/service/views/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/config.py` & `renku-2.4.0rc1/renku/ui/service/views/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/datasets.py` & `renku-2.4.0rc1/renku/ui/service/views/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/decorators.py` & `renku-2.4.0rc1/renku/ui/service/views/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -25,15 +24,15 @@
 from renku.ui.service.errors import ProgramContentTypeError, UserAnonymousError
 from renku.ui.service.serializers.headers import OptionalIdentityHeaders, RequiredIdentityHeaders
 from renku.ui.service.views.error_handlers import handle_redis_except
 
 
 def requires_identity(f):
     """Wrapper which indicates that route requires user identification."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kws):
         """Represents decorated function."""
         try:
             user_identity = RequiredIdentityHeaders().load(request.headers)
         except (ValidationError, KeyError) as e:
             raise UserAnonymousError(e)
@@ -54,26 +53,26 @@
 
     return decorated_function
 
 
 @handle_redis_except
 def requires_cache(f):
     """Wrapper which injects cache object into view."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         return f(cache, *args, **kwargs)
 
     return decorated_function
 
 
 def accepts_json(f):
     """Wrapper which ensures only JSON payload can be in request."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         content_type = "application/json"
         wrong_type = False
         if "Content-Type" not in request.headers:
             wrong_type = True
```

### Comparing `renku-2.3.2/renku/ui/service/views/error_handlers.py` & `renku-2.4.0rc1/renku/ui/service/views/error_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2022 - Swiss Data Science Center (SDSC)
+# Copyright 2022-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -82,30 +81,29 @@
 )
 from renku.ui.service.utils.squash import squash
 from renku.ui.service.views import error_response
 
 
 def handle_redis_except(f):
     """Wrapper which handles Redis exceptions."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except (RedisError, OSError) as e:
             raise IntermittentRedisError(e)
 
     return decorated_function
 
 
 def handle_validation_except(f):
     """Wrapper which handles marshmallow `ValidationError`."""
 
-    # noqa
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except ValidationError as e:
             items = squash(e.messages).items()
@@ -124,29 +122,29 @@
             raise UserInvalidGenericFieldsError(e, error_message)
 
     return decorated_function
 
 
 def handle_jwt_except(f):
     """Wrapper which handles invalid JWT."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except (AuthenticationError, ExpiredSignatureError, ImmatureSignatureError, InvalidIssuedAtError) as e:
             raise IntermittentAuthenticationError(e)
 
     return decorated_function
 
 
 def handle_renku_except(f):
     """Wrapper which handles `RenkuException`."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except MigrationRequired as e:
             raise UserOutdatedProjectError(e)
@@ -158,15 +156,15 @@
             raise ProgramRenkuError(e)
 
     return decorated_function
 
 
 def handle_git_except(f):
     """Wrapper which handles `RenkuException`."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except GitCommandError as e:
             error_message = e.stderr.lower() if e.stderr else ""
@@ -182,41 +180,41 @@
                 raise ProgramRepoUnknownError(e, error_message_safe)
 
     return decorated_function
 
 
 def handle_base_except(f):
     """Wrapper which handles base exceptions."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
 
         # NOTE: HTTPException are now handled in the entrypoint
         except ServiceError as e:
             return error_response(e)
         # NOTE: GitError here may not be necessary anymore
         except GitError as e:
             return error_response(ProgramGitError(e, cast(str, e.message) if hasattr(e, "message") else ""))
-        except (Exception, BaseException, OSError, IOError) as e:
+        except (Exception, BaseException, OSError) as e:
             if hasattr(e, "stderr") and e.stderr:
                 error_message = " ".join(e.stderr.strip().split("\n"))
             else:
                 error_message = str(e)
 
             return error_response(ProgramInternalError(e, error_message))
 
     return decorated_function
 
 
 def handle_common_except(f):
     """Handle common exceptions."""
-    # noqa
+
     @wraps(f)
     def dec(*args, **kwargs):
         """Decorated function."""
 
         @handle_base_except
         @handle_validation_except
         @handle_renku_except
@@ -228,15 +226,15 @@
         return _wrapped(*args, **kwargs)
 
     return dec
 
 
 def handle_templates_read_errors(f):
     """Wrapper which handles reading templates errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except InvalidTemplateError as e:
             raise UserTemplateInvalidError(e)
@@ -252,15 +250,15 @@
 
     return decorated_function
 
 
 @handle_templates_read_errors
 def handle_templates_create_errors(f):
     """Wrapper which handles template creating projects errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
 
         def get_schema_error_message(e):
             if isinstance(getattr(e, "messages", None), dict) and e.messages.get("_schema"):
                 message = (
@@ -284,15 +282,15 @@
                 raise ProgramProjectCreationError(e)
 
     return decorated_function
 
 
 def handle_project_write_errors(f):
     """Wrapper which handles writing project metadata errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except UserInvalidGenericFieldsError as e:
             if "Unknown field" in str(e):
@@ -300,15 +298,15 @@
             raise
 
     return decorated_function
 
 
 def handle_config_read_errors(f):
     """Wrapper which handles reading config errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except Exception as e:
             if str(e).startswith("Source contains parsing errors"):
@@ -317,15 +315,15 @@
 
     return decorated_function
 
 
 @handle_config_read_errors
 def handle_config_write_errors(f):
     """Wrapper which handles setting config errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except ParameterError as e:
             if "Invalid parameter value" in str(e):
@@ -337,15 +335,15 @@
             raise
 
     return decorated_function
 
 
 def handle_datasets_write_errors(f):
     """Wrapper which handles datasets write errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except DatasetImageError as e:
             error_message = str(e)
@@ -368,15 +366,15 @@
             raise
 
     return decorated_function
 
 
 def handle_workflow_errors(f):
     """Wrapper which handles workflow errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except WorkflowNotFoundError as e:
             raise IntermittentWorkflowNotFound(e, name_or_id=e.name_or_id)
@@ -384,15 +382,15 @@
             raise
 
     return decorated_function
 
 
 def handle_datasets_unlink_errors(f):
     """Wrapper which handles datasets unlink errors."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except RenkuException as e:
             if str(e).startswith("Invalid parameter") and "No records found" in str(e):
@@ -404,15 +402,15 @@
             raise
 
     return decorated_function
 
 
 def handle_migration_read_errors(f):
     """Wrapper which handles migrations read exceptions."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except TemplateMissingReferenceError as e:
             raise UserProjectTemplateReferenceError(e)
@@ -423,29 +421,29 @@
 
     return decorated_function
 
 
 @handle_migration_read_errors
 def handle_migration_write_errors(f):
     """Wrapper which handles migrations write exceptions."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         except (TemplateUpdateError, DockerfileUpdateError, MigrationError) as e:
             raise ProgramUpdateProjectError(e)
 
     return decorated_function
 
 
 def handle_graph_errors(f):
     """Wrapper which handles graph exceptions."""
-    # noqa
+
     @wraps(f)
     def decorated_function(*args, **kwargs):
         """Represents decorated function."""
         try:
             return f(*args, **kwargs)
         # TODO: handle user and program errors separately
         except (MemoryError, RenkuException, RequestException) as e:
```

### Comparing `renku-2.3.2/renku/ui/service/views/graph.py` & `renku-2.4.0rc1/renku/ui/service/views/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/jobs.py` & `renku-2.4.0rc1/renku/ui/service/views/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/project.py` & `renku-2.4.0rc1/renku/ui/service/views/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/templates.py` & `renku-2.4.0rc1/renku/ui/service/views/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/v1/__init__.py` & `renku-2.4.0rc1/renku/infrastructure/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2018-2023 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service v1.0 views."""
+"""Renku metadata storage/retrieval."""
```

### Comparing `renku-2.3.2/renku/ui/service/views/v1/cache.py` & `renku-2.4.0rc1/renku/ui/service/views/v1/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/v1/templates.py` & `renku-2.4.0rc1/renku/ui/service/views/v1/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/views/version.py` & `renku-2.4.0rc1/renku/ui/service/views/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.3.2/renku/ui/service/views/workflow_plans.py` & `renku-2.4.0rc1/renku/ui/service/views/workflow_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `renku-2.3.2/renku/ui/service/worker.py` & `renku-2.4.0rc1/renku/ui/service/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Copyright 2020 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -54,15 +53,15 @@
     yield build_worker()
 
 
 def check_queues(queue_list):
     """Check if listening on specified queues is possible."""
     for queue in queue_list:
         if queue and queue not in QUEUES:
-            err_msg = "Invalid queue name: {0}\n\n" "Valid queue names: \n{1}".format(queue, "\n".join(QUEUES))
+            err_msg = "Invalid queue name: {}\n\nValid queue names: \n{}".format(queue, "\n".join(QUEUES))
             raise UsageError(err_msg)
 
 
 def start_worker(queue_list):
     """Start worker."""
     q = [q.strip() for q in queue_list if q.strip()]
     check_queues(q)
```

### Comparing `renku-2.3.2/renku/version.py` & `renku-2.4.0rc1/renku/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2017-2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+# Copyright Swiss Data Science Center (SDSC). A partnership between
+# École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -22,15 +20,15 @@
 try:
     from importlib.metadata import distribution, version
 except ImportError:
     from importlib_metadata import distribution, version  # type: ignore
 
 __version__ = version("renku")
 __template_version__ = "0.5.0"
-__minimum_project_version__ = "2.1.0"
+__minimum_project_version__ = "2.4.0"
 
 
 def is_release():
     """Check if current version is a release semver."""
     if re.match(r"\d+.\d+.\d+$", __version__):
         return True
     return False
```

### Comparing `renku-2.3.2/PKG-INFO` & `renku-2.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: renku
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: Python SDK and CLI for the Renku platform.
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: service
 Requires-Dist: apispec (>=4.0.0,<5.3.0) ; extra == "service"
 Requires-Dist: apispec-webframeworks (>=0.5.2,<0.6) ; extra == "service"
@@ -37,31 +37,32 @@
 Requires-Dist: click (>=8.0,<8.1.4)
 Requires-Dist: click-option-group (>=0.5.2,<0.6.0)
 Requires-Dist: click-plugins (==1.1.1)
 Requires-Dist: coverage[toml] (>=4.5.3,<6.5)
 Requires-Dist: cryptography (>=38.0.0,<40.0.0)
 Requires-Dist: cwl-utils (>=0.12,<0.18)
 Requires-Dist: cwltool (==3.1.20220628170238)
+Requires-Dist: deal (>=4.24.0,<5.0.0)
 Requires-Dist: deepdiff (>=5.8.0,<6.0.0)
 Requires-Dist: deepmerge (==1.0.1)
 Requires-Dist: docker (>=3.7.2,<6)
 Requires-Dist: filelock (>=3.3.0,<3.8.1)
 Requires-Dist: flask (==2.1.1) ; extra == "service"
 Requires-Dist: gitpython (==3.1.27)
 Requires-Dist: grandalf (==0.7)
 Requires-Dist: gunicorn ; extra == "service"
 Requires-Dist: humanize (>=3.0.0,<4.1.0)
-Requires-Dist: importlib-resources (>=5.4.0,<5.10.0) ; python_full_version < "3.9.0"
+Requires-Dist: importlib-resources (>=5.12.0,<5.13.0)
 Requires-Dist: inject (>=4.3.0,<4.4.0)
 Requires-Dist: jinja2 (>=2.11.3,<3.1.3)
 Requires-Dist: marshmallow (>=3.18.0,<3.20.0) ; extra == "service"
 Requires-Dist: marshmallow-oneofschema (>=3.0.1,<4.0.0) ; extra == "service"
 Requires-Dist: networkx (>=2.6.0,<2.7)
-Requires-Dist: numpy (>=1.20.0,<1.22.0)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: numpy (>=1.24.0,<1.25.0)
+Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pathspec (>=0.8.0,<1.0.0)
 Requires-Dist: patool (==1.12)
 Requires-Dist: pillow (>=9.0.0,<9.4) ; extra == "service"
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: poetry-dynamic-versioning (==0.21.3)
 Requires-Dist: portalocker (>=2.2.1,<2.5)
 Requires-Dist: psutil (>=5.4.7,<5.9.2)
@@ -78,15 +79,15 @@
 Requires-Dist: rdflib (>=6.0.0,<7.0)
 Requires-Dist: redis (>=3.5.3,<4.2.0) ; extra == "service"
 Requires-Dist: requests (>=2.23.0,<2.28.2)
 Requires-Dist: rich (>=9.3.0,<12.6.0)
 Requires-Dist: rq (==1.11.0) ; extra == "service"
 Requires-Dist: rq-scheduler (==0.11.0) ; extra == "service"
 Requires-Dist: sentry-sdk[flask] (>=1.5.11,<1.5.12) ; extra == "service"
-Requires-Dist: shellingham (==1.5.0)
+Requires-Dist: shellingham (==1.5.0.post1)
 Requires-Dist: tabulate (>=0.7.7,<0.8.11)
 Requires-Dist: toil (==5.7.1)
 Requires-Dist: tqdm (>=4.48.1,<4.62.4)
 Requires-Dist: walrus (>=0.8.2,<0.10.0) ; extra == "service"
 Requires-Dist: werkzeug (>=1.0.0,<2.2.3)
 Requires-Dist: yagup (>=0.1.1)
 Requires-Dist: yaspin (==2.1.0)
@@ -94,15 +95,15 @@
 Requires-Dist: zodb (==5.6.0)
 Requires-Dist: zstandard (>=0.16.0,<0.18.0)
 Project-URL: Changelog, https://github.com/swissdatasciencecenter/renku-python/blob/master/CHANGES.rst
 Project-URL: Documentation, https://renku-python.rtfd.io/
 Description-Content-Type: text/x-rst
 
 ..
-    Copyright 2017-2022 - Swiss Data Science Center (SDSC)
+    Copyright 2017-2023 - Swiss Data Science Center (SDSC)
     A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
     Eidgenössische Technische Hochschule Zürich (ETHZ).
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
```

