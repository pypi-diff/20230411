# Comparing `tmp/oc4idskit-0.0.2.tar.gz` & `tmp/oc4idskit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc4idskit-0.0.2.tar", last modified: Thu Jan 13 03:46:39 2022, max compression
+gzip compressed data, was "oc4idskit-0.0.3.tar", last modified: Tue Apr 11 18:44:05 2023, max compression
```

## Comparing `oc4idskit-0.0.2.tar` & `oc4idskit-0.0.3.tar`

### file list

```diff
@@ -1,106 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12103 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/oc4idskit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/oc4idskit/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/oc4idskit/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/commands/combine_project_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/commands/convert_from_ocds.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/cli/commands/split_project_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/combine.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    36511 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/oc4idskit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/oc4idskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-13 03:46:39.000000 oc4idskit-0.0.2/oc4idskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.257973 oc4idskit-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_additional_classifications.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_administrative_entity.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_approval.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_fail.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_buyer_role.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_active.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_closed.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_pre_award.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_title.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_value.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_period.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_description.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_release_packages.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_releases.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_cost_estimate.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_not_tender.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_one.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_tender.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_duplicate_public_authority_role.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_environmental_impact.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_final_audit.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_funders.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_funders_budget.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_initial_tranform_state.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_land_and_settlement_impact.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_from_delivery_address.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_from_item_location.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_multiple_releases.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_not_inferred.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_multiple_administrative_entity_in_process.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_needs_assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_number_of_tenderers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_procuring_entity.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_procurment_process.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_project_scope.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_project_scope_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_public_authority_role.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_purpose_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_purpose_one.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_run_all.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_run_all_release_package.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_sector.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   109897 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_supplier.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_title.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    81450 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_title_from_tender.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   110211 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_transforms-test_initial_tranform_state.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    79912 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/cassettes/test_transforms-test_run_all_release_package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/commands/test_combine_project_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/commands/test_convert_from_ocds.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/commands/test_split_project_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 03:46:39.269974 oc4idskit-0.0.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/oc4ids-project-package_minimal.json
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/oc4ids-project_minimal.json
--rw-r--r--   0 runner    (1001) docker     (121)    49954 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/project_package.json
--rw-r--r--   0 runner    (1001) docker     (121)    30843 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/project_package_combined.json
--rw-r--r--   0 runner    (1001) docker     (121)    31422 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/project_package_split.json
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/release-package_additional-contact-points.json
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/fixtures/release_1.1.json
--rw-r--r--   0 runner    (1001) docker     (121)    65251 2022-01-13 03:46:31.000000 oc4idskit-0.0.2/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.401444 oc4idskit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 18:44:05.401444 oc4idskit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.377443 oc4idskit-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.381443 oc4idskit-0.0.3/oc4idskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.381443 oc4idskit-0.0.3/oc4idskit/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/commands/combine_project_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/commands/convert_from_ocds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/commands/split_project_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/oc4idskit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.381443 oc4idskit-0.0.3/oc4idskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 18:44:05.000000 oc4idskit-0.0.3/oc4idskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 18:44:05.401444 oc4idskit-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.381443 oc4idskit-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.397443 oc4idskit-0.0.3/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_additional_classifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_administrative_entity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_approval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_fail.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_buyer_role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_active.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_closed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_pre_award.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_period.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_release_packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_releases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_cost_estimate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_not_tender.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_one.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_tender.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_duplicate_public_authority_role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_environmental_impact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_final_audit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_funders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_funders_budget.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_initial_transform_state.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_land_and_settlement_impact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_from_delivery_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_from_item_location.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_multiple_releases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_not_inferred.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_multiple_administrative_entity_in_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_needs_assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_number_of_tenderers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_procuring_entity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_procurment_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_project_scope.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_project_scope_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_public_authority_role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_purpose_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_purpose_one.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_run_all.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_run_all_release_package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_sector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   109897 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_supplier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    81450 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_title_from_tender.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   110211 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_transforms-test_initial_transform_state.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    79912 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/cassettes/test_transforms-test_run_all_release_package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.401444 oc4idskit-0.0.3/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/commands/test_combine_project_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/commands/test_convert_from_ocds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/commands/test_split_project_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:44:05.401444 oc4idskit-0.0.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/oc4ids-project-package_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/oc4ids-project_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49954 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/project_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/project_package_combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31422 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/project_package_split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/release-package_additional-contact-points.json
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/fixtures/release_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65248 2023-04-11 18:43:49.000000 oc4idskit-0.0.3/tests/test_transforms.py
```

### Comparing `oc4idskit-0.0.2/LICENSE` & `oc4idskit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/PKG-INFO` & `oc4idskit-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: oc4idskit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A suite of command-line tools for working with OC4IDS data
 Home-page: https://github.com/open-contracting/oc4idskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
