# Comparing `tmp/vortexasdk-0.9.1.tar.gz` & `tmp/vortexasdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vortexasdk-0.9.1.tar", last modified: Mon Dec  9 11:47:52 2019, max compression
+gzip compressed data, was "dist/vortexasdk-0.9.2.tar", last modified: Wed Dec 11 09:51:44 2019, max compression
```

## Comparing `vortexasdk-0.9.1.tar` & `vortexasdk-0.9.2.tar`

### file list

```diff
@@ -1,139 +1,115 @@
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/
--rw-r--r--   0 kit        (501) staff       (20)     3334 2019-11-28 17:53:04.000000 vortexasdk-0.9.1/.all-contributorsrc
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/.circleci/
--rw-r--r--   0 kit        (501) staff       (20)     1127 2019-11-28 11:19:37.000000 vortexasdk-0.9.1/.circleci/config.yml
--rw-r--r--   0 kit        (501) staff       (20)     1794 2019-11-27 16:28:28.000000 vortexasdk-0.9.1/.gitignore
--rw-r--r--   0 kit        (501) staff       (20)      473 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 kit        (501) staff       (20)    16646 2019-12-09 11:47:46.000000 vortexasdk-0.9.1/CHANGELOG.md
--rw-r--r--   0 kit        (501) staff       (20)     3370 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 kit        (501) staff       (20)     3031 2019-11-27 16:48:59.000000 vortexasdk-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 kit        (501) staff       (20)    11357 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/LICENSE
--rw-r--r--   0 kit        (501) staff       (20)       63 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/MANIFEST.in
--rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/PKG-INFO
--rw-r--r--   0 kit        (501) staff       (20)     7259 2019-11-28 17:53:04.000000 vortexasdk-0.9.1/README.md
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/art/
--rw-r--r--   0 kit        (501) staff       (20)     5430 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/art/favicon.ico
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/docs/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/docs/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1875 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/docs/autogen.py
--rwxr-xr-x   0 kit        (501) staff       (20)       85 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/docs/build_docs.sh
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/docs/config/
--rw-r--r--   0 kit        (501) staff       (20)      753 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/docs/config/config.md
--rwxr-xr-x   0 kit        (501) staff       (20)       89 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/docs/deploy_docs.sh
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/docs/endpoints/
--rw-r--r--   0 kit        (501) staff       (20)      888 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/docs/endpoints/about-endpoints.md
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/docs/examples/
--rw-r--r--   0 kit        (501) staff       (20)     1297 2019-11-28 10:45:40.000000 vortexasdk-0.9.1/docs/examples/1_china.py
--rw-r--r--   0 kit        (501) staff       (20)     9911 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/docs/examples/2_all_vessel_movements.py
--rwxr-xr-x   0 kit        (501) staff       (20)      148 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/docs/serve_docs.sh
--rw-r--r--   0 kit        (501) staff       (20)      150 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/docs/utils.py
--rw-r--r--   0 kit        (501) staff       (20)     2153 2019-12-05 16:07:01.000000 vortexasdk-0.9.1/pydocmd.yml
--rw-r--r--   0 kit        (501) staff       (20)      174 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/pyproject.toml
--rw-r--r--   0 kit        (501) staff       (20)       67 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/pytest.ini
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/scripts/
--rwxr-xr-x   0 kit        (501) staff       (20)      652 2019-11-28 11:24:38.000000 vortexasdk-0.9.1/scripts/export_package.sh
--rwxr-xr-x   0 kit        (501) staff       (20)     1061 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/scripts/generate_stubs.sh
--rw-r--r--   0 kit        (501) staff       (20)      300 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/setup.cfg
--rw-r--r--   0 kit        (501) staff       (20)     1091 2019-12-09 11:46:58.000000 vortexasdk-0.9.1/setup.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/tests/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/__init__.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/tests/api/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/__init__.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/tests/api/examples/
--rw-r--r--   0 kit        (501) staff       (20)      443 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/cargo_event_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     2318 2019-12-06 14:39:12.000000 vortexasdk-0.9.1/tests/api/examples/cargo_movements.json
--rw-r--r--   0 kit        (501) staff       (20)      189 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/corporate_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)      168 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/corporate_entity2.json
--rw-r--r--   0 kit        (501) staff       (20)      599 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/corporations.json
--rw-r--r--   0 kit        (501) staff       (20)      170 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/geography_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     1768 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/geography_reference.json
--rw-r--r--   0 kit        (501) staff       (20)      192 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/product_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     1030 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/products.json
--rw-r--r--   0 kit        (501) staff       (20)      952 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/vessel_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     7818 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/vessel_movements.json
--rw-r--r--   0 kit        (501) staff       (20)     3322 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/vessels.json
--rw-r--r--   0 kit        (501) staff       (20)     2126 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/examples/vessels_reference.json
--rw-r--r--   0 kit        (501) staff       (20)     1121 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_cargo_event_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     7820 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_cargo_movement.py
--rw-r--r--   0 kit        (501) staff       (20)      676 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_corporate_entity.py
--rw-r--r--   0 kit        (501) staff       (20)      352 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_from_dict_mixin.py
--rw-r--r--   0 kit        (501) staff       (20)      729 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_geography_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     1042 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_product_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     1362 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/api/test_vessel_entity.py
--rw-r--r--   0 kit        (501) staff       (20)    18110 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/tests/api/test_vessel_movement.py
--rw-r--r--   0 kit        (501) staff       (20)       58 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/config.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/tests/conversions/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/conversions/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1312 2019-12-05 09:05:58.000000 vortexasdk-0.9.1/tests/conversions/test_conversions.py
--rw-r--r--   0 kit        (501) staff       (20)     1432 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/conversions/test_convert_vessels.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/tests/endpoints/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/endpoints/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     4893 2019-12-09 11:46:37.000000 vortexasdk-0.9.1/tests/endpoints/test_cargo_movements_real.py
--rw-r--r--   0 kit        (501) staff       (20)      412 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/tests/endpoints/test_corporations_real.py
--rw-r--r--   0 kit        (501) staff       (20)      800 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/endpoints/test_corporations_search_result.py
--rw-r--r--   0 kit        (501) staff       (20)      734 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/tests/endpoints/test_geographies_real.py
--rw-r--r--   0 kit        (501) staff       (20)      271 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/endpoints/test_products.py
--rw-r--r--   0 kit        (501) staff       (20)     2542 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/tests/endpoints/test_products_real.py
--rw-r--r--   0 kit        (501) staff       (20)      551 2019-12-05 09:05:58.000000 vortexasdk-0.9.1/tests/endpoints/test_reference_endpoints_real.py
--rw-r--r--   0 kit        (501) staff       (20)     1797 2019-12-05 10:08:34.000000 vortexasdk-0.9.1/tests/endpoints/test_vessel_movements_real.py
--rw-r--r--   0 kit        (501) staff       (20)      316 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/endpoints/test_vessels.py
--rw-r--r--   0 kit        (501) staff       (20)     2133 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/tests/endpoints/test_vessels_real.py
--rw-r--r--   0 kit        (501) staff       (20)     5483 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/endpoints/test_vessels_search_result.py
--rw-r--r--   0 kit        (501) staff       (20)     1306 2019-12-05 09:05:58.000000 vortexasdk-0.9.1/tests/mock_client.py
--rw-r--r--   0 kit        (501) staff       (20)     1234 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/test_id.py
--rw-r--r--   0 kit        (501) staff       (20)      434 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/test_to_ISODate.py
--rw-r--r--   0 kit        (501) staff       (20)      543 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/test_utils.py
--rw-r--r--   0 kit        (501) staff       (20)      469 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/tests/testcases.py
--rw-r--r--   0 kit        (501) staff       (20)      660 2019-12-09 11:46:30.000000 vortexasdk-0.9.1/tests/timer.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk/
--rw-r--r--   0 kit        (501) staff       (20)      166 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)      375 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/abstract_client.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk/api/
--rw-r--r--   0 kit        (501) staff       (20)      605 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1367 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/cargo_movement.py
--rw-r--r--   0 kit        (501) staff       (20)      693 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/corporation.py
--rw-r--r--   0 kit        (501) staff       (20)     3143 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/vortexasdk/api/entity_flattening.py
--rw-r--r--   0 kit        (501) staff       (20)     1857 2019-11-27 18:27:43.000000 vortexasdk-0.9.1/vortexasdk/api/entity_serializing.py
--rw-r--r--   0 kit        (501) staff       (20)      979 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/geography.py
--rw-r--r--   0 kit        (501) staff       (20)      615 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/id.py
--rw-r--r--   0 kit        (501) staff       (20)      702 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/product.py
--rw-r--r--   0 kit        (501) staff       (20)      905 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/api/search_result.py
--rw-r--r--   0 kit        (501) staff       (20)      459 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/serdes.py
--rw-r--r--   0 kit        (501) staff       (20)     1917 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/api/shared_types.py
--rw-r--r--   0 kit        (501) staff       (20)     1688 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/vessel.py
--rw-r--r--   0 kit        (501) staff       (20)     1079 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/api/vessel_movement.py
--rw-r--r--   0 kit        (501) staff       (20)     4576 2019-12-09 11:46:37.000000 vortexasdk-0.9.1/vortexasdk/client.py
--rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-06 12:16:12.000000 vortexasdk-0.9.1/vortexasdk/config.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk/conversions/
--rw-r--r--   0 kit        (501) staff       (20)      322 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/conversions/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1129 2019-11-27 16:28:28.000000 vortexasdk-0.9.1/vortexasdk/conversions/conversions.py
--rw-r--r--   0 kit        (501) staff       (20)      571 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/conversions/corporations.py
--rw-r--r--   0 kit        (501) staff       (20)      944 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/conversions/geographies.py
--rw-r--r--   0 kit        (501) staff       (20)      549 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/conversions/products.py
--rw-r--r--   0 kit        (501) staff       (20)     1614 2019-11-29 16:31:20.000000 vortexasdk-0.9.1/vortexasdk/conversions/vessels.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk/endpoints/
--rw-r--r--   0 kit        (501) staff       (20)      371 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/endpoints/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)    10057 2019-12-06 11:40:20.000000 vortexasdk-0.9.1/vortexasdk/endpoints/cargo_movements.py
--rw-r--r--   0 kit        (501) staff       (20)    32511 2019-12-05 10:08:34.000000 vortexasdk-0.9.1/vortexasdk/endpoints/cargo_movements_result.py
--rw-r--r--   0 kit        (501) staff       (20)     2603 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/vortexasdk/endpoints/corporations.py
--rw-r--r--   0 kit        (501) staff       (20)     1247 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/endpoints/corporations_result.py
--rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-05 16:07:01.000000 vortexasdk-0.9.1/vortexasdk/endpoints/endpoints.py
--rw-r--r--   0 kit        (501) staff       (20)     2378 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/vortexasdk/endpoints/geographies.py
--rw-r--r--   0 kit        (501) staff       (20)     1223 2019-12-05 16:04:14.000000 vortexasdk-0.9.1/vortexasdk/endpoints/geographies_result.py
--rw-r--r--   0 kit        (501) staff       (20)     3580 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/vortexasdk/endpoints/products.py
--rw-r--r--   0 kit        (501) staff       (20)     1378 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/endpoints/products_result.py
--rw-r--r--   0 kit        (501) staff       (20)     6776 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/vortexasdk/endpoints/vessel_movements.py
--rw-r--r--   0 kit        (501) staff       (20)    21116 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/vortexasdk/endpoints/vessel_movements_result.py
--rw-r--r--   0 kit        (501) staff       (20)     4434 2019-12-05 16:07:03.000000 vortexasdk-0.9.1/vortexasdk/endpoints/vessels.py
--rw-r--r--   0 kit        (501) staff       (20)     1218 2019-11-28 11:15:05.000000 vortexasdk-0.9.1/vortexasdk/endpoints/vessels_result.py
--rw-r--r--   0 kit        (501) staff       (20)      121 2019-12-05 09:05:58.000000 vortexasdk-0.9.1/vortexasdk/exceptions.py
--rw-r--r--   0 kit        (501) staff       (20)      785 2019-11-27 16:28:28.000000 vortexasdk-0.9.1/vortexasdk/logger.py
--rw-r--r--   0 kit        (501) staff       (20)     2128 2019-12-05 09:05:58.000000 vortexasdk-0.9.1/vortexasdk/operations.py
--rw-r--r--   0 kit        (501) staff       (20)     1118 2019-12-09 11:46:37.000000 vortexasdk-0.9.1/vortexasdk/retry_session.py
--rw-r--r--   0 kit        (501) staff       (20)      399 2019-11-26 16:53:26.000000 vortexasdk-0.9.1/vortexasdk/utils.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/
--rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/PKG-INFO
--rw-r--r--   0 kit        (501) staff       (20)     3600 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/SOURCES.txt
--rw-r--r--   0 kit        (501) staff       (20)        1 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/dependency_links.txt
--rw-r--r--   0 kit        (501) staff       (20)      184 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/requires.txt
--rw-r--r--   0 kit        (501) staff       (20)       22 2019-12-09 11:47:52.000000 vortexasdk-0.9.1/vortexasdk.egg-info/top_level.txt
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/
+-rw-r--r--   0 kit        (501) staff       (20)    17832 2019-12-11 09:50:07.000000 vortexasdk-0.9.2/CHANGELOG.md
+-rw-r--r--   0 kit        (501) staff       (20)     3370 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 kit        (501) staff       (20)     3031 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 kit        (501) staff       (20)       63 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/MANIFEST.in
+-rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/PKG-INFO
+-rw-r--r--   0 kit        (501) staff       (20)     7259 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/README.md
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/docs/
+-rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)     1875 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/autogen.py
+-rw-r--r--   0 kit        (501) staff       (20)      150 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/utils.py
+-rw-r--r--   0 kit        (501) staff       (20)      300 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/setup.cfg
+-rw-r--r--   0 kit        (501) staff       (20)     1091 2019-12-11 09:48:27.000000 vortexasdk-0.9.2/setup.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/
+-rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/__init__.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/api/
+-rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/__init__.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/api/examples/
+-rw-r--r--   0 kit        (501) staff       (20)      443 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/cargo_event_entity1.json
+-rw-r--r--   0 kit        (501) staff       (20)     2318 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/cargo_movements.json
+-rw-r--r--   0 kit        (501) staff       (20)      189 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporate_entity1.json
+-rw-r--r--   0 kit        (501) staff       (20)      168 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporate_entity2.json
+-rw-r--r--   0 kit        (501) staff       (20)      599 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporations.json
+-rw-r--r--   0 kit        (501) staff       (20)      170 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/geography_entity1.json
+-rw-r--r--   0 kit        (501) staff       (20)     1768 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/geography_reference.json
+-rw-r--r--   0 kit        (501) staff       (20)      192 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/product_entity1.json
+-rw-r--r--   0 kit        (501) staff       (20)     1030 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/products.json
+-rw-r--r--   0 kit        (501) staff       (20)      952 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessel_entity1.json
+-rw-r--r--   0 kit        (501) staff       (20)     7818 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessel_movements.json
+-rw-r--r--   0 kit        (501) staff       (20)     3322 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessels.json
+-rw-r--r--   0 kit        (501) staff       (20)     2126 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessels_reference.json
+-rw-r--r--   0 kit        (501) staff       (20)     1121 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_cargo_event_entity.py
+-rw-r--r--   0 kit        (501) staff       (20)     7820 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/api/test_cargo_movement.py
+-rw-r--r--   0 kit        (501) staff       (20)      676 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_corporate_entity.py
+-rw-r--r--   0 kit        (501) staff       (20)      352 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_from_dict_mixin.py
+-rw-r--r--   0 kit        (501) staff       (20)      729 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_geography_entity.py
+-rw-r--r--   0 kit        (501) staff       (20)     1042 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_product_entity.py
+-rw-r--r--   0 kit        (501) staff       (20)     1362 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_vessel_entity.py
+-rw-r--r--   0 kit        (501) staff       (20)    18110 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_vessel_movement.py
+-rw-r--r--   0 kit        (501) staff       (20)       58 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/config.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/conversions/
+-rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)     1312 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/test_conversions.py
+-rw-r--r--   0 kit        (501) staff       (20)     1432 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/test_convert_vessels.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/endpoints/
+-rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)     4893 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_cargo_movements_real.py
+-rw-r--r--   0 kit        (501) staff       (20)      412 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_corporations_real.py
+-rw-r--r--   0 kit        (501) staff       (20)      800 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_corporations_search_result.py
+-rw-r--r--   0 kit        (501) staff       (20)      734 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_geographies_real.py
+-rw-r--r--   0 kit        (501) staff       (20)      271 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_products.py
+-rw-r--r--   0 kit        (501) staff       (20)     2542 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_products_real.py
+-rw-r--r--   0 kit        (501) staff       (20)      551 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_reference_endpoints_real.py
+-rw-r--r--   0 kit        (501) staff       (20)     1797 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_vessel_movements_real.py
+-rw-r--r--   0 kit        (501) staff       (20)      316 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels.py
+-rw-r--r--   0 kit        (501) staff       (20)     2439 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels_real.py
+-rw-r--r--   0 kit        (501) staff       (20)     5483 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels_search_result.py
+-rw-r--r--   0 kit        (501) staff       (20)     1306 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/mock_client.py
+-rw-r--r--   0 kit        (501) staff       (20)     1234 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_id.py
+-rw-r--r--   0 kit        (501) staff       (20)      434 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_to_ISODate.py
+-rw-r--r--   0 kit        (501) staff       (20)      543 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_utils.py
+-rw-r--r--   0 kit        (501) staff       (20)      469 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/testcases.py
+-rw-r--r--   0 kit        (501) staff       (20)      660 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/timer.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/
+-rw-r--r--   0 kit        (501) staff       (20)      166 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)      375 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/abstract_client.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/api/
+-rw-r--r--   0 kit        (501) staff       (20)      605 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)     1367 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/cargo_movement.py
+-rw-r--r--   0 kit        (501) staff       (20)      693 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/corporation.py
+-rw-r--r--   0 kit        (501) staff       (20)     3143 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/entity_flattening.py
+-rw-r--r--   0 kit        (501) staff       (20)     1857 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/entity_serializing.py
+-rw-r--r--   0 kit        (501) staff       (20)      989 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/api/geography.py
+-rw-r--r--   0 kit        (501) staff       (20)      615 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/id.py
+-rw-r--r--   0 kit        (501) staff       (20)      702 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/product.py
+-rw-r--r--   0 kit        (501) staff       (20)      905 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/search_result.py
+-rw-r--r--   0 kit        (501) staff       (20)      459 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/serdes.py
+-rw-r--r--   0 kit        (501) staff       (20)     1917 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/api/shared_types.py
+-rw-r--r--   0 kit        (501) staff       (20)     1688 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/vessel.py
+-rw-r--r--   0 kit        (501) staff       (20)     1079 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/vessel_movement.py
+-rw-r--r--   0 kit        (501) staff       (20)     4634 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/vortexasdk/client.py
+-rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/config.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/conversions/
+-rw-r--r--   0 kit        (501) staff       (20)      322 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/conversions/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)     1129 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/conversions/conversions.py
+-rw-r--r--   0 kit        (501) staff       (20)      501 2019-12-11 09:35:37.000000 vortexasdk-0.9.2/vortexasdk/conversions/corporations.py
+-rw-r--r--   0 kit        (501) staff       (20)      668 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/conversions/geographies.py
+-rw-r--r--   0 kit        (501) staff       (20)      479 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/conversions/products.py
+-rw-r--r--   0 kit        (501) staff       (20)     1544 2019-12-11 09:35:37.000000 vortexasdk-0.9.2/vortexasdk/conversions/vessels.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/endpoints/
+-rw-r--r--   0 kit        (501) staff       (20)      371 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/__init__.py
+-rw-r--r--   0 kit        (501) staff       (20)    10213 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements.py
+-rw-r--r--   0 kit        (501) staff       (20)    32511 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements_result.py
+-rw-r--r--   0 kit        (501) staff       (20)     2598 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/endpoints/corporations.py
+-rw-r--r--   0 kit        (501) staff       (20)     1247 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/corporations_result.py
+-rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/endpoints.py
+-rw-r--r--   0 kit        (501) staff       (20)     2383 2019-12-10 19:19:59.000000 vortexasdk-0.9.2/vortexasdk/endpoints/geographies.py
+-rw-r--r--   0 kit        (501) staff       (20)     1223 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/geographies_result.py
+-rw-r--r--   0 kit        (501) staff       (20)     3586 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/endpoints/products.py
+-rw-r--r--   0 kit        (501) staff       (20)     1378 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/products_result.py
+-rw-r--r--   0 kit        (501) staff       (20)     6836 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements.py
+-rw-r--r--   0 kit        (501) staff       (20)    21116 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements_result.py
+-rw-r--r--   0 kit        (501) staff       (20)     4515 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessels.py
+-rw-r--r--   0 kit        (501) staff       (20)     1218 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessels_result.py
+-rw-r--r--   0 kit        (501) staff       (20)      121 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/exceptions.py
+-rw-r--r--   0 kit        (501) staff       (20)      785 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/logger.py
+-rw-r--r--   0 kit        (501) staff       (20)     2154 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/operations.py
+-rw-r--r--   0 kit        (501) staff       (20)     1118 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/retry_session.py
+-rw-r--r--   0 kit        (501) staff       (20)      399 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/utils.py
+drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/
+-rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/PKG-INFO
+-rw-r--r--   0 kit        (501) staff       (20)     3231 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 kit        (501) staff       (20)        1 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 kit        (501) staff       (20)      184 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/requires.txt
+-rw-r--r--   0 kit        (501) staff       (20)       22 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/top_level.txt
```

### Comparing `vortexasdk-0.9.1/CHANGELOG.md` & `vortexasdk-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+## [0.9.2](https://github.com/V0RT3X4/python-sdk/tree/0.9.2) (2019-12-11)
+
+[Full Changelog](https://github.com/V0RT3X4/python-sdk/compare/0.9.1...0.9.2)
+
+**Fixed bugs:**
+
+- Fix SDK Stability issues [\#127](https://github.com/V0RT3X4/python-sdk/issues/127)
+
+**Merged pull requests:**
+
+- refactor: Call doctests using pytest [\#137](https://github.com/V0RT3X4/python-sdk/pull/137) ([KitBurgess](https://github.com/KitBurgess))
+- test: Actually run doctest on all files [\#136](https://github.com/V0RT3X4/python-sdk/pull/136) ([KitBurgess](https://github.com/KitBurgess))
+- fix: search on vessel class is case insensitive [\#135](https://github.com/V0RT3X4/python-sdk/pull/135) ([Natday](https://github.com/Natday))
+- docs: Check doctests are valid code [\#133](https://github.com/V0RT3X4/python-sdk/pull/133) ([KitBurgess](https://github.com/KitBurgess))
+- docs: Add crude from saudi arabia to india example [\#132](https://github.com/V0RT3X4/python-sdk/pull/132) ([KitBurgess](https://github.com/KitBurgess))
+- perf: Shuffle offsets inplace for more accurate progress ETA, increas… [\#131](https://github.com/V0RT3X4/python-sdk/pull/131) ([KitBurgess](https://github.com/KitBurgess))
+
 ## [0.9.1](https://github.com/V0RT3X4/python-sdk/tree/0.9.1) (2019-12-09)
 
 [Full Changelog](https://github.com/V0RT3X4/python-sdk/compare/0.9.0...0.9.1)
 
 **Implemented enhancements:**
 
 - Show loading progress bar [\#123](https://github.com/V0RT3X4/python-sdk/issues/123)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vortexasdk-0.9.1/CODE_OF_CONDUCT.md` & `vortexasdk-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/CONTRIBUTING.md` & `vortexasdk-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/PKG-INFO` & `vortexasdk-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortexasdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Vortexa SDK
 Home-page: https://github.com/V0RT3X4/python-sdk
 Author: Vortexa Developers
 Author-email: developers@vortexa.com
 License: Apache License 2.0
 Description: # VortexaSDK
         [![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vortexasdk Version: 0.9.1 Summary: Vortexa SDK
+Metadata-Version: 2.1 Name: vortexasdk Version: 0.9.2 Summary: Vortexa SDK
 Home-page: https://github.com/V0RT3X4/python-sdk Author: Vortexa Developers
 Author-email: developers@vortexa.com License: Apache License 2.0 Description: #
 VortexaSDK [![All Contributors](https://img.shields.io/badge/all_contributors-
 12-orange.svg?style=flat-square)](#contributors) [![CircleCI](https://
 circleci.com/gh/V0RT3X4/python-sdk.svg?style=svg)](https://circleci.com/gh/
 V0RT3X4/python-sdk) [![Code style: black](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) The VortexaSDK is
```

### Comparing `vortexasdk-0.9.1/README.md` & `vortexasdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/docs/autogen.py` & `vortexasdk-0.9.2/docs/autogen.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/setup.py` & `vortexasdk-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vortexasdk",
-    version="0.9.1",
+    version="0.9.2",
     author="Vortexa Developers",
     author_email="developers@vortexa.com",
     description="Vortexa SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/V0RT3X4/python-sdk",
```

### Comparing `vortexasdk-0.9.1/tests/api/examples/cargo_movements.json` & `vortexasdk-0.9.2/tests/api/examples/cargo_movements.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/corporations.json` & `vortexasdk-0.9.2/tests/api/examples/corporations.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/geography_reference.json` & `vortexasdk-0.9.2/tests/api/examples/geography_reference.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/products.json` & `vortexasdk-0.9.2/tests/api/examples/products.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/vessel_entity1.json` & `vortexasdk-0.9.2/tests/api/examples/vessel_entity1.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/vessel_movements.json` & `vortexasdk-0.9.2/tests/api/examples/vessel_movements.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/vessels.json` & `vortexasdk-0.9.2/tests/api/examples/vessels.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/examples/vessels_reference.json` & `vortexasdk-0.9.2/tests/api/examples/vessels_reference.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_cargo_event_entity.py` & `vortexasdk-0.9.2/tests/api/test_cargo_event_entity.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_cargo_movement.py` & `vortexasdk-0.9.2/tests/api/test_cargo_movement.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_corporate_entity.py` & `vortexasdk-0.9.2/tests/api/test_corporate_entity.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_geography_entity.py` & `vortexasdk-0.9.2/tests/api/test_geography_entity.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_product_entity.py` & `vortexasdk-0.9.2/tests/api/test_product_entity.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_vessel_entity.py` & `vortexasdk-0.9.2/tests/api/test_vessel_entity.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/api/test_vessel_movement.py` & `vortexasdk-0.9.2/tests/api/test_vessel_movement.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/conversions/test_conversions.py` & `vortexasdk-0.9.2/tests/conversions/test_conversions.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/conversions/test_convert_vessels.py` & `vortexasdk-0.9.2/tests/conversions/test_convert_vessels.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_cargo_movements_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_cargo_movements_real.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_corporations_search_result.py` & `vortexasdk-0.9.2/tests/endpoints/test_corporations_search_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_geographies_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_geographies_real.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_products_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_products_real.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_reference_endpoints_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_reference_endpoints_real.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_vessel_movements_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_vessel_movements_real.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_vessels_real.py` & `vortexasdk-0.9.2/tests/endpoints/test_vessels_real.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,7 +64,17 @@
             result.to_list()
 
         with Timer("Dataframe"):
             df = result.to_df()
             print(df.head())
 
         assert len(result) >= 1_000
+
+    def test_search_is_case_agnostic(self):
+        uppercase = {
+            v.id for v in Vessels().search(vessel_classes="Suezmax").to_list()
+        }
+        lowercase = {
+            v.id for v in Vessels().search(vessel_classes="suezmax").to_list()
+        }
+
+        assert uppercase == lowercase
```

### Comparing `vortexasdk-0.9.1/tests/endpoints/test_vessels_search_result.py` & `vortexasdk-0.9.2/tests/endpoints/test_vessels_search_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/mock_client.py` & `vortexasdk-0.9.2/tests/mock_client.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/test_id.py` & `vortexasdk-0.9.2/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/test_utils.py` & `vortexasdk-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/tests/timer.py` & `vortexasdk-0.9.2/tests/timer.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/__init__.py` & `vortexasdk-0.9.2/vortexasdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/cargo_movement.py` & `vortexasdk-0.9.2/vortexasdk/api/cargo_movement.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/corporation.py` & `vortexasdk-0.9.2/vortexasdk/api/corporation.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/entity_flattening.py` & `vortexasdk-0.9.2/vortexasdk/api/entity_flattening.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/entity_serializing.py` & `vortexasdk-0.9.2/vortexasdk/api/entity_serializing.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/geography.py` & `vortexasdk-0.9.2/vortexasdk/api/geography.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class Geography(Node, IDNameLayer, FromDictMixin):
     """Represent a Geography reference record returned by the API."""
 
     bounding_box: Optional[BoundingBox]
     centre_point: Optional[Position]
     exclusion_rule: List[IDNameLayer]
     hierarchy: List[IDLayer]
-    location: Position
+    location: Optional[Position]
 
 
 @dataclass(frozen=True)
 class GeographyEntity(EntityWithProbability):
     """
     Represents a hierarchy tree of locational data.
```

### Comparing `vortexasdk-0.9.1/vortexasdk/api/id.py` & `vortexasdk-0.9.2/vortexasdk/api/id.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/product.py` & `vortexasdk-0.9.2/vortexasdk/api/product.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/search_result.py` & `vortexasdk-0.9.2/vortexasdk/api/search_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/shared_types.py` & `vortexasdk-0.9.2/vortexasdk/api/shared_types.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/vessel.py` & `vortexasdk-0.9.2/vortexasdk/api/vessel.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/api/vessel_movement.py` & `vortexasdk-0.9.2/vortexasdk/api/vessel_movement.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/client.py` & `vortexasdk-0.9.2/vortexasdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import functools
 import os
 from json import JSONDecodeError
 from multiprocessing.pool import ThreadPool
+from random import shuffle
 from typing import Dict, List
 
 from requests import Response
 from tqdm import tqdm
 
 from vortexasdk.abstract_client import AbstractVortexaClient
 from vortexasdk.api.id import ID
@@ -20,15 +21,15 @@
 logger = get_logger(__name__)
 
 
 class VortexaClient(AbstractVortexaClient):
     """The API client responsible for calling Vortexa's Public API."""
 
     _DEFAULT_PAGE_LOAD_SIZE = 10000
-    _N_THREADS = 4
+    _N_THREADS = 6
 
     def __init__(self, **kwargs):
         self.api_key = kwargs["api_key"]
 
     def get_reference(self, resource: str, id: ID) -> List[Dict]:
         """Lookup reference data."""
         url = self._create_url(f"{resource}/{id}")
@@ -37,15 +38,16 @@
 
     def search(self, resource: str, **data) -> List:
         """Search using `resource` using `**data` as filter params."""
         url = self._create_url(resource)
         payload = {k: v for k, v in data.items() if v is not None}
         total = _send_post_request(url, payload, size=1, offset=0)["total"]
         size = data.get("size", 1000)
-        offsets = range(0, total, size)
+        offsets = list(range(0, total, size))
+        shuffle(offsets)
 
         with tqdm(
             total=total, desc="Loading from API", disable=(len(offsets) == 1)
         ) as pbar:
             with ThreadPool(self._N_THREADS) as pool:
                 logger.debug(
                     f"{total} Results to retreive."
```

### Comparing `vortexasdk-0.9.1/vortexasdk/conversions/conversions.py` & `vortexasdk-0.9.2/vortexasdk/conversions/conversions.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/conversions/vessels.py` & `vortexasdk-0.9.2/vortexasdk/conversions/vessels.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     vessel_attributes: Union[List[Union[ID, str, int]], ID, str, int]
 ) -> List[ID]:
     """
     Convert a mixed list of names, IDs, IMOs, or MMSIs to vessel ids.
 
     # Example
     ```
-        >>> convert_to_vessel_ids(["Stallion", 9464326, 477639900, 'vlcc'])
-    ['e486ca3d2e58b61d683b5143a063ec309f2fa3bfd0b87d91984f43d9ee5071fb',...]
+    >>> convert_to_vessel_ids(["Stallion", 9464326, 477639900, 'vlcc'])
+    [...]
+
     ```
     """
 
     vessel_attributes_list = convert_to_list(vessel_attributes)
     ids, others = split_ids_other(vessel_attributes_list)
 
     vessel_classes = []
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/cargo_movements.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         # Example
 
         Let's load all cargo movements.
 
         ```python
         >>> from vortexasdk import CargoMovements
-        >>> df = CargoMovements().load_all().to_df()
+        >>> df = CargoMovements().load_all().to_df() # doctest: +SKIP
         ```
         """
         logger.info(
             f"Loading all Cargo Movements between {BEGINNING_OF_AVAILABLE_DATA} and {END_OF_AVAILABLE_DATA},"
             f" this will take 5-10mins."
         )
         return self.search(
@@ -119,22 +119,23 @@
         # Example
 
         * _Which cargoes were loaded from Rotterdam on the morning of 1st December 2018?_
 
 
         ```python
         >>> from vortexasdk import CargoMovements
-        >>> df = CargoMovements().search(
-            filter_origins="Rotterdam",
-            filter_activity='loading_state',
-            filter_time_min=datetime(2018, 12, 1),
-            filter_time_max=datetime(2018, 12, 1, 12),
-        ).to_df(columns=['product.grade.label', 'product.group.label', 'vessels.0.vessel_class'])
-        ```
+        >>> search_result = CargoMovements().search(
+        ...    filter_origins="Rotterdam",
+        ...    filter_activity='loading_state',
+        ...    filter_time_min=datetime(2018, 12, 1),
+        ...    filter_time_max=datetime(2018, 12, 1, 12))
+
+        >>> df = search_result.to_df(columns=['product.grade.label', 'product.group.label', 'vessels.0.vessel_class'])
 
+        ```
         |    | product.group.label   | product.grade.label             | vessels.0.vessel_class   |
         |---:|:----------------------|:--------------------------------|:-------------------------|
         |  0 | Clean products        | Pygas                           | general_purpose          |
         |  1 | Clean products        | Chemicals                       | tiny_tanker              |
         |  2 | Clean products        | Chemicals                       | tiny_tanker              |
         |  3 | Dirty products        | Low Sulphur VGO (LSVGO)         | general_purpose          |
         |  4 | Clean products        | ULSD (Ultra Low Sulphur Diesel) | general_purpose          |
@@ -144,24 +145,24 @@
         * _Which VLCC cargoes passed through the Suez canal en route to China?_
 
         Note here we include vessels.0..., vessels.1..., vessels.2... columns.
         This lets us view all vessels present in any STS operations.
 
         ```python
         >>> from vortexasdk import CargoMovements
+        >>> cargo_movement_search_result = CargoMovements().search(
+        ...    filter_destinations="China",
+        ...    filter_activity="loading_state",
+        ...    filter_waypoints="suez",
+        ...    filter_vessels="vlcc",
+        ...    filter_time_min=datetime(2018, 12, 1),
+        ...    filter_time_max=datetime(2018, 12, 1))
         >>> cols = ['vessels.0.name', 'vessels.0.vessel_class', 'vessels.1.name', 'vessels.1.vessel_class',  'vessels.2.name', 'vessels.2.vessel_class', 'product.group.label', 'quantity']
+        >>> cargo_movements_df = cargo_movement_search_result.to_df(columns=cols)
 
-        >>> df = CargoMovements().search(
-            filter_destinations="China",
-            filter_activity="loading_state",
-            filter_waypoints="suez",
-            filter_vessels="vlcc",
-            filter_time_min=datetime(2016, 12, 01),
-            filter_time_max=datetime(2018, 12, 01),
-        ).to_df(columns=cols)
         ```
 
         |    | vessels.0.name   | vessels.0.vessel_class   | vessels.1.name   | vessels.1.vessel_class   | vessels.2.name   | vessels.2.vessel_class   | product.group.label   |   quantity |
         |---:|:-----------------|:-------------------------|:-----------------|:-------------------------|:-----------------|:-------------------------|:----------------------|-----------:|
         |  0 | MINERVA MARINA   | suezmax                  | COSGLORY LAKE    | vlcc_plus                | nan              | nan                      | Crude                 |     700614 |
         |  1 | BUKHA            | vlcc_plus                | nan              | nan                      | nan              | nan                      | Crude                 |    1896374 |
         |  2 | ATHENIAN FREEDOM | vlcc_plus                | nan              | nan                      | nan              | nan                      | Crude                 |     183537 |
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/cargo_movements_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/corporations.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/corporations.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,28 +31,30 @@
 
 
         # Examples
 
         Let's load all corporations
         ```python
         >>> from vortexasdk import Corporations
-        >>> Corporations().search().to_df()
+        >>> df = Corporations().search().to_df()
+
         ```
         returns
 
         |    | id                                                               | name       | corporate_entity_type   |
         |---:|:-----------------------------------------------------------------|:-----------|:------------------------|
         |  0 | 04f418ee78c1e17744ad653e7815e8e28891ed9ba25a8427030e4478e5c00974 | 3J         | ['commercial_owner']    |
         |  1 | b6384cf17f1639a64bbff04cfd32257bf732a3a13e4b0532802a9ae84a36be34 | 5XJAPANESE | ['commercial_owner']    |
 
 
         Let's find all corporations with 'do' in the name.
         ```python
         >>> [x.name for x in Corporations().search(term="do").to_list()]
-            ['Donsotank', 'Dorval SC']
+        [...]
+
         ```
 
         # Further Documentation
 
         [VortexaAPI Corporation Reference](https://docs.vortexa.com/reference/POST/reference/charterers)
 
         """
@@ -69,11 +71,11 @@
         # Returns
         Corporation record matching the ID
 
         # Further Documentation:
         [VortexaAPI Corporation Reference](https://docs.vortexa.com/reference/GET/reference/charterers/%7Bid%7D)
 
         # Examples
-            >>> Corporations().reference(id='12345abcdef')
+        >>> Corporations().reference(id='12345abcdef') # doctest: +SKIP
 
         """
         return super().reference(id)
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/corporations_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/corporations_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/geographies.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/geographies.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 
 
         # Examples
 
         Find all geographies with `portsmouth` in the name.
         ```python
         >>> from vortexasdk import Geographies
-        >>> [x["name"] for x in Geographies().search(term="portsmouth")]
-            ['Portsmouth [GB]', 'Portsmouth, NH [US]']
+        >>> [x.name for x in Geographies().search(term="portsmouth").to_list()]
+        ['Portsmouth [GB]', 'Portsmouth, NH [US]']
+
         ```
 
         Search multiple geography terms
         ```python
         >>> df = Geographies().search(term=["Liverpool", "Southampton"]).to_df()
+
         ```
         returns
 
         |    | id                | name                   | layer        |
         |---:|:------------------|:-----------------------|:-------------|
         |  0 | b63d8f625669fd... | Liverpool [GB]         | ['port']     |
         |  1 | 0cb7d4566de0f2... | Southampton [GB]       | ['port']     |
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/geographies_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/geographies_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/products.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/products.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
         # Examples
 
         Let's look for products with in one of `['diesel', 'fuel oil', 'grane']` their name, or related names.
 
         ```python
         >>> from vortexasdk import Products
-        >>> Products().search(term=['diesel', 'fuel oil', 'grane']).to_df('all')
+        >>> df = Products().search(term=['diesel', 'fuel oil', 'grane']).to_df('all')
+
         ```
         Returns
 
         |    | id                 | name          | layer.0   | leaf   | parent.0.name   | parent.0.layer.0   | parent.0.id       |   meta.api_min |   meta.api_max | ref_type   |   meta.sulphur_min |   meta.sulphur_max |
         |---:|:-------------------|:--------------|:----------|:-------|:----------------|:-------------------|:------------------|---------------:|---------------:|:-----------|-------------------:|-------------------:|
         |  0 | 1c107b4317bc2c8... | Fuel Oil      | category  | False  | Dirty products  | product            | 5de0b00094e0fd... |        12.8878 |        12.8878 | product    |             nan    |             nan    |
         |  1 | fddedd17e02507f... | Grane         | grade     | True   | Medium-Sour     | subproduct_group   | a7e26956fbb917... |        29.2955 |        29.2955 | product    |               0.62 |               0.62 |
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/products_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/products_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/vessel_movements.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def load_all(self) -> VesselMovementsResult:
         """Load all available Vessel Movements.
         # Example
         Let's load all vessel movements as a `pd.DataFrame`.
 
         ```python
         >>> from vortexasdk import VesselMovements
-        >>> df = VesselMovements().load_all().to_df()
+        >>> df = VesselMovements().load_all().to_df() # doctest: +SKIP
         ```
         """
         logger.info(
             f"Loading all Vessel Movements between {BEGINNING_OF_AVAILABLE_DATA} and {END_OF_AVAILABLE_DATA},"
             f" this will take 5-10mins."
         )
 
@@ -104,19 +104,20 @@
 
 
         # Example
         Let's search for all vessels that departed from `Rotterdam [NL]` on the morning of 1st December 2018.
 
         ```python
         >>> from vortexasdk import VesselMovements
-        >>> df = VesselMovements().search(
-                filter_time_min=datetime(2017, 10, 1, 0, 0),
-                filter_time_max=datetime(2017, 10, 1, 0, 10),
-                filter_origins='rotterdam'
-        ).to_df().head(2)
+        >>> search_result = VesselMovements().search(
+        ...        filter_time_min=datetime(2017, 10, 1, 0, 0),
+        ...        filter_time_max=datetime(2017, 10, 1, 0, 10),
+        ...        filter_origins='rotterdam')
+        >>> df = search_result.to_df().head(2)
+
         ```
 
         |    | start_timestamp          | end_timestamp            |   vessel.imo | vessel.name   | vessel.vessel_class   | origin.location.country.label   | origin.location.port.label   | destination.location.country.label   | destination.location.port.label   |   cargoes.0.quantity | cargoes.0.product.grade.label   |
         |---:|:-------------------------|:-------------------------|-------------:|:--------------|:----------------------|:--------------------------------|:-----------------------------|:-------------------------------------|:----------------------------------|---------------------:|:--------------------------------|
         |  0 | 2017-09-30T15:30:27+0000 | 2017-10-03T01:46:06+0000 |  9.21091e+06 | ADEBOMI 3     | handysize             | Netherlands                     | Rotterdam [NL]               | Netherlands                          | Rotterdam [NL]                    |                  nan | nan                             |
         |  1 | 2017-08-29T14:51:32+0000 | 2017-10-04T14:46:21+0000 |  9.64544e+06 | AEGEAN VISION | suezmax               | Netherlands                     | Rotterdam [NL]               | Singapore                            | Singapore [SG]                    |               852261 | High Sulphur                    |
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/vessel_movements_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/vessels.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/vessels.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
         # Examples
 
         - Let's find all the VLCCs with 'ocean' in their name, or related names.
 
         ```python
         >>> from vortexasdk import Vessels
-        >>> Vessels().search(vessel_classes='vlcc', term='ocean').to_df(columns=['name', 'imo', 'mmsi', 'related_names'])
+        >>> vessels_df = Vessels().search(vessel_classes='vlcc', term='ocean').to_df(columns=['name', 'imo', 'mmsi', 'related_names'])
+
         ```
 
         |    | name         |     imo |      mmsi | related_names             |
         |---:|:-------------|--------:|----------:|:--------------------------|
         |  0 | OCEANIS      | 9532757 | 241089000 | ['OCEANIS']               |
         |  1 | AEGEAN       | 9732553 | 205761000 | ['GENER8 OCEANUS']        |
         |  2 | OCEANIA      | 9246633 | 205753000 | ['OCEANIA'| 'TI OCEANIA'] |
@@ -66,26 +67,29 @@
 
         Note the `term` search also looks for vessels with matching `related_names`
 
 
         - Let's find all the vessels currently carrying Crude.
 
         ```python
-        >>> Vessels().search(vessel_product_types='crude').to_df()
+        >>> vessels_df = Vessels().search(vessel_product_types='crude').to_df()
+
         ```
 
         # Further Documentation
 
         [VortexaAPI Vessel Reference](https://docs.vortexa.com/reference/POST/reference/vessels)
 
         """
         search_params = {
             "term": [str(e) for e in convert_to_list(term)],
             "ids": convert_to_list(ids),
-            "vessel_classes": convert_to_list(vessel_classes),
+            "vessel_classes": [
+                v.lower() for v in (convert_to_list(vessel_classes))
+            ],
             "vessel_product_types": convert_to_product_ids(
                 convert_to_list(vessel_product_types)
             ),
         }
 
         return VesselsResult(super().search(**search_params))
```

### Comparing `vortexasdk-0.9.1/vortexasdk/endpoints/vessels_result.py` & `vortexasdk-0.9.2/vortexasdk/endpoints/vessels_result.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/logger.py` & `vortexasdk-0.9.2/vortexasdk/logger.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk/operations.py` & `vortexasdk-0.9.2/vortexasdk/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             id: ID of the entity we're looking up
 
         # Returns
         An entity matching the ID
 
         # Examples
 
-            >>> Reference("/reference/geographies").reference(id='cfb8c4ef76585c3a37792b643791a0f4ff6d5656d5508927d8017319e21f2fca')
+        >>> Reference("/reference/geographies").reference(id='cfb8c4ef76585c3a37792b643791a0f4ff6d5656d5508927d8017319e21f2fca') # doctest: +SKIP
 
         """
         logger.info(
             f"Looking up {self.__class__.__name__} reference data with id: {id}"
         )
 
         data = default_client().get_reference(self._resource, id)
@@ -72,14 +72,14 @@
             params: Search parameters
 
         # Returns
         Result of VortexaAPI call from hitting querying the `resource` endpoint filtering with `params`.
 
         # Examples
 
-            >>> Search("/reference/vessels").search(term="DHT")
+        >>> Search("/reference/vessels").search(term="DHT") # doctest: +SKIP
 
         """
         logger.info(
             f"Searching {self.__class__.__name__} with params: {params}"
         )
         return default_client().search(self._resource, **params)
```

### Comparing `vortexasdk-0.9.1/vortexasdk/retry_session.py` & `vortexasdk-0.9.2/vortexasdk/retry_session.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.1/vortexasdk.egg-info/PKG-INFO` & `vortexasdk-0.9.2/vortexasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortexasdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Vortexa SDK
 Home-page: https://github.com/V0RT3X4/python-sdk
 Author: Vortexa Developers
 Author-email: developers@vortexa.com
 License: Apache License 2.0
 Description: # VortexaSDK
         [![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vortexasdk Version: 0.9.1 Summary: Vortexa SDK
+Metadata-Version: 2.1 Name: vortexasdk Version: 0.9.2 Summary: Vortexa SDK
 Home-page: https://github.com/V0RT3X4/python-sdk Author: Vortexa Developers
 Author-email: developers@vortexa.com License: Apache License 2.0 Description: #
 VortexaSDK [![All Contributors](https://img.shields.io/badge/all_contributors-
 12-orange.svg?style=flat-square)](#contributors) [![CircleCI](https://
 circleci.com/gh/V0RT3X4/python-sdk.svg?style=svg)](https://circleci.com/gh/
 V0RT3X4/python-sdk) [![Code style: black](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) The VortexaSDK is
```

### Comparing `vortexasdk-0.9.1/vortexasdk.egg-info/SOURCES.txt` & `vortexasdk-0.9.2/vortexasdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-.all-contributorsrc
-.gitignore
-.pre-commit-config.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
-LICENSE
 MANIFEST.in
 README.md
-pydocmd.yml
-pyproject.toml
-pytest.ini
 setup.cfg
 setup.py
-.circleci/config.yml
-art/favicon.ico
 docs/__init__.py
 docs/autogen.py
-docs/build_docs.sh
-docs/deploy_docs.sh
-docs/serve_docs.sh
 docs/utils.py
-docs/config/config.md
-docs/endpoints/about-endpoints.md
-docs/examples/1_china.py
-docs/examples/2_all_vessel_movements.py
-scripts/export_package.sh
-scripts/generate_stubs.sh
 tests/__init__.py
 tests/config.py
 tests/mock_client.py
 tests/test_id.py
 tests/test_to_ISODate.py
 tests/test_utils.py
 tests/testcases.py
```