@@ -35,9 +34,7 @@
    :target: https://pypi.org/project/oc4idskit/
 .. |Build Status| image:: https://github.com/open-contracting/oc4idskit/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/oc4idskit/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/oc4idskit/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/oc4idskit?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/oc4idskit.svg
    :target: https://pypi.org/project/oc4idskit/
-
-
```

### Comparing `oc4idskit-0.0.2/README.rst` & `oc4idskit-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/docs/Makefile` & `oc4idskit-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/docs/cli.rst` & `oc4idskit-0.0.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/docs/conf.py` & `oc4idskit-0.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OC4IDS Kit"
 copyright = "2021, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.0.2"
+version = "0.0.3"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `oc4idskit-0.0.2/oc4idskit/cli/commands/combine_project_packages.py` & `oc4idskit-0.0.3/oc4idskit/commands/combine_project_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ocdskit.cli.commands.base import OCDSCommand
+from ocdskit.commands.base import OCDSCommand
 
 from oc4idskit.combine import combine_project_packages
 
 
 class Command(OCDSCommand):
     name = 'combine-project-packages'
     help = 'reads project packages from standard input, collects projects, and prints one project package'
```

### Comparing `oc4idskit-0.0.2/oc4idskit/cli/commands/convert_from_ocds.py` & `oc4idskit-0.0.3/oc4idskit/commands/convert_from_ocds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
-from ocdskit.cli.commands.base import OCDSCommand
 from ocdskit.combine import _package
+from ocdskit.commands.base import OCDSCommand
 
 from oc4idskit import transforms
 
 logger = logging.getLogger("oc4idskit")
 
 
 class Command(OCDSCommand):
```

### Comparing `oc4idskit-0.0.2/oc4idskit/cli/commands/split_project_packages.py` & `oc4idskit-0.0.3/oc4idskit/commands/split_project_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ocdskit.cli.commands.base import OCDSCommand
+from ocdskit.commands.base import OCDSCommand
 
 
 class Command(OCDSCommand):
     name = "split-project-packages"
     help = "reads project packages from standard input, and prints many record packages for each"
 
     def add_arguments(self):
```

### Comparing `oc4idskit-0.0.2/oc4idskit/combine.py` & `oc4idskit-0.0.3/oc4idskit/combine.py`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/oc4idskit/transforms.py` & `oc4idskit-0.0.3/oc4idskit/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return ""
 
 
 def run_transforms(config, releases, project_id=None, records=None, output=None):
     """
     Transforms a list of OCDS releases into a OC4IDS project.
 
-    :param dict config: contains optional tranform options.
+    :param dict config: contains optional transform options.
     :param list releases: list of OCDS releases or release packages
     :param string project_id: project ID of resulting project
     :param list records: pre computed list of records
     :param dict output: initial project output template project where transformed data will be added
     """
     transforms_to_run = []
 
@@ -394,16 +394,16 @@
         state.output["title"] = concat_ocid_and_string(state, "/tender/title")
     elif len(titles) == 1:
         state.output["title"] = titles[0]
 
 
 def contracting_process_setup(state):
     """
-    This will initailly create the contracting process objects and the summary object within. All transforms that use
-    contracting processes need to run this tranform first.
+    This will initially create the contracting process objects and the summary object within. All transforms that use
+    contracting processes need to run this transform first.
     """
     state.output["contractingProcesses"] = []
 
     for compiled_release in state.compiled_releases:
         contracting_process = {
             "id": compiled_release.get("ocid"),
             "summary": {
@@ -433,15 +433,15 @@
     ):
         procuring_entities = []
         for party in check_type(compiled_release.get("parties"), list):
             if "procuringEntity" in check_type(party.get("roles"), list):
                 procuring_entities.append(party)
         if len(procuring_entities) > 1:
             logger.warning(
-                "More than one procuringEntity in contractingProcesses with ocid %s skipping tranform",
+                "More than one procuringEntity in contractingProcesses with ocid %s skipping transform",
                 compiled_release.get("ocid"),
             )
             continue
         if procuring_entities:
             contracting_process["summary"].setdefault("tender", {})
             organization_reference = {"id": procuring_entities[0].get("_new_id")}
             name = procuring_entities[0].get("name")
@@ -463,15 +463,15 @@
     ):
         administrative_entities = []
         for party in check_type(compiled_release.get("parties"), list):
             if "administrativeEntity" in check_type(party.get("roles"), list):
                 administrative_entities.append(party)
         if len(administrative_entities) > 1:
             logger.warning(
-                "More than one administrativeEntity in contractingProcesses with ocid %s skipping tranform",
+                "More than one administrativeEntity in contractingProcesses with ocid %s skipping transform",
                 compiled_release.get("ocid"),
             )
             continue
         if administrative_entities:
             contracting_process["summary"].setdefault("tender", {})
             contracting_process["summary"]["tender"]["administrativeEntity"] = {
                 "id": administrative_entities[0].get("_new_id"),
```

### Comparing `oc4idskit-0.0.2/oc4idskit/util.py` & `oc4idskit-0.0.3/oc4idskit/util.py`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/oc4idskit.egg-info/PKG-INFO` & `oc4idskit-0.0.3/oc4idskit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: oc4idskit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A suite of command-line tools for working with OC4IDS data
 Home-page: https://github.com/open-contracting/oc4idskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
@@ -35,9 +34,7 @@
    :target: https://pypi.org/project/oc4idskit/
 .. |Build Status| image:: https://github.com/open-contracting/oc4idskit/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/oc4idskit/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/oc4idskit/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/oc4idskit?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/oc4idskit.svg
    :target: https://pypi.org/project/oc4idskit/
-
-
```

### Comparing `oc4idskit-0.0.2/oc4idskit.egg-info/SOURCES.txt` & `oc4idskit-0.0.3/oc4idskit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
+setup.cfg
 docs/Makefile
 docs/changelog.rst
 docs/cli.rst
 docs/conf.py
 docs/index.rst
 docs/library.rst
 docs/requirements.txt
 oc4idskit/__init__.py
+oc4idskit/__main__.py
 oc4idskit/combine.py
 oc4idskit/exceptions.py
 oc4idskit/transforms.py
 oc4idskit/util.py
 oc4idskit.egg-info/PKG-INFO
 oc4idskit.egg-info/SOURCES.txt
 oc4idskit.egg-info/dependency_links.txt
 oc4idskit.egg-info/entry_points.txt
 oc4idskit.egg-info/requires.txt
 oc4idskit.egg-info/top_level.txt
-oc4idskit/cli/__init__.py
-oc4idskit/cli/__main__.py
-oc4idskit/cli/commands/__init__.py
-oc4idskit/cli/commands/combine_project_packages.py
-oc4idskit/cli/commands/convert_from_ocds.py
-oc4idskit/cli/commands/split_project_packages.py
+oc4idskit/commands/__init__.py
+oc4idskit/commands/combine_project_packages.py
+oc4idskit/commands/convert_from_ocds.py
+oc4idskit/commands/split_project_packages.py
 tests/__init__.py
 tests/conftest.py
 tests/test_transforms.py
 tests/cassettes/test_oc4ids_transforms-test_additional_classifications.yaml
 tests/cassettes/test_oc4ids_transforms-test_administrative_entity.yaml
 tests/cassettes/test_oc4ids_transforms-test_budget.yaml
 tests/cassettes/test_oc4ids_transforms-test_budget_approval.yaml
@@ -51,15 +51,15 @@
 tests/cassettes/test_oc4ids_transforms-test_description_one.yaml
 tests/cassettes/test_oc4ids_transforms-test_description_tender.yaml
 tests/cassettes/test_oc4ids_transforms-test_duplicate_public_authority_role.yaml
 tests/cassettes/test_oc4ids_transforms-test_environmental_impact.yaml
 tests/cassettes/test_oc4ids_transforms-test_final_audit.yaml
 tests/cassettes/test_oc4ids_transforms-test_funders.yaml
 tests/cassettes/test_oc4ids_transforms-test_funders_budget.yaml
-tests/cassettes/test_oc4ids_transforms-test_initial_tranform_state.yaml
+tests/cassettes/test_oc4ids_transforms-test_initial_transform_state.yaml
 tests/cassettes/test_oc4ids_transforms-test_land_and_settlement_impact.yaml
 tests/cassettes/test_oc4ids_transforms-test_location.yaml
 tests/cassettes/test_oc4ids_transforms-test_location_from_delivery_address.yaml
 tests/cassettes/test_oc4ids_transforms-test_location_from_item_location.yaml
 tests/cassettes/test_oc4ids_transforms-test_location_multiple.yaml
 tests/cassettes/test_oc4ids_transforms-test_location_multiple_releases.yaml
 tests/cassettes/test_oc4ids_transforms-test_location_not_inferred.yaml
@@ -75,15 +75,15 @@
 tests/cassettes/test_oc4ids_transforms-test_purpose_one.yaml
 tests/cassettes/test_oc4ids_transforms-test_run_all.yaml
 tests/cassettes/test_oc4ids_transforms-test_run_all_release_package.yaml
 tests/cassettes/test_oc4ids_transforms-test_sector.yaml
 tests/cassettes/test_oc4ids_transforms-test_supplier.yaml
 tests/cassettes/test_oc4ids_transforms-test_title.yaml
 tests/cassettes/test_oc4ids_transforms-test_title_from_tender.yaml
-tests/cassettes/test_transforms-test_initial_tranform_state.yaml
+tests/cassettes/test_transforms-test_initial_transform_state.yaml
 tests/cassettes/test_transforms-test_run_all_release_package.yaml
 tests/commands/__init__.py
 tests/commands/test_combine_project_packages.py
 tests/commands/test_convert_from_ocds.py
 tests/commands/test_split_project_packages.py
 tests/fixtures/oc4ids-project-package_minimal.json
 tests/fixtures/oc4ids-project_minimal.json
```

### Comparing `oc4idskit-0.0.2/tests/__init__.py` & `oc4idskit-0.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_additional_classifications.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_additional_classifications.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_administrative_entity.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_administrative_entity.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_approval.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_approval.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_fail.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_fail.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_budget_multiple.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_budget_multiple.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_buyer_role.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_buyer_role.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_active.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_active.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_closed.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_closed.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_status_pre_award.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_status_pre_award.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_title.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_title.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contract_value.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contract_value.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_period.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_period.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_description.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_description.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_release_packages.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_release_packages.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_releases.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_contracting_process_setup_releases.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_cost_estimate.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_cost_estimate.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_multiple.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_multiple.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_not_tender.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_not_tender.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_one.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_one.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_description_tender.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_description_tender.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_duplicate_public_authority_role.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_duplicate_public_authority_role.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_environmental_impact.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_environmental_impact.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_final_audit.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_final_audit.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_funders.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_funders.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_funders_budget.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_funders_budget.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_initial_tranform_state.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_initial_transform_state.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_land_and_settlement_impact.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_land_and_settlement_impact.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_from_delivery_address.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_from_delivery_address.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_from_item_location.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_from_item_location.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_multiple.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_multiple.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_multiple_releases.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_multiple_releases.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_location_not_inferred.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_location_not_inferred.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_multiple_administrative_entity_in_process.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_multiple_administrative_entity_in_process.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_needs_assessment.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_needs_assessment.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_number_of_tenderers.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_number_of_tenderers.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_procuring_entity.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_procuring_entity.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_procurment_process.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_procurment_process.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_project_scope.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_project_scope.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_project_scope_summary.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_project_scope_summary.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_public_authority_role.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_public_authority_role.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_purpose_multiple.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_purpose_multiple.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_purpose_one.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_purpose_one.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_run_all.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_run_all.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_run_all_release_package.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_run_all_release_package.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_sector.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_sector.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_supplier.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_supplier.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_title.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_title.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_oc4ids_transforms-test_title_from_tender.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_oc4ids_transforms-test_title_from_tender.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_transforms-test_initial_tranform_state.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_transforms-test_initial_transform_state.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/cassettes/test_transforms-test_run_all_release_package.yaml` & `oc4idskit-0.0.3/tests/cassettes/test_transforms-test_run_all_release_package.yaml`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/commands/test_convert_from_ocds.py` & `oc4idskit-0.0.3/tests/commands/test_convert_from_ocds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from oc4idskit.cli.__main__ import main
+from oc4idskit.__main__ import main
 from tests import assert_streaming
 
 
 def test_command(capsys, monkeypatch):
     assert_streaming(
         capsys,
         monkeypatch,
```

### Comparing `oc4idskit-0.0.2/tests/fixtures/oc4ids-project-package_minimal.json` & `oc4idskit-0.0.3/tests/fixtures/oc4ids-project-package_minimal.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/fixtures/oc4ids-project_minimal.json` & `oc4idskit-0.0.3/tests/fixtures/oc4ids-project_minimal.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/fixtures/project_package.json` & `oc4idskit-0.0.3/tests/fixtures/project_package.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/fixtures/project_package_combined.json` & `oc4idskit-0.0.3/tests/fixtures/project_package_combined.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/fixtures/project_package_split.json` & `oc4idskit-0.0.3/tests/fixtures/project_package_split.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/fixtures/release-package_additional-contact-points.json` & `oc4idskit-0.0.3/tests/fixtures/release-package_additional-contact-points.json`

 * *Files identical despite different names*

### Comparing `oc4idskit-0.0.2/tests/test_transforms.py` & `oc4idskit-0.0.3/tests/test_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 
 from oc4idskit import transforms
 from tests import read
 
 
 @pytest.mark.vcr()
-def test_initial_tranform_state():
+def test_initial_transform_state():
     releases = json.loads(read("release-package_additional-contact-points.json"))[
         "releases"
     ]
     transform_state = transforms.InitialTransformState(releases, "1")
     assert len(transform_state.compiled_releases) == 1
     assert len(transform_state.releases_by_ocid["ocds-213czf-1"]) == 2
 
@@ -285,18 +285,18 @@
             },
         }
     )
 
     output = transforms._run_transforms(releases, "1", transforms=[transforms.sector])
     assert output["sector"] == ["COFOG-04.5.1"]
 
-    # 2 contracting processes but differnt sector
+    # 2 contracting processes but different sector
     releases[1]["planning"]["project"]["sector"]["id"] = "2"
     output = transforms._run_transforms(releases, "1", transforms=[transforms.sector])
-    assert set(output["sector"]) == set(["COFOG-04.5.1", "COFOG-2"])
+    assert set(output["sector"]) == {"COFOG-04.5.1", "COFOG-2"}
 
 
 @pytest.mark.vcr()
 def test_additional_classifications():
     releases = [
         {
             "ocid": "ocds-213czf-1",
```

