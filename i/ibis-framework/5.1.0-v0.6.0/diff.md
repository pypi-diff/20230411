# Comparing `tmp/ibis_framework-5.1.0.tar.gz` & `tmp/ibis-framework-v0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis_framework-5.1.0.tar", max compression
+gzip compressed data, was "dist/ibis-framework-v0.6.0.tar", last modified: Mon Nov 30 09:48:46 2015, max compression
```

## Comparing `ibis_framework-5.1.0.tar` & `ibis-framework-v0.6.0.tar`

### file list

```diff
@@ -1,1336 +1,204 @@
--rw-r--r--   0        0        0    11358 2023-04-11 17:42:39.571847 ibis_framework-5.1.0/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2023-04-11 17:42:39.571847 ibis_framework-5.1.0/LICENSES/
--rw-r--r--   0        0        0    11594 2023-04-11 17:42:39.571847 ibis_framework-5.1.0/README.md
--rw-r--r--   0        0        0     3640 2023-04-11 17:43:46.967710 ibis_framework-5.1.0/ibis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/__init__.py
--rw-r--r--   0        0        0    30691 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/df/__init__.py
--rw-r--r--   0        0        0     7574 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/df/scope.py
--rw-r--r--   0        0        0    10096 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/df/timecontext.py
--rw-r--r--   0        0        0    11891 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/__init__.py
--rw-r--r--   0        0        0    23551 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/__init__.py
--rw-r--r--   0        0        0     1213 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/database.py
--rw-r--r--   0        0        0     9991 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/datatypes.py
--rw-r--r--   0        0        0      233 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/geospatial.py
--rw-r--r--   0        0        0    13298 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/query_builder.py
--rw-r--r--   0        0        0    22961 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/registry.py
--rw-r--r--   0        0        0     4556 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/translator.py
--rw-r--r--   0        0        0      559 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/compiler/__init__.py
--rw-r--r--   0        0        0     3177 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/compiler/base.py
--rw-r--r--   0        0        0    19661 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/compiler/query_builder.py
--rw-r--r--   0        0        0    12359 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/compiler/select_builder.py
--rw-r--r--   0        0        0    10785 2023-04-11 17:42:39.607849 ibis_framework-5.1.0/ibis/backends/base/sql/compiler/translator.py
--rw-r--r--   0        0        0    12801 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/ddl.py
--rw-r--r--   0        0        0      883 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/__init__.py
--rw-r--r--   0        0        0     1083 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/aggregate.py
--rw-r--r--   0        0        0     2746 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/binary_infix.py
--rw-r--r--   0        0        0     1705 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/case.py
--rw-r--r--   0        0        0     5007 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/geospatial.py
--rw-r--r--   0        0        0     1741 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/helpers.py
--rw-r--r--   0        0        0     2705 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/identifiers.py
--rw-r--r--   0        0        0     2477 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/literal.py
--rw-r--r--   0        0        0    13374 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/main.py
--rw-r--r--   0        0        0     3203 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/string.py
--rw-r--r--   0        0        0     2937 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/timestamp.py
--rw-r--r--   0        0        0     5790 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/base/sql/registry/window.py
--rw-r--r--   0        0        0    20562 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/__init__.py
--rw-r--r--   0        0        0     8255 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/client.py
--rw-r--r--   0        0        0     3880 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/compiler.py
--rw-r--r--   0        0        0     1544 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/custom_udfs.py
--rw-r--r--   0        0        0     2595 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/datatypes.py
--rw-r--r--   0        0        0      189 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/operations.py
--rw-r--r--   0        0        0    24328 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/registry.py
--rw-r--r--   0        0        0      819 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/rewrites.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/__init__.py
--rw-r--r--   0        0        0    10859 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/__init__.py
--rw-r--r--   0        0        0     2523 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/conftest.py
--rw-r--r--   0        0        0      160 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/snapshots/test_client/test_cross_project_query/out.sql
--rw-r--r--   0        0        0      309 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/snapshots/test_client/test_subquery_scalar_params/out.sql
--rw-r--r--   0        0        0    11517 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/test_client.py
--rw-r--r--   0        0        0     5217 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/test_connect.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/udf/__init__.py
--rw-r--r--   0        0        0      389 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/udf/snapshots/test_udf_execute/test_udf_with_struct/out.sql
--rw-r--r--   0        0        0     4220 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/system/udf/test_udf_execute.py
--rw-r--r--   0        0        0      117 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_median/out.sql
--rw-r--r--   0        0        0      108 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_nunique/out.sql
--rw-r--r--   0        0        0       91 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_median/out.sql
--rw-r--r--   0        0        0       82 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_nunique/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_binary/out.sql
--rw-r--r--   0        0        0       96 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_and/out.sql
--rw-r--r--   0        0        0       95 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_or/out.sql
--rw-r--r--   0        0        0       96 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_xor/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_and/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_or/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.611849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_xor/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/mean/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/sum/out.sql
--rw-r--r--   0        0        0      127 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_conj/out.sql
--rw-r--r--   0        0        0      103 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_simple/out.sql
--rw-r--r--   0        0        0      178 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bucket/out.sql
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0       87 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/pop/out.sql
--rw-r--r--   0        0        0       88 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/sample/out.sql
--rw-r--r--   0        0        0       69 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/index.sql
--rw-r--r--   0        0        0       71 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/name.sql
--rw-r--r--   0        0        0       83 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/index.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/name.sql
--rw-r--r--   0        0        0       69 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/index.sql
--rw-r--r--   0        0        0       71 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/name.sql
--rw-r--r--   0        0        0       83 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/index.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/name.sql
--rw-r--r--   0        0        0       83 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/index.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/name.sql
--rw-r--r--   0        0        0       69 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/index.sql
--rw-r--r--   0        0        0       71 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/name.sql
--rw-r--r--   0        0        0       97 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/floordiv/out.sql
--rw-r--r--   0        0        0       75 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/truediv/out.sql
--rw-r--r--   0        0        0       39 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/date/out.sql
--rw-r--r--   0        0        0       39 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/time/out.sql
--rw-r--r--   0        0        0       54 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_azimuth/out.sql
--rw-r--r--   0        0        0       61 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/contains/out.sql
--rw-r--r--   0        0        0       62 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covered_by/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covers/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/d_within/out.sql
--rw-r--r--   0        0        0       63 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/difference/out.sql
--rw-r--r--   0        0        0       61 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/disjoint/out.sql
--rw-r--r--   0        0        0       61 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/distance/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/geo_equals/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersection/out.sql
--rw-r--r--   0        0        0       63 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersects/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/max_distance/out.sql
--rw-r--r--   0        0        0       60 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/touches/out.sql
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/union/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/within/out.sql
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_max/out.sql
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_min/out.sql
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_max/out.sql
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_min/out.sql
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_point/out.sql
--rw-r--r--   0        0        0       53 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_simplify/out.sql
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/aread/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_binary/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_text/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/buffer/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/centroid/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/end_point/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/geometry_type/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.615849 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/length/out.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/npoints/out.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/perimeter/out.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/point_n/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/start_point/out.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary_union/out.sql
--rw-r--r--   0        0        0       39 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/x/out.sql
--rw-r--r--   0        0        0       39 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/y/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/binary/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/string/out.sql
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-binary/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-string/out.sql
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-binary/out.sql
--rw-r--r--   0        0        0       28 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-string/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-binary/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-string/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-binary/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-string/out.sql
--rw-r--r--   0        0        0      146 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_identical_to/out.sql
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ms/out.sql
--rw-r--r--   0        0        0       76 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ns/out.sql
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/s/out.sql
--rw-r--r--   0        0        0       43 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/us/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/datetime/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_time/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_timestamp/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/time/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/timestamp/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/date/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/datetime/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_date/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_timestamp/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp_date/out.sql
--rw-r--r--   0        0        0       35 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_now/out.sql
--rw-r--r--   0        0        0      387 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_projection_fusion_only_peeks_at_immediate_parent/out.sql
--rw-r--r--   0        0        0      182 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_foll/out.sql
--rw-r--r--   0        0        0      203 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_prec/out.sql
--rw-r--r--   0        0        0       97 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/difference/out.sql
--rw-r--r--   0        0        0      100 2023-04-11 17:42:39.619850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/intersect/out.sql
--rw-r--r--   0        0        0       91 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_all/out.sql
--rw-r--r--   0        0        0       96 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_distinct/out.sql
--rw-r--r--   0        0        0      117 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_substring/out.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-date/out.sql
--rw-r--r--   0        0        0       54 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-timestamp/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-time/out.sql
--rw-r--r--   0        0        0       55 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-timestamp/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-time/out.sql
--rw-r--r--   0        0        0       62 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-timestamp/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-time/out.sql
--rw-r--r--   0        0        0       62 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-timestamp/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-time/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-timestamp/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-date/out.sql
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-timestamp/out.sql
--rw-r--r--   0        0        0       53 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-date/out.sql
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-timestamp/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-time/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-timestamp/out.sql
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-date/out.sql
--rw-r--r--   0        0        0       63 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-timestamp/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-date/out.sql
--rw-r--r--   0        0        0       55 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-timestamp/out.sql
--rw-r--r--   0        0        0       87 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_no_timezone/out.sql
--rw-r--r--   0        0        0      119 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_timezone/out.sql
--rw-r--r--   0        0        0      229 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/days/out.sql
--rw-r--r--   0        0        0      174 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/five/out.sql
--rw-r--r--   0        0        0      229 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/hours/out.sql
--rw-r--r--   0        0        0      225 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/micros/out.sql
--rw-r--r--   0        0        0      229 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/minutes/out.sql
--rw-r--r--   0        0        0      227 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/seconds/out.sql
--rw-r--r--   0        0        0      264 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/two_days/out.sql
--rw-r--r--   0        0        0      233 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/week/out.sql
--rw-r--r--   0        0        0      237 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/years/out.sql
--rw-r--r--   0        0        0      373 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/False/out.sql
--rw-r--r--   0        0        0      378 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/True/out.sql
--rw-r--r--   0        0        0      807 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-False/out.sql
--rw-r--r--   0        0        0      812 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-True/out.sql
--rw-r--r--   0        0        0      812 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-False/out.sql
--rw-r--r--   0        0        0      817 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-True/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/current_foll/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_current/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_prec/out.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/following/out.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/preceding/out.sql
--rw-r--r--   0        0        0      919 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/test_client.py
--rw-r--r--   0        0        0    18521 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/test_compiler.py
--rw-r--r--   0        0        0     2770 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/test_datatypes.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/__init__.py
--rw-r--r--   0        0        0       76 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_assign/out.js
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/add/out.js
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/div/out.js
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/mul/out.js
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/sub/out.js
--rw-r--r--   0        0        0      178 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class/out.js
--rw-r--r--   0        0        0      125 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class_with_properties/out.js
--rw-r--r--   0        0        0      139 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_continue/out.js
--rw-r--r--   0        0        0      154 2023-04-11 17:42:39.623850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_delete/out.js
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_dict/out.js
--rw-r--r--   0        0        0       61 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_floordiv/out.js
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_function_def/out.js
--rw-r--r--   0        0        0      249 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_lambda_with_splat/out.js
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_len_rewrite/out.js
--rw-r--r--   0        0        0      138 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_list_comp/out.js
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_logical_not/out.js
--rw-r--r--   0        0        0       56 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_missing_vararg/out.js
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_pow/out.js
--rw-r--r--   0        0        0      323 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_scope_with_while/out.js
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_set_to_object/out.js
--rw-r--r--   0        0        0       78 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_setitem/out.js
--rw-r--r--   0        0        0      134 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_splat/out.js
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_str/out.js
--rw-r--r--   0        0        0      106 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_true_false_none/out.js
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_tuple/out.js
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_minus/out.js
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_plus/out.js
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_varargs/out.js
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_variable_declaration/out.js
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield/out.js
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield_from/out.js
--rw-r--r--   0        0        0      402 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_usage/test_multiple_calls_redefinition/out.sql
--rw-r--r--   0        0        0      212 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_usage/test_udf_determinism/False/out.sql
--rw-r--r--   0        0        0      194 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_usage/test_udf_determinism/None/out.sql
--rw-r--r--   0        0        0      208 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_usage/test_udf_determinism/True/out.sql
--rw-r--r--   0        0        0      128 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/snapshots/test_usage/test_udf_sql/out.sql
--rw-r--r--   0        0        0     6497 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/test_core.py
--rw-r--r--   0        0        0     1966 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/test_find.py
--rw-r--r--   0        0        0     2895 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/tests/unit/udf/test_usage.py
--rw-r--r--   0        0        0    13377 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/udf/__init__.py
--rw-r--r--   0        0        0    17180 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/udf/core.py
--rw-r--r--   0        0        0     1598 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/udf/find.py
--rw-r--r--   0        0        0     1255 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/bigquery/udf/rewrite.py
--rw-r--r--   0        0        0    20345 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/__init__.py
--rw-r--r--   0        0        0      363 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/compiler/__init__.py
--rw-r--r--   0        0        0     2621 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/compiler/core.py
--rw-r--r--   0        0        0     6701 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/compiler/relations.py
--rw-r--r--   0        0        0    39736 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/compiler/values.py
--rw-r--r--   0        0        0     7063 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/datatypes.py
--rw-r--r--   0        0        0     2113 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/identifiers.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/__init__.py
--rw-r--r--   0        0        0     4848 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/conftest.py
--rw-r--r--   0        0        0       36 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/count/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/max/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.627850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/mean/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/min/out.sql
--rw-r--r--   0        0        0       41 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/std/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/sum/out.sql
--rw-r--r--   0        0        0       38 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/var/out.sql
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/std/out.sql
--rw-r--r--   0        0        0       37 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/var/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float/out.sql
--rw-r--r--   0        0        0       37 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float32/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float64/out.sql
--rw-r--r--   0        0        0       35 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int16/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int8/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/date/out.sql
--rw-r--r--   0        0        0       35 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int16/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int8/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/mapstring_int64/out.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/string/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/structa_string_b_int64/out.sql
--rw-r--r--   0        0        0       43 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/timestamp/out.sql
--rw-r--r--   0        0        0      264 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_extract/out.sql
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_replace/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out1.sql
--rw-r--r--   0        0        0       29 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out2.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out3.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out4.sql
--rw-r--r--   0        0        0      105 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_none/out.sql
--rw-r--r--   0        0        0      137 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_zero/out.sql
--rw-r--r--   0        0        0      105 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/minus_none/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bigint_col/out.sql
--rw-r--r--   0        0        0        8 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bool_col/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/date_string_col/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/double_col/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/float_col/out.sql
--rw-r--r--   0        0        0        2 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/id/out.sql
--rw-r--r--   0        0        0        5 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/index/out.sql
--rw-r--r--   0        0        0        7 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/int_col/out.sql
--rw-r--r--   0        0        0        5 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/month/out.sql
--rw-r--r--   0        0        0       12 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/smallint_col/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/string_col/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/timestamp_col/out.sql
--rw-r--r--   0        0        0       11 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/tinyint_col/out.sql
--rw-r--r--   0        0        0        4 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/year/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out1.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out2.sql
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find_in_set/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out1.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out2.sql
--rw-r--r--   0        0        0       91 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out1.sql
--rw-r--r--   0        0        0       97 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out2.sql
--rw-r--r--   0        0        0       36 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out1.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.631850 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out2.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_from_integer/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/d/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/h/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/m/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/minute/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/w/out.sql
--rw-r--r--   0        0        0       57 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/y/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/abs/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/ceil/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/exp/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log10/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log2/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_0/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_2/out.sql
--rw-r--r--   0        0        0       41 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sign/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sqrt/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_quote/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_token/out.sql
--rw-r--r--   0        0        0        8 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/simple/out.sql
--rw-r--r--   0        0        0      177 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_complex_array_expr_projection/out.sql
--rw-r--r--   0        0        0       94 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out1.sql
--rw-r--r--   0        0        0       98 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out2.sql
--rw-r--r--   0        0        0      149 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_isnull_case_expr_rewrite_failure/out.sql
--rw-r--r--   0        0        0      126 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_join_self_reference/out.sql
--rw-r--r--   0        0        0      124 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out1.sql
--rw-r--r--   0        0        0      124 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out2.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_physical_table_reference_translate/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/add/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/now/out.sql
--rw-r--r--   0        0        0       54 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_self_reference_simple/out.sql
--rw-r--r--   0        0        0      118 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_inner_join/out.sql
--rw-r--r--   0        0        0      123 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_left_join/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-inner_join/out.sql
--rw-r--r--   0        0        0      125 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-left_join/out.sql
--rw-r--r--   0        0        0      119 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_inner_join/out.sql
--rw-r--r--   0        0        0      124 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_left_join/out.sql
--rw-r--r--   0        0        0      121 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-inner_join/out.sql
--rw-r--r--   0        0        0      126 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-left_join/out.sql
--rw-r--r--   0        0        0      113 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_scalar_aggregates/out.sql
--rw-r--r--   0        0        0      186 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_table_column_unbox/out.sql
--rw-r--r--   0        0        0      280 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_timestamp_extract_field/out.sql
--rw-r--r--   0        0        0      123 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_simple_comparisons/out.sql
--rw-r--r--   0        0        0       38 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_use_if/out.sql
--rw-r--r--   0        0        0      110 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_between/out.sql
--rw-r--r--   0        0        0       88 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_timestamp/out.sql
--rw-r--r--   0        0        0     5619 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_aggregations.py
--rw-r--r--   0        0        0     8359 2023-04-11 17:42:39.635851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_client.py
--rw-r--r--   0        0        0    13978 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_functions.py
--rw-r--r--   0        0        0     2402 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_literals.py
--rw-r--r--   0        0        0     8248 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_operators.py
--rw-r--r--   0        0        0    10985 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_select.py
--rw-r--r--   0        0        0     7301 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/clickhouse/tests/test_types.py
--rw-r--r--   0        0        0    23900 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/conftest.py
--rw-r--r--   0        0        0     4068 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/__init__.py
--rw-r--r--   0        0        0     3609 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/client.py
--rw-r--r--   0        0        0    15342 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/core.py
--rw-r--r--   0        0        0      803 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/dispatch.py
--rw-r--r--   0        0        0      950 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/__init__.py
--rw-r--r--   0        0        0     5431 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/aggregations.py
--rw-r--r--   0        0        0     1586 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/arrays.py
--rw-r--r--   0        0        0      687 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/decimal.py
--rw-r--r--   0        0        0    18196 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/generic.py
--rw-r--r--   0        0        0     1481 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/indexing.py
--rw-r--r--   0        0        0     3555 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/join.py
--rw-r--r--   0        0        0     3631 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/maps.py
--rw-r--r--   0        0        0     4832 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/numeric.py
--rw-r--r--   0        0        0     6842 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/reductions.py
--rw-r--r--   0        0        0     8395 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/selection.py
--rw-r--r--   0        0        0    11528 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/strings.py
--rw-r--r--   0        0        0     1093 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/structs.py
--rw-r--r--   0        0        0     6262 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/temporal.py
--rw-r--r--   0        0        0    11754 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/util.py
--rw-r--r--   0        0        0     4358 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/execution/window.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/__init__.py
--rw-r--r--   0        0        0     3682 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/__init__.py
--rw-r--r--   0        0        0     8048 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/conftest.py
--rw-r--r--   0        0        0     6233 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_arrays.py
--rw-r--r--   0        0        0     4777 2023-04-11 17:42:39.639851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_cast.py
--rw-r--r--   0        0        0     7065 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_functions.py
--rw-r--r--   0        0        0    16381 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_join.py
--rw-r--r--   0        0        0     3125 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_maps.py
--rw-r--r--   0        0        0    32685 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_operations.py
--rw-r--r--   0        0        0     4122 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_strings.py
--rw-r--r--   0        0        0     2754 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_structs.py
--rw-r--r--   0        0        0     7249 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_temporal.py
--rw-r--r--   0        0        0    10663 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_timecontext.py
--rw-r--r--   0        0        0      769 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/execution/test_util.py
--rw-r--r--   0        0        0     3832 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_client.py
--rw-r--r--   0        0        0     3300 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_core.py
--rw-r--r--   0        0        0     3128 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_datatypes.py
--rw-r--r--   0        0        0     2657 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_dispatcher.py
--rw-r--r--   0        0        0     5438 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_schema.py
--rw-r--r--   0        0        0    14988 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/tests/test_udf.py
--rw-r--r--   0        0        0     5489 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/trace.py
--rw-r--r--   0        0        0    10280 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/dask/udf.py
--rw-r--r--   0        0        0     9427 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/datafusion/__init__.py
--rw-r--r--   0        0        0    11861 2023-04-11 17:42:39.643851 ibis_framework-5.1.0/ibis/backends/datafusion/compiler.py
--rw-r--r--   0        0        0      128 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/datafusion/datatypes.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/datafusion/tests/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/datafusion/tests/conftest.py
--rw-r--r--   0        0        0      627 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/datafusion/tests/test_select.py
--rw-r--r--   0        0        0     1323 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/datafusion/tests/test_udf.py
--rw-r--r--   0        0        0     3625 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/__init__.py
--rw-r--r--   0        0        0      480 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/compiler.py
--rw-r--r--   0        0        0     1264 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/datatypes.py
--rw-r--r--   0        0        0     1710 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/tests/__init__.py
--rw-r--r--   0        0        0     4859 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/druid/tests/conftest.py
--rw-r--r--   0        0        0    28155 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/__init__.py
--rw-r--r--   0        0        0     1391 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/compiler.py
--rw-r--r--   0        0        0     4940 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/datatypes.py
--rw-r--r--   0        0        0    13551 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/__init__.py
--rw-r--r--   0        0        0     1811 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/conftest.py
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint16/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint32/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint64/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint8/out.sql
--rw-r--r--   0        0        0     3658 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/test_datatypes.py
--rw-r--r--   0        0        0     7550 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/duckdb/tests/test_register.py
--rw-r--r--   0        0        0    42057 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/__init__.py
--rw-r--r--   0        0        0    16276 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/client.py
--rw-r--r--   0        0        0      803 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/compat.py
--rw-r--r--   0        0        0     1056 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/compiler.py
--rw-r--r--   0        0        0     9307 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/ddl.py
--rw-r--r--   0        0        0     8623 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/metadata.py
--rw-r--r--   0        0        0     3344 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/pandas_interop.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/tests/__init__.py
--rw-r--r--   0        0        0    15563 2023-04-11 17:42:39.647851 ibis_framework-5.1.0/ibis/backends/impala/tests/conftest.py
--rw-r--r--   0        0        0      212 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/mocks.py
--rw-r--r--   0        0        0       25 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/first/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_arg/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_default/out.sql
--rw-r--r--   0        0        0       23 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_explicit_default/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/last/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_arg/out.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_default/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_explicit_default/out.sql
--rw-r--r--   0        0        0        8 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/ntile/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/percent_rank/out.sql
--rw-r--r--   0        0        0      491 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_assign_labels/out.sql
--rw-r--r--   0        0        0      159 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false/out.sql
--rw-r--r--   0        0        0      159 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_closed_right/out.sql
--rw-r--r--   0        0        0      205 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_include_under_include_over/out.sql
--rw-r--r--   0        0        0      160 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right/out.sql
--rw-r--r--   0        0        0      182 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_close_extreme_false_include_under/out.sql
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_include_over_include_under/out.sql
--rw-r--r--   0        0        0      160 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/default/out.sql
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under0/out.sql
--rw-r--r--   0        0        0       97 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under1/out.sql
--rw-r--r--   0        0        0      100 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under2/out.sql
--rw-r--r--   0        0        0      182 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under/out.sql
--rw-r--r--   0        0        0      205 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under_include_over/out.sql
--rw-r--r--   0        0        0       28 2023-04-11 17:42:39.651852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice_double/out.sql
--rw-r--r--   0        0        0       23 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_quantity/out.sql
--rw-r--r--   0        0        0       97 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to_special_case/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out1.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out2.sql
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_boolean/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_input/out.sql
--rw-r--r--   0        0        0       43 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_negate_boolean/out.sql
--rw-r--r--   0        0        0       92 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_search_case/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_simple_case/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_case_exprs/test_where_use_if/out.sql
--rw-r--r--   0        0        0       33 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_columns/out.sql
--rw-r--r--   0        0        0       29 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_scalar/out.sql
--rw-r--r--   0        0        0       33 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_columns/out.sql
--rw-r--r--   0        0        0       29 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_scalar/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_columns/out.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_scalar/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_string_key/out.sql
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_with_props/out.sql
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out1.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out2.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out3.sql
--rw-r--r--   0        0        0       82 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out4.sql
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out1.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out2.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out3.sql
--rw-r--r--   0        0        0       82 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out4.sql
--rw-r--r--   0        0        0       92 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_avro_other_formats/out.sql
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out1.sql
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out2.sql
--rw-r--r--   0        0        0      114 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_as/out.sql
--rw-r--r--   0        0        0      489 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_avro/out.sql
--rw-r--r--   0        0        0      239 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_delimited/out.sql
--rw-r--r--   0        0        0      126 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_like_parquet/out.sql
--rw-r--r--   0        0        0      116 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet/out.sql
--rw-r--r--   0        0        0      104 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_like_other/out.sql
--rw-r--r--   0        0        0      138 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_with_schema/out.sql
--rw-r--r--   0        0        0      124 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_with_location_compile/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_partition/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out1.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out2.sql
--rw-r--r--   0        0        0      100 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out1.sql
--rw-r--r--   0        0        0      110 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out2.sql
--rw-r--r--   0        0        0       69 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out1.sql
--rw-r--r--   0        0        0       79 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out2.sql
--rw-r--r--   0        0        0      121 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_no_overwrite/out.sql
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out1.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out2.sql
--rw-r--r--   0        0        0      280 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_exprs/test_filter_with_analytic/out.sql
--rw-r--r--   0        0        0      101 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/abc.sql
--rw-r--r--   0        0        0      101 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/foo.sql
--rw-r--r--   0        0        0      121 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_exprs/test_nunique_where/out.sql
--rw-r--r--   0        0        0       98 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_exprs/test_where_with_timestamp/out.sql
--rw-r--r--   0        0        0       28 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/isin/out.sql
--rw-r--r--   0        0        0       32 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/notin/out.sql
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/isin/out.sql
--rw-r--r--   0        0        0       63 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/notin/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/isin/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/notin/out.sql
--rw-r--r--   0        0        0      161 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_group_by_with_window_preserves_range/out.sql
--rw-r--r--   0        0        0       69 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/isnull/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.655852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/notnull/out.sql
--rw-r--r--   0        0        0      105 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens_identical_to/out.sql
--rw-r--r--   0        0        0      690 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_aliasing/out.sql
--rw-r--r--   0        0        0      894 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name/out.sql
--rw-r--r--   0        0        0      604 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name2/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/cross_join/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/inner_join/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/left_join/out.sql
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/outer_join/out.sql
--rw-r--r--   0        0        0      118 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_or_condition/out.sql
--rw-r--r--   0        0        0      172 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_xor_condition/out.sql
--rw-r--r--   0        0        0      109 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_limit_cte_extract/out.sql
--rw-r--r--   0        0        0       74 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_logically_negate_complex_boolean_expr/out.sql
--rw-r--r--   0        0        0      157 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters/out.sql
--rw-r--r--   0        0        0      195 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters2/out.sql
--rw-r--r--   0        0        0      234 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_base/out.sql
--rw-r--r--   0        0        0      657 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_multiple_ctes/out.sql
--rw-r--r--   0        0        0      470 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_nested_joins_single_cte/out.sql
--rw-r--r--   0        0        0       71 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_sql/test_relabel_projection/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_find/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/ascii_str/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/capitalize/out.sql
--rw-r--r--   0        0        0       31 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/extract_host/out.sql
--rw-r--r--   0        0        0       29 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find/out.sql
--rw-r--r--   0        0        0       36 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_multiple/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_single/out.sql
--rw-r--r--   0        0        0       32 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_with_offset/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/length/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like_multiple/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lower/out.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_char/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_default/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lstrip/out.sql
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_extract/out.sql
--rw-r--r--   0        0        0       44 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_replace/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_search/out.sql
--rw-r--r--   0        0        0       23 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/repeat/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/reverse/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rlike/out.sql
--rw-r--r--   0        0        0       26 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_char/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_default/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rstrip/out.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strip/out.sql
--rw-r--r--   0        0        0       25 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strright/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_0_3/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_2/out.sql
--rw-r--r--   0        0        0       33 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/translate/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/upper/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_join/out.sql
--rw-r--r--   0        0        0      169 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/False/out.sql
--rw-r--r--   0        0        0      194 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/True/out.sql
--rw-r--r--   0        0        0       99 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf/out.sql
--rw-r--r--   0        0        0      115 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf_type_conversions/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_aggregate/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_db/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_if_exists/out.sql
--rw-r--r--   0        0        0       41 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_simple/out.sql
--rw-r--r--   0        0        0       32 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs_like/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_list_udf/out.sql
--rw-r--r--   0        0        0       38 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_list_udfs_like/out.sql
--rw-r--r--   0        0        0       73 2023-04-11 17:42:39.659852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation/out.sql
--rw-r--r--   0        0        0       52 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation_from_infoclass/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_hash/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/log_with_base/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_expr/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_no_args/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_two/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_zero/out.sql
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_double/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_float/out.sql
--rw-r--r--   0        0        0       36 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_tinyint/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-abs/out.sql
--rw-r--r--   0        0        0       25 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_median/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_nunique/out.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ceil/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-exp/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-floor/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ln/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log10/out.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log2/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-nullifzero/out.sql
--rw-r--r--   0        0        0       18 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-sqrt/out.sql
--rw-r--r--   0        0        0       24 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-zeroifnull/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-abs/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_median/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_nunique/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ceil/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-exp/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-floor/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ln/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log10/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log2/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-nullifzero/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-sqrt/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-zeroifnull/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/avg/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/count/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/max/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/min/out.sql
--rw-r--r--   0        0        0       53 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_pop/out.sql
--rw-r--r--   0        0        0       54 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_samp/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/sum/out.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_pop/out.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_samp/out.sql
--rw-r--r--   0        0        0       12 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/all/out.sql
--rw-r--r--   0        0        0       12 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/any/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_all/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_any/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_between/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/add/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/and/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.663852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/div/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/eq/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ge/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/gt/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/le/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/lt/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/mul/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ne/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/or/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/pow/out.sql
--rw-r--r--   0        0        0        9 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/sub/out.sql
--rw-r--r--   0        0        0       46 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/xor/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/function_call/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/negation/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/parens_left/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int16/out.sql
--rw-r--r--   0        0        0       16 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int32/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int64/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-string/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/d-int8/out.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-double/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-timestamp/out.sql
--rw-r--r--   0        0        0       29 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_column_ref_table_aliases/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/column/out.sql
--rw-r--r--   0        0        0       35 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/literal/out.sql
--rw-r--r--   0        0        0       17 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/compound_isnull/out.sql
--rw-r--r--   0        0        0       11 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/isnull/out.sql
--rw-r--r--   0        0        0       15 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/notnull/out.sql
--rw-r--r--   0        0        0       13 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_double_quote/out.sql
--rw-r--r--   0        0        0       10 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_single_quote/out.sql
--rw-r--r--   0        0        0        5 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/false/out.sql
--rw-r--r--   0        0        0        3 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/float/out.sql
--rw-r--r--   0        0        0        1 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/int/out.sql
--rw-r--r--   0        0        0        8 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/simple/out.sql
--rw-r--r--   0        0        0        4 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/true/out.sql
--rw-r--r--   0        0        0       14 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_misc_conditionals/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/cast/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/compound_expr/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/spaces/out.sql
--rw-r--r--   0        0        0        4 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/a/out.sql
--rw-r--r--   0        0        0        4 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/f/out.sql
--rw-r--r--   0        0        0        7 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/h/out.sql
--rw-r--r--   0        0        0      134 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_sql_extract/out.sql
--rw-r--r--   0        0        0       30 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/full_name/out.sql
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/index/out.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out1.sql
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out2.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out1.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out2.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out1.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out2.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out1.sql
--rw-r--r--   0        0        0       50 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out2.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out1.sql
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out2.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out1.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out2.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out1.sql
--rw-r--r--   0        0        0       49 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out2.sql
--rw-r--r--   0        0        0       19 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/day/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.667852 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/hour/out.sql
--rw-r--r--   0        0        0       27 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/millisecond/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/minute/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/month/out.sql
--rw-r--r--   0        0        0       22 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/second/out.sql
--rw-r--r--   0        0        0       20 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/year/out.sql
--rw-r--r--   0        0        0       60 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/default/out.sql
--rw-r--r--   0        0        0       87 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/ms/out.sql
--rw-r--r--   0        0        0       90 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/us/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pd_timestamp/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pydatetime/out.sql
--rw-r--r--   0        0        0       21 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/timestamp_function/out.sql
--rw-r--r--   0        0        0        5 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_now/out.sql
--rw-r--r--   0        0        0      442 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_add_default_order_by/out.sql
--rw-r--r--   0        0        0       72 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_aggregate_in_projection/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out1.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out2.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out1.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out2.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out1.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out2.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out1.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out2.sql
--rw-r--r--   0        0        0      111 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_multiple_windows/out.sql
--rw-r--r--   0        0        0      112 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_nested_analytic_function/out.sql
--rw-r--r--   0        0        0       91 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out1.sql
--rw-r--r--   0        0        0      172 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out2.sql
--rw-r--r--   0        0        0      152 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_propagate_nested_windows/out.sql
--rw-r--r--   0        0        0      147 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_rank_functions/out.sql
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out1.sql
--rw-r--r--   0        0        0      111 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out2.sql
--rw-r--r--   0        0        0       88 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_row_number_properly_composes_with_arithmetic/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/cumulative/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_0/out.sql
--rw-r--r--   0        0        0      113 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_10_5/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2/out.sql
--rw-r--r--   0        0        0      112 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2_prec_0/out.sql
--rw-r--r--   0        0        0      113 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_5_10/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_0/out.sql
--rw-r--r--   0        0        0      120 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5/out.sql
--rw-r--r--   0        0        0      112 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_0/out.sql
--rw-r--r--   0        0        0      112 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_2/out.sql
--rw-r--r--   0        0        0      113 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/trailing_10/out.sql
--rw-r--r--   0        0        0     1210 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_analytic_functions.py
--rw-r--r--   0        0        0     2900 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_bucket_histogram.py
--rw-r--r--   0        0        0     2849 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_case_exprs.py
--rw-r--r--   0        0        0     8748 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_client.py
--rw-r--r--   0        0        0     1040 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_coalesce_greater_least.py
--rw-r--r--   0        0        0    10554 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_ddl.py
--rw-r--r--   0        0        0     9155 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_ddl_compilation.py
--rw-r--r--   0        0        0    20021 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_exprs.py
--rw-r--r--   0        0        0     1168 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_in_not_in.py
--rw-r--r--   0        0        0     3821 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_metadata.py
--rw-r--r--   0        0        0     5644 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_pandas_interop.py
--rw-r--r--   0        0        0     2814 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_parquet_ddl.py
--rw-r--r--   0        0        0     7442 2023-04-11 17:42:39.671853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_partition.py
--rw-r--r--   0        0        0     1666 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_patched.py
--rw-r--r--   0        0        0     9546 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_sql.py
--rw-r--r--   0        0        0     2550 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_string_builtins.py
--rw-r--r--   0        0        0    17831 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_udf.py
--rw-r--r--   0        0        0     3300 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_unary_builtins.py
--rw-r--r--   0        0        0     7931 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_value_exprs.py
--rw-r--r--   0        0        0     5053 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/tests/test_window.py
--rw-r--r--   0        0        0     8879 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/impala/udf.py
--rw-r--r--   0        0        0     2464 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/__init__.py
--rw-r--r--   0        0        0     1041 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/compiler.py
--rw-r--r--   0        0        0     4704 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/datatypes.py
--rw-r--r--   0        0        0     7201 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/tests/__init__.py
--rw-r--r--   0        0        0     2825 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/tests/conftest.py
--rw-r--r--   0        0        0     2869 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mssql/tests/test_client.py
--rw-r--r--   0        0        0     3977 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/__init__.py
--rw-r--r--   0        0        0     1258 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/compiler.py
--rw-r--r--   0        0        0     6966 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/datatypes.py
--rw-r--r--   0        0        0     7164 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/tests/__init__.py
--rw-r--r--   0        0        0     4106 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/tests/conftest.py
--rw-r--r--   0        0        0     2711 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/mysql/tests/test_client.py
--rw-r--r--   0        0        0     9724 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/__init__.py
--rw-r--r--   0        0        0    21377 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/aggcontext.py
--rw-r--r--   0        0        0     7317 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/client.py
--rw-r--r--   0        0        0    19213 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/core.py
--rw-r--r--   0        0        0     2834 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/dispatch.py
--rw-r--r--   0        0        0     4543 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/dispatcher.py
--rw-r--r--   0        0        0      772 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/__init__.py
--rw-r--r--   0        0        0     4343 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/arrays.py
--rw-r--r--   0        0        0     2153 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/constants.py
--rw-r--r--   0        0        0     4231 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/decimal.py
--rw-r--r--   0        0        0    47556 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/generic.py
--rw-r--r--   0        0        0     5056 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/join.py
--rw-r--r--   0        0        0     6386 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/maps.py
--rw-r--r--   0        0        0    10776 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/selection.py
--rw-r--r--   0        0        0    15744 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/strings.py
--rw-r--r--   0        0        0     1411 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/structs.py
--rw-r--r--   0        0        0    10775 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/temporal.py
--rw-r--r--   0        0        0     2855 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/timecontext.py
--rw-r--r--   0        0        0     4001 2023-04-11 17:42:39.675853 ibis_framework-5.1.0/ibis/backends/pandas/execution/util.py
--rw-r--r--   0        0        0    17392 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/execution/window.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/__init__.py
--rw-r--r--   0        0        0     2166 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/__init__.py
--rw-r--r--   0        0        0     7968 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/conftest.py
--rw-r--r--   0        0        0     6197 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_arrays.py
--rw-r--r--   0        0        0     5270 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_cast.py
--rw-r--r--   0        0        0     8441 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_functions.py
--rw-r--r--   0        0        0    17768 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_join.py
--rw-r--r--   0        0        0     2777 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_maps.py
--rw-r--r--   0        0        0    28578 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_operations.py
--rw-r--r--   0        0        0     4159 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_strings.py
--rw-r--r--   0        0        0     2371 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_structs.py
--rw-r--r--   0        0        0     5864 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_temporal.py
--rw-r--r--   0        0        0    14390 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_timecontext.py
--rw-r--r--   0        0        0    21503 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/execution/test_window.py
--rw-r--r--   0        0        0     3984 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_aggcontext.py
--rw-r--r--   0        0        0     4122 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_client.py
--rw-r--r--   0        0        0     4802 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_core.py
--rw-r--r--   0        0        0     7727 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_datatypes.py
--rw-r--r--   0        0        0     2664 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_dispatcher.py
--rw-r--r--   0        0        0     5681 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_schema.py
--rw-r--r--   0        0        0    12058 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/tests/test_udf.py
--rw-r--r--   0        0        0     5844 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/trace.py
--rw-r--r--   0        0        0     6207 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/pandas/udf.py
--rw-r--r--   0        0        0    13905 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/__init__.py
--rw-r--r--   0        0        0    26301 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/compiler.py
--rw-r--r--   0        0        0     2798 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/datatypes.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/tests/__init__.py
--rw-r--r--   0        0        0     2376 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/tests/conftest.py
--rw-r--r--   0        0        0     2176 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/tests/test_datatypes.py
--rw-r--r--   0        0        0     1381 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/polars/tests/test_udf.py
--rw-r--r--   0        0        0     8259 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/compiler.py
--rw-r--r--   0        0        0     5272 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/datatypes.py
--rw-r--r--   0        0        0    22985 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/__init__.py
--rw-r--r--   0        0        0     5047 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/conftest.py
--rw-r--r--   0        0        0       47 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/snapshots/test_client/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0      814 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/False/out.sql
--rw-r--r--   0        0        0      806 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/True/out.sql
--rw-r--r--   0        0        0     6851 2023-04-11 17:42:39.679853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_client.py
--rw-r--r--   0        0        0    42822 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_functions.py
--rw-r--r--   0        0        0    19731 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_geospatial.py
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_json.py
--rw-r--r--   0        0        0     9808 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_postgis.py
--rw-r--r--   0        0        0      452 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_string.py
--rw-r--r--   0        0        0     6006 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/tests/test_udf.py
--rw-r--r--   0        0        0     6113 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/postgres/udf.py
--rw-r--r--   0        0        0      651 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyarrow/__init__.py
--rw-r--r--   0        0        0     4360 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyarrow/datatypes.py
--rw-r--r--   0        0        0    21652 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/__init__.py
--rw-r--r--   0        0        0     5245 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/client.py
--rw-r--r--   0        0        0    58914 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/compiler.py
--rw-r--r--   0        0        0     4695 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/datatypes.py
--rw-r--r--   0        0        0     5285 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/ddl.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/__init__.py
--rw-r--r--   0        0        0    12986 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/conftest.py
--rw-r--r--   0        0        0      981 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_aggregation.py
--rw-r--r--   0        0        0     5168 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_array.py
--rw-r--r--   0        0        0     7806 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_basic.py
--rw-r--r--   0        0        0     6036 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_ddl.py
--rw-r--r--   0        0        0      821 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_null.py
--rw-r--r--   0        0        0     4012 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_timecontext.py
--rw-r--r--   0        0        0     2377 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_window.py
--rw-r--r--   0        0        0    13843 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/tests/test_window_context_adjustment.py
--rw-r--r--   0        0        0     2590 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/pyspark/timecontext.py
--rw-r--r--   0        0        0    13214 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/__init__.py
--rw-r--r--   0        0        0     2745 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/datatypes.py
--rw-r--r--   0        0        0    14164 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/tests/__init__.py
--rw-r--r--   0        0        0     4168 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/tests/conftest.py
--rw-r--r--   0        0        0      824 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/snowflake/tests/test_client.py
--rw-r--r--   0        0        0     9795 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/sqlite/__init__.py
--rw-r--r--   0        0        0     2077 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/sqlite/compiler.py
--rw-r--r--   0        0        0     1682 2023-04-11 17:42:39.683853 ibis_framework-5.1.0/ibis/backends/sqlite/datatypes.py
--rw-r--r--   0        0        0    11386 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/registry.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/__init__.py
--rw-r--r--   0        0        0     3505 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/conftest.py
--rw-r--r--   0        0        0       42 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/snapshots/test_client/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0     2651 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/test_client.py
--rw-r--r--   0        0        0    21361 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/test_functions.py
--rw-r--r--   0        0        0     2506 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/tests/test_types.py
--rw-r--r--   0        0        0     8544 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/sqlite/udf.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/__init__.py
--rw-r--r--   0        0        0     7953 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/base.py
--rw-r--r--   0        0        0     2637 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/data.py
--rw-r--r--   0        0        0      511 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/bigquery/out.sql
--rw-r--r--   0        0        0     1294 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/clickhouse/out.sql
--rw-r--r--   0        0        0      497 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/duckdb/out.sql
--rw-r--r--   0        0        0      513 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/impala/out.sql
--rw-r--r--   0        0        0      523 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mssql/out.sql
--rw-r--r--   0        0        0      535 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mysql/out.sql
--rw-r--r--   0        0        0      497 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/postgres/out.sql
--rw-r--r--   0        0        0      543 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/snowflake/out.sql
--rw-r--r--   0        0        0      523 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/sqlite/out.sql
--rw-r--r--   0        0        0      497 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/trino/out.sql
--rw-r--r--   0        0        0      267 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/bigquery/out.sql
--rw-r--r--   0        0        0      588 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/clickhouse/out.sql
--rw-r--r--   0        0        0      281 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/duckdb/out.sql
--rw-r--r--   0        0        0      267 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/impala/out.sql
--rw-r--r--   0        0        0      287 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mssql/out.sql
--rw-r--r--   0        0        0      302 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mysql/out.sql
--rw-r--r--   0        0        0      264 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/postgres/out.sql
--rw-r--r--   0        0        0      288 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/snowflake/out.sql
--rw-r--r--   0        0        0      287 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/sqlite/out.sql
--rw-r--r--   0        0        0      264 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/trino/out.sql
--rw-r--r--   0        0        0      387 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/bigquery/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/clickhouse/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/duckdb/out.sql
--rw-r--r--   0        0        0      387 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/impala/out.sql
--rw-r--r--   0        0        0      701 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mssql/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mysql/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/postgres/out.sql
--rw-r--r--   0        0        0      389 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/snowflake/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/sqlite/out.sql
--rw-r--r--   0        0        0      379 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/trino/out.sql
--rw-r--r--   0        0        0      169 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/bigquery/out.sql
--rw-r--r--   0        0        0      151 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/clickhouse/out.sql
--rw-r--r--   0        0        0      197 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/duckdb/out.sql
--rw-r--r--   0        0        0      180 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/impala/out.sql
--rw-r--r--   0        0        0      179 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mssql/out.sql
--rw-r--r--   0        0        0      179 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mysql/out.sql
--rw-r--r--   0        0        0      179 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/postgres/out.sql
--rw-r--r--   0        0        0      193 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/snowflake/out.sql
--rw-r--r--   0        0        0      179 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/sqlite/out.sql
--rw-r--r--   0        0        0      179 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_isin_bug/trino/out.sql
--rw-r--r--   0        0        0     6212 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/clickhouse/out.sql
--rw-r--r--   0        0        0     2824 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/duckdb/out.sql
--rw-r--r--   0        0        0     2895 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/postgres/out.sql
--rw-r--r--   0        0        0     3166 2023-04-11 17:42:39.687854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/trino/out.sql
--rw-r--r--   0        0        0      118 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/bigquery/out.sql
--rw-r--r--   0        0        0      100 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/clickhouse/out.sql
--rw-r--r--   0        0        0      311 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/duckdb/out.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/impala/out.sql
--rw-r--r--   0        0        0      332 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/mysql/out.sql
--rw-r--r--   0        0        0      302 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/postgres/out.sql
--rw-r--r--   0        0        0      372 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/snowflake/out.sql
--rw-r--r--   0        0        0      335 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/sqlite/out.sql
--rw-r--r--   0        0        0      324 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/snapshots/test_string/test_rlike/trino/out.sql
--rw-r--r--   0        0        0    43926 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_aggregation.py
--rw-r--r--   0        0        0     4052 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_api.py
--rw-r--r--   0        0        0    18412 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_array.py
--rw-r--r--   0        0        0     1063 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_binary.py
--rw-r--r--   0        0        0    37836 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_client.py
--rw-r--r--   0        0        0     1089 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_column.py
--rw-r--r--   0        0        0     5442 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_dot_sql.py
--rw-r--r--   0        0        0     7691 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_export.py
--rw-r--r--   0        0        0    35336 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_generic.py
--rw-r--r--   0        0        0     6933 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_join.py
--rw-r--r--   0        0        0     2661 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_json.py
--rw-r--r--   0        0        0     7471 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_map.py
--rw-r--r--   0        0        0     3427 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_network.py
--rw-r--r--   0        0        0    50136 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_numeric.py
--rw-r--r--   0        0        0     6248 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_param.py
--rw-r--r--   0        0        0    11871 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_register.py
--rw-r--r--   0        0        0     6841 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_set_ops.py
--rw-r--r--   0        0        0     6172 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_sql.py
--rw-r--r--   0        0        0    31330 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_string.py
--rw-r--r--   0        0        0     2737 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_struct.py
--rw-r--r--   0        0        0    78946 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_temporal.py
--rw-r--r--   0        0        0     3603 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_timecontext.py
--rw-r--r--   0        0        0     1869 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_uuid.py
--rw-r--r--   0        0        0    24095 2023-04-11 17:42:39.691854 ibis_framework-5.1.0/ibis/backends/tests/test_vectorized_udf.py
--rw-r--r--   0        0        0    33635 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/tests/test_window.py
--rw-r--r--   0        0        0     2843 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/trino/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/trino/compiler.py
--rw-r--r--   0        0        0     5700 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/trino/datatypes.py
--rw-r--r--   0        0        0    14301 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/trino/registry.py
--rw-r--r--   0        0        0     5542 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/backends/trino/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/__init__.py
--rw-r--r--   0        0        0    15880 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/annotations.py
--rw-r--r--   0        0        0     4050 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/caching.py
--rw-r--r--   0        0        0     6204 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/collections.py
--rw-r--r--   0        0        0     2931 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/dispatch.py
--rw-r--r--   0        0        0     2655 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/exceptions.py
--rw-r--r--   0        0        0     6318 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/graph.py
--rw-r--r--   0        0        0     7990 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/grounds.py
--rw-r--r--   0        0        0      978 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/parsing.py
--rw-r--r--   0        0        0      150 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/conftest.py
--rw-r--r--   0        0        0    11437 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_annotations.py
--rw-r--r--   0        0        0     6334 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_collections.py
--rw-r--r--   0        0        0     2407 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_dispatch.py
--rw-r--r--   0        0        0     4277 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_graph.py
--rw-r--r--   0        0        0    26172 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_grounds.py
--rw-r--r--   0        0        0     1023 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_grounds_py310.py
--rw-r--r--   0        0        0      322 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_typing.py
--rw-r--r--   0        0        0     8745 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/tests/test_validators.py
--rw-r--r--   0        0        0     1437 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/typing.py
--rw-r--r--   0        0        0    18013 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/common/validators.py
--rw-r--r--   0        0        0     5937 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/config.py
--rw-r--r--   0        0        0      686 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/conftest.py
--rw-r--r--   0        0        0      758 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/examples/CITATIONS.md
--rw-r--r--   0        0        0     2084 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/examples/__init__.py
--rw-r--r--   0        0        0    45010 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/examples/metadata.json
--rw-r--r--   0        0        0    39108 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/examples/registry.txt
--rw-r--r--   0        0        0     1296 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/examples/tests/test_examples.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.695854 ibis_framework-5.1.0/ibis/expr/__init__.py
--rw-r--r--   0        0        0    28489 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/analysis.py
--rw-r--r--   0        0        0    40193 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/api.py
--rw-r--r--   0        0        0     9416 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/builders.py
--rw-r--r--   0        0        0      523 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/__init__.py
--rw-r--r--   0        0        0     6868 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/cast.py
--rw-r--r--   0        0        0    24933 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/core.py
--rw-r--r--   0        0        0     5667 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/parse.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/tests/__init__.py
--rw-r--r--   0        0        0     1703 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/tests/test_cast.py
--rw-r--r--   0        0        0    14764 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/tests/test_core.py
--rw-r--r--   0        0        0     7175 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/tests/test_parse.py
--rw-r--r--   0        0        0     3037 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/tests/test_value.py
--rw-r--r--   0        0        0    11431 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/datatypes/value.py
--rw-r--r--   0        0        0    11092 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/decompile.py
--rw-r--r--   0        0        0     4601 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/deferred.py
--rw-r--r--   0        0        0    20314 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/format.py
--rw-r--r--   0        0        0     1068 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/analytic.py
--rw-r--r--   0        0        0     4125 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/arrays.py
--rw-r--r--   0        0        0     3053 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/core.py
--rw-r--r--   0        0        0     7187 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/generic.py
--rw-r--r--   0        0        0    10458 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/geospatial.py
--rw-r--r--   0        0        0     1480 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/histograms.py
--rw-r--r--   0        0        0      615 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/json.py
--rw-r--r--   0        0        0     6541 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/logical.py
--rw-r--r--   0        0        0     1764 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/maps.py
--rw-r--r--   0        0        0     6504 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/numeric.py
--rw-r--r--   0        0        0     6720 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/reductions.py
--rw-r--r--   0        0        0    18783 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/relations.py
--rw-r--r--   0        0        0      535 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/sortkeys.py
--rw-r--r--   0        0        0     5005 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/strings.py
--rw-r--r--   0        0        0      980 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/structs.py
--rw-r--r--   0        0        0     7847 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/temporal.py
--rw-r--r--   0        0        0     1096 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/vectorized.py
--rw-r--r--   0        0        0     3576 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/operations/window.py
--rw-r--r--   0        0        0    17954 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/rules.py
--rw-r--r--   0        0        0     9558 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/schema.py
--rw-r--r--   0        0        0      225 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/selectors.py
--rw-r--r--   0        0        0    10081 2023-04-11 17:42:39.699854 ibis_framework-5.1.0/ibis/expr/sql.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/tests/__init__.py
--rw-r--r--   0        0        0      206 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/tests/test_deferred.py
--rw-r--r--   0        0        0     9562 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/tests/test_rules.py
--rw-r--r--   0        0        0     9794 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/tests/test_schema.py
--rw-r--r--   0        0        0      861 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/__init__.py
--rw-r--r--   0        0        0    33476 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/arrays.py
--rw-r--r--   0        0        0      819 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/binary.py
--rw-r--r--   0        0        0      271 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/collections.py
--rw-r--r--   0        0        0    16532 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/core.py
--rw-r--r--   0        0        0    34589 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/generic.py
--rw-r--r--   0        0        0    20863 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/geospatial.py
--rw-r--r--   0        0        0    10060 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/groupby.py
--rw-r--r--   0        0        0      500 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/inet.py
--rw-r--r--   0        0        0     4997 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/json.py
--rw-r--r--   0        0        0     3247 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/logical.py
--rw-r--r--   0        0        0     5390 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/maps.py
--rw-r--r--   0        0        0    23885 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/numeric.py
--rw-r--r--   0        0        0    11977 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/pretty.py
--rw-r--r--   0        0        0   194743 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/relations.py
--rw-r--r--   0        0        0       37 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/ruff.toml
--rw-r--r--   0        0        0    50538 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/strings.py
--rw-r--r--   0        0        0     6274 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/structs.py
--rw-r--r--   0        0        0    16084 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/temporal.py
--rw-r--r--   0        0        0      146 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/typing.py
--rw-r--r--   0        0        0      312 2023-04-11 17:42:39.703855 ibis_framework-5.1.0/ibis/expr/types/uuid.py
--rw-r--r--   0        0        0     5371 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/expr/visualize.py
--rw-r--r--   0        0        0      171 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/interactive.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/py.typed
--rw-r--r--   0        0        0    12988 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/selectors.py
--rw-r--r--   0        0        0      609 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0    19098 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/benchmarks/test_benchmarks.py
--rw-r--r--   0        0        0      754 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/__init__.py
--rw-r--r--   0        0        0     2527 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/conftest.py
--rw-r--r--   0        0        0    15824 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/mocks.py
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/snapshots/test_interactive/test_default_limit/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/snapshots/test_interactive/test_disable_query_limit/out.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/snapshots/test_interactive/test_respect_set_limit/out.sql
--rw-r--r--   0        0        0     9636 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_analysis.py
--rw-r--r--   0        0        0     2732 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_analytics.py
--rw-r--r--   0        0        0     2708 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_case.py
--rw-r--r--   0        0        0     4070 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_decimal.py
--rw-r--r--   0        0        0     1855 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_decompile.py
--rw-r--r--   0        0        0     9573 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_format.py
--rw-r--r--   0        0        0     3259 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_interactive.py
--rw-r--r--   0        0        0     4802 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_literal.py
--rw-r--r--   0        0        0     6638 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_operations.py
--rw-r--r--   0        0        0      789 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_operations_py310.py
--rw-r--r--   0        0        0     1564 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_pipe.py
--rw-r--r--   0        0        0     4816 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_pretty_repr.py
--rw-r--r--   0        0        0    11230 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_selectors.py
--rw-r--r--   0        0        0     1217 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_set_operations.py
--rw-r--r--   0        0        0     2830 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_sql.py
--rw-r--r--   0        0        0     5858 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_sql_builtins.py
--rw-r--r--   0        0        0     3514 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_string.py
--rw-r--r--   0        0        0     2331 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_struct.py
--rw-r--r--   0        0        0    53587 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_table.py
--rw-r--r--   0        0        0    19806 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_temporal.py
--rw-r--r--   0        0        0     5476 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_timestamp.py
--rw-r--r--   0        0        0     2260 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_udf.py
--rw-r--r--   0        0        0    48206 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_value_exprs.py
--rw-r--r--   0        0        0     4733 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_visualize.py
--rw-r--r--   0        0        0    14988 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_window_frames.py
--rw-r--r--   0        0        0     1478 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/expr/test_window_functions.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/sql/__init__.py
--rw-r--r--   0        0        0     4844 2023-04-11 17:42:39.707855 ibis_framework-5.1.0/ibis/tests/sql/conftest.py
--rw-r--r--   0        0        0      207 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_agg_and_non_agg_filter/out.sql
--rw-r--r--   0        0        0      214 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_agg_filter/out.sql
--rw-r--r--   0        0        0      214 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_agg_filter_with_alias/out.sql
--rw-r--r--   0        0        0      582 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_distinct/decompiled.py
--rw-r--r--   0        0        0       59 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_distinct/out.sql
--rw-r--r--   0        0        0      128 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_expr_default_name/decompiled.py
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_expr_default_name/out.sql
--rw-r--r--   0        0        0      142 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/decompiled.py
--rw-r--r--   0        0        0       54 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/out.sql
--rw-r--r--   0        0        0      699 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_count_distinct/decompiled.py
--rw-r--r--   0        0        0      130 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_count_distinct/out.sql
--rw-r--r--   0        0        0     1049 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_difference_project_column/decompiled.py
--rw-r--r--   0        0        0      450 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_difference_project_column/out.sql
--rw-r--r--   0        0        0      201 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_having_from_filter/decompiled.py
--rw-r--r--   0        0        0       98 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_having_from_filter/out.sql
--rw-r--r--   0        0        0      114 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_having_size/out.sql
--rw-r--r--   0        0        0     1056 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_intersect_project_column/decompiled.py
--rw-r--r--   0        0        0      453 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_intersect_project_column/out.sql
--rw-r--r--   0        0        0      736 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/decompiled.py
--rw-r--r--   0        0        0      166 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/out.sql
--rw-r--r--   0        0        0      187 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_pushdown_with_or/out.sql
--rw-r--r--   0        0        0      169 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_simple_agg_filter/out.sql
--rw-r--r--   0        0        0      502 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_subquery_where_location/decompiled.py
--rw-r--r--   0        0        0      288 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_subquery_where_location/out.sql
--rw-r--r--   0        0        0     1020 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_difference/decompiled.py
--rw-r--r--   0        0        0      386 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_difference/out.sql
--rw-r--r--   0        0        0      619 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_distinct/decompiled.py
--rw-r--r--   0        0        0       73 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_distinct/out.sql
--rw-r--r--   0        0        0      427 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/decompiled.py
--rw-r--r--   0        0        0      335 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/out.sql
--rw-r--r--   0        0        0     1027 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_intersect/decompiled.py
--rw-r--r--   0        0        0      389 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_table_intersect/out.sql
--rw-r--r--   0        0        0      995 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union/decompiled.py
--rw-r--r--   0        0        0      385 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union/out.sql
--rw-r--r--   0        0        0      174 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union_order_by/decompiled.py
--rw-r--r--   0        0        0      160 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union_order_by/out.sql
--rw-r--r--   0        0        0     1000 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union_project_column/decompiled.py
--rw-r--r--   0        0        0      453 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_compiler/test_union_project_column/out.sql
--rw-r--r--   0        0        0      555 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/decompiled.py
--rw-r--r--   0        0        0      174 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/out.sql
--rw-r--r--   0        0        0       91 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_having/explicit.sql
--rw-r--r--   0        0        0       89 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_having/inline.sql
--rw-r--r--   0        0        0      172 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_projection_alias_bug/out.sql
--rw-r--r--   0        0        0      175 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered.sql
--rw-r--r--   0        0        0      164 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered2.sql
--rw-r--r--   0        0        0      100 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/filtered.sql
--rw-r--r--   0        0        0       71 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/proj.sql
--rw-r--r--   0        0        0      324 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_anti_join/decompiled.py
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_anti_join/out.sql
--rw-r--r--   0        0        0      197 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_bool_bool/decompiled.py
--rw-r--r--   0        0        0       73 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_bool_bool/out.sql
--rw-r--r--   0        0        0      359 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_bug_duplicated_where/out.sql
--rw-r--r--   0        0        0      567 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_bug_project_multiple_times/out.sql
--rw-r--r--   0        0        0      832 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_case_in_projection/decompiled.py
--rw-r--r--   0        0        0      255 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_case_in_projection/out.sql
--rw-r--r--   0        0        0      823 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_complex_union/result.sql
--rw-r--r--   0        0        0      274 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_double_nested_subquery_no_aliases/out.sql
--rw-r--r--   0        0        0      217 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_endswith/decompiled.py
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_endswith/out.sql
--rw-r--r--   0        0        0      180 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_filter_inside_exists/out.sql
--rw-r--r--   0        0        0      226 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_filter_predicates/out.sql
--rw-r--r--   0        0        0      344 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_filter_self_join_analysis_bug/result.sql
--rw-r--r--   0        0        0      126 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr3.sql
--rw-r--r--   0        0        0      132 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr4.sql
--rw-r--r--   0        0        0      300 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_fuse_projections/decompiled.py
--rw-r--r--   0        0        0      104 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_fuse_projections/project.sql
--rw-r--r--   0        0        0      121 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_fuse_projections/project_filter.sql
--rw-r--r--   0        0        0       66 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_identifier_quoting/out.sql
--rw-r--r--   0        0        0       79 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown/result.sql
--rw-r--r--   0        0        0       70 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown_with_literal/result.sql
--rw-r--r--   0        0        0      690 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_between_joins/decompiled.py
--rw-r--r--   0        0        0      316 2023-04-11 17:42:39.711855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_between_joins/out.sql
--rw-r--r--   0        0        0      409 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_filtered_tables_no_pushdown/out.sql
--rw-r--r--   0        0        0      848 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_just_materialized/decompiled.py
--rw-r--r--   0        0        0      172 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_just_materialized/out.sql
--rw-r--r--   0        0        0      286 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_projection_subquery_bug/out.sql
--rw-r--r--   0        0        0      131 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_join_with_limited_table/out.sql
--rw-r--r--   0        0        0      109 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_limit_cte_extract/out.sql
--rw-r--r--   0        0        0     2331 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/decompiled.py
--rw-r--r--   0        0        0     1205 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/out.sql
--rw-r--r--   0        0        0      323 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_loj_subquery_filter_handling/out.sql
--rw-r--r--   0        0        0      748 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_multiple_joins/decompiled.py
--rw-r--r--   0        0        0      301 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_multiple_joins/out.sql
--rw-r--r--   0        0        0      595 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_multiple_limits/decompiled.py
--rw-r--r--   0        0        0       48 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_multiple_limits/out.sql
--rw-r--r--   0        0        0       72 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_nameless_table/decompiled.py
--rw-r--r--   0        0        0       23 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_nameless_table/out.sql
--rw-r--r--   0        0        0      698 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/decompiled.py
--rw-r--r--   0        0        0      151 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/out.sql
--rw-r--r--   0        0        0       88 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_projection_filter_fuse/out.sql
--rw-r--r--   0        0        0       89 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_scalar_subquery_different_table/out.sql
--rw-r--r--   0        0        0      215 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/decompiled.py
--rw-r--r--   0        0        0       67 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/out.sql
--rw-r--r--   0        0        0      237 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/decompiled.py
--rw-r--r--   0        0        0       83 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/out.sql
--rw-r--r--   0        0        0      190 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/decompiled.py
--rw-r--r--   0        0        0       40 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/decompiled.py
--rw-r--r--   0        0        0       51 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/out.sql
--rw-r--r--   0        0        0      148 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/decompiled.py
--rw-r--r--   0        0        0       34 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/decompiled.py
--rw-r--r--   0        0        0       81 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/out.sql
--rw-r--r--   0        0        0      151 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/decompiled.py
--rw-r--r--   0        0        0       43 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/out.sql
--rw-r--r--   0        0        0      195 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/decompiled.py
--rw-r--r--   0        0        0       58 2023-04-11 17:42:39.715855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/out.sql
--rw-r--r--   0        0        0      145 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/decompiled.py
--rw-r--r--   0        0        0       25 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/out.sql
--rw-r--r--   0        0        0      177 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/decompiled.py
--rw-r--r--   0        0        0       45 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/out.sql
--rw-r--r--   0        0        0      328 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/decompiled.py
--rw-r--r--   0        0        0       28 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/out.sql
--rw-r--r--   0        0        0      233 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_self_join_subquery_distinct_equal/out.sql
--rw-r--r--   0        0        0      324 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_semi_join/decompiled.py
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_semi_join/out.sql
--rw-r--r--   0        0        0      363 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_simple_joins/decompiled.py
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_simple_joins/inner.sql
--rw-r--r--   0        0        0      121 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_simple_joins/inner_two_preds.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_simple_joins/left.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_simple_joins/outer.sql
--rw-r--r--   0        0        0      148 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result1.sql
--rw-r--r--   0        0        0      148 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result2.sql
--rw-r--r--   0        0        0      219 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_startswith/decompiled.py
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_startswith/out.sql
--rw-r--r--   0        0        0      530 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_factor_correlated_subquery/out.sql
--rw-r--r--   0        0        0       94 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr.sql
--rw-r--r--   0        0        0      122 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr2.sql
--rw-r--r--   0        0        0      620 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_in_union/decompiled.py
--rw-r--r--   0        0        0      531 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_in_union/out.sql
--rw-r--r--   0        0        0      418 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_subquery_used_for_self_join/out.sql
--rw-r--r--   0        0        0      422 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_topk_analysis_bug/out.sql
--rw-r--r--   0        0        0      234 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_topk_operation/e1.sql
--rw-r--r--   0        0        0      232 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_topk_operation/e2.sql
--rw-r--r--   0        0        0      476 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_topk_predicate_pushdown_bug/out.sql
--rw-r--r--   0        0        0      157 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_topk_to_aggregate/out.sql
--rw-r--r--   0        0        0      698 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_tpch_self_join_failure/out.sql
--rw-r--r--   0        0        0      808 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/decompiled.py
--rw-r--r--   0        0        0      237 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/out.sql
--rw-r--r--   0        0        0      406 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/decompiled.py
--rw-r--r--   0        0        0      164 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/out.sql
--rw-r--r--   0        0        0      440 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_with_between/decompiled.py
--rw-r--r--   0        0        0       82 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_with_between/out.sql
--rw-r--r--   0        0        0      416 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_with_join/decompiled.py
--rw-r--r--   0        0        0      156 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_select_sql/test_where_with_join/out.sql
--rw-r--r--   0        0        0       94 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_count/out.sql
--rw-r--r--   0        0        0       94 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_sum/out.sql
--rw-r--r--   0        0        0       70 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_aggregate/single/out.sql
--rw-r--r--   0        0        0       88 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_aggregate/two/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_between/out.sql
--rw-r--r--   0        0        0       86 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/and/out.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/or/out.sql
--rw-r--r--   0        0        0      168 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_coalesce/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/eq/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ge/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/gt/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/le/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/lt/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ne/out.sql
--rw-r--r--   0        0        0      167 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_cte_factor_distinct_but_equal/out.sql
--rw-r--r--   0        0        0       77 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_distinct/count_distinct/out.sql
--rw-r--r--   0        0        0      107 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_distinct/group_by_count_distinct/out.sql
--rw-r--r--   0        0        0       76 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_distinct/projection_distinct/out.sql
--rw-r--r--   0        0        0       62 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_distinct/single_column_projection_distinct/out.sql
--rw-r--r--   0        0        0      252 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_distinct/table_distinct/out.sql
--rw-r--r--   0        0        0      161 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_exists/e1.sql
--rw-r--r--   0        0        0      181 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_exists/e2.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_filter_group_by_agg_with_same_name/out.sql
--rw-r--r--   0        0        0      631 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_gh_1045/out.sql
--rw-r--r--   0        0        0       68 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/isnull/out.sql
--rw-r--r--   0        0        0       72 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/notnull/out.sql
--rw-r--r--   0        0        0      390 2023-04-11 17:42:39.719855 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_join_just_materialized/out.sql
--rw-r--r--   0        0        0      200 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/inner/out.sql
--rw-r--r--   0        0        0      153 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/inner_select/out.sql
--rw-r--r--   0        0        0      211 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/left/out.sql
--rw-r--r--   0        0        0      164 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/left_select/out.sql
--rw-r--r--   0        0        0      211 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/outer/out.sql
--rw-r--r--   0        0        0      164 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_joins/outer_select/out.sql
--rw-r--r--   0        0        0       73 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn0/out.sql
--rw-r--r--   0        0        0       82 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn1/out.sql
--rw-r--r--   0        0        0       90 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_limit_filter/out.sql
--rw-r--r--   0        0        0      197 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_limit_subquery/out.sql
--rw-r--r--   0        0        0      489 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/decompiled.py
--rw-r--r--   0        0        0      459 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/out.sql
--rw-r--r--   0        0        0      252 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_multi_join/out.sql
--rw-r--r--   0        0        0      173 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_mutate_filter_join_no_cross_join/out.sql
--rw-r--r--   0        0        0       64 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_named_expr/out.sql
--rw-r--r--   0        0        0       65 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_negate/out.sql
--rw-r--r--   0        0        0      576 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_no_cart_join/out.sql
--rw-r--r--   0        0        0      241 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_no_cross_join/out.sql
--rw-r--r--   0        0        0      187 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_not_exists/out.sql
--rw-r--r--   0        0        0       85 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_order_by/ascending/out.sql
--rw-r--r--   0        0        0       80 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_order_by/column/out.sql
--rw-r--r--   0        0        0       93 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_order_by/mixed/out.sql
--rw-r--r--   0        0        0       84 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_order_by/random/out.sql
--rw-r--r--   0        0        0      139 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_order_by_expr/out.sql
--rw-r--r--   0        0        0      176 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_searched_case/out.sql
--rw-r--r--   0        0        0      399 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/anti.sql
--rw-r--r--   0        0        0      373 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/semi.sql
--rw-r--r--   0        0        0      108 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_self_reference_join/out.sql
--rw-r--r--   0        0        0      108 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_simple_case/out.sql
--rw-r--r--   0        0        0      192 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_sort_aggregation_translation_failure/out.sql
--rw-r--r--   0        0        0      203 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_subquery_aliased/out.sql
--rw-r--r--   0        0        0      840 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_tpc_h11/out.sql
--rw-r--r--   0        0        0      344 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_tpc_h17/out.sql
--rw-r--r--   0        0        0      183 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery/out.sql
--rw-r--r--   0        0        0      542 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery_with_join/out.sql
--rw-r--r--   0        0        0      200 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/decompiled.py
--rw-r--r--   0        0        0      101 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/out.sql
--rw-r--r--   0        0        0      130 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/snapshots/test_sqlalchemy/test_where_uncorrelated_subquery/out.sql
--rw-r--r--   0        0        0     2145 2023-04-11 17:42:39.723856 ibis_framework-5.1.0/ibis/tests/sql/test_ast_builder.py
--rw-r--r--   0        0        0     7587 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/sql/test_compiler.py
--rw-r--r--   0        0        0    26246 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/sql/test_select_sql.py
--rw-r--r--   0        0        0    18400 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/sql/test_sqlalchemy.py
--rw-r--r--   0        0        0     5712 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/strategies.py
--rw-r--r--   0        0        0     1865 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/test_api.py
--rw-r--r--   0        0        0      356 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/test_config.py
--rw-r--r--   0        0        0     4647 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/test_strategies.py
--rw-r--r--   0        0        0     1453 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/test_util.py
--rw-r--r--   0        0        0      190 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/test_version.py
--rw-r--r--   0        0        0     1328 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/tests/util.py
--rw-r--r--   0        0        0        0 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/udf/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/udf/validate.py
--rw-r--r--   0        0        0    11811 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/udf/vectorized.py
--rw-r--r--   0        0        0    12966 2023-04-11 17:42:39.727856 ibis_framework-5.1.0/ibis/util.py
--rw-r--r--   0        0        0    15616 2023-04-11 17:43:50.475905 ibis_framework-5.1.0/pyproject.toml
--rw-r--r--   0        0        0    87581 1970-01-01 00:00:00.000000 ibis_framework-5.1.0/setup.py
--rw-r--r--   0        0        0    16783 1970-01-01 00:00:00.000000 ibis_framework-5.1.0/PKG-INFO
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/docs/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      925 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/build-notebooks.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/docs/sphinxext/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/sphinxext/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/docs/sphinxext/ipython_sphinxext/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-10-07 03:41:44.000000 ibis-framework-v0.6.0/docs/sphinxext/ipython_sphinxext/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      116 2015-10-07 03:41:44.000000 ibis-framework-v0.6.0/docs/sphinxext/ipython_sphinxext/LICENSE
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    37645 2015-10-07 03:41:44.000000 ibis-framework-v0.6.0/docs/sphinxext/ipython_sphinxext/ipython_directive.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4181 2015-10-07 03:41:44.000000 ibis-framework-v0.6.0/docs/sphinxext/ipython_sphinxext/ipython_console_highlighting.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)       74 2015-06-10 22:32:58.000000 ibis-framework-v0.6.0/docs/README
+-rw-r--r--   0 wesm      (1000) wesm      (1000)       26 2015-06-10 22:32:58.000000 ibis-framework-v0.6.0/docs/requirements-docs.txt
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/docs/source/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8595 2015-10-07 03:41:44.000000 ibis-framework-v0.6.0/docs/source/conf.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      236 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/docs/source/tutorial.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    23073 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/docs/source/impala.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1722 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/source/developer.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2578 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/docs/source/index.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3190 2015-09-02 07:50:13.000000 ibis-framework-v0.6.0/docs/source/configuration.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    10447 2015-11-30 09:40:30.000000 ibis-framework-v0.6.0/docs/source/release.rst
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/docs/source/_templates/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      487 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/source/_templates/layout.html
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    33258 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/docs/source/sql.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    11507 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/source/legal.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      102 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/source/type-system.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4044 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/docs/source/getting-started.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8770 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/docs/source/api.rst
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6464 2015-06-10 22:32:58.000000 ibis-framework-v0.6.0/docs/make.bat
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     7377 2015-07-24 17:45:25.000000 ibis-framework-v0.6.0/docs/Makefile
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1750 2015-11-05 21:11:43.000000 ibis-framework-v0.6.0/README.md
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        5 2015-11-30 09:48:45.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/top_level.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      841 2015-11-30 09:48:45.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/PKG-INFO
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        1 2015-11-30 09:48:45.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4409 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)       46 2015-11-30 09:48:45.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/pbr.json
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      119 2015-11-30 09:48:45.000000 ibis-framework-v0.6.0/ibis_framework.egg-info/requires.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    62474 2015-10-08 04:18:58.000000 ibis-framework-v0.6.0/versioneer.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1383 2015-08-25 05:04:44.000000 ibis-framework-v0.6.0/ibis/config_init.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3771 2015-10-08 04:18:58.000000 ibis-framework-v0.6.0/ibis/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2416 2015-05-11 04:48:02.000000 ibis-framework-v0.6.0/ibis/wire.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     7815 2015-08-25 05:04:44.000000 ibis-framework-v0.6.0/ibis/tasks.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    32671 2015-01-21 05:11:59.000000 ibis-framework-v0.6.0/ibis/comms.pyx
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    31387 2015-08-24 21:56:32.000000 ibis-framework-v0.6.0/ibis/cloudpickle.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    20779 2015-07-13 05:54:08.000000 ibis-framework-v0.6.0/ibis/config.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    13243 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/client.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/spark/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/spark/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/spark/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/spark/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1619 2015-11-01 14:03:25.000000 ibis-framework-v0.6.0/ibis/compat.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/src/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2239 2015-01-24 22:13:49.000000 ibis-framework-v0.6.0/ibis/src/ipc_support.c
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1445 2015-01-21 05:11:59.000000 ibis-framework-v0.6.0/ibis/src/ipc_support.h
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/hive/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/hive/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/hive/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/hive/tests/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-05-11 04:48:04.000000 ibis-framework-v0.6.0/ibis/sql/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    23190 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/sql/alchemy.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/redshift/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/redshift/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/redshift/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/redshift/tests/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2768 2015-10-08 04:27:31.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/client.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1400 2015-10-08 04:27:31.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/api.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4806 2015-10-08 03:41:51.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/compiler.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9911 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/test_functions.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      616 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/conftest.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1970 2015-09-02 00:57:42.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/common.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3047 2015-10-08 04:27:31.000000 ibis-framework-v0.6.0/ibis/sql/sqlite/tests/test_client.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3701 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/sql/transforms.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/presto/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/presto/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/presto/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/presto/tests/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/postgres/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/sql/postgres/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/postgres/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/sql/postgres/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      616 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/sql/postgres/tests/conftest.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/vertica/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/vertica/__init__.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/vertica/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/sql/vertica/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    43932 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/sql/compiler.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/sql/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-05-11 04:48:05.000000 ibis-framework-v0.6.0/ibis/sql/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      616 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/sql/tests/conftest.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    59525 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/sql/tests/test_compiler.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    18028 2015-09-10 15:51:22.000000 ibis-framework-v0.6.0/ibis/sql/tests/test_sqlalchemy.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     5330 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/util.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      472 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/_version.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/impala/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/impala/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9517 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/impala/udf.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2672 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/impala/identifiers.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8436 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/impala/metadata.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    62350 2015-11-30 09:40:30.000000 ibis-framework-v0.6.0/ibis/impala/client.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3428 2015-08-20 06:26:34.000000 ibis-framework-v0.6.0/ibis/impala/madlib.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      728 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/impala/compat.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      649 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/impala/parquet.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3531 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/impala/api.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    24037 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/impala/ddl.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    37724 2015-11-29 21:58:21.000000 ibis-framework-v0.6.0/ibis/impala/compiler.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/impala/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/impala/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      616 2015-08-14 15:53:00.000000 ibis-framework-v0.6.0/ibis/impala/tests/conftest.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8090 2015-09-03 06:45:25.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_window.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    47622 2015-11-29 21:58:21.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_exprs.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1100 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_sql.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    36166 2015-11-30 09:40:30.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_ddl.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4536 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_metadata.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    18191 2015-08-27 14:46:57.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_udf.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1787 2015-09-09 04:43:12.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_madlib.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6556 2015-11-22 23:43:12.000000 ibis-framework-v0.6.0/ibis/impala/tests/common.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9610 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_pandas_interop.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    10737 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_client.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8670 2015-11-30 09:43:53.000000 ibis-framework-v0.6.0/ibis/impala/tests/test_partition.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6233 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/impala/pandas_interop.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9745 2015-08-24 21:56:32.000000 ibis-framework-v0.6.0/ibis/server.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4129 2015-01-21 05:11:59.000000 ibis-framework-v0.6.0/ibis/comms.pxd
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/expr/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-05-11 04:48:06.000000 ibis-framework-v0.6.0/ibis/expr/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     8784 2015-09-16 18:48:19.000000 ibis-framework-v0.6.0/ibis/expr/format.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     7295 2015-06-29 06:28:49.000000 ibis-framework-v0.6.0/ibis/expr/temporal.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    26447 2015-09-16 18:48:19.000000 ibis-framework-v0.6.0/ibis/expr/analysis.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    11262 2015-11-05 19:34:31.000000 ibis-framework-v0.6.0/ibis/expr/datatypes.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    27030 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/expr/types.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    51662 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/expr/operations.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     7032 2015-09-09 04:43:12.000000 ibis-framework-v0.6.0/ibis/expr/groupby.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     7688 2015-09-03 06:45:25.000000 ibis-framework-v0.6.0/ibis/expr/window.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    49858 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/expr/api.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    19387 2015-08-24 21:56:32.000000 ibis-framework-v0.6.0/ibis/expr/rules.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     5516 2015-08-11 20:25:43.000000 ibis-framework-v0.6.0/ibis/expr/analytics.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/expr/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)        0 2015-05-11 04:48:08.000000 ibis-framework-v0.6.0/ibis/expr/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      616 2015-09-01 04:13:53.000000 ibis-framework-v0.6.0/ibis/expr/tests/conftest.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2858 2015-09-02 23:21:36.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_interactive.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3386 2015-08-05 16:09:03.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_case.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     5034 2015-09-03 06:45:25.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_window_functions.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6266 2015-09-16 18:48:19.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_format.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9216 2015-09-16 18:48:19.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_analysis.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3313 2015-06-29 06:28:49.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_decimal.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6270 2015-10-08 04:09:39.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_sql_builtins.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    20407 2015-11-30 09:38:55.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_value_exprs.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     5955 2015-08-24 21:56:32.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_temporal.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    13673 2015-09-09 04:43:12.000000 ibis-framework-v0.6.0/ibis/expr/tests/mocks.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3282 2015-10-07 04:53:40.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_string.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1850 2015-06-29 06:28:49.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_pipe.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3299 2015-08-11 20:30:38.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_analytics.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     3624 2015-10-08 05:36:22.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_timestamp.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    38376 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/expr/tests/test_table.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      997 2015-07-13 05:54:08.000000 ibis-framework-v0.6.0/ibis/common.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/ibis/tests/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      573 2015-06-29 06:28:49.000000 ibis-framework-v0.6.0/ibis/tests/__init__.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     2688 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/ibis/tests/conftest.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    11505 2015-06-29 06:28:49.000000 ibis-framework-v0.6.0/ibis/tests/test_comms.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    10953 2015-08-24 21:56:32.000000 ibis-framework-v0.6.0/ibis/tests/test_tasks.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     6059 2015-11-22 23:42:20.000000 ibis-framework-v0.6.0/ibis/tests/test_server.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      956 2015-08-25 05:04:44.000000 ibis-framework-v0.6.0/ibis/tests/util.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    16773 2015-09-02 07:50:13.000000 ibis-framework-v0.6.0/ibis/tests/test_filesystems.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     9550 2015-08-25 05:04:44.000000 ibis-framework-v0.6.0/ibis/filesystems.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      841 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/PKG-INFO
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/scripts/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      753 2015-01-21 05:11:59.000000 ibis-framework-v0.6.0/scripts/semaphore_perf.py
+-rwxr-xr-x   0 wesm      (1000) wesm      (1000)     4139 2015-10-08 03:41:51.000000 ibis-framework-v0.6.0/scripts/run_jenkins.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1268 2015-09-10 05:09:43.000000 ibis-framework-v0.6.0/scripts/airline.py
+-rwxr-xr-x   0 wesm      (1000) wesm      (1000)    17250 2015-09-10 05:09:43.000000 ibis-framework-v0.6.0/scripts/test_data_admin.py
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      212 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/setup.cfg
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/hdfs/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      776 2015-09-11 17:09:40.000000 ibis-framework-v0.6.0/conda-recipes/hdfs/meta.yaml
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      219 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/hdfs/build.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      236 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/hdfs/bld.bat
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/impyla/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1117 2015-11-01 14:03:25.000000 ibis-framework-v0.6.0/conda-recipes/impyla/meta.yaml
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      219 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/impyla/build.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      236 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/impyla/bld.bat
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/ibis-framework/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      971 2015-11-10 22:41:53.000000 ibis-framework-v0.6.0/conda-recipes/ibis-framework/meta.yaml
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      294 2015-11-01 14:03:25.000000 ibis-framework-v0.6.0/conda-recipes/ibis-framework/build.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      314 2015-11-01 14:03:25.000000 ibis-framework-v0.6.0/conda-recipes/ibis-framework/bld.bat
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/thrift/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      498 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/thrift/meta.yaml
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      219 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/thrift/build.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      236 2015-08-07 16:53:33.000000 ibis-framework-v0.6.0/conda-recipes/thrift/bld.bat
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/conda-recipes/thrift_sasl/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      554 2015-09-11 17:09:40.000000 ibis-framework-v0.6.0/conda-recipes/thrift_sasl/meta.yaml
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      219 2015-09-11 17:09:40.000000 ibis-framework-v0.6.0/conda-recipes/thrift_sasl/build.sh
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      236 2015-09-11 17:09:40.000000 ibis-framework-v0.6.0/conda-recipes/thrift_sasl/bld.bat
+-rw-r--r--   0 wesm      (1000) wesm      (1000)      561 2015-10-08 04:18:58.000000 ibis-framework-v0.6.0/MANIFEST.in
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     4200 2015-11-01 14:02:52.000000 ibis-framework-v0.6.0/setup.py
+drwxr-xr-x   0 wesm      (1000) wesm      (1000)        0 2015-11-30 09:48:46.000000 ibis-framework-v0.6.0/LICENSES/
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1061 2015-06-11 06:57:54.000000 ibis-framework-v0.6.0/LICENSES/hdfscli.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)     1838 2015-06-04 20:35:47.000000 ibis-framework-v0.6.0/LICENSES/pandas.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)       84 2015-11-10 22:41:53.000000 ibis-framework-v0.6.0/requirements.txt
+-rw-r--r--   0 wesm      (1000) wesm      (1000)    11358 2015-03-11 21:51:00.000000 ibis-framework-v0.6.0/LICENSE.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ibis_framework-5.1.0/LICENSE.txt` & `ibis-framework-v0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ibis_framework-5.1.0/ibis/backends/base/__init__.py` & `ibis-framework-v0.6.0/ibis/impala/ddl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1043 +1,811 @@
-from __future__ import annotations
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import abc
-import collections.abc
-import functools
-import importlib.metadata
-import keyword
+from ibis.compat import StringIO
 import re
-import sys
-import urllib.parse
-from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    ClassVar,
-    Iterable,
-    Iterator,
-    Mapping,
-    MutableMapping,
-)
-
-import ibis
-import ibis.common.exceptions as exc
-import ibis.config
-import ibis.expr.operations as ops
-import ibis.expr.types as ir
-from ibis import util
-from ibis.common.caching import RefCountedCache
-
-if TYPE_CHECKING:
-    import pandas as pd
-    import pyarrow as pa
 
-__all__ = ('BaseBackend', 'Database', 'connect')
+from ibis.sql.compiler import DDL
+from .compiler import quote_identifier, _type_to_sql_string
 
+from ibis.expr.datatypes import validate_type
+from ibis.compat import py_string
+import ibis.expr.rules as rules
 
-class Database:
-    """Generic Database class."""
 
-    def __init__(self, name: str, client: Any) -> None:
-        self.name = name
-        self.client = client
+fully_qualified_re = re.compile("(.*)\.(?:`(.*)`|(.*))")
 
-    def __repr__(self) -> str:
-        """Return type name and the name of the database."""
-        return f'{type(self).__name__}({self.name!r})'
-
-    def __dir__(self) -> list[str]:
-        """Return the attributes and tables of the database.
-
-        Returns
-        -------
-        list[str]
-            A list of the attributes and tables available in the database.
-        """
-        attrs = dir(type(self))
-        unqualified_tables = [self._unqualify(x) for x in self.tables]
-        return sorted(frozenset(attrs + unqualified_tables))
-
-    def __contains__(self, table: str) -> bool:
-        """Check if the given table is available in the current database.
-
-        Parameters
-        ----------
-        table
-            Table name
-
-        Returns
-        -------
-        bool
-            True if the given table is available in the current database.
-        """
-        return table in self.tables
-
-    @property
-    def tables(self) -> list[str]:
-        """Return a list with all available tables.
-
-        Returns
-        -------
-        list[str]
-            The list of tables in the database
-        """
-        return self.list_tables()
-
-    def __getitem__(self, table: str) -> ir.Table:
-        """Return a Table for the given table name.
-
-        Parameters
-        ----------
-        table
-            Table name
-
-        Returns
-        -------
-        Table
-            Table expression
-        """
-        return self.table(table)
-
-    def __getattr__(self, table: str) -> ir.Table:
-        """Return a Table for the given table name.
-
-        Parameters
-        ----------
-        table
-            Table name
-
-        Returns
-        -------
-        Table
-            Table expression
-        """
-        return self.table(table)
-
-    def _qualify(self, value):
-        return value
-
-    def _unqualify(self, value):
-        return value
-
-    def drop(self, force: bool = False) -> None:
-        """Drop the database.
-
-        Parameters
-        ----------
-        force
-            If `True`, drop any objects that exist, and do not fail if the
-            database does not exist.
-        """
-        self.client.drop_database(self.name, force=force)
-
-    def table(self, name: str) -> ir.Table:
-        """Return a table expression referencing a table in this database.
-
-        Parameters
-        ----------
-        name
-            The name of a table
-
-        Returns
-        -------
-        Table
-            Table expression
-        """
-        qualified_name = self._qualify(name)
-        return self.client.table(qualified_name, self.name)
-
-    def list_tables(self, like=None, database=None):
-        """List the tables in the database.
-
-        Parameters
-        ----------
-        like
-            A pattern to use for listing tables.
-        database
-            The database to perform the list against
-        """
-        return self.client.list_tables(like, database=database or self.name)
-
-
-class TablesAccessor(collections.abc.Mapping):
-    """A mapping-like object for accessing tables off a backend.
-
-    Tables may be accessed by name using either index or attribute access:
-
-    Examples
-    --------
-    >>> con = ibis.sqlite.connect("example.db")
-    >>> people = con.tables['people']  # access via index
-    >>> people = con.tables.people  # access via attribute
-    """
 
-    def __init__(self, backend: BaseBackend):
-        self._backend = backend
+def _is_fully_qualified(x):
+    m = fully_qualified_re.search(x)
+    return bool(m)
 
-    def __getitem__(self, name) -> ir.Table:
-        try:
-            return self._backend.table(name)
-        except Exception as exc:  # noqa: BLE001
-            raise KeyError(name) from exc
-
-    def __getattr__(self, name) -> ir.Table:
-        if name.startswith("_"):
-            raise AttributeError(name)
-        try:
-            return self._backend.table(name)
-        except Exception as exc:  # noqa: BLE001
-            raise AttributeError(name) from exc
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(sorted(self._backend.list_tables()))
-
-    def __len__(self) -> int:
-        return len(self._backend.list_tables())
-
-    def __dir__(self) -> list[str]:
-        o = set()
-        o.update(dir(type(self)))
-        o.update(
-            name
-            for name in self._backend.list_tables()
-            if name.isidentifier() and not keyword.iskeyword(name)
-        )
-        return list(o)
-
-    def __repr__(self) -> str:
-        tables = self._backend.list_tables()
-        rows = ["Tables", "------"]
-        rows.extend(f"- {name}" for name in sorted(tables))
-        return "\n".join(rows)
-
-    def _ipython_key_completions_(self) -> list[str]:
-        return self._backend.list_tables()
-
-
-class _FileIOHandler:
-    @staticmethod
-    def _import_pyarrow():
-        try:
-            import pyarrow  # noqa: ICN001
-        except ImportError:
-            raise ModuleNotFoundError(
-                "Exporting to arrow formats requires `pyarrow` but it is not installed"
-            )
-        else:
-            return pyarrow
 
-    @util.experimental
-    def to_pyarrow(
-        self,
-        expr: ir.Expr,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        **kwargs: Any,
-    ) -> pa.Table:
-        """Execute expression and return results in as a pyarrow table.
-
-        This method is eager and will execute the associated expression
-        immediately.
-
-        Parameters
-        ----------
-        expr
-            Ibis expression to export to pyarrow
-        params
-            Mapping of scalar parameter expressions to value.
-        limit
-            An integer to effect a specific row limit. A value of `None` means
-            "no limit". The default is in `ibis/config.py`.
-        kwargs
-            Keyword arguments
-
-        Returns
-        -------
-        Table
-            A pyarrow table holding the results of the executed expression.
-        """
-        pa = self._import_pyarrow()
-        try:
-            # Can't construct an array from record batches
-            # so construct at one column table (if applicable)
-            # then return the column _from_ the table
-            table = pa.Table.from_batches(
-                self.to_pyarrow_batches(expr, params=params, limit=limit, **kwargs)
-            )
-        except ValueError:
-            # The pyarrow batches iterator is empty so pass in an empty
-            # iterator and a pyarrow schema
-            schema = expr.as_table().schema()
-            table = pa.Table.from_batches([], schema=schema.to_pyarrow())
-
-        if isinstance(expr, ir.Table):
-            return table
-        elif isinstance(expr, ir.Column):
-            # Column will be a ChunkedArray, `combine_chunks` will
-            # flatten it
-            if len(table.columns[0]):
-                return table.columns[0].combine_chunks()
-            else:
-                return pa.array(table.columns[0])
-        elif isinstance(expr, ir.Scalar):
-            return table.columns[0][0]
+def _is_quoted(x):
+    regex = re.compile("(?:`(.*)`|(.*))")
+    quoted, unquoted = regex.match(x).groups()
+    return quoted is not None
+
+
+class ImpalaDDL(DDL):
+
+    def _get_scoped_name(self, obj_name, database):
+        if database:
+            scoped_name = '{0}.`{1}`'.format(database, obj_name)
         else:
-            raise ValueError
+            if not _is_fully_qualified(obj_name):
+                if _is_quoted(obj_name):
+                    return obj_name
+                else:
+                    return '`{0}`'.format(obj_name)
+            else:
+                return obj_name
+        return scoped_name
+
+
+class CreateDDL(ImpalaDDL):
+
+    def _if_exists(self):
+        return 'IF NOT EXISTS ' if self.can_exist else ''
+
+
+_format_aliases = {
+    'TEXT': 'TEXTFILE'
+}
 
-    @util.experimental
-    def to_pyarrow_batches(
-        self,
-        expr: ir.Expr,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        chunk_size: int = 1_000_000,
-        **kwargs: Any,
-    ) -> pa.ipc.RecordBatchReader:
-        """Execute expression and return a RecordBatchReader.
-
-        This method is eager and will execute the associated expression
-        immediately.
-
-        Parameters
-        ----------
-        expr
-            Ibis expression to export to pyarrow
-        limit
-            An integer to effect a specific row limit. A value of `None` means
-            "no limit". The default is in `ibis/config.py`.
-        params
-            Mapping of scalar parameter expressions to value.
-        chunk_size
-            Maximum number of rows in each returned record batch.
-        kwargs
-            Keyword arguments
-
-        Returns
-        -------
-        results
-            RecordBatchReader
-        """
-        raise NotImplementedError
 
-    def read_parquet(
-        self, path: str | Path, table_name: str | None = None, **kwargs: Any
-    ) -> ir.Table:
-        """Register a parquet file as a table in the current backend.
-
-        Parameters
-        ----------
-        path
-            The data source.
-        table_name
-            An optional name to use for the created table. This defaults to
-            a sequentially generated name.
-        **kwargs
-            Additional keyword arguments passed to the backend loading function.
-
-        Returns
-        -------
-        ir.Table
-            The just-registered table
-        """
-        raise NotImplementedError(
-            f"{self.name} does not support direct registration of parquet data."
-        )
-
-    def read_csv(
-        self, path: str | Path, table_name: str | None = None, **kwargs: Any
-    ) -> ir.Table:
-        """Register a CSV file as a table in the current backend.
-
-        Parameters
-        ----------
-        path
-            The data source. A string or Path to the CSV file.
-        table_name
-            An optional name to use for the created table. This defaults to
-            a sequentially generated name.
-        **kwargs
-            Additional keyword arguments passed to the backend loading function.
-
-        Returns
-        -------
-        ir.Table
-            The just-registered table
-        """
-        raise NotImplementedError(
-            f"{self.name} does not support direct registration of CSV data."
-        )
-
-    @util.experimental
-    def to_parquet(
-        self,
-        expr: ir.Table,
-        path: str | Path,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Write the results of executing the given expression to a parquet file.
-
-        This method is eager and will execute the associated expression
-        immediately.
-
-        Parameters
-        ----------
-        expr
-            The ibis expression to execute and persist to parquet.
-        path
-            The data source. A string or Path to the parquet file.
-        params
-            Mapping of scalar parameter expressions to value.
-        **kwargs
-            Additional keyword arguments passed to pyarrow.parquet.ParquetWriter
-
-        https://arrow.apache.org/docs/python/generated/pyarrow.parquet.ParquetWriter.html
-        """
-        self._import_pyarrow()
-        import pyarrow.parquet as pq
-
-        batch_reader = expr.to_pyarrow_batches(params=params)
-
-        with pq.ParquetWriter(path, batch_reader.schema) as writer:
-            for batch in batch_reader:
-                writer.write_batch(batch)
-
-    @util.experimental
-    def to_csv(
-        self,
-        expr: ir.Table,
-        path: str | Path,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Write the results of executing the given expression to a CSV file.
-
-        This method is eager and will execute the associated expression
-        immediately.
-
-        Parameters
-        ----------
-        expr
-            The ibis expression to execute and persist to CSV.
-        path
-            The data source. A string or Path to the CSV file.
-        params
-            Mapping of scalar parameter expressions to value.
-        kwargs
-            Additional keyword arguments passed to pyarrow.csv.CSVWriter
-
-        https://arrow.apache.org/docs/python/generated/pyarrow.csv.CSVWriter.html
-        """
-        self._import_pyarrow()
-        import pyarrow.csv as pcsv
-
-        batch_reader = expr.to_pyarrow_batches(params=params)
-
-        with pcsv.CSVWriter(path, batch_reader.schema) as writer:
-            for batch in batch_reader:
-                writer.write_batch(batch)
+def _sanitize_format(format):
+    if format is None:
+        return
+    format = format.upper()
+    format = _format_aliases.get(format, format)
+    if format not in ('PARQUET', 'AVRO', 'TEXTFILE'):
+        raise ValueError('Invalid format: {0}'.format(format))
 
+    return format
 
-class BaseBackend(abc.ABC, _FileIOHandler):
-    """Base backend class.
 
-    All Ibis backends must subclass this class and implement all the
-    required methods.
+def _format_properties(props):
+    tokens = []
+    for k, v in sorted(props.items()):
+        tokens.append("'{0!s}'='{1!s}'".format(k, v))
+
+    return '({0})'.format(', '.join(tokens))
+
+
+class CreateTable(CreateDDL):
+
     """
 
-    database_class = Database
-    table_class: type[ops.DatabaseTable] = ops.DatabaseTable
-    name: ClassVar[str]
-
-    def __init__(self, *args, **kwargs):
-        self._con_args: tuple[Any] = args
-        self._con_kwargs: dict[str, Any] = kwargs
-        # expression cache
-        self._query_cache = RefCountedCache(
-            populate=self._load_into_cache,
-            lookup=lambda name: self.table(name).op(),
-            finalize=self._clean_up_cached_table,
-            generate_name=functools.partial(util.gen_name, "cache"),
-            key=lambda expr: expr.op(),
-        )
-
-    def __getstate__(self):
-        return dict(
-            database_class=self.database_class,
-            table_class=self.table_class,
-            _con_args=self._con_args,
-            _con_kwargs=self._con_kwargs,
-        )
-
-    def __rich_repr__(self):
-        yield "name", self.name
-
-    def __hash__(self):
-        return hash(self.db_identity)
-
-    def __eq__(self, other):
-        return self.db_identity == other.db_identity
-
-    @functools.cached_property
-    def db_identity(self) -> str:
-        """Return the identity of the database.
-
-        Multiple connections to the same
-        database will return the same value for `db_identity`.
-
-        The default implementation assumes connection parameters uniquely
-        specify the database.
-
-        Returns
-        -------
-        Hashable
-            Database identity
-        """
-        parts = [self.table_class.__name__]
-        parts.extend(self._con_args)
-        parts.extend(f'{k}={v}' for k, v in self._con_kwargs.items())
-        return '_'.join(map(str, parts))
-
-    def connect(self, *args, **kwargs) -> BaseBackend:
-        """Connect to the database.
-
-        Parameters
-        ----------
-        *args
-            Mandatory connection parameters, see the docstring of `do_connect`
-            for details.
-        **kwargs
-            Extra connection parameters, see the docstring of `do_connect` for
-            details.
-
-        Notes
-        -----
-        This creates a new backend instance with saved `args` and `kwargs`,
-        then calls `reconnect` and finally returns the newly created and
-        connected backend instance.
-
-        Returns
-        -------
-        BaseBackend
-            An instance of the backend
-        """
-        new_backend = self.__class__(*args, **kwargs)
-        new_backend.reconnect()
-        return new_backend
-
-    def _from_url(self, url: str, **kwargs) -> BaseBackend:
-        """Construct an ibis backend from a SQLAlchemy-conforming URL."""
-        raise NotImplementedError(
-            f"`_from_url` not implemented for the {self.name} backend"
-        )
-
-    @staticmethod
-    def _convert_kwargs(kwargs: MutableMapping) -> None:
-        """Manipulate keyword arguments to `.connect` method."""
-
-    def reconnect(self) -> None:
-        """Reconnect to the database already configured with connect."""
-        self.do_connect(*self._con_args, **self._con_kwargs)
-
-    def do_connect(self, *args, **kwargs) -> None:
-        """Connect to database specified by `args` and `kwargs`."""
-
-    @util.deprecated(instead='use equivalent methods in the backend')
-    def database(self, name: str | None = None) -> Database:
-        """Return a `Database` object for the `name` database.
-
-        Parameters
-        ----------
-        name
-            Name of the database to return the object for.
-
-        Returns
-        -------
-        Database
-            A database object for the specified database.
-        """
-        return self.database_class(name=name or self.current_database, client=self)
-
-    @property
-    @abc.abstractmethod
-    def current_database(self) -> str | None:
-        """Return the name of the current database.
-
-        Backends that don't support different databases will return None.
-
-        Returns
-        -------
-        str | None
-            Name of the current database.
-        """
-
-    @abc.abstractmethod
-    def list_databases(self, like: str = None) -> list[str]:
-        """List existing databases in the current connection.
-
-        Parameters
-        ----------
-        like
-            A pattern in Python's regex format to filter returned database
-            names.
-
-        Returns
-        -------
-        list[str]
-            The database names that exist in the current connection, that match
-            the `like` pattern if provided.
-        """
-
-    @staticmethod
-    def _filter_with_like(
-        values: Iterable[str],
-        like: str | None = None,
-    ) -> list[str]:
-        """Filter names with a `like` pattern (regex).
-
-        The methods `list_databases` and `list_tables` accept a `like`
-        argument, which filters the returned tables with tables that match the
-        provided pattern.
-
-        We provide this method in the base backend, so backends can use it
-        instead of reinventing the wheel.
-
-        Parameters
-        ----------
-        values
-            Iterable of strings to filter
-        like
-            Pattern to use for filtering names
-
-        Returns
-        -------
-        list[str]
-            Names filtered by the `like` pattern.
-        """
-        if like is None:
-            return list(values)
-
-        pattern = re.compile(like)
-        return sorted(filter(lambda t: pattern.findall(t), values))
-
-    @abc.abstractmethod
-    def list_tables(
-        self, like: str | None = None, database: str | None = None
-    ) -> list[str]:
-        """Return the list of table names in the current database.
-
-        For some backends, the tables may be files in a directory,
-        or other equivalent entities in a SQL database.
-
-        Parameters
-        ----------
-        like : str, optional
-            A pattern in Python's regex format.
-        database : str, optional
-            The database to list tables of, if not the current one.
-
-        Returns
-        -------
-        list[str]
-            The list of the table names that match the pattern `like`.
-        """
-
-    @abc.abstractmethod
-    def table(self, name: str, database: str | None = None) -> ir.Table:
-        """Construct a table expression.
-
-        Parameters
-        ----------
-        name
-            Table name
-        database
-            Database name
-
-        Returns
-        -------
-        Table
-            Table expression
-        """
-
-    @functools.cached_property
-    def tables(self):
-        """An accessor for tables in the database.
-
-        Tables may be accessed by name using either index or attribute access:
-
-        Examples
-        --------
-        >>> con = ibis.sqlite.connect("example.db")
-        >>> people = con.tables['people']  # access via index
-        >>> people = con.tables.people  # access via attribute
-        """
-        return TablesAccessor(self)
-
-    @property
-    @abc.abstractmethod
-    def version(self) -> str:
-        """Return the version of the backend engine.
-
-        For database servers, return the server version.
-
-        For others such as SQLite and pandas return the version of the
-        underlying library or application.
-
-        Returns
-        -------
-        str
-            The backend version
-        """
-
-    @classmethod
-    def register_options(cls) -> None:
-        """Register custom backend options."""
-        options = ibis.config.options
-        backend_name = cls.name
-        try:
-            backend_options = cls.Options()
-        except AttributeError:
-            pass
+    Parameters
+    ----------
+    partition :
+
+    """
+
+    def __init__(self, table_name, database=None, external=False,
+                 format='parquet', can_exist=False,
+                 partition=None, path=None):
+        self.table_name = table_name
+        self.database = database
+        self.partition = partition
+        self.path = path
+        self.external = external
+        self.can_exist = can_exist
+        self.format = _sanitize_format(format)
+
+    def _create_line(self):
+        scoped_name = self._get_scoped_name(self.table_name, self.database)
+
+        if self.external:
+            create_decl = 'CREATE EXTERNAL TABLE'
         else:
-            try:
-                setattr(options, backend_name, backend_options)
-            except ValueError as e:
-                raise exc.BackendConfigurationNotRegistered(backend_name) from e
-
-    def compile(
-        self,
-        expr: ir.Expr,
-        params: Mapping[ir.Expr, Any] | None = None,
-    ) -> Any:
-        """Compile an expression."""
-        return self.compiler.to_sql(expr, params=params)
-
-    def _to_sql(self, expr: ir.Expr, **kwargs) -> str:
-        """Convert an expression to a SQL string.
-
-        Called by `ibis.to_sql`/`ibis.show_sql`, gives the backend an
-        opportunity to generate nicer SQL for human consumption.
-        """
-        raise NotImplementedError(f"Backend '{self.name}' backend doesn't support SQL")
-
-    def execute(self, expr: ir.Expr) -> Any:
-        """Execute an expression."""
-
-    def add_operation(self, operation: ops.Node) -> Callable:
-        """Add a translation function to the backend for a specific operation.
-
-        Operations are defined in `ibis.expr.operations`, and a translation
-        function receives the translator object and an expression as
-        parameters, and returns a value depending on the backend. For example,
-        in SQL backends, a NullLiteral operation could be translated to the
-        string `"NULL"`.
-
-        Examples
-        --------
-        >>> @ibis.sqlite.add_operation(ibis.expr.operations.NullLiteral)
-        ... def _null_literal(translator, expression):
-        ...     return 'NULL'
-        """
-        if not hasattr(self, 'compiler'):
-            raise RuntimeError('Only SQL-based backends support `add_operation`')
-
-        def decorator(translation_function: Callable) -> None:
-            self.compiler.translator_class.add_operation(
-                operation, translation_function
-            )
-
-        return decorator
-
-    def create_database(self, name: str, force: bool = False) -> None:
-        """Create a new database.
-
-        Not all backends implement this method.
-
-        Parameters
-        ----------
-        name
-            Name of the new database.
-        force
-            If `False`, an exception is raised if the database already exists.
-        """
-        raise NotImplementedError(
-            f'Backend "{self.name}" does not implement "create_database"'
-        )
-
-    @abc.abstractmethod
-    def create_table(
-        self,
-        name: str,
-        obj: pd.DataFrame | ir.Table | None = None,
-        *,
-        schema: ibis.Schema | None = None,
-        database: str | None = None,
-        temp: bool = False,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        """Create a new table.
-
-        Parameters
-        ----------
-        name
-            Name of the new table.
-        obj
-            An Ibis table expression or pandas table that will be used to
-            extract the schema and the data of the new table. If not provided,
-            `schema` must be given.
-        schema
-            The schema for the new table. Only one of `schema` or `obj` can be
-            provided.
-        database
-            Name of the database where the table will be created, if not the
-            default.
-        temp
-            Whether a table is temporary or not
-        overwrite
-            Whether to clobber existing data
-
-        Returns
-        -------
-        Table
-            The table that was created.
-        """
-
-    @abc.abstractmethod
-    def drop_table(
-        self,
-        name: str,
-        *,
-        database: str | None = None,
-        force: bool = False,
-    ) -> None:
-        """Drop a table.
-
-        Parameters
-        ----------
-        name
-            Name of the table to drop.
-        database
-            Name of the database where the table exists, if not the default.
-        force
-            If `False`, an exception is raised if the table does not exist.
-        """
-        raise NotImplementedError(
-            f'Backend "{self.name}" does not implement "drop_table"'
-        )
-
-    @abc.abstractmethod
-    def create_view(
-        self,
-        name: str,
-        obj: ir.Table,
-        *,
-        database: str | None = None,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        """Create a new view from an expression.
-
-        Parameters
-        ----------
-        name
-            Name of the new view.
-        obj
-            An Ibis table expression that will be used to create the view.
-        database
-            Name of the database where the view will be created, if not
-            provided the database's default is used.
-        overwrite
-            Whether to clobber an existing view with the same name
-
-        Returns
-        -------
-        Table
-            The view that was created.
-        """
-
-    @abc.abstractmethod
-    def drop_view(
-        self, name: str, *, database: str | None = None, force: bool = False
-    ) -> None:
-        """Drop a view.
-
-        Parameters
-        ----------
-        name
-            Name of the view to drop.
-        database
-            Name of the database where the view exists, if not the default.
-        force
-            If `False`, an exception is raised if the view does not exist.
-        """
-
-    @classmethod
-    def has_operation(cls, operation: type[ops.Value]) -> bool:
-        """Return whether the backend implements support for `operation`.
-
-        Parameters
-        ----------
-        operation
-            A class corresponding to an operation.
-
-        Returns
-        -------
-        bool
-            Whether the backend implements the operation.
-
-        Examples
-        --------
-        >>> import ibis
-        >>> import ibis.expr.operations as ops
-        >>> ibis.sqlite.has_operation(ops.ArrayIndex)
-        False
-        >>> ibis.postgres.has_operation(ops.ArrayIndex)
-        True
-        """
-        raise NotImplementedError(
-            f"{cls.name} backend has not implemented `has_operation` API"
-        )
-
-    def _cached(self, expr: ir.Table):
-        """Cache the provided expression.
-
-        All subsequent operations on the returned expression will be performed on the cached data.
-
-        Parameters
-        ----------
-        expr
-            Table expression to cache
-
-        Returns
-        -------
-        Expr
-            Cached table
-
-        """
-        op = expr.op()
-        if (result := self._query_cache.get(op)) is None:
-            self._query_cache.store(expr)
-            result = self._query_cache[op]
-        return ir.CachedTable(result)
-
-    def _release_cached(self, expr: ir.CachedTable) -> None:
-        """Releases the provided cached expression.
-
-        Parameters
-        ----------
-        expr
-            Cached expression to release
-        """
-        del self._query_cache[expr.op()]
-
-    def _load_into_cache(self, name, expr):
-        raise NotImplementedError(self.name)
-
-    def _clean_up_cached_table(self, op):
-        raise NotImplementedError(self.name)
-
-
-@functools.lru_cache(maxsize=None)
-def _get_backend_names() -> frozenset[str]:
-    """Return the set of known backend names.
-
-    Notes
-    -----
-    This function returns a frozenset to prevent cache pollution.
+            create_decl = 'CREATE TABLE'
+
+        create_line = '{0} {1}{2}'.format(create_decl, self._if_exists(),
+                                          scoped_name)
+        return create_line
+
+    def _location(self):
+        if self.path:
+            return "\nLOCATION '{0}'".format(self.path)
+        return ''
+
+    def _storage(self):
+        storage_lines = {
+            'PARQUET': '\nSTORED AS PARQUET',
+            'AVRO': '\nSTORED AS AVRO'
+        }
+        return storage_lines[self.format]
+
+
+class CTAS(CreateTable):
+
+    """
+    Create Table As Select
+    """
+
+    def __init__(self, table_name, select, database=None,
+                 external=False, format='parquet', can_exist=False,
+                 path=None):
+        self.select = select
+        CreateTable.__init__(self, table_name, database=database,
+                             external=external, format=format,
+                             can_exist=can_exist, path=path)
+
+    def compile(self):
+        buf = StringIO()
+        buf.write(self._create_line())
+        buf.write(self._storage())
+        buf.write(self._location())
+
+        select_query = self.select.compile()
+        buf.write('\nAS\n{0}'.format(select_query))
+        return buf.getvalue()
+
+
+class CreateView(CreateDDL):
 
-    If a `set` is used, then any in-place modifications to the set
-    are visible to every caller of this function.
     """
+    Create Table As Select
+    """
+
+    def __init__(self, name, select, database=None, can_exist=False):
+        self.name = name
+        self.database = database
+        self.select = select
+        self.can_exist = can_exist
+
+    def compile(self):
+        buf = StringIO()
+        buf.write(self._create_line())
+
+        select_query = self.select.compile()
+        buf.write('\nAS\n{0}'.format(select_query))
+        return buf.getvalue()
+
+    def _create_line(self):
+        scoped_name = self._get_scoped_name(self.name, self.database)
+        return '{0} {1}{2}'.format('CREATE VIEW', self._if_exists(),
+                                   scoped_name)
+
+
+class CreateTableParquet(CreateTable):
+
+    def __init__(self, table_name, path,
+                 example_file=None,
+                 example_table=None,
+                 schema=None,
+                 external=True,
+                 **kwargs):
+        self.example_file = example_file
+        self.example_table = example_table
+        self.schema = schema
+        CreateTable.__init__(self, table_name, external=external,
+                             format='parquet', path=path, **kwargs)
+
+        self._validate()
+
+    def _validate(self):
+        pass
+
+    def compile(self):
+        buf = StringIO()
+        buf.write(self._create_line())
+
+        if self.example_file is not None:
+            buf.write("\nLIKE PARQUET '{0}'".format(self.example_file))
+        elif self.example_table is not None:
+            buf.write("\nLIKE {0}".format(self.example_table))
+        elif self.schema is not None:
+            schema = format_schema(self.schema)
+            buf.write('\n{0}'.format(schema))
+        else:
+            raise NotImplementedError
+
+        buf.write(self._storage())
+        buf.write(self._location())
+        return buf.getvalue()
+
+
+class CreateTableWithSchema(CreateTable):
+
+    def __init__(self, table_name, schema, table_format, **kwargs):
+        self.schema = schema
+        self.table_format = table_format
+
+        CreateTable.__init__(self, table_name, **kwargs)
+
+    def compile(self):
+        from ibis.expr.api import Schema
+
+        buf = StringIO()
+        buf.write(self._create_line())
+
+        def _push_schema(x):
+            formatted = format_schema(x)
+            buf.write('{0}'.format(formatted))
+
+        if self.partition is not None:
+            main_schema = self.schema
+            part_schema = self.partition
+            if not isinstance(part_schema, Schema):
+                part_schema = Schema(
+                    part_schema,
+                    [self.schema[name] for name in part_schema])
+
+            to_delete = []
+            for name in self.partition:
+                if name in self.schema:
+                    to_delete.append(name)
+
+            if len(to_delete):
+                main_schema = main_schema.delete(to_delete)
+
+            buf.write('\n')
+            _push_schema(main_schema)
+            buf.write('\nPARTITIONED BY ')
+            _push_schema(part_schema)
+        else:
+            buf.write('\n')
+            _push_schema(self.schema)
+
+        format_ddl = self.table_format.to_ddl()
+        if format_ddl:
+            buf.write(format_ddl)
+
+        buf.write(self._location())
 
-    if sys.version_info < (3, 10):
-        entrypoints = importlib.metadata.entry_points()["ibis.backends"]
+        return buf.getvalue()
+
+
+class NoFormat(object):
+
+    def to_ddl(self):
+        return None
+
+
+class DelimitedFormat(object):
+
+    def __init__(self, path, delimiter=None, escapechar=None,
+                 na_rep=None, lineterminator=None):
+        self.path = path
+        self.delimiter = delimiter
+        self.escapechar = escapechar
+        self.lineterminator = lineterminator
+        self.na_rep = na_rep
+
+    def to_ddl(self):
+        buf = StringIO()
+
+        buf.write("\nROW FORMAT DELIMITED")
+
+        if self.delimiter is not None:
+            buf.write("\nFIELDS TERMINATED BY '{0}'".format(self.delimiter))
+
+        if self.escapechar is not None:
+            buf.write("\nESCAPED BY '{0}'".format(self.escapechar))
+
+        if self.lineterminator is not None:
+            buf.write("\nLINES TERMINATED BY '{0}'"
+                      .format(self.lineterminator))
+
+        buf.write("\nLOCATION '{0}'".format(self.path))
+
+        if self.na_rep is not None:
+            buf.write("\nTBLPROPERTIES('serialization.null.format'='{0}')"
+                      .format(self.na_rep))
+
+        return buf.getvalue()
+
+
+class AvroFormat(object):
+
+    def __init__(self, path, avro_schema):
+        self.path = path
+        self.avro_schema = avro_schema
+
+    def to_ddl(self):
+        import json
+
+        buf = StringIO()
+        buf.write('\nSTORED AS AVRO')
+        buf.write("\nLOCATION '{0}'".format(self.path))
+
+        schema = json.dumps(self.avro_schema, indent=2, sort_keys=True)
+        schema = '\n'.join([x.rstrip() for x in schema.split('\n')])
+        buf.write("\nTBLPROPERTIES ('avro.schema.literal'='{0}')"
+                  .format(schema))
+
+        return buf.getvalue()
+
+
+class CreateTableDelimited(CreateTableWithSchema):
+
+    def __init__(self, table_name, path, schema,
+                 delimiter=None, escapechar=None, lineterminator=None,
+                 na_rep=None, external=True, **kwargs):
+        table_format = DelimitedFormat(path, delimiter=delimiter,
+                                       escapechar=escapechar,
+                                       lineterminator=lineterminator,
+                                       na_rep=na_rep)
+        CreateTableWithSchema.__init__(self, table_name, schema,
+                                       table_format, external=external,
+                                       **kwargs)
+
+
+class CreateTableAvro(CreateTable):
+
+    def __init__(self, table_name, path, avro_schema, external=True, **kwargs):
+        self.table_format = AvroFormat(path, avro_schema)
+
+        CreateTable.__init__(self, table_name, external=external, **kwargs)
+
+    def compile(self):
+        buf = StringIO()
+        buf.write(self._create_line())
+
+        format_ddl = self.table_format.to_ddl()
+        buf.write(format_ddl)
+
+        return buf.getvalue()
+
+
+class InsertSelect(ImpalaDDL):
+
+    def __init__(self, table_name, select_expr, database=None,
+                 partition=None,
+                 partition_schema=None,
+                 overwrite=False):
+        self.table_name = table_name
+        self.database = database
+        self.select = select_expr
+
+        self.partition = partition
+        self.partition_schema = partition_schema
+
+        self.overwrite = overwrite
+
+    def compile(self):
+        if self.overwrite:
+            cmd = 'INSERT OVERWRITE'
+        else:
+            cmd = 'INSERT INTO'
+
+        if self.partition is not None:
+            part = _format_partition(self.partition,
+                                     self.partition_schema)
+            partition = ' {0} '.format(part)
+        else:
+            partition = ''
+
+        select_query = self.select.compile()
+        scoped_name = self._get_scoped_name(self.table_name, self.database)
+        return'{0} {1}{2}\n{3}'.format(cmd, scoped_name, partition,
+                                       select_query)
+
+
+def _format_partition(partition, partition_schema):
+    tokens = []
+    if isinstance(partition, dict):
+        for name in partition_schema:
+            if name in partition:
+                tok = '{0}={1}'.format(name, partition[name])
+            else:
+                # dynamic partitioning
+                tok = name
+            tokens.append(tok)
     else:
-        entrypoints = importlib.metadata.entry_points(group="ibis.backends")
-    return frozenset(ep.name for ep in entrypoints)
+        for name, value in zip(partition_schema, partition):
+            tok = '{0}={1}'.format(name, value)
+            tokens.append(tok)
 
+    return 'PARTITION ({0})'.format(', '.join(tokens))
 
-def connect(resource: Path | str, **kwargs: Any) -> BaseBackend:
-    """Connect to `resource`, inferring the backend automatically.
 
-    Parameters
-    ----------
-    resource
-        A URL or path to the resource to be connected to.
-    kwargs
-        Backend specific keyword arguments
-
-    Examples
-    --------
-    Connect to an in-memory duckdb database:
-    >>> con = ibis.connect("duckdb://")
-
-    Connect to an on-disk sqlite database:
-    >>> con = ibis.connect("sqlite://relative/path/to/data.db")
-    >>> con = ibis.connect("sqlite:///absolute/path/to/data.db")
+class LoadData(ImpalaDDL):
 
-    Connect to a postgres server:
-    >>> con = ibis.connect("postgres://user:password@hostname:5432")
     """
-    url = resource = str(resource)
+    Generate DDL for LOAD DATA command. Cannot be cancelled
+    """
 
-    if re.match("[A-Za-z]:", url):
-        # windows path with drive, treat it as a file
-        url = f"file://{url}"
-
-    parsed = urllib.parse.urlparse(url)
-    scheme = parsed.scheme or "file"
-
-    orig_kwargs = kwargs.copy()
-    kwargs = dict(urllib.parse.parse_qsl(parsed.query))
-
-    if scheme == "file":
-        path = parsed.netloc + parsed.path
-        # Merge explicit kwargs with query string, explicit kwargs
-        # taking precedence
-        kwargs.update(orig_kwargs)
-        if path.endswith(".duckdb"):
-            return ibis.duckdb.connect(path, **kwargs)
-        elif path.endswith((".sqlite", ".db")):
-            return ibis.sqlite.connect(path, **kwargs)
-        elif path.endswith((".parquet", ".csv", ".csv.gz")):
-            # Load parquet/csv/csv.gz files with duckdb by default
-            con = ibis.duckdb.connect(**kwargs)
-            con.register(path)
-            return con
+    def __init__(self, table_name, path, database=None,
+                 partition=None, partition_schema=None,
+                 overwrite=False):
+        self.table_name = table_name
+        self.database = database
+        self.path = path
+
+        self.partition = partition
+        self.partition_schema = partition_schema
+
+        self.overwrite = overwrite
+
+    def compile(self):
+        overwrite = 'OVERWRITE ' if self.overwrite else ''
+
+        if self.partition is not None:
+            partition = '\n' + _format_partition(self.partition,
+                                                 self.partition_schema)
         else:
-            raise ValueError(f"Don't know how to connect to {resource!r}")
+            partition = ''
+
+        scoped_name = self._get_scoped_name(self.table_name, self.database)
+        return ("LOAD DATA INPATH '{0}' {1}INTO TABLE {2}{3}"
+                .format(self.path, overwrite, scoped_name, partition))
+
+
+class AlterTable(ImpalaDDL):
+
+    def __init__(self, table, location=None, format=None, tbl_properties=None,
+                 serde_properties=None):
+        self.table = table
+        self.location = location
+        self.format = _sanitize_format(format)
+        self.tbl_properties = tbl_properties
+        self.serde_properties = serde_properties
+
+    def _wrap_command(self, cmd):
+        return 'ALTER TABLE {0}'.format(cmd)
 
-    if kwargs:
-        # If there are kwargs (either explicit or from the query string),
-        # re-add them to the parsed URL
-        query = urllib.parse.urlencode(kwargs)
-        parsed = parsed._replace(query=query)
-
-    if scheme in ("postgres", "postgresql"):
-        # Treat `postgres://` and `postgresql://` the same, just as postgres
-        # does. We normalize to `postgresql` since that's what SQLAlchemy
-        # accepts.
-        scheme = "postgres"
-        parsed = parsed._replace(scheme="postgresql")
-
-    # Convert all arguments back to a single URL string
-    url = parsed.geturl()
-    if "://" not in url:
-        # SQLAlchemy requires a `://`, while urllib may roundtrip
-        # `duckdb://` to `duckdb:`. Here we re-add the missing `//`.
-        url = url.replace(":", "://", 1)
-    if scheme in ("duckdb", "sqlite", "pyspark"):
-        # SQLAlchemy wants an extra slash for URLs where the path
-        # maps to a relative/absolute location on the filesystem
-        url = url.replace(":", ":/", 1)
-
-    try:
-        backend = getattr(ibis, scheme)
-    except AttributeError:
-        raise ValueError(f"Don't know how to connect to {resource!r}") from None
+    def _format_properties(self, prefix=''):
+        tokens = []
 
-    return backend._from_url(url, **orig_kwargs)
+        if self.location is not None:
+            tokens.append("LOCATION '{0}'".format(self.location))
+
+        if self.format is not None:
+            tokens.append("FILEFORMAT {0}".format(self.format))
+
+        if self.tbl_properties is not None:
+            props = _format_properties(self.tbl_properties)
+            tokens.append('TBLPROPERTIES {0}'.format(props))
+
+        if self.serde_properties is not None:
+            props = _format_properties(self.serde_properties)
+            tokens.append('SERDEPROPERTIES {0}'.format(props))
+
+        if len(tokens) > 0:
+            return '\n{0}{1}'.format(prefix, '\n'.join(tokens))
+        else:
+            return ''
+
+    def compile(self):
+        props = self._format_properties()
+        action = '{0} SET {1}'.format(self.table, props)
+        return self._wrap_command(action)
+
+
+class PartitionProperties(AlterTable):
+
+    def __init__(self, table, partition, partition_schema,
+                 location=None, format=None,
+                 tbl_properties=None, serde_properties=None):
+        self.partition = partition
+        self.partition_schema = partition_schema
+
+        AlterTable.__init__(self, table, location=location, format=format,
+                            tbl_properties=tbl_properties,
+                            serde_properties=serde_properties)
+
+    def _compile(self, cmd, property_prefix=''):
+        part = _format_partition(self.partition, self.partition_schema)
+        if cmd:
+            part = '{0} {1}'.format(cmd, part)
+
+        props = self._format_properties(property_prefix)
+        action = '{0} {1}{2}'.format(self.table, part, props)
+        return self._wrap_command(action)
+
+
+class AddPartition(PartitionProperties):
+
+    def __init__(self, table, partition, partition_schema, location=None):
+        PartitionProperties.__init__(self, table, partition,
+                                     partition_schema,
+                                     location=location)
+
+    def compile(self):
+        return self._compile('ADD')
+
+
+class AlterPartition(PartitionProperties):
+
+    def compile(self):
+        return self._compile('', 'SET ')
+
+
+class DropPartition(PartitionProperties):
+
+    def __init__(self, table, partition, partition_schema):
+        PartitionProperties.__init__(self, table, partition,
+                                     partition_schema)
+
+    def compile(self):
+        return self._compile('DROP')
+
+
+class RenameTable(AlterTable):
+
+    def __init__(self, old_name, new_name, old_database=None,
+                 new_database=None):
+        # if either database is None, the name is assumed to be fully scoped
+        self.old_name = old_name
+        self.old_database = old_database
+        self.new_name = new_name
+        self.new_database = new_database
+
+        new_qualified_name = new_name
+        if new_database is not None:
+            new_qualified_name = self._get_scoped_name(new_name, new_database)
+
+        old_qualified_name = old_name
+        if old_database is not None:
+            old_qualified_name = self._get_scoped_name(old_name, old_database)
+
+        self.old_qualified_name = old_qualified_name
+        self.new_qualified_name = new_qualified_name
+
+    def compile(self):
+        cmd = '{0} RENAME TO {1}'.format(self.old_qualified_name,
+                                         self.new_qualified_name)
+        return self._wrap_command(cmd)
+
+
+class DropObject(ImpalaDDL):
+
+    def __init__(self, must_exist=True):
+        self.must_exist = must_exist
+
+    def compile(self):
+        if_exists = '' if self.must_exist else 'IF EXISTS '
+        object_name = self._object_name()
+        drop_line = 'DROP {0} {1}{2}'.format(self._object_type, if_exists,
+                                             object_name)
+        return drop_line
+
+
+class DropTable(DropObject):
+
+    _object_type = 'TABLE'
+
+    def __init__(self, table_name, database=None, must_exist=True):
+        self.table_name = table_name
+        self.database = database
+        DropObject.__init__(self, must_exist=must_exist)
+
+    def _object_name(self):
+        return self._get_scoped_name(self.table_name, self.database)
+
+
+class TruncateTable(ImpalaDDL):
+
+    _object_type = 'TABLE'
+
+    def __init__(self, table_name, database=None):
+        self.table_name = table_name
+        self.database = database
+
+    def compile(self):
+        name = self._get_scoped_name(self.table_name, self.database)
+        return 'TRUNCATE TABLE {0}'.format(name)
+
+
+class DropView(DropTable):
+
+    _object_type = 'VIEW'
+
+
+class CacheTable(ImpalaDDL):
+
+    def __init__(self, table_name, database=None, pool='default'):
+        self.table_name = table_name
+        self.database = database
+        self.pool = pool
+
+    def compile(self):
+        scoped_name = self._get_scoped_name(self.table_name, self.database)
+        cache_line = ('ALTER TABLE {0} SET CACHED IN \'{1}\''
+                      .format(scoped_name, self.pool))
+        return cache_line
+
+
+class CreateDatabase(CreateDDL):
+
+    def __init__(self, name, path=None, can_exist=False):
+        self.name = name
+        self.path = path
+        self.can_exist = can_exist
+
+    def compile(self):
+        name = quote_identifier(self.name)
+
+        create_decl = 'CREATE DATABASE'
+        create_line = '{0} {1}{2}'.format(create_decl, self._if_exists(),
+                                          name)
+        if self.path is not None:
+            create_line += "\nLOCATION '{0}'".format(self.path)
+
+        return create_line
+
+
+class DropDatabase(DropObject):
+
+    _object_type = 'DATABASE'
+
+    def __init__(self, name, must_exist=True):
+        self.name = name
+        DropObject.__init__(self, must_exist=must_exist)
+
+    def _object_name(self):
+        return self.name
+
+
+def format_schema(schema):
+    elements = [_format_schema_element(name, t)
+                for name, t in zip(schema.names, schema.types)]
+    return '({0})'.format(',\n '.join(elements))
+
+
+def _format_schema_element(name, t):
+    return '{0} {1}'.format(quote_identifier(name, force=True),
+                            _type_to_sql_string(t))
+
+
+class CreateFunctionBase(ImpalaDDL):
+
+    _object_type = 'FUNCTION'
+
+    def __init__(self, lib_path, inputs, output, name, database=None):
+        self.lib_path = lib_path
+
+        self.inputs, self.output = inputs, output
+        self.input_sig = _impala_signature(inputs)
+        self.output_sig = _arg_to_string(output)
+
+        self.name = name
+        self.database = database
+
+    def _create_line(self):
+        scoped_name = self._get_scoped_name(self.name, self.database)
+        return ('{0!s}({1!s}) returns {2!s}'
+                .format(scoped_name, self.input_sig, self.output_sig))
+
+
+class CreateFunction(CreateFunctionBase):
+
+    def __init__(self, lib_path, so_symbol, inputs, output,
+                 name, database=None):
+        self.so_symbol = so_symbol
+
+        CreateFunctionBase.__init__(self, lib_path, inputs, output,
+                                    name, database=database)
+
+    def compile(self):
+        create_decl = 'CREATE FUNCTION'
+        create_line = self._create_line()
+        param_line = ("location '{0!s}' symbol='{1!s}'"
+                      .format(self.lib_path, self.so_symbol))
+        full_line = ' '.join([create_decl, create_line, param_line])
+        return full_line
+
+
+class CreateAggregateFunction(CreateFunction):
+
+    def __init__(self, lib_path, inputs, output, update_fn, init_fn,
+                 merge_fn, serialize_fn, finalize_fn, name, database):
+        self.init = init_fn
+        self.update = update_fn
+        self.merge = merge_fn
+        self.serialize = serialize_fn
+        self.finalize = finalize_fn
+
+        CreateFunctionBase.__init__(self, lib_path, inputs, output,
+                                    name, database=database)
+
+    def compile(self):
+        create_decl = 'CREATE AGGREGATE FUNCTION'
+        create_line = self._create_line()
+        tokens = ["location '{0!s}'".format(self.lib_path)]
+
+        if self.init is not None:
+            tokens.append("init_fn='{0}'".format(self.init))
+
+        tokens.append("update_fn='{0}'".format(self.update))
+
+        if self.merge is not None:
+            tokens.append("merge_fn='{0}'".format(self.merge))
+
+        if self.serialize is not None:
+            tokens.append("serialize_fn='{0}'".format(self.serialize))
+
+        if self.finalize is not None:
+            tokens.append("finalize_fn='{0}'".format(self.finalize))
+
+        full_line = (' '.join([create_decl, create_line]) + ' ' +
+                     '\n'.join(tokens))
+        return full_line
+
+
+class DropFunction(DropObject):
+
+    def __init__(self, name, inputs, must_exist=True,
+                 aggregate=False, database=None):
+        self.name = name
+
+        self.inputs = inputs
+        self.input_sig = _impala_signature(inputs)
+
+        self.must_exist = must_exist
+        self.aggregate = aggregate
+        self.database = database
+        DropObject.__init__(self, must_exist=must_exist)
+
+    def _object_name(self):
+        return self.name
+
+    def _function_sig(self):
+        full_name = self._get_scoped_name(self.name, self.database)
+        return '{0!s}({1!s})'.format(full_name, self.input_sig)
+
+    def compile(self):
+        tokens = ['DROP']
+        if self.aggregate:
+            tokens.append('AGGREGATE')
+        tokens.append('FUNCTION')
+        if not self.must_exist:
+            tokens.append('IF EXISTS')
+
+        tokens.append(self._function_sig())
+        return ' '.join(tokens)
+
+
+class ListFunction(ImpalaDDL):
+
+    def __init__(self, database, like=None, aggregate=False):
+        self.database = database
+        self.like = like
+        self.aggregate = aggregate
+
+    def compile(self):
+        statement = 'SHOW '
+        if self.aggregate:
+            statement += 'AGGREGATE '
+        statement += 'FUNCTIONS IN {0}'.format(self.database)
+        if self.like:
+            statement += " LIKE '{0}'".format(self.like)
+        return statement
+
+
+def _impala_signature(sig):
+    if isinstance(sig, rules.TypeSignature):
+        if isinstance(sig, rules.VarArgs):
+            val = _arg_to_string(sig.arg_type)
+            return '{0}...'.format(val)
+        else:
+            return ', '.join([_arg_to_string(arg) for arg in sig.types])
+    else:
+        return ', '.join([_type_to_sql_string(validate_type(x))
+                          for x in sig])
+
+
+def _arg_to_string(arg):
+    if isinstance(arg, rules.ValueTyped):
+        types = arg.types
+        if len(types) > 1:
+            raise NotImplementedError
+        return _type_to_sql_string(types[0])
+    elif isinstance(arg, py_string):
+        return _type_to_sql_string(validate_type(arg))
+    else:
+        raise NotImplementedError
```

### Comparing `ibis_framework-5.1.0/ibis/backends/base/sql/alchemy/__init__.py` & `ibis-framework-v0.6.0/ibis/sql/alchemy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,725 +1,875 @@
-from __future__ import annotations
+# Copyright 2015 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import abc
-import atexit
-import contextlib
-import getpass
-import warnings
-from operator import methodcaller
-from typing import TYPE_CHECKING, Any, Iterable, Literal, Mapping
+import operator
+import six
 
 import sqlalchemy as sa
+import sqlalchemy.sql as sql
 
-import ibis
-import ibis.common.exceptions as com
+from ibis.client import SQLClient, AsyncQuery, Query
+from ibis.sql.compiler import Select, Union, TableSetFormatter
+import ibis.common as com
+import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
-import ibis.expr.schema as sch
 import ibis.expr.types as ir
-from ibis import util
-from ibis.backends.base.sql import BaseSQLBackend
-from ibis.backends.base.sql.alchemy.database import AlchemyDatabase, AlchemyTable
-from ibis.backends.base.sql.alchemy.datatypes import schema_from_table, to_sqla_type
-from ibis.backends.base.sql.alchemy.geospatial import geospatial_supported
-from ibis.backends.base.sql.alchemy.query_builder import AlchemyCompiler
-from ibis.backends.base.sql.alchemy.registry import (
-    fixed_arity,
-    get_sqla_table,
-    reduction,
-    sqlalchemy_operation_registry,
-    sqlalchemy_window_functions_registry,
-    unary,
-    varargs,
-    variance_reduction,
-)
-from ibis.backends.base.sql.alchemy.translator import (
-    AlchemyContext,
-    AlchemyExprTranslator,
-)
-
-if TYPE_CHECKING:
-    import pandas as pd
-
-    import ibis.expr.datatypes as dt
-
-__all__ = (
-    'BaseAlchemyBackend',
-    'AlchemyExprTranslator',
-    'AlchemyContext',
-    'AlchemyCompiler',
-    'AlchemyTable',
-    'AlchemyDatabase',
-    'AlchemyContext',
-    'sqlalchemy_operation_registry',
-    'sqlalchemy_window_functions_registry',
-    'reduction',
-    'variance_reduction',
-    'fixed_arity',
-    'unary',
-    'infix_op',
-    'get_sqla_table',
-    'to_sqla_type',
-    'schema_from_table',
-    'varargs',
-)
-
-
-class BaseAlchemyBackend(BaseSQLBackend):
-    """Backend class for backends that compile to SQLAlchemy expressions."""
-
-    database_class = AlchemyDatabase
-    table_class = AlchemyTable
-    compiler = AlchemyCompiler
-
-    def _build_alchemy_url(self, url, host, port, user, password, database, driver):
-        if url is not None:
-            return sa.engine.url.make_url(url)
-
-        user = user or getpass.getuser()
-        return sa.engine.url.URL.create(
-            driver,
-            host=host,
-            port=port,
-            username=user,
-            password=password,
-            database=database,
-        )
+import ibis.sql.compiler as comp
+import ibis.sql.transforms as transforms
+import ibis.util as util
+import ibis
+
+
+_ibis_type_to_sqla = {
+    dt.Int8: sa.types.SmallInteger,
+    dt.Int16: sa.types.SmallInteger,
+    dt.Int32: sa.types.Integer,
+    dt.Int64: sa.types.BigInteger,
+
+    # Mantissa-based
+    dt.Float: sa.types.Float(precision=24),
+    dt.Double: sa.types.Float(precision=53),
+
+    dt.Boolean: sa.types.Boolean,
+
+    dt.String: sa.types.String,
+
+    dt.Timestamp: sa.types.DateTime,
+
+    dt.Decimal: sa.types.NUMERIC,
+}
+
+_sqla_type_mapping = {
+    sa.types.SmallInteger: dt.Int16,
+    sa.types.INTEGER: dt.Int64,
+    sa.types.BOOLEAN: dt.Boolean,
+    sa.types.BIGINT: dt.Int64,
+    sa.types.FLOAT: dt.Double,
+    sa.types.REAL: dt.Double,
+
+    sa.types.TEXT: dt.String,
+    sa.types.NullType: dt.String,
+    sa.types.Text: dt.String,
+}
+
+_sqla_type_to_ibis = dict((v, k) for k, v in
+                          _ibis_type_to_sqla.items())
+_sqla_type_to_ibis.update(_sqla_type_mapping)
+
+
+def schema_from_table(table):
+    # Convert SQLA table to Ibis schema
+    names = table.columns.keys()
+
+    types = []
+    for c in table.columns.values():
+        type_class = type(c.type)
+
+        if isinstance(c.type, sa.types.NUMERIC):
+            t = dt.Decimal(c.type.precision,
+                           c.type.scale,
+                           nullable=c.nullable)
+        else:
+            if c.type in _sqla_type_to_ibis:
+                ibis_class = _sqla_type_to_ibis[c.type]
+            elif type_class in _sqla_type_to_ibis:
+                ibis_class = _sqla_type_to_ibis[type_class]
+            else:
+                raise NotImplementedError(c.type)
+            t = ibis_class(c.nullable)
+
+        types.append(t)
+
+    return dt.Schema(names, types)
+
+
+def table_from_schema(name, meta, schema):
+    # Convert Ibis schema to SQLA table
+    sqla_cols = []
+
+    for cname, itype in zip(schema.names, schema.types):
+        ctype = _to_sqla_type(itype)
+
+        col = sa.Column(cname, ctype, nullable=itype.nullable)
+        sqla_cols.append(col)
+
+    return sa.Table(name, meta, *sqla_cols)
+
+
+def _to_sqla_type(itype):
+    if isinstance(itype, dt.Decimal):
+        return sa.types.NUMERIC(itype.precision, itype.scale)
+    else:
+        return _ibis_type_to_sqla[type(itype)]
+
+
+def fixed_arity(sa_func, arity):
+    if isinstance(sa_func, six.string_types):
+        sa_func = getattr(sa.func, sa_func)
+
+    def formatter(t, expr):
+        if arity != len(expr.op().args):
+            raise com.IbisError('incorrect number of args')
+
+        return _varargs_call(sa_func, t, expr)
+
+    return formatter
+
+
+def varargs(sa_func):
+    def formatter(t, expr):
+        op = expr.op()
+        trans_args = [t.translate(arg) for arg in op.args]
+        return sa_func(*trans_args)
+    return formatter
+
+
+def _varargs_call(sa_func, t, expr):
+    op = expr.op()
+    trans_args = [t.translate(arg) for arg in op.args]
+    return sa_func(*trans_args)
+
+
+def _table_column(t, expr):
+    op = expr.op()
+    ctx = t.context
+    table = op.table
+
+    sa_table = _get_sqla_table(ctx, table)
+    out_expr = getattr(sa_table.c, op.name)
+
+    # If the column does not originate from the table set in the current SELECT
+    # context, we should format as a subquery
+    if t.permit_subquery and ctx.is_foreign_expr(table):
+        return sa.select([out_expr])
+
+    return out_expr
+
+
+def _get_sqla_table(ctx, table):
+    if ctx.has_ref(table):
+        ctx_level = ctx
+        sa_table = ctx_level.get_table(table)
+        while sa_table is None and ctx_level.parent is not ctx_level:
+            ctx_level = ctx_level.parent
+            sa_table = ctx_level.get_table(table)
+    else:
+        sa_table = table.op().sqla_table
+
+    return sa_table
+
+
+def _table_array_view(t, expr):
+    ctx = t.context
+    table = ctx.get_compiled_expr(expr.op().table)
+    return table
+
+
+def _exists_subquery(t, expr):
+    op = expr.op()
+    ctx = t.context
+
+    filtered = (op.foreign_table.filter(op.predicates)
+                .projection([ir.literal(1).name(ir.unnamed)]))
+
+    sub_ctx = ctx.subcontext()
+    clause = to_sqlalchemy(filtered, context=sub_ctx, exists=True)
+
+    if isinstance(op, transforms.NotExistsSubquery):
+        clause = sa.not_(clause)
+
+    return clause
+
+
+def _cast(t, expr):
+    op = expr.op()
+    arg, target_type = op.args
+    sa_arg = t.translate(arg)
+    sa_type = t.get_sqla_type(target_type)
+
+    if isinstance(arg, ir.CategoryValue) and target_type == 'int32':
+        return sa_arg
+    else:
+        return sa.cast(sa_arg, sa_type)
+
+
+def _contains(t, expr):
+    op = expr.op()
+
+    left, right = [t.translate(arg) for arg in op.args]
+    return left.in_(right)
+
+
+def _reduction(sa_func):
+    def formatter(t, expr):
+        op = expr.op()
+
+        # HACK: support trailing arguments
+        arg, where = op.args[:2]
+
+        return _reduction_format(t, sa_func, arg, where)
+    return formatter
+
+
+def _reduction_format(t, sa_func, arg, where):
+    if where is not None:
+        case = where.ifelse(arg, ibis.NA)
+        arg = t.translate(case)
+    else:
+        arg = t.translate(arg)
+
+    return sa_func(arg)
+
+
+def _literal(t, expr):
+    return sa.literal(expr.op().value)
+
+
+def _value_list(t, expr):
+    return [t.translate(x) for x in expr.op().values]
+
+
+def _is_null(t, expr):
+    arg = t.translate(expr.op().args[0])
+    return arg.is_(sa.null())
+
+
+def _not_null(t, expr):
+    arg = t.translate(expr.op().args[0])
+    return arg.isnot(sa.null())
+
+
+def _round(t, expr):
+    op = expr.op()
+    arg, digits = op.args
+    sa_arg = t.translate(arg)
+
+    f = sa.func.round
+
+    if digits is not None:
+        sa_digits = t.translate(digits)
+        return f(sa_arg, sa_digits)
+    else:
+        return f(sa_arg)
+
+
+def _count_distinct(t, expr):
+    arg, = expr.op().args
+    sa_arg = t.translate(arg)
+    return sa.func.count(sa_arg.distinct())
+
+
+def _simple_case(t, expr):
+    op = expr.op()
+
+    cases = [op.base == case for case in op.cases]
+    return _translate_case(t, cases, op.results, op.default)
+
+
+def _searched_case(t, expr):
+    op = expr.op()
+    return _translate_case(t, op.cases, op.results, op.default)
+
+
+def _translate_case(t, cases, results, default):
+    case_args = [t.translate(arg) for arg in cases]
+    result_args = [t.translate(arg) for arg in results]
+
+    whens = zip(case_args, result_args)
+    default = t.translate(default)
+
+    return sa.case(whens, else_=default)
+
+
+def unary(sa_func):
+    return fixed_arity(sa_func, 1)
+
+
+_operation_registry = {
+    ops.And: fixed_arity(sql.and_, 2),
+    ops.Or: fixed_arity(sql.or_, 2),
+
+    ops.Abs: unary(sa.func.abs),
+
+    ops.Cast: _cast,
+
+    ops.Coalesce: varargs(sa.func.coalesce),
+
+    ops.NullIf: fixed_arity(sa.func.nullif, 2),
+
+    ops.Contains: _contains,
+
+    ops.Count: _reduction(sa.func.count),
+    ops.Sum: _reduction(sa.func.sum),
+    ops.Mean: _reduction(sa.func.avg),
+    ops.Min: _reduction(sa.func.min),
+    ops.Max: _reduction(sa.func.max),
+
+    ops.CountDistinct: _count_distinct,
+
+    ops.GroupConcat: fixed_arity(sa.func.group_concat, 2),
+
+    ops.Between: fixed_arity(sa.between, 3),
+
+    ops.IsNull: _is_null,
+    ops.NotNull: _not_null,
+    ops.Negate: unary(sa.not_),
+
+    ops.Round: _round,
+
+    ops.TypeOf: unary(sa.func.typeof),
+
+    ir.Literal: _literal,
+    ir.ValueList: _value_list,
+    ir.NullLiteral: lambda *args: sa.null(),
+
+    ops.SimpleCase: _simple_case,
+    ops.SearchedCase: _searched_case,
+
+    ops.TableColumn: _table_column,
+    ops.TableArrayView: _table_array_view,
+
+    transforms.ExistsSubquery: _exists_subquery,
+    transforms.NotExistsSubquery: _exists_subquery,
+}
+
+
+# TODO: unit tests for each of these
+_binary_ops = {
+    # Binary arithmetic
+    ops.Add: operator.add,
+    ops.Subtract: operator.sub,
+    ops.Multiply: operator.mul,
+    ops.Divide: operator.truediv,
+    ops.Power: operator.pow,
+    ops.Modulus: operator.mod,
+
+    # Comparisons
+    ops.Equals: operator.eq,
+    ops.NotEquals: operator.ne,
+    ops.Less: operator.lt,
+    ops.LessEqual: operator.le,
+    ops.Greater: operator.gt,
+    ops.GreaterEqual: operator.ge,
+
+    # Boolean comparisons
+
+    # TODO
+}
+
+for _k, _v in _binary_ops.items():
+    _operation_registry[_k] = fixed_arity(_v, 2)
+
+
+class AlchemySelectBuilder(comp.SelectBuilder):
 
     @property
-    def _current_schema(self) -> str | None:
-        return None
+    def _select_class(self):
+        return AlchemySelect
+
+    def _convert_group_by(self, exprs):
+        return exprs
+
+
+class AlchemyContext(comp.QueryContext):
+
+    def __init__(self, *args, **kwargs):
+        self._table_objects = {}
+        self.dialect = kwargs.pop('dialect', AlchemyDialect)
+        comp.QueryContext.__init__(self, *args, **kwargs)
+
+    def subcontext(self):
+        return type(self)(dialect=self.dialect, parent=self)
+
+    def _to_sql(self, expr, ctx):
+        return to_sqlalchemy(expr, context=ctx)
+
+    def _compile_subquery(self, expr):
+        sub_ctx = self.subcontext()
+        return self._to_sql(expr, sub_ctx)
+
+    def has_table(self, expr, parent_contexts=False):
+        key = self._get_table_key(expr)
+        return self._key_in(key, '_table_objects',
+                            parent_contexts=parent_contexts)
+
+    def set_table(self, expr, obj):
+        key = self._get_table_key(expr)
+        self._table_objects[key] = obj
 
-    def do_connect(self, con: sa.engine.Engine) -> None:
-        self.con = con
-        self._inspector = sa.inspect(self.con)
-        self._schemas: dict[str, sch.Schema] = {}
-        self._temp_views: set[str] = set()
+    def get_table(self, expr):
+        """
+        Get the memoized SQLAlchemy expression object
+        """
+        return self._get_table_item('_table_objects', expr)
+
+
+class AlchemyQueryBuilder(comp.QueryBuilder):
+
+    select_builder = AlchemySelectBuilder
+
+    def __init__(self, expr, context=None, dialect=None):
+        if dialect is None:
+            dialect = AlchemyDialect
+
+        self.dialect = dialect
+        comp.QueryBuilder.__init__(self, expr, context=context)
+
+    def _make_context(self):
+        return AlchemyContext(dialect=self.dialect)
 
     @property
-    def version(self):
-        return '.'.join(map(str, self.con.dialect.server_version_info))
+    def _union_class(self):
+        return AlchemyUnion
 
-    def list_tables(self, like=None, database=None):
-        tables = self.inspector.get_table_names(schema=database)
-        views = self.inspector.get_view_names(schema=database)
-        return self._filter_with_like(tables + views, like)
-
-    def list_databases(self, like=None):
-        """List databases in the current server."""
-        databases = self.inspector.get_schema_names()
-        return self._filter_with_like(databases, like)
+
+def to_sqlalchemy(expr, context=None, exists=False, dialect=None):
+    if context is not None:
+        dialect = dialect or context.dialect
+
+    ast = build_ast(expr, context=context, dialect=dialect)
+    query = ast.queries[0]
+
+    if exists:
+        query.exists = exists
+
+    return query.compile()
+
+
+def build_ast(expr, context=None, dialect=None):
+    builder = AlchemyQueryBuilder(expr, context=context, dialect=dialect)
+    return builder.get_result()
+
+
+class AlchemyTable(ops.DatabaseTable):
+
+    def __init__(self, table, source):
+        self.sqla_table = table
+
+        schema = schema_from_table(table)
+        name = table.name
+
+        ops.TableNode.__init__(self, [name, schema, source])
+        ops.HasSchema.__init__(self, schema, name=name)
+
+
+class AlchemyExprTranslator(comp.ExprTranslator):
+
+    _registry = _operation_registry
+    _rewrites = comp.ExprTranslator._rewrites.copy()
+    _type_map = _ibis_type_to_sqla
+
+    def name(self, translated, name, force=True):
+        return translated.label(name)
 
     @property
-    def inspector(self):
-        self._inspector.info_cache.clear()
-        return self._inspector
-
-    def _to_sql(self, expr: ir.Expr, **kwargs) -> str:
-        # For `ibis.to_sql` calls we render with literal binds and qmark params
-        dialect_class = sa.dialects.registry.load(
-            self.compiler.translator_class._dialect_name
-        )
-        sql = self.compile(expr, **kwargs).compile(
-            dialect=dialect_class(paramstyle="qmark"),
-            compile_kwargs=dict(literal_binds=True),
-        )
-        return str(sql)
-
-    @contextlib.contextmanager
-    def _safe_raw_sql(self, *args, **kwargs):
-        with self.begin() as con:
-            yield con.execute(*args, **kwargs)
-
-    @staticmethod
-    def _to_geodataframe(df, schema):
-        """Convert `df` to a `GeoDataFrame`.
+    def _context_class(self):
+        return AlchemyContext
+
+    def get_sqla_type(self, data_type):
+        return self._type_map[type(data_type)]
 
-        Required libraries for geospatial support must be installed and
-        a geospatial column is present in the dataframe.
-        """
-        import geopandas as gpd
-        from geoalchemy2 import shape
 
-        geom_col = None
-        for name, dtype in schema.items():
-            if dtype.is_geospatial():
-                geom_col = geom_col or name
-                df[name] = df[name].map(
-                    lambda row: None if row is None else shape.to_shape(row)
-                )
-        if geom_col:
-            df[geom_col] = gpd.array.GeometryArray(df[geom_col].values)
-            df = gpd.GeoDataFrame(df, geometry=geom_col)
-        return df
+rewrites = AlchemyExprTranslator.rewrites
+compiles = AlchemyExprTranslator.compiles
 
-    def fetch_from_cursor(self, cursor, schema: sch.Schema) -> pd.DataFrame:
+
+class AlchemyQuery(Query):
+
+    def _fetch(self, cursor):
+        # No guarantees that the DBAPI cursor has data types
         import pandas as pd
+        proxy = cursor.proxy
+        rows = proxy.fetchall()
+        colnames = proxy.keys()
+        return pd.DataFrame.from_records(rows, columns=colnames,
+                                         coerce_float=True)
+
 
-        df = pd.DataFrame.from_records(cursor, columns=schema.names, coerce_float=True)
-        df = schema.apply_to(df)
-        if not df.empty and geospatial_supported:
-            return self._to_geodataframe(df, schema)
-        return df
-
-    @contextlib.contextmanager
-    def begin(self):
-        with self.con.begin() as bind:
-            yield bind
-
-    def create_table(
-        self,
-        name: str,
-        obj: pd.DataFrame | ir.Table | None = None,
-        *,
-        schema: sch.Schema | None = None,
-        database: str | None = None,
-        temp: bool = False,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        """Create a table.
+class AlchemyAsyncQuery(AsyncQuery):
+    pass
+
+
+class AlchemyDialect(object):
+
+    translator = AlchemyExprTranslator
+
+
+class AlchemyClient(SQLClient):
+
+    dialect = AlchemyDialect
+    sync_query = AlchemyQuery
+
+    @property
+    def async_query(self):
+        raise NotImplementedError
+
+    def create_table(self, name, expr=None, schema=None, database=None):
+        pass
+
+    def list_tables(self, like=None, database=None):
+        """
+        List tables in the current (or indicated) database.
 
         Parameters
         ----------
-        name
-            Name of the new table.
-        obj
-            An Ibis table expression or pandas table that will be used to
-            extract the schema and the data of the new table. If not provided,
-            `schema` must be given.
-        schema
-            The schema for the new table. Only one of `schema` or `obj` can be
-            provided.
-        database
-            Name of the database where the table will be created, if not the
-            default.
-        temp
-            Should the table be temporary for the session.
-        overwrite
-            Clobber existing data
+        like : string, default None
+          Checks for this string contained in name
+        database : string, default None
+          If not passed, uses the current/default database
 
         Returns
         -------
-        Table
-            The table that was created.
+        tables : list of strings
         """
-        if obj is None and schema is None:
-            raise com.IbisError("The schema or obj parameter is required")
+        if database is None:
+            database = self.current_database
+        names = self.con.table_names(schema=database)
+        if like is not None:
+            names = [x for x in names if like in x]
+        return names
 
-        import pandas as pd
+    def _execute(self, query, results=True):
+        return AlchemyProxy(self.con.execute(query))
+
+    def _build_ast(self, expr):
+        return build_ast(expr, dialect=self.dialect)
+
+    def _get_sqla_table(self, name):
+        return sa.Table(name, self.meta, autoload=True)
+
+    def _sqla_table_to_expr(self, table):
+        node = AlchemyTable(table, self)
+        return self._table_expr_klass(node)
+
+
+class AlchemySelect(Select):
+
+    def __init__(self, *args, **kwargs):
+        self.exists = kwargs.pop('exists', False)
+        Select.__init__(self, *args, **kwargs)
+
+    def compile(self):
+        # Can't tell if this is a hack or not. Revisit later
+        self.context.set_query(self)
+
+        self._compile_subqueries()
+
+        frag = self._compile_table_set()
+        steps = [self._add_select,
+                 self._add_groupby,
+                 self._add_where,
+                 self._add_order_by,
+                 self._add_limit]
+
+        for step in steps:
+            frag = step(frag)
+
+        return frag
+
+    def _compile_subqueries(self):
+        if len(self.subqueries) == 0:
+            return
+
+        for expr in self.subqueries:
+            result = self.context.get_compiled_expr(expr)
+            alias = self.context.get_ref(expr)
+            result = result.cte(alias)
+            self.context.set_table(expr, result)
+
+    def _compile_table_set(self):
+        if self.table_set is not None:
+            helper = _AlchemyTableSet(self, self.table_set)
+            return helper.get_result()
+        else:
+            return None
 
-        if isinstance(obj, pd.DataFrame):
-            obj = ibis.memtable(obj)
+    def _add_select(self, table_set):
+        to_select = []
+        for expr in self.select_set:
+            if isinstance(expr, ir.ValueExpr):
+                arg = self._translate(expr, named=True)
+            elif isinstance(expr, ir.TableExpr):
+                if expr.equals(self.table_set):
+                    cached_table = self.context.get_table(expr)
+                    if cached_table is None:
+                        # the select * case from materialized join
+                        arg = '*'
+                    else:
+                        arg = table_set
+                else:
+                    arg = self.context.get_table(expr)
+                    if arg is None:
+                        raise ValueError(expr)
 
-        if database == self.current_database:
-            # avoid fully qualified name
-            database = None
-
-        if database is not None:
-            raise NotImplementedError(
-                "Creating tables from a different database is not yet implemented"
-            )
-
-        if obj is not None and schema is not None:
-            if not obj.schema().equals(ibis.schema(schema)):
-                raise com.IbisTypeError(
-                    'Expression schema is not equal to passed schema. '
-                    'Try passing the expression without the schema'
-                )
-        if schema is None:
-            schema = obj.schema()
-
-        self._schemas[self._fully_qualified_name(name, database)] = schema
-        table = self._table_from_schema(
-            name,
-            schema,
-            database=database or self.current_database,
-            temp=temp,
-        )
-
-        if has_expr := obj is not None:
-            # this has to happen outside the `begin` block, so that in-memory
-            # tables are visible inside the transaction created by it
-            self._register_in_memory_tables(obj)
-
-        with self.begin() as bind:
-            if overwrite:
-                table.drop(bind=bind, checkfirst=True)
-            table.create(bind=bind)
-            if has_expr:
-                method = self._get_insert_method(obj)
-                bind.execute(method(table.insert()))
-        return self.table(name, database=database)
-
-    def _get_insert_method(self, expr):
-        compiled = self.compile(expr)
-
-        # if in memory tables aren't cheap then try to pull out their data
-        # FIXME: queries that *select* from in memory tables are still broken
-        # for mysql/sqlite/postgres because the generated SQL is wrong
-        if (
-            not self.compiler.cheap_in_memory_tables
-            and self.compiler.support_values_syntax_in_select
-            and isinstance(expr.op(), ops.InMemoryTable)
-        ):
-            (from_,) = compiled.get_final_froms()
-            try:
-                (rows,) = from_._data
-            except AttributeError:
-                return methodcaller("from_select", list(expr.columns), from_)
+            to_select.append(arg)
+
+        if self.exists:
+            clause = sa.exists(to_select)
+        else:
+            clause = sa.select(to_select)
+
+        if self.distinct:
+            clause = clause.distinct()
+
+        if table_set is not None:
+            return clause.select_from(table_set)
+        else:
+            return clause
+
+    def _add_groupby(self, fragment):
+        # GROUP BY and HAVING
+        if not len(self.group_by):
+            return fragment
+
+        group_keys = [self._translate(arg) for arg in self.group_by]
+        fragment = fragment.group_by(*group_keys)
+
+        if len(self.having) > 0:
+            having_args = [self._translate(arg) for arg in self.having]
+            having_clause = _and_all(having_args)
+            fragment = fragment.having(having_clause)
+
+        return fragment
+
+    def _add_where(self, fragment):
+        if not len(self.where):
+            return fragment
+
+        args = [self._translate(pred, permit_subquery=True)
+                for pred in self.where]
+        clause = _and_all(args)
+        return fragment.where(clause)
+
+    def _add_order_by(self, fragment):
+        if not len(self.order_by):
+            return fragment
+
+        clauses = []
+        for expr in self.order_by:
+            key = expr.op()
+            sort_expr = key.expr
+
+            # here we have to determine if key.expr is in the select set (as it
+            # will be in the case of order_by fused with an aggregation
+            if _can_lower_sort_column(self.table_set, sort_expr):
+                arg = sort_expr.get_name()
             else:
-                return methodcaller("values", rows)
+                arg = self._translate(sort_expr)
 
-        return methodcaller("from_select", list(expr.columns), compiled)
+            if not key.ascending:
+                arg = sa.desc(arg)
 
-    def _columns_from_schema(self, name: str, schema: sch.Schema) -> list[sa.Column]:
-        dialect = self.con.dialect
-        return [
-            sa.Column(
-                colname,
-                to_sqla_type(dialect, dtype),
-                nullable=dtype.nullable,
-                quote=self.compiler.translator_class._quote_column_names,
-            )
-            for colname, dtype in zip(schema.names, schema.types)
-        ]
-
-    def _table_from_schema(
-        self, name: str, schema: sch.Schema, temp: bool = False, **_: Any
-    ) -> sa.Table:
-        prefixes = []
-        if temp:
-            prefixes.append('TEMPORARY')
-        columns = self._columns_from_schema(name, schema)
-        return sa.Table(
-            name,
-            sa.MetaData(),
-            *columns,
-            prefixes=prefixes,
-            quote=self.compiler.translator_class._quote_table_names,
-        )
-
-    def drop_table(
-        self, name: str, *, database: str | None = None, force: bool = False
-    ) -> None:
-        """Drop a table.
+            clauses.append(arg)
 
-        Parameters
-        ----------
-        name
-            Table to drop
-        database
-            Database to drop table from
-        force
-            Check for existence before dropping
-        """
-        if database == self.current_database:
-            # avoid fully qualified name
-            database = None
-
-        if database is not None:
-            raise com.IbisInputError(
-                "Dropping tables from a different database is not yet implemented"
-            )
-
-        t = self._get_sqla_table(name, schema=database, autoload=False)
-        with self.begin() as bind:
-            t.drop(bind=bind, checkfirst=force)
-
-        qualified_name = self._fully_qualified_name(name, database)
-
-        with contextlib.suppress(KeyError):
-            # schemas won't be cached if created with raw_sql
-            del self._schemas[qualified_name]
-
-    @util.deprecated(
-        as_of="5.0", removed_in="6.0", instead="Use create_table(overwrite=True)"
-    )
-    def load_data(
-        self,
-        table_name: str,
-        data: pd.DataFrame,
-        database: str | None = None,
-        if_exists: Literal['fail', 'replace', 'append'] = 'fail',
-    ) -> None:
-        """Load data from a dataframe to the backend.
+        return fragment.order_by(*clauses)
 
-        Parameters
-        ----------
-        table_name
-            Name of the table in which to load data
-        data
-            Pandas DataFrame
-        database
-            Database in which the table exists
-        if_exists
-            What to do when data in `name` already exists
-
-        Raises
-        ------
-        NotImplementedError
-            Loading data to a table from a different database is not
-            yet implemented
-        """
-        if database == self.current_database:
-            # avoid fully qualified name
-            database = None
-
-        if database is not None:
-            raise NotImplementedError(
-                'Loading data to a table from a different database is not '
-                'yet implemented'
-            )
-
-        data.to_sql(
-            table_name,
-            con=self.con,
-            index=False,
-            if_exists=if_exists,
-            schema=self._current_schema,
-        )
-
-    def truncate_table(self, name: str, database: str | None = None) -> None:
-        t = self._get_sqla_table(name, schema=database)
-        with self.begin() as con:
-            con.execute(t.delete())
+    def _among_select_set(self, expr):
+        for other in self.select_set:
+            if expr.equals(other):
+                return True
+        return False
 
-    def schema(self, name: str) -> sch.Schema:
-        """Get an ibis schema from the current database for the table `name`.
+    def _add_limit(self, fragment):
+        if self.limit is None:
+            return fragment
 
-        Parameters
-        ----------
-        name
-            Table name
+        n, offset = self.limit['n'], self.limit['offset']
+        fragment = fragment.limit(n)
+        if offset is not None and offset != 0:
+            fragment = fragment.offset(offset)
 
-        Returns
-        -------
-        Schema
-            The ibis schema of `name`
-        """
-        return self.database().schema(name)
+        return fragment
 
     @property
-    def current_database(self) -> str:
-        """The name of the current database this client is connected to."""
-        return self.database_name
-
-    def _log(self, sql):
-        try:
-            query_str = str(sql)
-        except sa.exc.UnsupportedCompilationError:
-            pass
+    def translator(self):
+        return self.dialect.translator
+
+    @property
+    def dialect(self):
+        return self.context.dialect
+
+
+class _AlchemyTableSet(TableSetFormatter):
+
+    def get_result(self):
+        # Got to unravel the join stack; the nesting order could be
+        # arbitrary, so we do a depth first search and push the join tokens
+        # and predicates onto a flat list, then format them
+        op = self.expr.op()
+
+        if isinstance(op, ops.Join):
+            self._walk_join_tree(op)
         else:
-            util.log(query_str)
+            self.join_tables.append(self._format_table(self.expr))
 
-    def _get_sqla_table(
-        self, name: str, schema: str | None = None, autoload: bool = True, **_: Any
-    ) -> sa.Table:
-        # If the underlying table (or more likely, view) has changed, remove it
-        # to ensure a correct reflection
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore", message="Did not recognize type", category=sa.exc.SAWarning
-            )
-            table = sa.Table(
-                name,
-                sa.MetaData(),
-                schema=schema,
-                autoload_with=self.con if autoload else None,
-                quote=self.compiler.translator_class._quote_table_names,
-            )
-            nulltype_cols = frozenset(
-                col.name for col in table.c if isinstance(col.type, sa.types.NullType)
-            )
-
-            if not nulltype_cols:
-                return table
-            return self._handle_failed_column_type_inference(table, nulltype_cols)
-
-    def _handle_failed_column_type_inference(
-        self, table: sa.Table, nulltype_cols: Iterable[str]
-    ) -> sa.Table:
-        """Handle cases where SQLAlchemy cannot infer the column types of `table`."""
-
-        self.inspector.reflect_table(table, table.columns)
-        dialect = self.con.dialect
-        quoted_name = dialect.identifier_preparer.quote(table.name)
-
-        for colname, type in self._metadata(quoted_name):
-            if colname in nulltype_cols:
-                # replace null types discovered by sqlalchemy with non null
-                # types
-                table.append_column(
-                    sa.Column(
-                        colname,
-                        to_sqla_type(dialect, type),
-                        nullable=type.nullable,
-                        quote=self.compiler.translator_class._quote_column_names,
-                    ),
-                    replace_existing=True,
-                )
-        return table
-
-    def _sqla_table_to_expr(self, table: sa.Table) -> ir.Table:
-        schema = self._schemas.get(table.name)
-        node = self.table_class(
-            source=self,
-            sqla_table=table,
-            name=table.name,
-            schema=schema,
-        )
-        return self.table_expr_class(node)
+        result = self.join_tables[0]
+        for jtype, table, preds in zip(self.join_types,
+                                       self.join_tables[1:],
+                                       self.join_predicates):
+            if len(preds):
+                sqla_preds = [self._translate(pred) for pred in preds]
+                onclause = _and_all(sqla_preds)
+            else:
+                onclause = None
 
-    def raw_sql(self, query) -> None:
-        """Execute a query string.
+            if jtype in (ops.InnerJoin, ops.CrossJoin):
+                result = result.join(table, onclause)
+            elif jtype is ops.LeftJoin:
+                result = result.join(table, onclause, isouter=True)
+            elif jtype is ops.RightJoin:
+                result = table.join(result, onclause, isouter=True)
+            elif jtype is ops.OuterJoin:
+                result = result.outerjoin(table, onclause)
+            else:
+                raise NotImplementedError(jtype)
 
-        !!! warning "The returned cursor object must be **manually** released."
+        return result
 
-        Parameters
-        ----------
-        query
-            DDL or DML statement
-        """
-        return self.con.connect().execute(
-            sa.text(query) if isinstance(query, str) else query
-        )
-
-    def table(
-        self,
-        name: str,
-        database: str | None = None,
-        schema: str | None = None,
-    ) -> ir.Table:
-        """Create a table expression from a table in the database.
+    def _get_join_type(self, op):
+        return type(op)
 
-        Parameters
-        ----------
-        name
-            Table name
-        database
-            The database the table resides in
-        schema
-            The schema inside `database` where the table resides.
+    def _format_table(self, expr):
+        ctx = self.context
+        ref_expr = expr
+        op = ref_op = expr.op()
 
-            !!! warning "`schema` refers to database organization"
+        if isinstance(op, ops.SelfReference):
+            ref_expr = op.table
+            ref_op = ref_expr.op()
 
-                The `schema` parameter does **not** refer to the column names
-                and types of `table`.
+        alias = ctx.get_ref(expr)
 
-        Returns
-        -------
-        Table
-            Table expression
-        """
-        if database is not None:
-            if not isinstance(database, str):
-                raise com.IbisTypeError(
-                    f"`database` must be a string; got {type(database)}"
-                )
-            if database != self.current_database:
-                return self.database(name=database).table(name=name, schema=schema)
-        sqla_table = self._get_sqla_table(name, database=database, schema=schema)
-        return self._sqla_table_to_expr(sqla_table)
-
-    def _insert_dataframe(
-        self, table_name: str, df: pd.DataFrame, overwrite: bool
-    ) -> None:
-        schema = self._current_schema
-
-        t = self._get_sqla_table(table_name, schema=schema)
-        with self.con.begin() as con:
-            if overwrite:
-                con.execute(t.delete())
-            con.execute(t.insert(), df.to_dict(orient="records"))
-
-    def insert(
-        self,
-        table_name: str,
-        obj: pd.DataFrame | ir.Table | list | dict,
-        database: str | None = None,
-        overwrite: bool = False,
-    ) -> None:
-        """Insert data into a table.
+        if isinstance(ref_op, AlchemyTable):
+            result = ref_op.sqla_table
+        else:
+            # A subquery
+            if ctx.is_extracted(ref_expr):
+                # Was put elsewhere, e.g. WITH block, we just need to grab
+                # its alias
+                alias = ctx.get_ref(expr)
+
+                # hack
+                if isinstance(op, ops.SelfReference):
+                    table = ctx.get_table(ref_expr)
+                    self_ref = table.alias(alias)
+                    ctx.set_table(expr, self_ref)
+                    return self_ref
+                else:
+                    return ctx.get_table(expr)
+
+            result = ctx.get_compiled_expr(expr)
+            alias = ctx.get_ref(expr)
+
+        result = result.alias(alias)
+        ctx.set_table(expr, result)
+        return result
+
+
+def _can_lower_sort_column(table_set, expr):
+    # we can currently sort by just-appeared aggregate metrics, but the way
+    # these are references in the expression DSL is as a SortBy (blocking
+    # table operation) on an aggregation. There's a hack in _collect_SortBy
+    # in the generic SQL compiler that "fuses" the sort with the
+    # aggregation so they appear in same query. It's generally for
+    # cosmetics and doesn't really affect query semantics.
+    bases = ir.find_all_base_tables(expr)
+    if len(bases) > 1:
+        return False
+
+    base = list(bases.values())[0]
+    base_op = base.op()
+
+    if isinstance(base_op, ops.Aggregation):
+        return base_op.table.equals(table_set)
+    elif isinstance(base_op, ops.Projection):
+        return base.equals(table_set)
+    else:
+        return False
+
+
+def _and_all(clauses):
+    result = clauses[0]
+    for clause in clauses[1:]:
+        result = sql.and_(result, clause)
+    return result
 
-        Parameters
-        ----------
-        table_name
-            The name of the table to which data needs will be inserted
-        obj
-            The source data or expression to insert
-        database
-            Name of the attached database that the table is located in.
-        overwrite
-            If `True` then replace existing contents of table
-
-        Raises
-        ------
-        NotImplementedError
-            If inserting data from a different database
-        ValueError
-            If the type of `obj` isn't supported
-        """
 
-        import pandas as pd
+class AlchemyUnion(Union):
 
-        if database == self.current_database:
-            # avoid fully qualified name
-            database = None
-
-        if database is not None:
-            raise NotImplementedError(
-                'Inserting data to a table from a different database is not '
-                'yet implemented'
-            )
-
-        # If we've been passed a `memtable`, pull out the underlying dataframe
-        if isinstance(obj, ir.Table) and isinstance(
-            in_mem_table := obj.op(), ops.InMemoryTable
-        ):
-            obj = in_mem_table.data.to_frame()
-
-        if isinstance(obj, pd.DataFrame):
-            self._insert_dataframe(table_name, obj, overwrite=overwrite)
-        elif isinstance(obj, ir.Table):
-            to_table_expr = self.table(table_name)
-            to_table_schema = to_table_expr.schema()
-
-            if overwrite:
-                self.drop_table(table_name, database=database)
-                self.create_table(
-                    table_name,
-                    schema=to_table_schema,
-                    database=database,
-                )
-
-            to_table = self._get_sqla_table(table_name, schema=database)
-
-            from_table_expr = obj
-
-            with self.begin() as bind:
-                if from_table_expr is not None:
-                    compiled = from_table_expr.compile()
-                    columns = [
-                        self.con.dialect.normalize_name(c)
-                        for c in from_table_expr.columns
-                    ]
-                    bind.execute(to_table.insert().from_select(columns, compiled))
-        elif isinstance(obj, (list, dict)):
-            to_table = self._get_sqla_table(table_name, schema=database)
-
-            with self.begin() as bind:
-                if overwrite:
-                    bind.execute(to_table.delete())
-                bind.execute(to_table.insert().values(obj))
+    def compile(self):
+        context = self.context
 
+        if self.distinct:
+            sa_func = sa.union
         else:
-            raise ValueError(
-                "No operation is being performed. Either the obj parameter "
-                "is not a pandas DataFrame or is not a ibis Table."
-                f"The given obj is of type {type(obj).__name__} ."
-            )
-
-    def _quote(self, name: str) -> str:
-        """Quote an identifier."""
-        preparer = self.con.dialect.identifier_preparer
-        if self.compiler.translator_class._quote_table_names:
-            return preparer.quote_identifier(name)
-        return preparer.quote(name)
-
-    def _get_temp_view_definition(
-        self, name: str, definition: sa.sql.compiler.Compiled
-    ) -> str:
-        raise NotImplementedError(
-            f"The {self.name} backend does not implement temporary view creation"
-        )
-
-    def _register_temp_view_cleanup(self, name: str, raw_name: str) -> None:
-        query = f"DROP VIEW IF EXISTS {name}"
-
-        def drop(self, raw_name: str, query: str):
-            with self.begin() as con:
-                con.exec_driver_sql(query)
-            self._temp_views.discard(raw_name)
-
-        atexit.register(drop, self, raw_name, query)
-
-    def _get_compiled_statement(
-        self,
-        definition: sa.sql.Selectable,
-        name: str,
-        compile_kwargs: Mapping[str, Any] | None = None,
-    ):
-        if compile_kwargs is None:
-            compile_kwargs = {}
-        compiled = definition.compile(
-            dialect=self.con.dialect, compile_kwargs=compile_kwargs
-        )
-        lines = self._get_temp_view_definition(name, definition=compiled)
-        return lines, compiled.params
-
-    def _create_temp_view(self, view: sa.Table, definition: sa.sql.Selectable) -> None:
-        raw_name = view.name
-        if raw_name not in self._temp_views and raw_name in self.list_tables():
-            raise ValueError(f"{raw_name} already exists as a table or view")
-        name = self._quote(raw_name)
-        lines, params = self._get_compiled_statement(definition, name)
-        with self.begin() as con:
-            for line in lines:
-                con.exec_driver_sql(line, parameters=params or ())
-        self._temp_views.add(raw_name)
-        self._register_temp_view_cleanup(name, raw_name)
-
-    @abc.abstractmethod
-    def _metadata(self, query: str) -> Iterable[tuple[str, dt.DataType]]:
-        ...
-
-    def _get_schema_using_query(self, query: str) -> sch.Schema:
-        """Return an ibis Schema from a backend-specific SQL string."""
-        return sch.Schema.from_tuples(self._metadata(query))
-
-    def _load_into_cache(self, name, expr):
-        self.create_table(name, expr, schema=expr.schema(), temp=True)
-
-    def _clean_up_cached_table(self, op):
-        self.drop_table(op.name)
-
-    def create_view(
-        self,
-        name: str,
-        obj: ir.Table,
-        *,
-        database: str | None = None,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        import sqlalchemy_views as sav
-
-        source = self.compile(obj)
-        view = sav.CreateView(
-            sa.Table(
-                name,
-                sa.MetaData(),
-                schema=database,
-                quote=self.compiler.translator_class._quote_table_names,
-            ),
-            source,
-            or_replace=overwrite,
-        )
-        with self.begin() as con:
-            con.execute(view)
-        return self.table(name, database=database)
-
-    def drop_view(
-        self, name: str, *, database: str | None = None, force: bool = False
-    ) -> None:
-        import sqlalchemy_views as sav
-
-        view = sav.DropView(
-            sa.Table(
-                name,
-                sa.MetaData(),
-                schema=database,
-                quote=self.compiler.translator_class._quote_table_names,
-            ),
-            if_exists=not force,
-        )
+            sa_func = sa.union_all
+
+        left_set = context.get_compiled_expr(self.left)
+        right_set = context.get_compiled_expr(self.right)
+
+        return sa_func(left_set, right_set)
+
+
+class AlchemyProxy(object):
+    """
+    Wraps a SQLAlchemy ResultProxy and ensures that .close() is called on
+    garbage collection
+    """
+    def __init__(self, proxy):
+        self.proxy = proxy
+
+    def __del__(self):
+        self._close_cursor()
+
+    def _close_cursor(self):
+        self.proxy.close()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type, value, tb):
+        self._close_cursor()
+
+    def fetchall(self):
+        return self.proxy.fetchall()
+
+
+@rewrites(ops.NullIfZero)
+def _nullifzero(expr):
+    arg = expr.op().args[0]
+    return (arg == 0).ifelse(ibis.NA, arg)
+
+
+@compiles(ops.Divide)
+def _true_divide(t, expr):
+    op = expr.op()
+    left, right = op.args
+
+    if util.all_of(op.args, ir.IntegerValue):
+        new_expr = left.div(right.cast('double'))
+        return t.translate(new_expr)
+
+    return fixed_arity(lambda x, y: x / y, 2)(t, expr)
+
+
+@compiles(ops.FloorDivide)
+def _floor_divide(t, expr):
+    op = expr.op()
+    left, right = op.args
+
+    if util.any_of(op.args, ir.FloatingValue):
+        new_expr = expr.floor()
+        return t.translate(new_expr)
 
-        with self.begin() as con:
-            con.execute(view)
+    return fixed_arity(lambda x, y: x / y, 2)(t, expr)
```

### Comparing `ibis_framework-5.1.0/ibis/backends/base/sql/compiler/base.py` & `ibis-framework-v0.6.0/ibis/sql/transforms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,131 @@
-from __future__ import annotations
+# Copyright 2015 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import abc
-from itertools import chain
 
-import toolz
-
-import ibis.expr.analysis as an
+import ibis.expr.analysis as L
 import ibis.expr.operations as ops
-from ibis import util
+import ibis.expr.types as ir
+import ibis.util as util
 
 
-class DML(abc.ABC):
-    @abc.abstractmethod
-    def compile(self):
-        pass
+class ExistsExpr(ir.AnalyticExpr):
 
+    def type(self):
+        return 'exists'
 
-class DDL(abc.ABC):
-    @abc.abstractmethod
-    def compile(self):
-        pass
 
+class ExistsSubquery(ir.Node):
 
-class QueryAST:
-    __slots__ = 'context', 'dml', 'setup_queries', 'teardown_queries'
+    """
+    Helper class
+    """
 
-    def __init__(self, context, dml, setup_queries=None, teardown_queries=None):
-        self.context = context
-        self.dml = dml
-        self.setup_queries = setup_queries
-        self.teardown_queries = teardown_queries
-
-    @property
-    def queries(self):
-        return [self.dml]
-
-    def compile(self):
-        compiled_setup_queries = [q.compile() for q in self.setup_queries]
-        compiled_queries = [q.compile() for q in self.queries]
-        compiled_teardown_queries = [q.compile() for q in self.teardown_queries]
-        return self.context.collapse(
-            list(
-                chain(
-                    compiled_setup_queries,
-                    compiled_queries,
-                    compiled_teardown_queries,
-                )
-            )
-        )
-
-
-class SetOp(DML):
-    def __init__(self, tables, node, context, distincts):
-        assert isinstance(node, ops.Node)
-        assert all(isinstance(table, ops.Node) for table in tables)
+    def __init__(self, foreign_table, predicates):
+        self.foreign_table = foreign_table
+        self.predicates = predicates
+        ir.Node.__init__(self, [foreign_table, predicates])
+
+    def output_type(self):
+        return ExistsExpr
+
+
+class NotExistsSubquery(ir.Node):
+
+    def __init__(self, foreign_table, predicates):
+        self.foreign_table = foreign_table
+        self.predicates = predicates
+        ir.Node.__init__(self, [foreign_table, predicates])
+
+    def output_type(self):
+        return ExistsExpr
+
+
+class AnyToExistsTransform(object):
+
+    """
+    Some code duplication with the correlated ref check; should investigate
+    better code reuse.
+    """
+
+    def __init__(self, context, expr, parent_table):
         self.context = context
-        self.tables = tables
-        self.table_set = node
-        self.distincts = distincts
-        self.filters = []
-
-    @classmethod
-    def keyword(cls, distinct):
-        return cls._keyword + (not distinct) * " ALL"
-
-    def _get_keyword_list(self):
-        return map(self.keyword, self.distincts)
-
-    def _extract_subqueries(self):
-        # extract any subquery to avoid generating incorrect sql when at least
-        # one of the set operands is invalid outside of being a subquery
-        #
-        # for example: SELECT * FROM t ORDER BY x UNION ...
-        self.subqueries = an.find_subqueries(
-            [self.table_set, *self.filters], min_dependents=1
-        )
-        for subquery in self.subqueries:
-            self.context.set_extracted(subquery)
-
-    def format_subqueries(self):
-        context = self.context
-        subqueries = self.subqueries
-
-        return ',\n'.join(
-            '{} AS (\n{}\n)'.format(
-                context.get_ref(expr),
-                util.indent(context.get_compiled_expr(expr), 2),
-            )
-            for expr in subqueries
-        )
-
-    def format_relation(self, expr):
-        ref = self.context.get_ref(expr)
-        if ref is not None:
-            return f'SELECT *\nFROM {ref}'
-        return self.context.get_compiled_expr(expr)
-
-    def compile(self):
-        self._extract_subqueries()
-
-        extracted = self.format_subqueries()
-
-        buf = []
-
-        if extracted:
-            buf.append(f'WITH {extracted}')
-
-        buf.extend(
-            toolz.interleave(
-                (
-                    map(self.format_relation, self.tables),
-                    self._get_keyword_list(),
-                )
-            )
-        )
-        return '\n'.join(buf)
+        self.expr = expr
+        self.parent_table = parent_table
+
+        qroots = self.parent_table._root_tables()
+        self.query_roots = util.IbisSet.from_list(qroots)
+
+    def get_result(self):
+        self.foreign_table = None
+        self.predicates = []
+
+        self._visit(self.expr)
+
+        if type(self.expr.op()) == ops.Any:
+            op = ExistsSubquery(self.foreign_table, self.predicates)
+        else:
+            op = NotExistsSubquery(self.foreign_table, self.predicates)
+
+        return ir.BooleanArray(op)
+
+    def _visit(self, expr):
+        node = expr.op()
+
+        for arg in node.flat_args():
+            if isinstance(arg, ir.TableExpr):
+                self._visit_table(arg)
+            elif isinstance(arg, ir.BooleanArray):
+                for sub_expr in L.unwrap_ands(arg):
+                    self.predicates.append(sub_expr)
+                    self._visit(sub_expr)
+            elif isinstance(arg, ir.Expr):
+                self._visit(arg)
+            else:
+                continue
+
+    def _visit_table(self, expr):
+        node = expr.op()
+
+        if isinstance(expr, ir.TableExpr):
+            base_table = _find_blocking_table(expr)
+            if base_table is not None:
+                base_node = base_table.op()
+                if self._is_root(base_node):
+                    pass
+                else:
+                    # Foreign ref
+                    self.foreign_table = expr
+        else:
+            if not isinstance(node, ir.BlockingTableNode):
+                for arg in node.flat_args():
+                    if isinstance(arg, ir.Expr):
+                        self._visit(arg)
+
+    def _is_root(self, what):
+        if isinstance(what, ir.Expr):
+            what = what.op()
+        return what in self.query_roots
+
+
+def _find_blocking_table(expr):
+    node = expr.op()
+
+    if isinstance(node, ir.BlockingTableNode):
+        return expr
+
+    for arg in node.flat_args():
+        if isinstance(arg, ir.Expr):
+            result = _find_blocking_table(arg)
+            if result is not None:
+                return result
```

### Comparing `ibis_framework-5.1.0/ibis/backends/base/sql/compiler/select_builder.py` & `ibis-framework-v0.6.0/ibis/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,361 +1,471 @@
-from __future__ import annotations
-
-import functools
-from collections.abc import Mapping
-from typing import NamedTuple
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from ibis.compat import zip as czip
+from ibis.config import options
+import ibis.expr.types as ir
+import ibis.expr.operations as ops
+import ibis.sql.compiler as comp
+import ibis.common as com
+import ibis.util as util
 
-import toolz
 
-import ibis.common.exceptions as com
-import ibis.expr.analysis as an
-import ibis.expr.datatypes as dt
-import ibis.expr.operations as ops
+class Client(object):
 
+    pass
 
-class _LimitSpec(NamedTuple):
-    n: int
-    offset: int
 
+class Query(object):
 
-def _get_scalar(field):
-    def scalar_handler(results):
-        return results[field][0]
+    """
+    Abstraction for DDL query execution to enable both synchronous and
+    asynchronous queries, progress, cancellation and more (for backends
+    supporting such functionality).
+    """
 
-    return scalar_handler
+    def __init__(self, client, ddl):
+        self.client = client
 
+        if isinstance(ddl, comp.DDL):
+            self.compiled_ddl = ddl.compile()
+        else:
+            self.compiled_ddl = ddl
 
-def _get_column(name):
-    def column_handler(results):
-        return results[name]
+        self.result_wrapper = getattr(ddl, 'result_handler', None)
 
-    return column_handler
+    def execute(self):
+        # synchronous by default
+        with self.client._execute(self.compiled_ddl, results=True) as cur:
+            result = self._fetch(cur)
+
+        return self._wrap_result(result)
+
+    def _wrap_result(self, result):
+        if self.result_wrapper is not None:
+            result = self.result_wrapper(result)
+        return result
+
+    def _fetch(self, cursor):
+        import pandas as pd
+        rows = cursor.fetchall()
+        # TODO(wesm): please evaluate/reimpl to optimize for perf/memory
+        dtypes = [self._db_type_to_dtype(x[1]) for x in cursor.description]
+        names = [x[0] for x in cursor.description]
+        cols = {}
+        for (col, name, dtype) in czip(czip(*rows), names, dtypes):
+            try:
+                cols[name] = pd.Series(col, dtype=dtype)
+            except TypeError:
+                # coercing to specified dtype failed, e.g. NULL vals in int col
+                cols[name] = pd.Series(col)
+        return pd.DataFrame(cols, columns=names)
 
+    def _db_type_to_dtype(self, db_type):
+        raise NotImplementedError
 
-class SelectBuilder:
-    """Transforms expression IR to a query pipeline.
 
-    There will typically be a primary SELECT query, perhaps with some
-    subqueries and other DDL to ingest and tear down intermediate data sources.
+class AsyncQuery(Query):
 
-    Walks the expression tree and catalogues distinct query units,
-    builds select statements (and other DDL types, where necessary), and
-    records relevant query unit aliases to be used when actually
-    generating SQL.
+    """
+    Abstract asynchronous query
     """
 
-    def to_select(
-        self,
-        select_class,
-        table_set_formatter_class,
-        node,
-        context,
-        translator_class,
-    ):
-        self.select_class = select_class
-        self.table_set_formatter_class = table_set_formatter_class
-        self.context = context
-        self.translator_class = translator_class
-
-        self.op, self.result_handler = self._adapt_operation(node)
-        assert isinstance(self.op, ops.Node), type(self.op)
-
-        self.table_set = None
-        self.select_set = None
-        self.group_by = None
-        self.having = None
-        self.filters = []
-        self.limit = None
-        self.order_by = []
-        self.subqueries = []
-        self.distinct = False
-
-        select_query = self._build_result_query()
-
-        self.queries = [select_query]
-
-        return select_query
-
-    @staticmethod
-    def _adapt_operation(node):
-        # Non-table expressions need to be adapted to some well-formed table
-        # expression, along with a way to adapt the results to the desired
-        # arity (whether array-like or scalar, for example)
-        #
-        # Canonical case is scalar values or arrays produced by some reductions
-        # (simple reductions, or distinct, say)
-        if isinstance(node, ops.TableNode):
-            return node, toolz.identity
-
-        elif isinstance(node, ops.Value):
-            if node.output_shape.is_scalar():
-                if an.is_scalar_reduction(node):
-                    table_expr = an.reduction_to_aggregation(node)
-                    return table_expr.op(), _get_scalar(node.name)
-                else:
-                    return node, _get_scalar(node.name)
-            elif node.output_shape.is_columnar():
-                if isinstance(node, ops.TableColumn):
-                    table_expr = node.table.to_expr()[[node.name]]
-                    result_handler = _get_column(node.name)
-                else:
-                    table_expr = node.to_expr().as_table()
-                    result_handler = _get_column(node.name)
-
-                return table_expr.op(), result_handler
-            else:
-                raise com.TranslationError(f"Unexpected shape {node.output_shape}")
-        else:
-            raise com.TranslationError(f'Do not know how to execute: {type(node)}')
+    def execute(self):
+        raise NotImplementedError
 
-    def _build_result_query(self):
-        self._collect_elements()
-        self._analyze_subqueries()
-        self._populate_context()
-
-        return self.select_class(
-            self.table_set,
-            list(self.select_set),
-            translator_class=self.translator_class,
-            table_set_formatter_class=self.table_set_formatter_class,
-            context=self.context,
-            subqueries=self.subqueries,
-            where=self.filters,
-            group_by=self.group_by,
-            having=self.having,
-            limit=self.limit,
-            order_by=self.order_by,
-            distinct=self.distinct,
-            result_handler=self.result_handler,
-            parent_op=self.op,
-        )
-
-    def _populate_context(self):
-        # Populate aliases for the distinct relations used to output this
-        # select statement.
-        if self.table_set is not None:
-            self._make_table_aliases(self.table_set)
-
-    # TODO(kszucs): should be rewritten using lin.traverse()
-    def _make_table_aliases(self, node):
-        ctx = self.context
-
-        if isinstance(node, ops.Join):
-            for arg in node.args:
-                if isinstance(arg, ops.TableNode):
-                    self._make_table_aliases(arg)
-        elif not ctx.is_extracted(node):
-            ctx.make_alias(node)
+    def is_finished(self):
+        raise NotImplementedError
+
+    def cancel(self):
+        raise NotImplementedError
+
+    def get_result(self):
+        raise NotImplementedError
+
+
+class SQLClient(Client):
+
+    sync_query = Query
+    async_query = Query
+
+    def table(self, name, database=None):
+        """
+        Create a table expression that references a particular table in the
+        database
+
+        Parameters
+        ----------
+        name : string
+        database : string, optional
+
+        Returns
+        -------
+        table : TableExpr
+        """
+        qualified_name = self._fully_qualified_name(name, database)
+        schema = self._get_table_schema(qualified_name)
+        node = ops.DatabaseTable(qualified_name, schema, self)
+        return self._table_expr_klass(node)
+
+    @property
+    def _table_expr_klass(self):
+        return ir.TableExpr
+
+    @property
+    def current_database(self):
+        return self.con.database
+
+    def database(self, name=None):
+        """
+        Create a Database object for a given database name that can be used for
+        exploring and manipulating the objects (tables, functions, views, etc.)
+        inside
+
+        Parameters
+        ----------
+        name : string
+          Name of database
+
+        Returns
+        -------
+        database : Database
+        """
+        # TODO: validate existence of database
+        if name is None:
+            name = self.current_database
+        return self.database_class(name, self)
+
+    def _fully_qualified_name(self, name, database):
+        # XXX
+        return name
+
+    def _execute(self, query, results=False):
+        cur = self.con.execute(query)
+        if results:
+            return cur
         else:
-            # The compiler will apply a prefix only if the current context
-            # contains two or more table references. So, if we've extracted
-            # a subquery into a CTE, we need to propagate that reference
-            # down to child contexts so that they aren't missing any refs.
-            ctx.set_ref(node, ctx.top_context.get_ref(node))
-
-    # ---------------------------------------------------------------------
-    # Analysis of table set
-
-    def _collect_elements(self):
-        # If expr is a Value, we must seek out the Tables that it
-        # references, build their ASTs, and mark them in our QueryContext
-
-        # For now, we need to make the simplifying assumption that a value
-        # expression that is being translated only depends on a single table
-        # expression.
-
-        if isinstance(self.op, ops.TableNode):
-            self._collect(self.op, toplevel=True)
-            assert self.table_set is not None
+            cur.release()
+
+    def sql(self, query):
+        """
+        Convert a SQL query to an Ibis table expression
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        table : TableExpr
+        """
+        # Get the schema by adding a LIMIT 0 on to the end of the query. If
+        # there is already a limit in the query, we find and remove it
+        limited_query = """\
+SELECT *
+FROM (
+{0}
+) t0
+LIMIT 0""".format(query)
+        schema = self._get_schema_using_query(limited_query)
+
+        node = ops.SQLQueryResult(query, schema, self)
+        return ir.TableExpr(node)
+
+    def raw_sql(self, query, results=False):
+        """
+        Execute a given query string. Could have unexpected results if the
+        query modifies the behavior of the session in a way unknown to Ibis; be
+        careful.
+
+        Parameters
+        ----------
+        query : string
+          SQL or DDL statement
+        results : boolean, default False
+          Pass True if the query as a result set
+
+        Returns
+        -------
+        cur : ImpalaCursor if results=True, None otherwise
+          You must call cur.release() after you are finished using the cursor.
+        """
+        return self._execute(query, results=results)
+
+    def execute(self, expr, params=None, limit='default', async=False):
+        """
+        Compile and execute Ibis expression using this backend client
+        interface, returning results in-memory in the appropriate object type
+
+        Parameters
+        ----------
+        expr : Expr
+        limit : int, default None
+          For expressions yielding result yets; retrieve at most this number of
+          values/rows. Overrides any limit already set on the expression.
+        params : not yet implemented
+        async : boolean, default False
+
+        Returns
+        -------
+        output : input type dependent
+          Table expressions: pandas.DataFrame
+          Array expressions: pandas.Series
+          Scalar expressions: Python scalar value
+        """
+        ast = self._build_ast_ensure_limit(expr, limit)
+
+        if len(ast.queries) > 1:
+            raise NotImplementedError
         else:
-            self.select_set = [self.op]
+            return self._execute_query(ast.queries[0], async=async)
 
-    def _collect(self, op, toplevel=False):
-        method = f'_collect_{type(op).__name__}'
+    def _execute_query(self, ddl, async=False):
+        klass = self.async_query if async else self.sync_query
+        return klass(self, ddl).execute()
+
+    def compile(self, expr, params=None, limit=None):
+        """
+        Translate expression to one or more queries according to backend target
+
+        Returns
+        -------
+        output : single query or list of queries
+        """
+        ast = self._build_ast_ensure_limit(expr, limit)
+        queries = [query.compile() for query in ast.queries]
+        return queries[0] if len(queries) == 1 else queries
+
+    def _build_ast_ensure_limit(self, expr, limit):
+        ast = self._build_ast(expr)
+        # note: limit can still be None at this point, if the global
+        # default_limit is None
+        for query in reversed(ast.queries):
+            if (isinstance(query, comp.Select) and
+                    not isinstance(expr, ir.ScalarExpr) and
+                    query.table_set is not None):
+                if query.limit is None:
+                    if limit == 'default':
+                        query_limit = options.sql.default_limit
+                    else:
+                        query_limit = limit
+                    if query_limit:
+                        query.limit = {
+                            'n': query_limit,
+                            'offset': 0
+                        }
+                elif limit is not None and limit != 'default':
+                    query.limit = {'n': limit,
+                                   'offset': query.limit['offset']}
+        return ast
+
+    def explain(self, expr):
+        """
+        Query for and return the query plan associated with the indicated
+        expression or SQL query.
+
+        Returns
+        -------
+        plan : string
+        """
+        if isinstance(expr, ir.Expr):
+            ast = self._build_ast(expr)
+            if len(ast.queries) > 1:
+                raise Exception('Multi-query expression')
 
-        if hasattr(self, method):
-            f = getattr(self, method)
-            f(op, toplevel=toplevel)
-        elif isinstance(op, (ops.PhysicalTable, ops.SQLQueryResult)):
-            self._collect_PhysicalTable(op, toplevel=toplevel)
-        elif isinstance(op, ops.Join):
-            self._collect_Join(op, toplevel=toplevel)
+            query = ast.queries[0].compile()
         else:
-            raise NotImplementedError(type(op))
+            query = expr
+
+        statement = 'EXPLAIN {0}'.format(query)
+
+        with self._execute(statement, results=True) as cur:
+            result = self._get_list(cur)
+
+        return 'Query:\n{0}\n\n{1}'.format(util.indent(query, 2),
+                                           '\n'.join(result))
+
+    def _build_ast(self, expr):
+        # Implement in clients
+        raise NotImplementedError
+
+
+class QueryPipeline(object):
+    """
+    Execute a series of queries, possibly asynchronously, and capture any
+    result sets generated
+
+    Note: No query pipelines have yet been implemented
+    """
+    pass
+
+
+def execute(expr, limit='default', async=False):
+    backend = find_backend(expr)
+    return backend.execute(expr, limit=limit, async=async)
+
+
+def compile(expr, limit=None):
+    backend = find_backend(expr)
+    return backend.compile(expr, limit=limit)
+
+
+def find_backend(expr):
+    backends = []
+
+    def walk(expr):
+        node = expr.op()
+        for arg in node.flat_args():
+            if isinstance(arg, Client):
+                backends.append(arg)
+            elif isinstance(arg, ir.Expr):
+                walk(arg)
+
+    walk(expr)
+    backends = util.unique_by_key(backends, id)
+
+    if len(backends) > 1:
+        raise ValueError('Multiple backends found')
+    elif len(backends) == 0:
+        default = options.default_backend
+        if default is None:
+            raise com.IbisError('Expression depends on no backends, '
+                                'and found no default')
+        return default
+
+    return backends[0]
 
-    def _collect_Distinct(self, op, toplevel=False):
-        if toplevel:
-            self.distinct = True
-
-        self._collect(op.table, toplevel=toplevel)
-
-    def _collect_DropNa(self, op, toplevel=False):
-        if toplevel:
-            if op.subset is None:
-                columns = [
-                    ops.TableColumn(op.table, name) for name in op.table.schema.names
-                ]
-            else:
-                columns = op.subset
-            if columns:
-                filters = [
-                    functools.reduce(
-                        ops.And if op.how == "any" else ops.Or,
-                        [ops.NotNull(c) for c in columns],
-                    )
-                ]
-            elif op.how == "all":
-                filters = [ops.Literal(False, dtype=dt.bool)]
-            else:
-                filters = []
-            self.table_set = op.table
-            self.select_set = [op.table]
-            self.filters = filters
-
-    def _collect_FillNa(self, op, toplevel=False):
-        if toplevel:
-            table = op.table.to_expr()
-            if isinstance(op.replacements, Mapping):
-                mapping = op.replacements
-            else:
-                mapping = {
-                    name: op.replacements
-                    for name, type in table.schema().items()
-                    if type.nullable
-                }
-            new_op = table.mutate(
-                [
-                    table[name].fillna(value).name(name)
-                    for name, value in mapping.items()
-                ]
-            ).op()
-            self._collect(new_op, toplevel=toplevel)
-
-    def _collect_Limit(self, op, toplevel=False):
-        if not toplevel:
-            return
 
-        n = op.n
-        offset = op.offset or 0
+class Database(object):
 
-        if self.limit is None:
-            self.limit = _LimitSpec(n, offset)
+    def __init__(self, name, client):
+        self.name = name
+        self.client = client
+
+    def __repr__(self):
+        return "{0}('{1}')".format('Database', self.name)
+
+    def __dir__(self):
+        attrs = dir(type(self))
+        unqualified_tables = [self._unqualify(x) for x in self.tables]
+        return list(sorted(set(attrs + unqualified_tables)))
+
+    def __contains__(self, key):
+        return key in self.tables
+
+    @property
+    def tables(self):
+        return self.list_tables()
+
+    def __getitem__(self, key):
+        return self.table(key)
+
+    def __getattr__(self, key):
+        special_attrs = ['_ipython_display_', 'trait_names',
+                         '_getAttributeNames']
+
+        try:
+            return object.__getattribute__(self, key)
+        except AttributeError:
+            if key in special_attrs:
+                raise
+            return self.table(key)
+
+    def _qualify(self, value):
+        return value
+
+    def _unqualify(self, value):
+        return value
+
+    def drop(self, force=False):
+        """
+        Drop the database
+
+        Parameters
+        ----------
+        drop : boolean, default False
+          Drop any objects if they exist, and do not fail if the databaes does
+          not exist
+        """
+        self.client.drop_database(self.name, force=force)
+
+    def namespace(self, ns):
+        """
+        Creates a derived Database instance for collections of objects having a
+        common prefix. For example, for tables fooa, foob, and fooc, creating
+        the "foo" namespace would enable you to reference those objects as a,
+        b, and c, respectively.
+
+        Returns
+        -------
+        ns : DatabaseNamespace
+        """
+        return DatabaseNamespace(self, ns)
+
+    def table(self, name):
+        """
+        Return a table expression referencing a table in this database
+
+        Returns
+        -------
+        table : TableExpr
+        """
+        qualified_name = self._qualify(name)
+        return self.client.table(qualified_name, self.name)
+
+    def list_tables(self, like=None):
+        return self.client.list_tables(like=self._qualify_like(like),
+                                       database=self.name)
+
+    def _qualify_like(self, like):
+        return like
+
+
+class DatabaseNamespace(Database):
+
+    def __init__(self, parent, namespace):
+        self.parent = parent
+        self.namespace = namespace
+
+    def __repr__(self):
+        return ("{0}(database={1!r}, namespace={2!r})"
+                .format('DatabaseNamespace', self.name, self.namespace))
+
+    @property
+    def client(self):
+        return self.parent.client
+
+    @property
+    def name(self):
+        return self.parent.name
+
+    def _qualify(self, value):
+        return self.namespace + value
+
+    def _unqualify(self, value):
+        return value.replace(self.namespace, '', 1)
+
+    def _qualify_like(self, like):
+        if like:
+            return self.namespace + like
         else:
-            self.limit = _LimitSpec(
-                min(n, self.limit.n),
-                offset + self.limit.offset,
-            )
-
-        self._collect(op.table, toplevel=toplevel)
-
-    def _collect_Union(self, op, toplevel=False):
-        if toplevel:
-            self.table_set = op
-            self.select_set = [op]
-
-    def _collect_Difference(self, op, toplevel=False):
-        if toplevel:
-            self.table_set = op
-            self.select_set = [op]
-
-    def _collect_Intersection(self, op, toplevel=False):
-        if toplevel:
-            self.table_set = op
-            self.select_set = [op]
-
-    def _collect_Aggregation(self, op, toplevel=False):
-        # The select set includes the grouping keys (if any), and these are
-        # duplicated in the group_by set. SQL translator can decide how to
-        # format these depending on the database. Most likely the
-        # GROUP BY 1, 2, ... style
-        if toplevel:
-            sub_op = an.substitute_parents(op)
-
-            self.group_by = self._convert_group_by(sub_op.by)
-            self.having = sub_op.having
-            self.select_set = sub_op.by + sub_op.metrics
-            self.table_set = sub_op.table
-            self.filters = sub_op.predicates
-            self.order_by = sub_op.sort_keys
-
-            self._collect(op.table)
-
-    def _collect_Selection(self, op, toplevel=False):
-        table = op.table
-
-        if toplevel:
-            if isinstance(table, ops.Join):
-                self._collect_Join(table)
-            else:
-                self._collect(table)
-
-            selections = op.selections
-            sort_keys = op.sort_keys
-            filters = op.predicates
-
-            if not selections:
-                # select *
-                selections = [table]
-
-            self.order_by = sort_keys
-            self.select_set = selections
-            self.table_set = table
-            self.filters = filters
-
-    def _collect_InMemoryTable(self, node, toplevel=False):
-        if toplevel:
-            self.select_set = [node]
-            self.table_set = node
-
-    def _convert_group_by(self, nodes):
-        return list(range(len(nodes)))
-
-    def _collect_Join(self, op, toplevel=False):
-        if toplevel:
-            subbed = an.substitute_parents(op)
-            self.table_set = subbed
-            self.select_set = [subbed]
-
-    def _collect_PhysicalTable(self, op, toplevel=False):
-        if toplevel:
-            self.select_set = [op]
-            self.table_set = op
-
-    def _collect_SelfReference(self, op, toplevel=False):
-        if toplevel:
-            self._collect(op.table, toplevel=toplevel)
-
-    # --------------------------------------------------------------------
-    # Subquery analysis / extraction
-
-    def _analyze_subqueries(self):
-        # Somewhat temporary place for this. A little bit tricky, because
-        # subqueries can be found in many places
-        # - With the table set
-        # - Inside the where clause (these may be able to place directly, some
-        #   cases not)
-        # - As support queries inside certain expressions (possibly needing to
-        #   be extracted and joined into the table set where they are
-        #   used). More complex transformations should probably not occur here,
-        #   though.
-        #
-        # Duplicate subqueries might appear in different parts of the query
-        # structure, e.g. beneath two aggregates that are joined together, so
-        # we have to walk the entire query structure.
-        #
-        # The default behavior is to only extract into a WITH clause when a
-        # subquery appears multiple times (for DRY reasons). At some point we
-        # can implement a more aggressive policy so that subqueries always
-        # appear in the WITH part of the SELECT statement, if that's what you
-        # want.
-
-        # Find the subqueries, and record them in the passed query context.
-        subqueries = an.find_subqueries(
-            [self.table_set, *self.filters], min_dependents=2
-        )
-
-        self.subqueries = []
-        for node in subqueries:
-            # See #173. Might have been extracted already in a parent context.
-            if not self.context.is_extracted(node):
-                self.subqueries.append(node)
-                self.context.set_extracted(node)
+            return '{0}*'.format(self.namespace)
+
+
+class DatabaseEntity(object):
+    pass
+
+
+class View(DatabaseEntity):
+
+    def drop(self):
+        pass
```

### Comparing `ibis_framework-5.1.0/ibis/backends/base/sql/registry/identifiers.py` & `ibis-framework-v0.6.0/ibis/impala/identifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from __future__ import annotations
-
 # Copyright 2014 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Base identifiers
+# Impala identifiers
 
-base_identifiers = [
+impala_identifiers = [
     'add',
     'aggregate',
     'all',
     'alter',
     'and',
     'api_version',
     'as',
@@ -157,9 +155,9 @@
     'update_fn',
     'use',
     'using',
     'values',
     'view',
     'when',
     'where',
-    'with',
+    'with'
 ]
```

### Comparing `ibis_framework-5.1.0/ibis/backends/datafusion/__init__.py` & `ibis-framework-v0.6.0/ibis/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,292 +1,330 @@
-from __future__ import annotations
-
-import re
-from functools import lru_cache
-from pathlib import Path
-from typing import Any, Mapping
-
-import pyarrow as pa
-
-import ibis.common.exceptions as com
-import ibis.expr.analysis as an
-import ibis.expr.operations as ops
-import ibis.expr.schema as sch
-import ibis.expr.types as ir
-from ibis.backends.base import BaseBackend
-from ibis.backends.datafusion.compiler import translate
-from ibis.util import gen_name, normalize_filename
-
-try:
-    from datafusion import ExecutionContext as SessionContext
-except ImportError:
-    from datafusion import SessionContext
-
-import datafusion
-
-
-class Backend(BaseBackend):
-    name = 'datafusion'
-    builder = None
-
-    @property
-    def version(self):
-        import importlib.metadata
-
-        return importlib.metadata.version("datafusion")
-
-    def do_connect(
-        self,
-        config: Mapping[str, str | Path] | SessionContext | None = None,
-    ) -> None:
-        """Create a Datafusion backend for use with Ibis.
-
-        Parameters
-        ----------
-        config
-            Mapping of table names to files.
-
-        Examples
-        --------
-        >>> import ibis
-        >>> config = {"t": "path/to/file.parquet", "s": "path/to/file.csv"}
-        >>> ibis.datafusion.connect(config)
-        """
-        if isinstance(config, SessionContext):
-            self._context = config
+# Daemon and worker server processes, heavily modified from PySpark (used as
+# permitted under the Apache License 2.0)
+#
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+
+import argparse
+import errno
+import numbers
+import os
+import select
+import signal
+import socket
+import struct
+import sys
+import time
+import threading
+import traceback
+
+
+from ibis.tasks import IbisTaskMessage, IbisTaskExecutor
+
+
+SELECT_TIMEOUT = 0.25
+
+
+def pack_uint32(val):
+    return struct.pack('I', val)
+
+
+class IbisTaskHandler(object):
+
+    def __init__(self, sock):
+        self.sock = sock
+
+    def run(self):
+        # TODO: task execution class should acquire OS semaphore, execute
+        # task, then release the semaphore.
+
+        encoded_task = self.sock.recv(1024)
+        if not encoded_task:
+            raise ValueError('Request was empty')
+
+        try:
+            task_msg = IbisTaskMessage.decode(encoded_task)
+        except:
+            self.sock.send(traceback.format_exc())
         else:
-            self._context = SessionContext()
+            # Acknowledge successful receipt
+            self.sock.send('ok')
+        finally:
+            self.sock.close()
 
-        config = config or {}
+        self.execute(task_msg)
 
-        for name, path in config.items():
-            self.register(path, table_name=name)
+    def execute(self, task_msg):
+        executor = IbisTaskExecutor(task_msg)
+        return executor.execute()
 
-    def current_database(self) -> str:
-        raise NotImplementedError()
-
-    def list_databases(self, like: str | None = None) -> list[str]:
-        raise NotImplementedError()
-
-    def list_tables(
-        self,
-        like: str | None = None,
-        database: str | None = None,
-    ) -> list[str]:
-        """List the available tables."""
-        tables = list(self._context.tables())
-        if like is not None:
-            pattern = re.compile(like)
-            return list(filter(lambda t: pattern.findall(t), tables))
-        return tables
-
-    def table(self, name: str, schema: sch.Schema | None = None) -> ir.Table:
-        """Get an ibis expression representing a DataFusion table.
-
-        Parameters
-        ----------
-        name
-            The name of the table to retreive
-        schema
-            An optional schema for the table
-
-        Returns
-        -------
-        Table
-            A table expression
-        """
-        catalog = self._context.catalog()
-        database = catalog.database('public')
-        table = database.table(name)
-        schema = sch.schema(table.schema)
-        return self.table_class(name, schema, self).to_expr()
-
-    def register(
-        self, source: str | Path, table_name: str | None = None, **kwargs: Any
-    ) -> ir.Table:
-        """Register a CSV or Parquet file with `table_name` located at `source`.
-
-        Parameters
-        ----------
-        source
-            The path to the file
-        table_name
-            The name of the table
-        kwargs
-            Datafusion-specific keyword arguments
-        """
-        if isinstance(source, (str, Path)):
-            first = str(source)
-        else:
-            raise ValueError("`source` must be either a string or a pathlib.Path")
 
-        if first.startswith(("parquet://", "parq://")) or first.endswith(
-            ("parq", "parquet")
-        ):
-            return self.read_parquet(source, table_name=table_name, **kwargs)
-        elif first.startswith(("csv://", "txt://")) or first.endswith(
-            ("csv", "tsv", "txt")
-        ):
-            return self.read_csv(source, table_name=table_name, **kwargs)
-        else:
-            self._register_failure()
-            return None
+def compute_real_exit_code(exit_code):
+    # SystemExit's code can be integer or string, but os._exit only accepts
+    # integers
+    if isinstance(exit_code, numbers.Integral):
+        return exit_code
+    else:
+        return 1
 
-    def _register_failure(self):
-        import inspect
 
-        msg = ", ".join(
-            m[0] for m in inspect.getmembers(self) if m[0].startswith("read_")
-        )
-        raise ValueError(
-            f"Cannot infer appropriate read function for input, "
-            f"please call one of {msg} directly"
-        )
-
-    def read_csv(
-        self, path: str | Path, table_name: str | None = None, **kwargs: Any
-    ) -> ir.Table:
-        """Register a CSV file as a table in the current database.
-
-        Parameters
-        ----------
-        path
-            The data source. A string or Path to the CSV file.
-        table_name
-            An optional name to use for the created table. This defaults to
-            a sequentially generated name.
-        **kwargs
-            Additional keyword arguments passed to Datafusion loading function.
-
-        Returns
-        -------
-        ir.Table
-            The just-registered table
-        """
-        path = normalize_filename(path)
-        table_name = table_name or gen_name("read_csv")
-        # Our other backends support overwriting views / tables when reregistering
-        self._context.deregister_table(table_name)
-        self._context.register_csv(table_name, path, **kwargs)
-        return self.table(table_name)
-
-    def read_parquet(
-        self, path: str | Path, table_name: str | None = None, **kwargs: Any
-    ) -> ir.Table:
-        """Register a parquet file as a table in the current database.
-
-        Parameters
-        ----------
-        path
-            The data source.
-        table_name
-            An optional name to use for the created table. This defaults to
-            a sequentially generated name.
-        **kwargs
-            Additional keyword arguments passed to Datafusion loading function.
-
-        Returns
-        -------
-        ir.Table
-            The just-registered table
-        """
-        path = normalize_filename(path)
-        table_name = table_name or gen_name("read_parquet")
-        # Our other backends support overwriting views / tables when reregistering
-        self._context.deregister_table(table_name)
-        self._context.register_parquet(table_name, path, **kwargs)
-        return self.table(table_name)
-
-    def _get_frame(
-        self,
-        expr: ir.Expr,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        **kwargs: Any,
-    ) -> datafusion.DataFrame:
-        if isinstance(expr, ir.Table):
-            return self.compile(expr, params, **kwargs)
-        elif isinstance(expr, ir.Column):
-            # expression must be named for the projection
-            expr = expr.name('tmp').as_table()
-            return self.compile(expr, params, **kwargs)
-        elif isinstance(expr, ir.Scalar):
-            if an.find_immediate_parent_tables(expr.op()):
-                # there are associated datafusion tables so convert the expr
-                # to a selection which we can directly convert to a datafusion
-                # plan
-                expr = expr.name('tmp').as_table()
-                frame = self.compile(expr, params, **kwargs)
-            else:
-                # doesn't have any tables associated so create a plan from a
-                # dummy datafusion table
-                compiled = self.compile(expr, params, **kwargs)
-                frame = self._context.empty_table().select(compiled)
-            return frame
-        else:
-            raise com.IbisError(f"Cannot execute expression of type: {type(expr)}")
+def _eintr_retry(func, *args):
+    """restart a system call interrupted by EINTR"""
+    while True:
+        try:
+            return func(*args)
+        except (OSError, select.error) as e:
+            if e.args[0] != errno.EINTR:
+                raise
+
+# ---------------------------------------------------------------------
+# Daemon logic for spawning new child workers
 
-    def to_pyarrow_batches(
-        self,
-        expr: ir.Expr,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        chunk_size: int = 1_000_000,
-        **kwargs: Any,
-    ) -> pa.ipc.RecordBatchReader:
-        pa = self._import_pyarrow()
-        frame = self._get_frame(expr, params, limit, **kwargs)
-        return pa.ipc.RecordBatchReader.from_batches(frame.schema(), frame.collect())
-
-    def execute(
-        self,
-        expr: ir.Expr,
-        params: Mapping[ir.Expr, object] = None,
-        limit: int | str | None = "default",
-        **kwargs: Any,
-    ):
-        output = self.to_pyarrow(expr, params=params, limit=limit, **kwargs)
-        if isinstance(expr, ir.Table):
-            return output.to_pandas()
-        elif isinstance(expr, ir.Column):
-            series = output.to_pandas()
-            series.name = expr.get_name()
-            return series
-        elif isinstance(expr, ir.Scalar):
-            return output.as_py()
+
+class IbisServerNode(object):
+
+    """
+    This can be a daemon (for launching subprocesses) or a worker
+    """
+
+    def __init__(self, server_port=17001, daemon=True,
+                 task_handler=IbisTaskHandler):
+        self.server_port = server_port
+        self.task_handler = task_handler
+
+        self.setup_server_socket()
+
+        # Can trigger shutdown to occur
+        self._shutdown_request = False
+        self._is_shutdown = threading.Event()
+        self._is_shutdown.clear()
+
+        self.is_daemon = daemon
+
+        self.threaded_worker = False
+
+        if self.is_daemon:
+            # Create a new process group to corral our children
+            os.setpgid(0, 0)
+            self.set_daemon_signal_handlers()
         else:
-            raise com.IbisError(f"Cannot execute expression of type: {type(expr)}")
+            self.set_worker_signal_handlers()
 
-    def compile(
-        self,
-        expr: ir.Expr,
-        params: Mapping[ir.Expr, object] = None,
-        **kwargs: Any,
-    ):
-        return translate(expr.op())
-
-    @classmethod
-    @lru_cache
-    def _get_operations(cls):
-        from ibis.backends.datafusion.compiler import translate
-
-        return frozenset(op for op in translate.registry if issubclass(op, ops.Value))
-
-    @classmethod
-    def has_operation(cls, operation: type[ops.Value]) -> bool:
-        op_classes = cls._get_operations()
-        return operation in op_classes or any(
-            issubclass(operation, op_impl) for op_impl in op_classes
-        )
-
-    def create_table(self, *_, **__) -> ir.Table:
-        raise NotImplementedError(self.name)
+    def set_daemon_signal_handlers(self):
+        # Gracefully exit on SIGTERM
+        signal.signal(signal.SIGTERM, self.handle_sigterm)
+
+        # Don't die on SIGHUP
+        signal.signal(signal.SIGHUP, signal.SIG_IGN)
+
+    def handle_sigterm(self, *args):
+        self.shutdown()
+
+    def sighup_worker(self, *args):
+        self._shutdown_request = True
+
+    def sigint_worker(self, *args):
+        # Terminate, with extreme prejudice
+        self.listen_sock.close()
+        self.shutdown()
+        sys.exit(0)
+
+    def set_worker_signal_handlers(self):
+        signal.signal(signal.SIGHUP, self.sighup_worker)
+        signal.signal(signal.SIGCHLD, signal.SIG_DFL)
+        signal.signal(signal.SIGTERM, signal.SIG_DFL)
+
+        # signal.signal(signal.SIGKILL, self.sigkill_worker)
+
+        # restore the handler for SIGINT,
+        # it's useful for debugging (show the stacktrace before exit)
+        signal.signal(signal.SIGINT, self.sigint_worker)
+
+    def shutdown(self):
+        # Do we actually need this? Cannot be called when run from a thread
+        # signal.signal(SIGTERM, SIG_DFL)
+
+        if self.is_daemon:
+            # Send SIGHUP to notify workers of shutdown
+            os.kill(0, signal.SIGHUP)
+        self._shutdown_request = True
+
+    def setup_server_socket(self):
+        # Bind the daemon socket listener
+        self.listen_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.listen_sock.bind(('127.0.0.1', 0))
+        self.listen_sock.listen(socket.SOMAXCONN)
+        _, self.listen_port = self.listen_sock.getsockname()
+
+    def report_daemon(self):
+        print('Running daemon at port %d' % self.listen_port)
+        self._server_send(pack_uint32(self.listen_port))
+
+    def report_worker_info(self):
+        print('Running worker at port %d' % self.listen_port)
+        # Port and process id (as uint32)
+        msg = struct.pack('II', self.listen_port, os.getpid())
+        self._server_send(msg)
+
+    def _server_send(self, msg):
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.connect(('localhost', self.server_port))
+        sock.send(msg)
+
+        data = sock.recv(1024)
+        if data != 'ok':
+            raise Exception('Server said: %s' % data)
+
+    def run_daemon(self):
+        self.report_daemon()
+
+        while True:
+            if self._shutdown_request:
+                # shutdown was called
+                self.listen_sock.close()
+                self._is_shutdown.set()
+                break
+
+            ready_fds = _eintr_retry(select.select, [self.listen_sock],
+                                     [], [], SELECT_TIMEOUT)[0]
+
+            # cleanup in signal handler will cause deadlock
+            self.cleanup_zombies()
+
+            if self.listen_sock not in ready_fds:
+                continue
+
+            sock, _ = _eintr_retry(self.listen_sock.accept)
+            msg = sock.recv(1024)
+
+            if msg == 'new':
+                try:
+                    fork_ind = os.fork()
+                except OSError as e:
+                    if e.errno in (errno.EAGAIN, errno.EINTR):
+                        time.sleep(1)
+                        fork_ind = os.fork()  # error here will shutdown daemon
+                    else:
+                        # Signal that the fork failed
+                        sock.send(pack_uint32(e.errno))
+                        sock.close()
+                        continue
+
+                # Fork succeeded
+                if fork_ind == 0:
+                    self.become_worker(sock)
+                else:
+                    # Daemon process
+                    sock.send('ok')
+                    sock.close()
+            elif msg == 'shutdown':
+                self.shutdown()
+                sock.send('ok')
+                sock.close()
+                continue
+            elif msg.startswith('kill'):
+                # e.g. kill 12345
+                worker_pid = int(msg[4:])
+                print('Killing %d' % worker_pid)
+                try:
+                    os.kill(worker_pid, signal.SIGINT)
+                except OSError:
+                    pass  # process already died
+                sock.send('ok')
+                sock.close()
+
+    def cleanup_zombies(self):
+        try:
+            while True:
+                pid, _ = os.waitpid(0, os.WNOHANG)
+                if not pid:
+                    break
+        except:
+            pass
 
-    def create_view(self, *_, **__) -> ir.Table:
-        raise NotImplementedError(self.name)
+    def become_worker(self, sock):
+        """
+        sock :
+        """
+        # in child process, close the server socket
+        self.listen_sock.close()
 
-    def drop_table(self, *_, **__) -> ir.Table:
-        raise NotImplementedError(self.name)
+        self.is_daemon = False
 
-    def drop_view(self, *_, **__) -> ir.Table:
-        raise NotImplementedError(self.name)
+        # Setup a new socket server on some available port
+        self.setup_server_socket()
+        self.set_worker_signal_handlers()
+        self.run_worker()
+
+    def run_worker(self):
+        self.report_worker_info()
+
+        while True:
+            if self._shutdown_request:
+                # Triggered by SIGHUP
+                self.listen_sock.close()
+                self._is_shutdown.set()
+                break
+
+            # Await instructions
+            ready_fds = _eintr_retry(select.select, [self.listen_sock],
+                                     [], [], SELECT_TIMEOUT)[0]
+            if not ready_fds:
+                continue
+
+            sock, _ = _eintr_retry(self.listen_sock.accept)
+
+            task = self.task_handler(sock)
+
+            if self.threaded_worker:
+                # Spawn task in a daemon. These threads should not stay alive
+                # if main worker thread exits. Revisit this at some point.
+                t = threading.Thread(target=task.run)
+                t.daemon = True
+                t.start()
+            else:
+                # Run the task synchronously
+                try:
+                    task.run()
+                except:
+                    # Exception reporting is the task's job
+                    pass
+
+
+def parse_cl_args():
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('-D', '--daemon', dest='is_daemon',
+                        default=True, action='store_true')
+
+    parser.add_argument('-p', '--port', type=int, dest='impala_port',
+                        default=17001, action='store')
+
+    return parser.parse_known_args()[0]
+
+
+if __name__ == '__main__':
+    args = parse_cl_args()
+
+    if args.is_daemon:
+        node = IbisServerNode(args.impala_port)
+        try:
+            node.run_daemon()
+        except SystemExit:
+            pass
+        except:
+            node.shutdown()
+            traceback.print_exc()
+    else:
+        raise NotImplementedError
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/__init__.py` & `ibis-framework-v0.6.0/ibis/expr/tests/test_table.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1347 +1,1122 @@
-"""Impala backend."""
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from ibis.expr.types import ArrayExpr, TableExpr, RelationError
+from ibis.common import ExpressionError
+from ibis.expr.datatypes import array_type
+import ibis.expr.api as api
+import ibis.expr.types as ir
+import ibis.expr.operations as ops
+import ibis
 
-from __future__ import annotations
+from ibis.compat import unittest
+from ibis.expr.tests.mocks import MockConnection, BasicTestCase
 
-import contextlib
-import io
-import operator
-import os
-import re
-import weakref
-from pathlib import Path
-from posixpath import join as pjoin
-from typing import TYPE_CHECKING, Any, Literal
-
-import fsspec
-import numpy as np
-
-import ibis.common.exceptions as com
-import ibis.config
-import ibis.expr.datatypes as dt
-import ibis.expr.rules as rlz
-import ibis.expr.schema as sch
-import ibis.expr.types as ir
-from ibis import util
-from ibis.backends.base.sql import BaseSQLBackend
-from ibis.backends.base.sql.ddl import (
-    CTAS,
-    CreateDatabase,
-    CreateTableWithSchema,
-    CreateView,
-    DropDatabase,
-    DropTable,
-    DropView,
-    TruncateTable,
-    fully_qualified_re,
-    is_fully_qualified,
-)
-from ibis.backends.impala import ddl, udf
-from ibis.backends.impala.client import ImpalaConnection, ImpalaDatabase, ImpalaTable
-from ibis.backends.impala.compat import HS2Error, ImpylaError
-from ibis.backends.impala.compiler import ImpalaCompiler
-from ibis.backends.impala.pandas_interop import DataFrameWriter
-from ibis.backends.impala.udf import (
-    aggregate_function,
-    scalar_function,
-    wrap_uda,
-    wrap_udf,
-)
-from ibis.config import options
-
-if TYPE_CHECKING:
-    import pandas as pd
-
-
-__all__ = (
-    "Backend",
-    "aggregate_function",
-    "scalar_function",
-    "wrap_uda",
-    "wrap_udf",
-)
-
-_HS2_TTypeId_to_dtype = {
-    'BOOLEAN': 'bool',
-    'TINYINT': 'int8',
-    'SMALLINT': 'int16',
-    'INT': 'int32',
-    'BIGINT': 'int64',
-    'TIMESTAMP': 'datetime64[ns]',
-    'FLOAT': 'float32',
-    'DOUBLE': 'float64',
-    'STRING': 'object',
-    'DECIMAL': 'object',
-    'BINARY': 'object',
-    'VARCHAR': 'object',
-    'CHAR': 'object',
-    'DATE': 'datetime64[ns]',
-    'VOID': None,
-}
-
-
-def _split_signature(x):
-    name, rest = x.split('(', 1)
-    return name, rest[:-1]
-
-
-_arg_type = re.compile(r'(.*)\.\.\.|([^\.]*)')
-
-
-class _type_parser:
-    NORMAL, IN_PAREN = 0, 1
-
-    def __init__(self, value):
-        self.value = value
-        self.state = self.NORMAL
-        self.buf = io.StringIO()
-        self.types = []
-        for c in value:
-            self._step(c)
-        self._push()
-
-    def _push(self):
-        val = self.buf.getvalue().strip()
-        if val:
-            self.types.append(val)
-        self.buf = io.StringIO()
-
-    def _step(self, c):
-        if self.state == self.NORMAL:
-            if c == '(':
-                self.state = self.IN_PAREN
-            elif c == ',':
-                self._push()
-                return
-        elif self.state == self.IN_PAREN:
-            if c == ')':
-                self.state = self.NORMAL
-        self.buf.write(c)
-
-
-def _chunks_to_pandas_array(chunks):
-    total_length = 0
-    have_nulls = False
-    for c in chunks:
-        total_length += len(c)
-        have_nulls = have_nulls or c.nulls.any()
-
-    type_ = chunks[0].data_type
-    numpy_type = _HS2_TTypeId_to_dtype[type_]
-
-    def fill_nonnull(target, chunks):
-        pos = 0
-        for c in chunks:
-            target[pos : pos + len(c)] = c.values
-            pos += len(c.values)
-
-    def fill(target, chunks, na_rep):
-        pos = 0
-        for c in chunks:
-            nulls = c.nulls.copy()
-            nulls.bytereverse()
-            bits = np.frombuffer(nulls.tobytes(), dtype='u1')
-            mask = np.unpackbits(bits).view(np.bool_)
-
-            k = len(c)
-
-            dest = target[pos : pos + k]
-            dest[:] = c.values
-            dest[mask[:k]] = na_rep
-
-            pos += k
-
-    if have_nulls:
-        if numpy_type in ('bool', 'datetime64[ns]'):
-            target = np.empty(total_length, dtype='O')
-            na_rep = np.nan
-        elif numpy_type.startswith('int'):
-            target = np.empty(total_length, dtype='f8')
-            na_rep = np.nan
-        else:
-            target = np.empty(total_length, dtype=numpy_type)
-            na_rep = np.nan
-
-        fill(target, chunks, na_rep)
-    else:
-        target = np.empty(total_length, dtype=numpy_type)
-        fill_nonnull(target, chunks)
-
-    return target
-
-
-def _column_batches_to_dataframe(names, batches):
-    import pandas as pd
-
-    cols = {}
-    for name, chunks in zip(names, zip(*(b.columns for b in batches))):
-        cols[name] = _chunks_to_pandas_array(chunks)
-    return pd.DataFrame(cols, columns=names)
-
-
-class Backend(BaseSQLBackend):
-    name = 'impala'
-    # not 100% accurate, but very close
-    _sqlglot_dialect = "hive"
-    database_class = ImpalaDatabase
-    table_expr_class = ImpalaTable
-    compiler = ImpalaCompiler
-
-    class Options(ibis.config.Config):
-        """Impala specific options.
-
-        Parameters
-        ----------
-        temp_db : str, default "__ibis_tmp"
-            Database to use for temporary objects.
-        temp_hdfs_path : str, default "/tmp/ibis"
-            HDFS path for storage of temporary data.
-        """
-
-        temp_db: str = "__ibis_tmp"
-        temp_hdfs_path: str = "/tmp/hdfs"
-
-    @staticmethod
-    def hdfs_connect(
-        *args: Any,
-        protocol: str = "webhdfs",
-        **kwargs: Any,
-    ) -> fsspec.spec.AbstractFileSystem:
-        return fsspec.filesystem(protocol, *args, **kwargs)
-
-    def do_connect(
-        self,
-        host: str = "localhost",
-        port: int = 21050,
-        database: str = "default",
-        timeout: int = 45,
-        use_ssl: bool = False,
-        ca_cert: str | Path | None = None,
-        user: str | None = None,
-        password: str | None = None,
-        auth_mechanism: Literal["NOSASL", "PLAIN", "GSSAPI", "LDAP"] = "NOSASL",
-        kerberos_service_name: str = "impala",
-        pool_size: int = 8,
-        hdfs_client: fsspec.spec.AbstractFileSystem | None = None,
-    ):
-        """Create an Impala Backend for use with Ibis.
-
-        Parameters
-        ----------
-        host
-            Host name of the impalad or HiveServer2 in Hive
-        port
-            Impala's HiveServer2 port
-        database
-            Default database when obtaining new cursors
-        timeout
-            Connection timeout in seconds when communicating with HiveServer2
-        use_ssl
-            Use SSL when connecting to HiveServer2
-        ca_cert
-            Local path to 3rd party CA certificate or copy of server
-            certificate for self-signed certificates. If SSL is enabled, but
-            this argument is ``None``, then certificate validation is skipped.
-        user
-            LDAP user to authenticate
-        password
-            LDAP password to authenticate
-        auth_mechanism
-            |   Value    | Meaning                        |
-            | :--------: | :----------------------------- |
-            | `'NOSASL'` | insecure Impala connections    |
-            | `'PLAIN'`  | insecure Hive clusters         |
-            |  `'LDAP'`  | LDAP authenticated connections |
-            | `'GSSAPI'` | Kerberos-secured clusters      |
-        kerberos_service_name
-            Specify a particular `impalad` service principal.
-        pool_size
-            Size of the connection pool. Typically this is not necessary to configure.
-        hdfs_client
-            An existing HDFS client.
-
-        Examples
-        --------
-        >>> import os
-        >>> import ibis
-        >>> hdfs_host = os.environ.get('IBIS_TEST_NN_HOST', 'localhost')
-        >>> hdfs_port = int(os.environ.get('IBIS_TEST_NN_PORT', 50070))
-        >>> impala_host = os.environ.get('IBIS_TEST_IMPALA_HOST', 'localhost')
-        >>> impala_port = int(os.environ.get('IBIS_TEST_IMPALA_PORT', 21050))
-        >>> hdfs = ibis.impala.hdfs_connect(host=hdfs_host, port=hdfs_port)
-        >>> client = ibis.impala.connect(
-        ...     host=impala_host,
-        ...     port=impala_port,
-        ...     hdfs_client=hdfs,
-        ... )
-        >>> client  # doctest: +ELLIPSIS
-        <ibis.backends.impala.Backend object at 0x...>
-        """
-        self._temp_objects = set()
-        self._hdfs = hdfs_client
-
-        params = {
-            'host': host,
-            'port': port,
-            'database': database,
-            'timeout': timeout,
-            'use_ssl': use_ssl,
-            'ca_cert': str(ca_cert),
-            'user': user,
-            'password': password,
-            'auth_mechanism': auth_mechanism,
-            'kerberos_service_name': kerberos_service_name,
+import ibis.common as com
+import ibis.config as config
+
+
+from ibis.tests.util import assert_equal
+
+
+class TestTableExprBasics(BasicTestCase, unittest.TestCase):
+
+    def test_empty_schema(self):
+        table = api.table([], 'foo')
+        assert len(table.schema()) == 0
+
+    def test_columns(self):
+        t = self.con.table('alltypes')
+        result = t.columns
+        expected = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i']
+        assert result == expected
+
+    def test_view_new_relation(self):
+        # For assisting with self-joins and other self-referential operations
+        # where we need to be able to treat instances of the same TableExpr as
+        # semantically distinct
+        #
+        # This thing is not exactly a projection, since it has no semantic
+        # meaning when it comes to execution
+        tview = self.table.view()
+
+        roots = tview._root_tables()
+        assert len(roots) == 1
+        assert roots[0] is tview.op()
+
+    def test_get_type(self):
+        for k, v in self.schema_dict.items():
+            assert self.table._get_type(k) == v
+
+    def test_getitem_column_select(self):
+        for k, v in self.schema_dict.items():
+            col = self.table[k]
+
+            # Make sure it's the right type
+            assert isinstance(col, ArrayExpr)
+            assert isinstance(col, array_type(v))
+
+            # Ensure we have a field selection with back-reference to the table
+            parent = col.parent()
+            assert isinstance(parent, ops.TableColumn)
+            assert parent.parent() is self.table
+
+    def test_getitem_attribute(self):
+        result = self.table.a
+        assert_equal(result, self.table['a'])
+
+        assert 'a' in dir(self.table)
+
+        # Project and add a name that conflicts with a TableExpr built-in
+        # attribute
+        view = self.table[[self.table, self.table['a'].name('schema')]]
+        assert not isinstance(view.schema, ArrayExpr)
+
+    def test_projection(self):
+        cols = ['f', 'a', 'h']
+
+        proj = self.table[cols]
+        assert isinstance(proj, TableExpr)
+        assert isinstance(proj.op(), ops.Projection)
+
+        assert proj.schema().names == cols
+        for c in cols:
+            expr = proj[c]
+            assert isinstance(expr, type(self.table[c]))
+
+    def test_projection_no_list(self):
+        expr = (self.table.f * 2).name('bar')
+        result = self.table.select(expr)
+        expected = self.table.projection([expr])
+        assert_equal(result, expected)
+
+    def test_projection_with_exprs(self):
+        # unnamed expr to test
+        mean_diff = (self.table['a'] - self.table['c']).mean()
+
+        col_exprs = [self.table['b'].log().name('log_b'),
+                     mean_diff.name('mean_diff')]
+
+        proj = self.table[col_exprs + ['g']]
+        schema = proj.schema()
+        assert schema.names == ['log_b', 'mean_diff', 'g']
+        assert schema.types == ['double', 'double', 'string']
+
+        # Test with unnamed expr
+        self.assertRaises(ExpressionError, self.table.projection,
+                          ['g', self.table['a'] - self.table['c']])
+
+    def test_projection_duplicate_names(self):
+        self.assertRaises(com.IntegrityError, self.table.projection,
+                          [self.table.c, self.table.c])
+
+    def test_projection_invalid_root(self):
+        schema1 = {
+            'foo': 'double',
+            'bar': 'int32'
         }
-        self.con = ImpalaConnection(pool_size=pool_size, **params)
 
-        self._ensure_temp_db_exists()
+        left = api.table(schema1, name='foo')
+        right = api.table(schema1, name='bar')
 
-    @property
-    def version(self):
-        cursor = self.raw_sql('select version()')
-        result = cursor.fetchone()[0]
-        cursor.release()
-        return result
-
-    def list_databases(self, like=None):
-        cur = self.raw_sql('SHOW DATABASES')
-        databases = self._get_list(cur)
-        cur.release()
-        return self._filter_with_like(databases, like)
-
-    def list_tables(self, like=None, database=None):
-        statement = 'SHOW TABLES'
-        if database is not None:
-            statement += f' IN {database}'
-        if like:
-            m = fully_qualified_re.match(like)
-            if m:
-                database, quoted, unquoted = m.groups()
-                like = quoted or unquoted
-                return self.list_tables(like=like, database=database)
-            statement += f" LIKE '{like}'"
-
-        return self._filter_with_like(
-            [row[0] for row in self.raw_sql(statement).fetchall()]
-        )
-
-    def fetch_from_cursor(self, cursor, schema):
-        batches = cursor.fetchall(columnar=True)
-        names = [x[0] for x in cursor.description]
-        df = _column_batches_to_dataframe(names, batches)
-        if schema:
-            return schema.apply_to(df)
-        return df
-
-    @property
-    def hdfs(self):
-        if self._hdfs is None:
-            raise com.IbisError(
-                'No HDFS connection; must pass connection '
-                'using the hdfs_client argument to '
-                'ibis.impala.connect'
-            )
-        return self._hdfs
-
-    @property
-    def kudu(self):
-        raise NotImplementedError(
-            "kudu support using kudu-python is no longer supported; "
-            "use impala facilities to manage kudu tables; "
-            "see https://kudu.apache.org/docs/kudu_impala_integration.html"
-        )
-
-    def close(self):
-        """Close the connection and drop temporary objects."""
-        while self._temp_objects:
-            finalizer = self._temp_objects.pop()
-            with contextlib.suppress(HS2Error):
-                finalizer()
-
-        self.con.close()
-
-    def disable_codegen(self, disabled=True):
-        """Turn off or on LLVM codegen in Impala query execution.
-
-        Parameters
-        ----------
-        disabled
-            To disable codegen, pass with no argument or True. To enable
-            codegen, pass False.
-        """
-        self.con.disable_codegen(disabled)
-
-    def _fully_qualified_name(self, name, database):
-        if is_fully_qualified(name):
-            return name
-
-        database = database or self.current_database
-        return f'{database}.`{name}`'
-
-    def _get_list(self, cur):
-        tuples = cur.fetchall()
-        return list(map(operator.itemgetter(0), tuples))
-
-    @property
-    def current_database(self):
-        # XXX The parent `Client` has a generic method that calls this same
-        # method in the backend. But for whatever reason calling this code from
-        # that method doesn't seem to work. Maybe `con` is a copy?
-        return self.con.database
-
-    def create_database(self, name, path=None, force=False):
-        """Create a new Impala database.
-
-        Parameters
-        ----------
-        name
-            Database name
-        path
-            HDFS path where to store the database data; otherwise uses Impala
-            default
-        force
-            Forcibly create the database
-        """
-        if path:
-            # explicit mkdir ensures the user own the dir rather than impala,
-            # which is easier for manual cleanup, if necessary
-            self.hdfs.mkdir(path)
-        statement = CreateDatabase(name, path=path, can_exist=force)
-        return self.raw_sql(statement)
-
-    def drop_database(self, name, force=False):
-        """Drop an Impala database.
-
-        Parameters
-        ----------
-        name
-            Database name
-        force
-            If False and there are any tables in this database, raises an
-            IntegrityError
-        """
-        if not force or name in self.list_databases():
-            tables = self.list_tables(database=name)
-            udfs = self.list_udfs(database=name)
-            udas = self.list_udas(database=name)
-        else:
-            tables = []
-            udfs = []
-            udas = []
-        if force:
-            for table in tables:
-                util.log('Dropping {}'.format(f'{name}.{table}'))
-                self.drop_table_or_view(table, database=name)
-            for func in udfs:
-                util.log(f'Dropping function {func.name}({func.inputs})')
-                self.drop_udf(
-                    func.name,
-                    input_types=func.inputs,
-                    database=name,
-                    force=True,
-                )
-            for func in udas:
-                util.log(f'Dropping aggregate function {func.name}({func.inputs})')
-                self.drop_uda(
-                    func.name,
-                    input_types=func.inputs,
-                    database=name,
-                    force=True,
-                )
-        elif tables or udfs or udas:
-            raise com.IntegrityError(
-                f"Database {name} must be empty before "
-                "being dropped, or set force=True"
-            )
-        statement = DropDatabase(name, must_exist=not force)
-        return self.raw_sql(statement)
-
-    def get_schema(
-        self,
-        table_name: str,
-        database: str | None = None,
-    ) -> sch.Schema:
-        """Return a Schema object for the indicated table and database.
-
-        Parameters
-        ----------
-        table_name
-            Table name
-        database
-            Database name
-
-        Returns
-        -------
-        Schema
-            Ibis schema
-        """
-        qualified_name = self._fully_qualified_name(table_name, database)
-        query = f'DESCRIBE {qualified_name}'
-
-        # only pull out the first two columns which are names and types
-        pairs = [row[:2] for row in self.con.fetchall(query)]
-        names, types = zip(*pairs)
-
-        ibis_types = [udf.parse_type(type.lower()) for type in types]
-        ibis_fields = dict(zip(names, ibis_types))
-        return sch.Schema(ibis_fields)
-
-    @property
-    def client_options(self):
-        return self.con.options
-
-    def get_options(self):
-        """Return current query options for the Impala session."""
-        return dict(row[:2] for row in self.con.fetchall("SET"))
-
-    def set_options(self, options):
-        self.con.set_options(options)
-
-    def reset_options(self):
-        # Must nuke all cursors
-        raise NotImplementedError
-
-    def set_compression_codec(self, codec):
-        if codec is None:
-            codec = 'none'
-        else:
-            codec = codec.lower()
-
-        if codec not in ('none', 'gzip', 'snappy'):
-            raise ValueError(f'Unknown codec: {codec}')
-
-        self.set_options({'COMPRESSION_CODEC': codec})
-
-    def create_view(
-        self,
-        name: str,
-        obj: ir.Table,
-        *,
-        database: str | None = None,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        ast = self.compiler.to_ast(obj)
-        select = ast.queries[0]
-        statement = CreateView(name, select, database=database, can_exist=overwrite)
-        self.raw_sql(statement)
-        return self.table(name, database=database)
-
-    def drop_view(self, name, database=None, force=False):
-        statement = DropView(name, database=database, must_exist=not force)
-        return self.raw_sql(statement)
-
-    @contextlib.contextmanager
-    def _setup_insert(self, obj):
-        import pandas as pd
-
-        if isinstance(obj, pd.DataFrame):
-            with DataFrameWriter(self, obj) as writer:
-                yield writer.delimited_table(writer.write_temp_csv())
-        else:
-            yield obj
-
-    def create_table(
-        self,
-        name: str,
-        obj: ir.Table | None = None,
-        *,
-        schema=None,
-        database=None,
-        temp: bool | None = None,
-        overwrite: bool = False,
-        external: bool = False,
-        # HDFS options
-        format='parquet',
-        location=None,
-        partition=None,
-        like_parquet=None,
-    ) -> ir.Table:
-        """Create a new table in Impala using an Ibis table expression.
-
-        This is currently designed for tables whose data is stored in HDFS.
-
-        Parameters
-        ----------
-        name
-            Table name
-        obj
-            If passed, creates table from select statement results
-        schema
-            Mutually exclusive with obj, creates an empty table with a
-            particular schema
-        database
-            Database name
-        temp
-            Whether a table is temporary
-        overwrite
-            Do not create table if table with indicated name already exists
-        external
-            Create an external table; Impala will not delete the underlying
-            data when the table is dropped
-        format
-            File format
-        location
-            Specify the directory location where Impala reads and writes files
-            for the table
-        partition
-            Must pass a schema to use this. Cannot partition from an
-            expression.
-        like_parquet
-            Can specify instead of a schema
-        """
-        if obj is None and schema is None:
-            raise com.IbisError("The schema or obj parameter is required")
-
-        if temp is not None:
-            raise NotImplementedError(
-                "Impala backend does not yet support temporary tables"
-            )
-        if like_parquet is not None:
-            raise NotImplementedError
-
-        if obj is not None:
-            with self._setup_insert(obj) as to_insert:
-                ast = self.compiler.to_ast(to_insert)
-                select = ast.queries[0]
-
-                if overwrite:
-                    self.drop_table(name, force=True)
-                self.raw_sql(
-                    CTAS(
-                        name,
-                        select,
-                        database=database,
-                        format=format,
-                        external=external,
-                        partition=partition,
-                        path=location,
-                    )
-                )
-        else:  # schema is not None
-            if overwrite:
-                self.drop_table(name, force=True)
-            self.raw_sql(
-                CreateTableWithSchema(
-                    name,
-                    schema,
-                    database=database,
-                    format=format,
-                    external=external,
-                    path=location,
-                    partition=partition,
-                )
-            )
-        return self.table(name, database=database)
-
-    def avro_file(
-        self,
-        hdfs_dir,
-        avro_schema,
-        name=None,
-        database=None,
-        external=True,
-        persist=False,
-    ):
-        """Create a table to read a collection of Avro data.
-
-        Parameters
-        ----------
-        hdfs_dir
-            Absolute HDFS path to directory containing avro files
-        avro_schema
-            The Avro schema for the data as a Python dict
-        name
-            Table name
-        database
-            Database name
-        external
-            Whether the table is external
-        persist
-            Persist the table
-
-        Returns
-        -------
-        ImpalaTable
-            Impala table expression
-        """
-        name, database = self._get_concrete_table_path(name, database, persist=persist)
-
-        stmt = ddl.CreateTableAvro(
-            name, hdfs_dir, avro_schema, database=database, external=external
-        )
-        self.raw_sql(stmt)
-        return self._wrap_new_table(name, database, persist)
-
-    def delimited_file(
-        self,
-        hdfs_dir,
-        schema,
-        name=None,
-        database=None,
-        delimiter=',',
-        na_rep=None,
-        escapechar=None,
-        lineterminator=None,
-        external=True,
-        persist=False,
-    ):
-        """Interpret delimited text files as an Ibis table expression.
-
-        See the `parquet_file` method for more details on what happens under
-        the hood.
-
-        Parameters
-        ----------
-        hdfs_dir
-            HDFS directory containing delimited text files
-        schema
-            Ibis schema
-        name
-            Name for temporary or persistent table; otherwise random names are
-            generated
-        database
-            Database to create the table in
-        delimiter
-            Character used to delimit columns
-        na_rep
-            Character used to represent NULL values
-        escapechar
-            Character used to escape special characters
-        lineterminator
-            Character used to delimit lines
-        external
-            Create table as EXTERNAL (data will not be deleted on drop). Not
-            that if persist=False and external=False, whatever data you
-            reference will be deleted
-        persist
-            If True, do not delete the table upon garbage collection of ibis
-            table object
-
-        Returns
-        -------
-        ImpalaTable
-            Impala table expression
-        """
-        name, database = self._get_concrete_table_path(name, database, persist=persist)
-
-        stmt = ddl.CreateTableDelimited(
-            name,
-            hdfs_dir,
-            schema,
-            database=database,
-            delimiter=delimiter,
-            external=external,
-            na_rep=na_rep,
-            lineterminator=lineterminator,
-            escapechar=escapechar,
-        )
-        self.raw_sql(stmt)
-        return self._wrap_new_table(name, database, persist)
-
-    def parquet_file(
-        self,
-        hdfs_dir,
-        schema=None,
-        name=None,
-        database=None,
-        external=True,
-        like_file=None,
-        like_table=None,
-        persist=False,
-    ):
-        """Make indicated parquet file in HDFS available as an Ibis table.
-
-        The table created can be optionally named and persisted, otherwise a
-        unique name will be generated. Temporarily, for any non-persistent
-        external table created by Ibis we will attempt to drop it when the
-        underlying object is garbage collected (or the Python interpreter shuts
-        down normally).
-
-        Parameters
-        ----------
-        hdfs_dir
-            Path in HDFS
-        schema
-            If no schema provided, and neither of the like_* argument is
-            passed, one will be inferred from one of the parquet files in the
-            directory.
-        like_file
-            Absolute path to Parquet file in HDFS to use for schema
-            definitions. An alternative to having to supply an explicit schema
-        like_table
-            Fully scoped and escaped string to an Impala table whose schema we
-            will use for the newly created table.
-        name
-            Random unique name generated otherwise
-        database
-            Database to create the (possibly temporary) table in
-        external
-            If a table is external, the referenced data will not be deleted
-            when the table is dropped in Impala. Otherwise (external=False)
-            Impala takes ownership of the Parquet file.
-        persist
-            Do not drop the table during garbage collection
-
-        Returns
-        -------
-        ImpalaTable
-            Impala table expression
-        """
-        name, database = self._get_concrete_table_path(name, database, persist=persist)
-
-        # If no schema provided, need to find some absolute path to a file in
-        # the HDFS directory
-        if like_file is None and like_table is None and schema is None:
-            try:
-                file_name = next(
-                    fn
-                    for fn in (
-                        os.path.basename(f["name"])
-                        for f in self.hdfs.ls(hdfs_dir, detail=True)
-                        if f["type"].lower() == "file"
-                    )
-                    if not fn.startswith(("_", "."))
-                    if not fn.endswith((".tmp", ".copying"))
-                )
-            except StopIteration:
-                raise com.IbisError("No files found in the passed directory")
-            else:
-                like_file = pjoin(hdfs_dir, file_name)
-
-        stmt = ddl.CreateTableParquet(
-            name,
-            hdfs_dir,
-            schema=schema,
-            database=database,
-            example_file=like_file,
-            example_table=like_table,
-            external=external,
-            can_exist=False,
-        )
-        self.raw_sql(stmt)
-        return self._wrap_new_table(name, database, persist)
-
-    def _get_concrete_table_path(self, name, database, persist=False):
-        if not persist:
-            if name is None:
-                name = f'__ibis_tmp_{util.guid()}'
-
-            if database is None:
-                self._ensure_temp_db_exists()
-                database = options.impala.temp_db
-            return name, database
-        else:
-            if name is None:
-                raise com.IbisError('Must pass table name if persist=True')
-            return name, database
-
-    def _ensure_temp_db_exists(self):
-        # TODO: session memoize to avoid unnecessary `SHOW DATABASES` calls
-        name, path = options.impala.temp_db, options.impala.temp_hdfs_path
-        if name not in self.list_databases():
-            if self._hdfs is not None:
-                self.create_database(name, path=path, force=True)
-
-    def _drop_table(self, name: str) -> None:
-        # database might have been dropped, so we suppress the
-        # corresponding Exception
-        with contextlib.suppress(ImpylaError):
-            self.drop_table(name)
-
-    def _wrap_new_table(self, name, database, persist):
-        qualified_name = self._fully_qualified_name(name, database)
-        t = self.table(qualified_name)
-        if not persist:
-            self._temp_objects.add(
-                # weakref the op instead of the expression because the table is
-                # potentially collected after subsequent use when `_erase_expr`
-                # unwraps the Expr layer
-                weakref.finalize(t.op(), self._drop_table, qualified_name)
-            )
-
-        # Compute number of rows in table for better default query planning
-        cardinality = t.count().execute()
-        set_card = (
-            "alter table {} set tblproperties('numRows'='{}', "
-            "'STATS_GENERATED_VIA_STATS_TASK' = 'true')".format(
-                qualified_name, cardinality
-            )
-        )
-        self.raw_sql(set_card)
-
-        return t
-
-    def text_file(self, hdfs_path, column_name='value'):
-        """Interpret text data as a table with a single string column."""
-
-    def insert(
-        self,
-        table_name,
-        obj=None,
-        database=None,
-        overwrite=False,
-        partition=None,
-        values=None,
-        validate=True,
-    ):
-        """Insert data into an existing table.
-
-        See
-        [`ImpalaTable.insert`][ibis.backends.impala.client.ImpalaTable.insert]
-        for parameters.
-
-        Examples
-        --------
-        >>> table = 'my_table'
-        >>> con.insert(table, table_expr)  # doctest: +SKIP
-
-        Completely overwrite contents
-        >>> con.insert(table, table_expr, overwrite=True)  # doctest: +SKIP
-        """
-        table = self.table(table_name, database=database)
-        return table.insert(
-            obj=obj,
-            overwrite=overwrite,
-            partition=partition,
-            values=values,
-            validate=validate,
-        )
-
-    @util.deprecated(
-        as_of="5.0", removed_in="6.0", instead="Use create_table(overwrite=True)"
-    )
-    def load_data(
-        self,
-        table_name,
-        path,
-        database=None,
-        overwrite=False,
-        partition=None,
-    ):
-        """Loads data into an Impala table by physically moving data files."""
-        table = self.table(table_name, database=database)
-        return table.load_data(path, overwrite=overwrite, partition=partition)
-
-    def drop_table(
-        self, name: str, *, database: str | None = None, force: bool = False
-    ) -> None:
-        """Drop an Impala table.
-
-        Parameters
-        ----------
-        name
-            Table name
-        database
-            Database name
-        force
-            Database may throw exception if table does not exist
-
-        Examples
-        --------
-        >>> table = 'my_table'
-        >>> db = 'operations'
-        >>> con.drop_table(table, database=db, force=True)  # doctest: +SKIP
-        """
-        statement = DropTable(name, database=database, must_exist=not force)
-        self.raw_sql(statement)
-
-    def truncate_table(self, name: str, database: str | None = None) -> None:
-        """Delete all rows from an existing table.
-
-        Parameters
-        ----------
-        name
-            Table name
-        database
-            Database name
-        """
-        statement = TruncateTable(name, database=database)
-        self.raw_sql(statement)
-
-    def drop_table_or_view(self, name, *, database=None, force=False):
-        """Drop view or table."""
-        try:
-            self.drop_table(name, database=database)
-        except Exception as e:  # noqa: BLE001
+        exprs = [right['foo'], right['bar']]
+        self.assertRaises(RelationError, left.projection, exprs)
+
+    def test_projection_unnamed_literal_interactive_blowup(self):
+        # #147 and #153 alike
+        table = self.con.table('functional_alltypes')
+
+        with config.option_context('interactive', True):
             try:
-                self.drop_view(name, database=database)
-            except Exception:  # noqa: BLE001
-                raise e
-
-    def cache_table(self, table_name, *, database=None, pool='default'):
-        """Caches a table in cluster memory in the given pool.
-
-        Parameters
-        ----------
-        table_name
-            Table name
-        database
-            Database name
-        pool
-            The name of the pool in which to cache the table
-
-        Examples
-        --------
-        >>> table = 'my_table'
-        >>> db = 'operations'
-        >>> pool = 'op_4GB_pool'
-        >>> con.cache_table('my_table', database=db, pool=pool)  # doctest: +SKIP
-        """
-        statement = ddl.CacheTable(table_name, database=database, pool=pool)
-        self.raw_sql(statement)
-
-    def _get_schema_using_query(self, query):
-        cur = self.raw_sql(f"SELECT * FROM ({query}) t0 LIMIT 0")
-        # resets the state of the cursor and closes operation
-        cur.fetchall()
-        ibis_fields = self._adapt_types(cur.description)
-        cur.release()
-
-        return sch.Schema(ibis_fields)
-
-    def create_function(self, func, name=None, database=None):
-        """Create a function within Impala.
-
-        Parameters
-        ----------
-        func
-            UDF or UDAF
-        name
-            Function name
-        database
-            Database name
-        """
-        if name is None:
-            name = func.name
-        database = database or self.current_database
-
-        if isinstance(func, udf.ImpalaUDF):
-            stmt = ddl.CreateUDF(func, name=name, database=database)
-        elif isinstance(func, udf.ImpalaUDA):
-            stmt = ddl.CreateUDA(func, name=name, database=database)
-        else:
-            raise TypeError(func)
-        self.raw_sql(stmt)
-
-    def drop_udf(
-        self,
-        name,
-        input_types=None,
-        database=None,
-        force=False,
-        aggregate=False,
-    ):
-        """Drop a UDF.
-
-        If only name is given, this will search for the relevant UDF and drop
-        it. To delete an overloaded UDF, give only a name and force=True
-
-        Parameters
-        ----------
-        name
-            Function name
-        input_types
-            Input types
-        force
-            Must be set to `True` to drop overloaded UDFs
-        database
-            Database name
-        aggregate
-            Whether the function is an aggregate
-        """
-        if not input_types:
-            if not database:
-                database = self.current_database
-            result = self.list_udfs(database=database, like=name)
-            if len(result) > 1:
-                if force:
-                    for func in result:
-                        self._drop_single_function(
-                            func.name,
-                            func.inputs,
-                            database=database,
-                            aggregate=aggregate,
-                        )
-                    return
-                else:
-                    raise Exception(
-                        f"More than one function with {name} found. Please specify force=True"
-                    )
-            elif len(result) == 1:
-                func = result.pop()
-                self._drop_single_function(
-                    func.name,
-                    func.inputs,
-                    database=database,
-                    aggregate=aggregate,
-                )
-                return
-            else:
-                raise Exception(f"No function found with name {name}")
-        self._drop_single_function(
-            name, input_types, database=database, aggregate=aggregate
-        )
-
-    def drop_uda(self, name, input_types=None, database=None, force=False):
-        """Drop an aggregate function."""
-        return self.drop_udf(
-            name, input_types=input_types, database=database, force=force
-        )
-
-    def _drop_single_function(self, name, input_types, database=None, aggregate=False):
-        stmt = ddl.DropFunction(
-            name,
-            input_types,
-            must_exist=False,
-            aggregate=aggregate,
-            database=database,
-        )
-        self.raw_sql(stmt)
-
-    def _drop_all_functions(self, database):
-        udfs = self.list_udfs(database=database)
-        for fnct in udfs:
-            stmt = ddl.DropFunction(
-                fnct.name,
-                fnct.inputs,
-                must_exist=False,
-                aggregate=False,
-                database=database,
-            )
-            self.raw_sql(stmt)
-        udafs = self.list_udas(database=database)
-        for udaf in udafs:
-            stmt = ddl.DropFunction(
-                udaf.name,
-                udaf.inputs,
-                must_exist=False,
-                aggregate=True,
-                database=database,
-            )
-            self.raw_sql(stmt)
-
-    def list_udfs(self, database=None, like=None):
-        """Lists all UDFs associated with given database."""
-        if not database:
-            database = self.current_database
-        statement = ddl.ListFunction(database, like=like, aggregate=False)
-        cur = self.raw_sql(statement)
-        result = self._get_udfs(cur, udf.ImpalaUDF)
-        cur.release()
-        return result
-
-    def list_udas(self, database=None, like=None):
-        """Lists all UDAFs associated with a given database."""
-        if not database:
-            database = self.current_database
-        statement = ddl.ListFunction(database, like=like, aggregate=True)
-        cur = self.raw_sql(statement)
-        result = self._get_udfs(cur, udf.ImpalaUDA)
-        cur.release()
-
-        return result
-
-    def _get_udfs(self, cur, klass):
-        def _to_type(x):
-            ibis_type = udf._impala_type_to_ibis(x.lower())
-            return dt.dtype(ibis_type)
-
-        tuples = cur.fetchall()
-        if len(tuples) > 0:
-            result = []
-            for tup in tuples:
-                out_type, sig = tup[:2]
-                name, types = _split_signature(sig)
-                types = _type_parser(types).types
-
-                inputs = []
-                for arg in types:
-                    argm = _arg_type.match(arg)
-                    var, simple = argm.groups()
-                    if simple:
-                        t = _to_type(simple)
-                        inputs.append(t)
-                    else:
-                        t = _to_type(var)
-                        inputs = rlz.listof(t)
-                        # TODO
-                        # inputs.append(varargs(t))
-                        break
-
-                output = udf._impala_type_to_ibis(out_type.lower())
-                result.append(klass(inputs, output, name=name))
-            return result
-        else:
-            return []
-
-    def exists_udf(self, name: str, database: str | None = None) -> bool:
-        """Checks if a given UDF exists within a specified database."""
-        return bool(self.list_udfs(database=database, like=name))
-
-    def exists_uda(self, name: str, database: str | None = None) -> bool:
-        """Checks if a given UDAF exists within a specified database."""
-        return bool(self.list_udas(database=database, like=name))
-
-    def compute_stats(
-        self,
-        name: str,
-        database: str | None = None,
-        incremental: bool = False,
-    ) -> None:
-        """Issue a `COMPUTE STATS` command for a given table.
-
-        Parameters
-        ----------
-        name
-            Can be fully qualified (with database name)
-        database
-            Database name
-        incremental
-            If True, issue COMPUTE INCREMENTAL STATS
-        """
-        maybe_inc = 'INCREMENTAL ' if incremental else ''
-        cmd = f'COMPUTE {maybe_inc}STATS'
-
-        stmt = self._table_command(cmd, name, database=database)
-        self.raw_sql(stmt)
-
-    def invalidate_metadata(
-        self,
-        name: str | None = None,
-        database: str | None = None,
-    ) -> None:
-        """Issue an `INVALIDATE METADATA` command.
-
-        Optionally this applies to a specific table. See Impala documentation.
-
-        Parameters
-        ----------
-        name
-            Table name. Can be fully qualified (with database)
-        database
-            Database name
-        """
-        stmt = 'INVALIDATE METADATA'
-        if name is not None:
-            stmt = self._table_command(stmt, name, database=database)
-        self.raw_sql(stmt)
-
-    def refresh(self, name: str, database: str | None = None) -> None:
-        """Reload HDFS block location metadata for a table.
-
-        This can be useful after ingesting data as part of an ETL pipeline, for
-        example.
-
-        Related to `INVALIDATE METADATA`. See Impala documentation for more.
-
-        Parameters
-        ----------
-        name
-            Table name. Can be fully qualified (with database)
-        database
-            Database name
-        """
-        # TODO(wesm): can this statement be cancelled?
-        stmt = self._table_command('REFRESH', name, database=database)
-        self.raw_sql(stmt)
-
-    def describe_formatted(
-        self,
-        name: str,
-        database: str | None = None,
-    ) -> pd.DataFrame:
-        """Retrieve the results of a `DESCRIBE FORMATTED` command.
-
-        See Impala documentation for more.
-
-        Parameters
-        ----------
-        name
-            Table name. Can be fully qualified (with database)
-        database
-            Database name
-        """
-        from ibis.backends.impala.metadata import parse_metadata
-
-        stmt = self._table_command('DESCRIBE FORMATTED', name, database=database)
-        result = self._exec_statement(stmt)
-
-        # Leave formatting to pandas
-        for c in result.columns:
-            result[c] = result[c].str.strip()
-
-        return parse_metadata(result)
-
-    def show_files(
-        self,
-        name: str,
-        database: str | None = None,
-    ) -> pd.DataFrame:
-        """Retrieve results of a `SHOW FILES` command for a table.
-
-        See Impala documentation for more.
-
-        Parameters
-        ----------
-        name
-            Table name. Can be fully qualified (with database)
-        database
-            Database name
-        """
-        stmt = self._table_command('SHOW FILES IN', name, database=database)
-        return self._exec_statement(stmt)
-
-    def list_partitions(self, name, database=None):
-        stmt = self._table_command('SHOW PARTITIONS', name, database=database)
-        return self._exec_statement(stmt)
-
-    def table_stats(self, name, database=None):
-        """Return results of `SHOW TABLE STATS` for the table `name`."""
-        stmt = self._table_command('SHOW TABLE STATS', name, database=database)
-        return self._exec_statement(stmt)
-
-    def column_stats(self, name, database=None):
-        """Return results of `SHOW COLUMN STATS` for the table `name`."""
-        stmt = self._table_command('SHOW COLUMN STATS', name, database=database)
-        return self._exec_statement(stmt)
-
-    def _exec_statement(self, stmt):
-        return self.fetch_from_cursor(self.raw_sql(stmt), schema=None)
-
-    def _table_command(self, cmd, name, database=None):
-        qualified_name = self._fully_qualified_name(name, database)
-        return f'{cmd} {qualified_name}'
-
-    def _adapt_types(self, descr):
-        names = []
-        adapted_types = []
-        for col in descr:
-            names.append(col[0])
-            impala_typename = col[1]
-            typename = udf._impala_to_ibis_type[impala_typename.lower()]
-
-            if typename == 'decimal':
-                precision, scale = col[4:6]
-                adapted_types.append(dt.Decimal(precision, scale))
-            else:
-                adapted_types.append(typename)
-        return dict(zip(names, adapted_types))
-
-    def write_dataframe(
-        self,
-        df: pd.DataFrame,
-        path: str,
-        format: Literal['csv'] = 'csv',
-    ) -> Any:
-        """Write a pandas DataFrame to indicated file path.
-
-        Parameters
-        ----------
-        df
-            Pandas DataFrame
-        path
-            Absolute file path
-        format
-            File format
-        """
-        writer = DataFrameWriter(self, df)
-        return writer.write_csv(path)
+                table.select([table.bigint_col, ibis.literal(5)])
+            except Exception as e:
+                assert 'named' in e.args[0]
+
+    def test_projection_of_aggregated(self):
+        # Fully-formed aggregations "block"; in a projection, column
+        # expressions referencing table expressions below the aggregation are
+        # invalid.
+        pass
+
+    def test_projection_with_star_expr(self):
+        new_expr = (self.table['a'] * 5).name('bigger_a')
+
+        t = self.table
+
+        # it lives!
+        proj = t[t, new_expr]
+        repr(proj)
+
+        ex_names = self.table.schema().names + ['bigger_a']
+        assert proj.schema().names == ex_names
+
+        # cannot pass an invalid table expression
+        t2 = t.aggregate([t['a'].sum().name('sum(a)')], by=['g'])
+        self.assertRaises(RelationError, t.__getitem__, [t2])
+
+        # TODO: there may be some ways this can be invalid
+
+    def test_projection_convenient_syntax(self):
+        proj = self.table[self.table, self.table['a'].name('foo')]
+        proj2 = self.table[[self.table, self.table['a'].name('foo')]]
+        assert_equal(proj, proj2)
+
+    def test_projection_mutate_analysis_bug(self):
+        # GH #549
+
+        t = self.con.table('airlines')
+
+        # it works!
+        (t[t.depdelay.notnull()]
+         .mutate(leg=ibis.literal('-').join([t.origin, t.dest]))
+         ['year', 'month', 'day', 'depdelay', 'leg'])
+
+    def test_projection_self(self):
+        result = self.table[self.table]
+        expected = self.table.projection(self.table)
+
+        assert_equal(result, expected)
+
+    def test_projection_array_expr(self):
+        result = self.table[self.table.a]
+        expected = self.table[[self.table.a]]
+        assert_equal(result, expected)
+
+    def test_add_column(self):
+        # Creates a projection with a select-all on top of a non-projection
+        # TableExpr
+        new_expr = (self.table['a'] * 5).name('bigger_a')
+
+        t = self.table
+
+        result = t.add_column(new_expr)
+        expected = t[[t, new_expr]]
+        assert_equal(result, expected)
+
+        result = t.add_column(new_expr, 'wat')
+        expected = t[[t, new_expr.name('wat')]]
+        assert_equal(result, expected)
+
+    def test_add_column_scalar_expr(self):
+        # Check literals, at least
+        pass
+
+    def test_add_column_aggregate_crossjoin(self):
+        # A new column that depends on a scalar value produced by this or some
+        # other table.
+        #
+        # For example:
+        # SELECT *, b - VAL
+        # FROM table1
+        #
+        # Here, VAL could be something produced by aggregating table1 or any
+        # other table for that matter.
+        pass
+
+    def test_add_column_existing_projection(self):
+        # The "blocking" predecessor table is a projection; we can simply add
+        # the column to the existing projection
+        foo = (self.table.f * 2).name('foo')
+        bar = (self.table.f * 4).name('bar')
+        t2 = self.table.add_column(foo)
+        t3 = t2.add_column(bar)
+
+        expected = self.table[self.table, foo, bar]
+        assert_equal(t3, expected)
+
+    def test_mutate(self):
+        one = self.table.f * 2
+        foo = (self.table.a + self.table.b).name('foo')
+
+        expr = self.table.mutate(foo, one=one, two=2)
+        expected = self.table[self.table, foo, one.name('one'),
+                              ibis.literal(2).name('two')]
+        assert_equal(expr, expected)
+
+    def test_mutate_alter_existing_columns(self):
+        new_f = self.table.f * 2
+        foo = self.table.d * 2
+        expr = self.table.mutate(f=new_f, foo=foo)
+
+        expected = self.table['a', 'b', 'c', 'd', 'e',
+                              new_f.name('f'), 'g', 'h',
+                              foo.name('foo')]
+
+        assert_equal(expr, expected)
+
+    def test_replace_column(self):
+        tb = api.table([
+            ('a', 'int32'),
+            ('b', 'double'),
+            ('c', 'string')
+        ])
+
+        expr = tb.b.cast('int32')
+        tb2 = tb.set_column('b', expr)
+        expected = tb[tb.a, expr.name('b'), tb.c]
+
+        assert_equal(tb2, expected)
+
+    def test_filter_no_list(self):
+        pred = self.table.a > 5
+
+        result = self.table.filter(pred)
+        expected = self.table[pred]
+        assert_equal(result, expected)
+
+    def test_add_predicate(self):
+        pred = self.table['a'] > 5
+        result = self.table[pred]
+        assert isinstance(result.op(), ops.Filter)
+
+    def test_filter_root_table_preserved(self):
+        result = self.table[self.table['a'] > 5]
+        roots = result.op().root_tables()
+        assert roots[0] is self.table.op()
+
+    def test_invalid_predicate(self):
+        # a lookalike
+        table2 = api.table(self.schema, name='bar')
+        self.assertRaises(RelationError, self.table.__getitem__,
+                          table2['a'] > 5)
+
+    def test_add_predicate_coalesce(self):
+        # Successive predicates get combined into one rather than nesting. This
+        # is mainly to enhance readability since we could handle this during
+        # expression evaluation anyway.
+        pred1 = self.table['a'] > 5
+        pred2 = self.table['b'] > 0
+
+        result = self.table[pred1][pred2]
+        expected = self.table.filter([pred1, pred2])
+        assert_equal(result, expected)
+
+        # 59, if we are not careful, we can obtain broken refs
+        interm = self.table[pred1]
+        result = interm.filter([interm['b'] > 0])
+        assert_equal(result, expected)
+
+    def test_repr_same_but_distinct_objects(self):
+        t = self.con.table('test1')
+        t_copy = self.con.table('test1')
+        table2 = t[t_copy['f'] > 0]
+
+        result = repr(table2)
+        assert result.count('DatabaseTable') == 1
+
+    def test_filter_fusion_distinct_table_objects(self):
+        t = self.con.table('test1')
+        tt = self.con.table('test1')
+
+        expr = t[t.f > 0][t.c > 0]
+        expr2 = t[t.f > 0][tt.c > 0]
+        expr3 = t[tt.f > 0][tt.c > 0]
+        expr4 = t[tt.f > 0][t.c > 0]
+
+        assert_equal(expr, expr2)
+        assert repr(expr) == repr(expr2)
+        assert_equal(expr, expr3)
+        assert_equal(expr, expr4)
+
+    def test_column_relabel(self):
+        # GH #551. Keeping the test case very high level to not presume that
+        # the relabel is necessarily implemented using a projection
+        types = ['int32', 'string', 'double']
+        table = api.table(zip(['foo', 'bar', 'baz'], types))
+        result = table.relabel({'foo': 'one', 'baz': 'three'})
+
+        schema = result.schema()
+        ex_schema = api.schema(zip(['one', 'bar', 'three'], types))
+        assert_equal(schema, ex_schema)
+
+    def test_limit(self):
+        limited = self.table.limit(10, offset=5)
+        assert limited.op().n == 10
+        assert limited.op().offset == 5
+
+    def test_sort_by(self):
+        # Commit to some API for ascending and descending
+        #
+        # table.sort_by(['g', expr1, desc(expr2), desc(expr3)])
+        #
+        # Default is ascending for anything coercable to an expression,
+        # and we'll have ascending/descending wrappers to help.
+        result = self.table.sort_by(['f'])
+        sort_key = result.op().keys[0].op()
+        assert_equal(sort_key.expr, self.table.f)
+        assert sort_key.ascending
+
+        # non-list input. per #150
+        result2 = self.table.sort_by('f')
+        assert_equal(result, result2)
+
+        result2 = self.table.sort_by([('f', False)])
+        result3 = self.table.sort_by([('f', 'descending')])
+        result4 = self.table.sort_by([('f', 0)])
+
+        key2 = result2.op().keys[0].op()
+        key3 = result3.op().keys[0].op()
+        key4 = result4.op().keys[0].op()
+
+        assert not key2.ascending
+        assert not key3.ascending
+        assert not key4.ascending
+        assert_equal(result2, result3)
+
+    def test_sort_by_desc_deferred_sort_key(self):
+        result = (self.table.group_by('g')
+                  .size()
+                  .sort_by(ibis.desc('count')))
+
+        tmp = self.table.group_by('g').size()
+        expected = tmp.sort_by((tmp['count'], False))
+        expected2 = tmp.sort_by(ibis.desc(tmp['count']))
+
+        assert_equal(result, expected)
+        assert_equal(result, expected2)
+
+    def test_slice_convenience(self):
+        expr = self.table[:5]
+        expr2 = self.table[:5:1]
+        assert_equal(expr, self.table.limit(5))
+        assert_equal(expr, expr2)
+
+        expr = self.table[2:7]
+        expr2 = self.table[2:7:1]
+        assert_equal(expr, self.table.limit(5, offset=2))
+        assert_equal(expr, expr2)
+
+        self.assertRaises(ValueError, self.table.__getitem__, slice(2, 15, 2))
+        self.assertRaises(ValueError, self.table.__getitem__, slice(5, None))
+        self.assertRaises(ValueError, self.table.__getitem__, slice(None, -5))
+        self.assertRaises(ValueError, self.table.__getitem__, slice(-10, -5))
+
+
+class TestAggregation(BasicTestCase, unittest.TestCase):
+
+    def test_count(self):
+        result = self.table['a'].count()
+        assert isinstance(result, api.Int64Scalar)
+        assert isinstance(result.op(), ops.Count)
+
+    def test_table_count(self):
+        result = self.table.count()
+        assert isinstance(result, api.Int64Scalar)
+        assert isinstance(result.op(), ops.Count)
+        assert result.get_name() == 'count'
+
+    def test_len_raises_expression_error(self):
+        with self.assertRaises(com.ExpressionError):
+            len(self.table)
+
+    def test_sum_expr_basics(self):
+        # Impala gives bigint for all integer types
+        ex_class = api.Int64Scalar
+        for c in self.int_cols + self.bool_cols:
+            result = self.table[c].sum()
+            assert isinstance(result, ex_class)
+            assert isinstance(result.op(), ops.Sum)
+
+        # Impala gives double for all floating point types
+        ex_class = api.DoubleScalar
+        for c in self.float_cols:
+            result = self.table[c].sum()
+            assert isinstance(result, ex_class)
+            assert isinstance(result.op(), ops.Sum)
+
+    def test_mean_expr_basics(self):
+        cols = self.int_cols + self.float_cols + self.bool_cols
+        for c in cols:
+            result = self.table[c].mean()
+            assert isinstance(result, api.DoubleScalar)
+            assert isinstance(result.op(), ops.Mean)
+
+    def test_aggregate_no_keys(self):
+        agg_exprs = [self.table['a'].sum().name('sum(a)'),
+                     self.table['c'].mean().name('mean(c)')]
+
+        # A TableExpr, which in SQL at least will yield a table with a single
+        # row
+        result = self.table.aggregate(agg_exprs)
+        assert isinstance(result, TableExpr)
+
+    def test_aggregate_keys_basic(self):
+        agg_exprs = [self.table['a'].sum().name('sum(a)'),
+                     self.table['c'].mean().name('mean(c)')]
+
+        # A TableExpr, which in SQL at least will yield a table with a single
+        # row
+        result = self.table.aggregate(agg_exprs, by=['g'])
+        assert isinstance(result, TableExpr)
+
+        # it works!
+        repr(result)
+
+    def test_aggregate_non_list_inputs(self):
+        # per #150
+        metric = self.table.f.sum().name('total')
+        by = 'g'
+        having = self.table.c.sum() > 10
+
+        result = self.table.aggregate(metric, by=by, having=having)
+        expected = self.table.aggregate([metric], by=[by], having=[having])
+        assert_equal(result, expected)
+
+    def test_aggregate_keywords(self):
+        t = self.table
+
+        expr = t.aggregate(foo=t.f.sum(), bar=lambda x: x.f.mean(),
+                           by='g')
+        expr2 = t.group_by('g').aggregate(foo=t.f.sum(),
+                                          bar=lambda x: x.f.mean())
+        expected = t.aggregate([t.f.mean().name('bar'),
+                                t.f.sum().name('foo')], by='g')
+
+        assert_equal(expr, expected)
+        assert_equal(expr2, expected)
+
+    def test_summary_expand_list(self):
+        summ = self.table.f.summary()
+
+        metric = self.table.g.group_concat().name('bar')
+        result = self.table.aggregate([metric, summ])
+        expected = self.table.aggregate([metric] + summ.exprs())
+        assert_equal(result, expected)
+
+    def test_aggregate_invalid(self):
+        # Pass a non-aggregation or non-scalar expr
+        pass
+
+    def test_filter_aggregate_pushdown_predicate(self):
+        # In the case where we want to add a predicate to an aggregate
+        # expression after the fact, rather than having to backpedal and add it
+        # before calling aggregate.
+        #
+        # TODO (design decision): This could happen automatically when adding a
+        # predicate originating from the same root table; if an expression is
+        # created from field references from the aggregated table then it
+        # becomes a filter predicate applied on top of a view
+
+        pred = self.table.f > 0
+        metrics = [self.table.a.sum().name('total')]
+        agged = self.table.aggregate(metrics, by=['g'])
+        filtered = agged.filter([pred])
+        expected = self.table[pred].aggregate(metrics, by=['g'])
+        assert_equal(filtered, expected)
+
+    def test_filter_aggregate_partial_pushdown(self):
+        pass
+
+    def test_aggregate_post_predicate(self):
+        # Test invalid having clause
+        metrics = [self.table.f.sum().name('total')]
+        by = ['g']
+
+        invalid_having_cases = [
+            self.table.f.sum(),
+            self.table.f > 2
+        ]
+        for case in invalid_having_cases:
+            self.assertRaises(com.ExpressionError, self.table.aggregate,
+                              metrics, by=by, having=[case])
+
+    def test_group_by_having_api(self):
+        # #154, add a HAVING post-predicate in a composable way
+        metric = self.table.f.sum().name('foo')
+        postp = self.table.d.mean() > 1
+
+        expr = (self.table
+                .group_by('g')
+                .having(postp)
+                .aggregate(metric))
+
+        expected = self.table.aggregate(metric, by='g', having=postp)
+        assert_equal(expr, expected)
+
+    def test_aggregate_root_table_internal(self):
+        pass
+
+    def test_compound_aggregate_expr(self):
+        # See ibis #24
+        compound_expr = (self.table['a'].sum() /
+                         self.table['a'].mean()).name('foo')
+        assert ops.is_reduction(compound_expr)
+
+        # Validates internally
+        self.table.aggregate([compound_expr])
+
+    def test_groupby_convenience(self):
+        metrics = [self.table.f.sum().name('total')]
+
+        expr = self.table.group_by('g').aggregate(metrics)
+        expected = self.table.aggregate(metrics, by=['g'])
+        assert_equal(expr, expected)
+
+        group_expr = self.table.g.cast('double').name('g')
+        expr = self.table.group_by(group_expr).aggregate(metrics)
+        expected = self.table.aggregate(metrics, by=[group_expr])
+        assert_equal(expr, expected)
+
+    def test_group_by_count_size(self):
+        # #148, convenience for interactive use, and so forth
+        result1 = self.table.group_by('g').size()
+        result2 = self.table.group_by('g').count()
+
+        expected = (self.table.group_by('g')
+                    .aggregate([self.table.count().name('count')]))
+
+        assert_equal(result1, expected)
+        assert_equal(result2, expected)
+
+        result = self.table.group_by('g').count('foo')
+        expected = (self.table.group_by('g')
+                    .aggregate([self.table.count().name('foo')]))
+        assert_equal(result, expected)
+
+    def test_group_by_column_select_api(self):
+        grouped = self.table.group_by('g')
+
+        result = grouped.f.sum()
+        expected = grouped.aggregate(self.table.f.sum().name('sum(f)'))
+        assert_equal(result, expected)
+
+        supported_functions = ['sum', 'mean', 'count', 'size', 'max', 'min']
+
+        # make sure they all work
+        for fn in supported_functions:
+            getattr(grouped.f, fn)()
+
+    def test_value_counts_convenience(self):
+        # #152
+        result = self.table.g.value_counts()
+        expected = (self.table.group_by('g')
+                    .aggregate(self.table.count().name('count')))
+
+        assert_equal(result, expected)
+
+    def test_isin_value_counts(self):
+        # #157, this code path was untested before
+        bool_clause = self.table.g.notin(['1', '4', '7'])
+        # it works!
+        bool_clause.name('notin').value_counts()
+
+    def test_value_counts_unnamed_expr(self):
+        nation = self.con.table('tpch_nation')
+
+        expr = nation.n_name.lower().value_counts()
+        expected = nation.n_name.lower().name('unnamed').value_counts()
+        assert_equal(expr, expected)
+
+    def test_aggregate_unnamed_expr(self):
+        nation = self.con.table('tpch_nation')
+        expr = nation.n_name.lower().left(1)
+        self.assertRaises(com.ExpressionError, nation.group_by(expr).aggregate,
+                          nation.count().name('metric'))
+
+    def test_default_reduction_names(self):
+        d = self.table.f
+        cases = [
+            (d.count(), 'count'),
+            (d.sum(), 'sum'),
+            (d.mean(), 'mean'),
+            (d.approx_nunique(), 'approx_nunique'),
+            (d.approx_median(), 'approx_median'),
+            (d.min(), 'min'),
+            (d.max(), 'max')
+        ]
+
+        for expr, ex_name in cases:
+            assert expr.get_name() == ex_name
+
+
+class TestJoinsUnions(BasicTestCase, unittest.TestCase):
+
+    def test_join_no_predicate_list(self):
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+
+        pred = region.r_regionkey == nation.n_regionkey
+        joined = region.inner_join(nation, pred)
+        expected = region.inner_join(nation, [pred])
+        assert_equal(joined, expected)
+
+    def test_equijoin_schema_merge(self):
+        table1 = ibis.table([('key1',  'string'), ('value1', 'double')])
+        table2 = ibis.table([('key2',  'string'), ('stuff', 'int32')])
+
+        pred = table1['key1'] == table2['key2']
+        join_types = ['inner_join', 'left_join', 'outer_join']
+
+        ex_schema = api.Schema(['key1', 'value1', 'key2', 'stuff'],
+                               ['string', 'double', 'string', 'int32'])
+
+        for fname in join_types:
+            f = getattr(table1, fname)
+            joined = f(table2, [pred]).materialize()
+            assert_equal(joined.schema(), ex_schema)
+
+    def test_join_combo_with_projection(self):
+        # Test a case where there is column name overlap, but the projection
+        # passed makes it a non-issue. Highly relevant with self-joins
+        #
+        # For example, where left/right have some field names in common:
+        # SELECT left.*, right.a, right.b
+        # FROM left join right on left.key = right.key
+        t = self.table
+        t2 = t.add_column(t['f'] * 2, 'foo')
+        t2 = t2.add_column(t['f'] * 4, 'bar')
+
+        # this works
+        joined = t.left_join(t2, [t['g'] == t2['g']])
+        proj = joined.projection([t, t2['foo'], t2['bar']])
+        repr(proj)
+
+    def test_join_getitem_projection(self):
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+
+        pred = region.r_regionkey == nation.n_regionkey
+        joined = region.inner_join(nation, pred)
+
+        result = joined[nation]
+        expected = joined.projection(nation)
+        assert_equal(result, expected)
+
+    def test_self_join(self):
+        # Self-joins are problematic with this design because column
+        # expressions may reference either the left or right self. For example:
+        #
+        # SELECT left.key, sum(left.value - right.value) as total_deltas
+        # FROM table left
+        #  INNER JOIN table right
+        #    ON left.current_period = right.previous_period + 1
+        # GROUP BY 1
+        #
+        # One way around the self-join issue is to force the user to add
+        # prefixes to the joined fields, then project using those. Not that
+        # satisfying, though.
+        left = self.table
+        right = self.table.view()
+        metric = (left['a'] - right['b']).mean().name('metric')
+
+        joined = left.inner_join(right, [right['g'] == left['g']])
+        # basic check there's no referential problems
+        result_repr = repr(joined)
+        assert 'ref_0' in result_repr
+        assert 'ref_1' in result_repr
+
+        # Cannot be immediately materialized because of the schema overlap
+        self.assertRaises(RelationError, joined.materialize)
+
+        # Project out left table schema
+        proj = joined[[left]]
+        assert_equal(proj.schema(), left.schema())
+
+        # Try aggregating on top of joined
+        aggregated = joined.aggregate([metric], by=[left['g']])
+        ex_schema = api.Schema(['g', 'metric'], ['string', 'double'])
+        assert_equal(aggregated.schema(), ex_schema)
+
+    def test_self_join_no_view_convenience(self):
+        # #165, self joins ought to be possible when the user specifies the
+        # column names to join on rather than referentially-valid expressions
+
+        result = self.table.join(self.table, [('g', 'g')])
+
+        t2 = self.table.view()
+        expected = self.table.join(t2, self.table.g == t2.g)
+        assert_equal(result, expected)
+
+    def test_materialized_join_reference_bug(self):
+        # GH#403
+        orders = self.con.table('tpch_orders')
+        customer = self.con.table('tpch_customer')
+        lineitem = self.con.table('tpch_lineitem')
+
+        items = (orders
+                 .join(lineitem, orders.o_orderkey == lineitem.l_orderkey)
+                 [lineitem, orders.o_custkey, orders.o_orderpriority]
+                 .join(customer, [('o_custkey', 'c_custkey')])
+                 .materialize())
+        items['o_orderpriority'].value_counts()
+
+    def test_join_project_after(self):
+        # e.g.
+        #
+        # SELECT L.foo, L.bar, R.baz, R.qux
+        # FROM table1 L
+        #   INNER JOIN table2 R
+        #     ON L.key = R.key
+        #
+        # or
+        #
+        # SELECT L.*, R.baz
+        # ...
+        #
+        # The default for a join is selecting all fields if possible
+        table1 = ibis.table([('key1',  'string'), ('value1', 'double')])
+        table2 = ibis.table([('key2',  'string'), ('stuff', 'int32')])
+
+        pred = table1['key1'] == table2['key2']
+
+        joined = table1.left_join(table2, [pred])
+        projected = joined.projection([table1, table2['stuff']])
+        assert projected.schema().names == ['key1', 'value1', 'stuff']
+
+        projected = joined.projection([table2, table1['key1']])
+        assert projected.schema().names == ['key2', 'stuff', 'key1']
+
+    def test_semi_join_schema(self):
+        # A left semi join discards the schema of the right table
+        table1 = ibis.table([('key1',  'string'), ('value1', 'double')])
+        table2 = ibis.table([('key2',  'string'), ('stuff', 'double')])
+
+        pred = table1['key1'] == table2['key2']
+        semi_joined = table1.semi_join(table2, [pred]).materialize()
+
+        result_schema = semi_joined.schema()
+        assert_equal(result_schema, table1.schema())
+
+    def test_cross_join(self):
+        agg_exprs = [self.table['a'].sum().name('sum_a'),
+                     self.table['b'].mean().name('mean_b')]
+        scalar_aggs = self.table.aggregate(agg_exprs)
+
+        joined = self.table.cross_join(scalar_aggs).materialize()
+        agg_schema = api.Schema(['sum_a', 'mean_b'], ['int64', 'double'])
+        ex_schema = self.table.schema().append(agg_schema)
+        assert_equal(joined.schema(), ex_schema)
+
+    def test_cross_join_multiple(self):
+        a = self.table['a', 'b', 'c']
+        b = self.table['d', 'e']
+        c = self.table['f', 'h']
+
+        joined = ibis.cross_join(a, b, c)
+        expected = a.cross_join(b.cross_join(c))
+        assert joined.equals(expected)
+
+    def test_join_compound_boolean_predicate(self):
+        # The user might have composed predicates through logical operations
+        pass
+
+    def test_filter_join_unmaterialized(self):
+        table1 = ibis.table({'key1': 'string', 'key2': 'string',
+                            'value1': 'double'})
+        table2 = ibis.table({'key3': 'string', 'value2': 'double'})
+
+        # It works!
+        joined = table1.inner_join(table2, [table1['key1'] == table2['key3']])
+        filtered = joined.filter([table1.value1 > 0])
+        repr(filtered)
+
+    def test_join_overlapping_column_names(self):
+        t1 = ibis.table([('foo', 'string'),
+                         ('bar', 'string'),
+                         ('value1', 'double')])
+        t2 = ibis.table([('foo', 'string'),
+                         ('bar', 'string'),
+                         ('value2', 'double')])
+
+        joined = t1.join(t2, 'foo')
+        expected = t1.join(t2, t1.foo == t2.foo)
+        assert_equal(joined, expected)
+
+        joined = t1.join(t2, ['foo', 'bar'])
+        expected = t1.join(t2, [t1.foo == t2.foo,
+                                t1.bar == t2.bar])
+        assert_equal(joined, expected)
+
+    def test_join_key_alternatives(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        # Join with tuples
+        joined = t1.inner_join(t2, [('foo_id', 'foo_id')])
+        joined2 = t1.inner_join(t2, [(t1.foo_id, t2.foo_id)])
+
+        # Join with single expr
+        joined3 = t1.inner_join(t2, t1.foo_id == t2.foo_id)
+
+        expected = t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+
+        assert_equal(joined, expected)
+        assert_equal(joined2, expected)
+        assert_equal(joined3, expected)
+
+        self.assertRaises(com.ExpressionError, t1.inner_join, t2,
+                          [('foo_id', 'foo_id', 'foo_id')])
+
+    def test_join_invalid_refs(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+        t3 = self.con.table('star3')
+
+        predicate = t1.bar_id == t3.bar_id
+        self.assertRaises(com.RelationError, t1.inner_join, t2, [predicate])
+
+    def test_join_non_boolean_expr(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        # oops
+        predicate = t1.f * t2.value1
+        self.assertRaises(com.ExpressionError, t1.inner_join, t2, [predicate])
+
+    def test_unravel_compound_equijoin(self):
+        t1 = ibis.table([
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('key3', 'string'),
+            ('value1', 'double')
+        ], 'foo_table')
+
+        t2 = ibis.table([
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('key3', 'string'),
+            ('value2', 'double')
+        ], 'bar_table')
+
+        p1 = t1.key1 == t2.key1
+        p2 = t1.key2 == t2.key2
+        p3 = t1.key3 == t2.key3
+
+        joined = t1.inner_join(t2, [p1 & p2 & p3])
+        expected = t1.inner_join(t2, [p1, p2, p3])
+        assert_equal(joined, expected)
+
+    def test_join_add_prefixes(self):
+        pass
+
+    def test_join_nontrivial_exprs(self):
+        pass
+
+    def test_union(self):
+        schema1 = [
+            ('key', 'string'),
+            ('value', 'double')
+        ]
+        schema2 = [
+            ('key', 'string'),
+            ('key2', 'string'),
+            ('value', 'double')
+        ]
+        t1 = ibis.table(schema1, 'foo')
+        t2 = ibis.table(schema1, 'bar')
+        t3 = ibis.table(schema2, 'baz')
+
+        result = t1.union(t2)
+        assert isinstance(result.op(), ops.Union)
+        assert not result.op().distinct
+
+        result = t1.union(t2, distinct=True)
+        assert isinstance(result.op(), ops.Union)
+        assert result.op().distinct
+
+        self.assertRaises(ir.RelationError, t1.union, t3)
+
+    def test_column_ref_on_projection_rename(self):
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+        customer = self.con.table('tpch_customer')
+
+        joined = (region.inner_join(
+            nation, [region.r_regionkey == nation.n_regionkey])
+            .inner_join(
+                customer, [customer.c_nationkey == nation.n_nationkey]))
+
+        proj_exprs = [customer, nation.n_name.name('nation'),
+                      region.r_name.name('region')]
+        joined = joined.projection(proj_exprs)
+
+        metrics = [joined.c_acctbal.sum().name('metric')]
+
+        # it works!
+        joined.aggregate(metrics, by=['region'])
+
+
+class TestSemiAntiJoinPredicates(unittest.TestCase):
+
+    def setUp(self):
+        self.con = MockConnection()
+
+        self.t1 = ibis.table([
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('value1', 'double')
+        ], 'foo')
+
+        self.t2 = ibis.table([
+            ('key1', 'string'),
+            ('key2', 'string')
+        ], 'bar')
+
+    def test_simple_existence_predicate(self):
+        cond = (self.t1.key1 == self.t2.key1).any()
+
+        assert isinstance(cond, ir.BooleanArray)
+        op = cond.op()
+        assert isinstance(op, ops.Any)
+
+        # it works!
+        expr = self.t1[cond]
+        assert isinstance(expr.op(), ops.Filter)
+
+    def test_cannot_use_existence_expression_in_join(self):
+        # Join predicates must consist only of comparisons
+        pass
+
+    def test_not_exists_predicate(self):
+        cond = -(self.t1.key1 == self.t2.key1).any()
+        assert isinstance(cond.op(), ops.NotAny)
+
+
+class TestLateBindingFunctions(BasicTestCase, unittest.TestCase):
+
+    def test_aggregate_metrics(self):
+        functions = [lambda x: x.e.sum().name('esum'),
+                     lambda x: x.f.sum().name('fsum')]
+        exprs = [self.table.e.sum().name('esum'),
+                 self.table.f.sum().name('fsum')]
+
+        result = self.table.aggregate(functions[0])
+        expected = self.table.aggregate(exprs[0])
+        assert_equal(result, expected)
+
+        result = self.table.aggregate(functions)
+        expected = self.table.aggregate(exprs)
+        assert_equal(result, expected)
+
+    def test_group_by_keys(self):
+        m = self.table.mutate(foo=self.table.f * 2,
+                              bar=self.table.e / 2)
+
+        expr = m.group_by(lambda x: x.foo).size()
+        expected = m.group_by('foo').size()
+        assert_equal(expr, expected)
+
+        expr = m.group_by([lambda x: x.foo, lambda x: x.bar]).size()
+        expected = m.group_by(['foo', 'bar']).size()
+        assert_equal(expr, expected)
+
+    def test_having(self):
+        m = self.table.mutate(foo=self.table.f * 2,
+                              bar=self.table.e / 2)
+
+        expr = (m.group_by('foo')
+                .having(lambda x: x.foo.sum() > 10)
+                .size())
+        expected = (m.group_by('foo')
+                    .having(m.foo.sum() > 10)
+                    .size())
+
+        assert_equal(expr, expected)
+
+    def test_filter(self):
+        m = self.table.mutate(foo=self.table.f * 2,
+                              bar=self.table.e / 2)
+
+        result = m.filter(lambda x: x.foo > 10)
+        result2 = m[lambda x: x.foo > 10]
+        expected = m[m.foo > 10]
+
+        assert_equal(result, expected)
+        assert_equal(result2, expected)
+
+        result = m.filter([lambda x: x.foo > 10,
+                           lambda x: x.bar < 0])
+        expected = m.filter([m.foo > 10, m.bar < 0])
+        assert_equal(result, expected)
+
+    def test_sort_by(self):
+        m = self.table.mutate(foo=self.table.e + self.table.f)
+
+        result = m.sort_by(lambda x: -x.foo)
+        expected = m.sort_by(-m.foo)
+        assert_equal(result, expected)
+
+        result = m.sort_by(lambda x: ibis.desc(x.foo))
+        expected = m.sort_by(ibis.desc('foo'))
+        assert_equal(result, expected)
+
+        result = m.sort_by(ibis.desc(lambda x: x.foo))
+        expected = m.sort_by(ibis.desc('foo'))
+        assert_equal(result, expected)
+
+    def test_projection(self):
+        m = self.table.mutate(foo=self.table.f * 2)
+
+        def f(x):
+            return (x.foo * 2).name('bar')
+
+        result = m.projection([f, 'f'])
+        result2 = m[f, 'f']
+        expected = m.projection([f(m), 'f'])
+        assert_equal(result, expected)
+        assert_equal(result2, expected)
+
+    def test_mutate(self):
+        m = self.table.mutate(foo=self.table.f * 2)
+
+        def g(x):
+            return x.foo * 2
+
+        def h(x):
+            return x.bar * 2
+
+        result = m.mutate(bar=g).mutate(baz=h)
+
+        m2 = m.mutate(bar=g(m))
+        expected = m2.mutate(baz=h(m2))
+
+        assert_equal(result, expected)
+
+    def test_add_column(self):
+        def g(x):
+            return x.f * 2
+
+        result = self.table.add_column(g, name='foo')
+        expected = self.table.mutate(foo=g)
+        assert_equal(result, expected)
+
+    def test_groupby_mutate(self):
+        t = self.table
+
+        g = t.group_by('g').order_by('f')
+        expr = g.mutate(foo=lambda x: x.f.lag(),
+                        bar=lambda x: x.f.rank())
+        expected = g.mutate(foo=t.f.lag(),
+                            bar=t.f.rank())
+
+        assert_equal(expr, expected)
+
+    def test_groupby_projection(self):
+        t = self.table
+
+        g = t.group_by('g').order_by('f')
+        expr = g.projection([lambda x: x.f.lag().name('foo'),
+                             lambda x: x.f.rank().name('bar')])
+        expected = g.projection([t.f.lag().name('foo'),
+                                 t.f.rank().name('bar')])
+
+        assert_equal(expr, expected)
+
+    def test_set_column(self):
+        def g(x):
+            return x.f * 2
+
+        result = self.table.set_column('f', g)
+        expected = self.table.set_column('f', self.table.f * 2)
+        assert_equal(result, expected)
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/compat.py` & `ibis-framework-v0.6.0/ibis/impala/compat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from __future__ import annotations
-
 # Copyright 2015 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import impala.dbapi as impyla
-from impala.error import Error as ImpylaError
-from impala.error import HiveServer2Error as HS2Error
 
-__all__ = (
-    "impyla",
-    "ImpylaError",
-    "HS2Error",
-)
+from impala.error import Error as ImpylaError  # noqa
+from impala.error import HiveServer2Error as HS2Error  # noqa
+import impala.dbapi as impyla  # noqa
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/ddl.py` & `ibis-framework-v0.6.0/ibis/impala/metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,335 +1,320 @@
-from __future__ import annotations
-
 # Copyright 2014 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
 
-from ibis.backends.base.sql.ddl import (
-    AlterTable,
-    BaseDDL,
-    CreateTable,
-    CreateTableWithSchema,
-    DropFunction,
-    format_partition,
-    format_schema,
-    format_tblproperties,
-)
-from ibis.backends.base.sql.registry import type_to_sql_string
-
-
-class CreateTableParquet(CreateTable):
-    def __init__(
-        self,
-        table_name,
-        path,
-        example_file=None,
-        example_table=None,
-        schema=None,
-        external=True,
-        **kwargs,
-    ):
-        super().__init__(
-            table_name,
-            external=external,
-            format='parquet',
-            path=path,
-            **kwargs,
-        )
-        self.example_file = example_file
-        self.example_table = example_table
-        self.schema = schema
+from six import StringIO
+import pandas as pd
 
-    @property
-    def _pieces(self):
-        if self.example_file is not None:
-            yield f"LIKE PARQUET '{self.example_file}'"
-        elif self.example_table is not None:
-            yield f"LIKE {self.example_table}"
-        elif self.schema is not None:
-            yield format_schema(self.schema)
+
+def parse_metadata(descr_table):
+    parser = MetadataParser(descr_table)
+    return parser.parse()
+
+
+def _noop(tup):
+    return None
+
+
+def _item_converter(i):
+    def _get_item(converter=None):
+        def _converter(tup):
+            result = tup[i]
+            if converter is not None:
+                result = converter(result)
+            return result
+
+        return _converter
+
+    return _get_item
+
+_get_type = _item_converter(1)
+_get_comment = _item_converter(2)
+
+
+def _try_timestamp(x):
+    try:
+        return pd.Timestamp(x)
+    except (ValueError, TypeError):
+        return x
+
+
+def _try_unix_timestamp(x):
+    try:
+        return pd.Timestamp.fromtimestamp(int(x))
+    except (ValueError, TypeError):
+        return x
+
+
+def _try_boolean(x):
+    try:
+        x = x.lower()
+        if x in ('true', 'yes'):
+            return True
+        elif x in ('false', 'no'):
+            return False
+        return x
+    except (ValueError, TypeError):
+        return x
+
+
+def _try_int(x):
+    try:
+        return int(x)
+    except (ValueError, TypeError):
+        return x
+
+
+class MetadataParser(object):
+
+    """
+    A simple state-ish machine to parse the results of DESCRIBE FORMATTED
+    """
+
+    def __init__(self, table):
+        self.table = table
+        self.tuples = list(self.table.itertuples(index=False))
+
+    def _reset(self):
+        self.pos = 0
+        self.schema = None
+        self.partitions = None
+        self.info = None
+        self.storage = None
+
+    def _next_tuple(self):
+        if self.pos == len(self.tuples):
+            raise StopIteration
+
+        result = self.tuples[self.pos]
+        self.pos += 1
+        return result
+
+    def parse(self):
+        self._reset()
+        self._parse()
+
+        return TableMetadata(self.schema, self.info, self.storage,
+                             partitions=self.partitions)
+
+    def _parse(self):
+        self.schema = self._parse_schema()
+
+        next_section = self._next_tuple()
+        if 'partition' in next_section[0].lower():
+            self._parse_partitions()
         else:
-            raise NotImplementedError
+            self._parse_info()
+
+    def _parse_partitions(self):
+        self.partitions = self._parse_schema()
+
+        next_section = self._next_tuple()
+        if 'table information' not in next_section[0].lower():
+            raise ValueError('Table information not present')
+
+        self._parse_info()
+
+    def _parse_schema(self):
+        tup = self._next_tuple()
+        if 'col_name' not in tup[0]:
+            raise ValueError('DESCRIBE FORMATTED did not return '
+                             'the expected results: {0}'
+                             .format(tup))
+        self._next_tuple()
+
+        # Use for both main schema and partition schema (if any)
+        schema = []
+        while True:
+            tup = self._next_tuple()
+            if tup[0].strip() == '':
+                break
+            schema.append((tup[0], tup[1]))
+
+        return schema
+
+    def _parse_info(self):
+        self.info = {}
+        while True:
+            tup = self._next_tuple()
+            orig_key = tup[0].strip(':')
+            key = _clean_param_name(tup[0])
+
+            if key == '' or key.startswith('#'):
+                # section is done
+                break
+
+            if key == 'table parameters':
+                self._parse_table_parameters()
+            elif key in self._info_cleaners:
+                result = self._info_cleaners[key](tup)
+                self.info[orig_key] = result
+            else:
+                self.info[orig_key] = tup[1]
+
+        if 'storage information' not in key:
+            raise ValueError('Storage information not present')
+
+        self._parse_storage_info()
+
+    _info_cleaners = {
+        'database': _get_type(),
+        'owner': _get_type(),
+        'createtime': _get_type(_try_timestamp),
+        'lastaccesstime': _get_type(_try_timestamp),
+        'protect mode': _get_type(),
+        'retention': _get_type(_try_int),
+        'location': _get_type(),
+        'table type': _get_type()
+    }
+
+    def _parse_table_parameters(self):
+        params = self._parse_nested_params(self._table_param_cleaners)
+        self.info['Table Parameters'] = params
+
+    _table_param_cleaners = {
+        'external': _try_boolean,
+        'column_stats_accurate': _try_boolean,
+        'numfiles': _try_int,
+        'totalsize': _try_int,
+        'stats_generated_via_stats_task': _try_boolean,
+        'numrows': _try_int,
+        'transient_lastddltime': _try_unix_timestamp,
+    }
+
+    def _parse_storage_info(self):
+        self.storage = {}
+        while True:
+            # end of the road
+            try:
+                tup = self._next_tuple()
+            except StopIteration:
+                break
+
+            orig_key = tup[0].strip(':')
+            key = _clean_param_name(tup[0])
+
+            if key == '' or key.startswith('#'):
+                # section is done
+                break
+
+            if key == 'storage desc params':
+                self._parse_storage_desc_params()
+            elif key in self._storage_cleaners:
+                result = self._storage_cleaners[key](tup)
+                self.storage[orig_key] = result
+            else:
+                self.storage[orig_key] = tup[1]
+
+    _storage_cleaners = {
+        'compressed': _get_type(_try_boolean),
+        'num buckets': _get_type(_try_int),
+    }
+
+    def _parse_storage_desc_params(self):
+        params = self._parse_nested_params(self._storage_param_cleaners)
+        self.storage['Desc Params'] = params
+
+    _storage_param_cleaners = {}
+
+    def _parse_nested_params(self, cleaners):
+        params = {}
+        while True:
+            try:
+                tup = self._next_tuple()
+            except StopIteration:
+                break
+            if pd.isnull(tup[1]):
+                break
+
+            key, value = tup[1:]
+
+            if key.lower() in cleaners:
+                cleaner = cleaners[key.lower()]
+                value = cleaner(value)
+            params[key] = value
+
+        return params
 
-        yield self._storage()
-        yield self._location()
 
+def _clean_param_name(x):
+    return x.strip().strip(':').lower()
 
-class DelimitedFormat:
-    def __init__(
-        self,
-        path,
-        delimiter=None,
-        escapechar=None,
-        na_rep=None,
-        lineterminator=None,
-    ):
-        self.path = path
-        self.delimiter = delimiter
-        self.escapechar = escapechar
-        self.lineterminator = lineterminator
-        self.na_rep = na_rep
-
-    def to_ddl(self):
-        yield 'ROW FORMAT DELIMITED'
-
-        if self.delimiter is not None:
-            yield f"FIELDS TERMINATED BY '{self.delimiter}'"
-
-        if self.escapechar is not None:
-            yield f"ESCAPED BY '{self.escapechar}'"
-
-        if self.lineterminator is not None:
-            yield f"LINES TERMINATED BY '{self.lineterminator}'"
-
-        yield 'STORED AS TEXTFILE'
-        yield f"LOCATION '{self.path}'"
-
-        if self.na_rep is not None:
-            props = {'serialization.null.format': self.na_rep}
-            yield format_tblproperties(props)
-
-
-class AvroFormat:
-    def __init__(self, path, avro_schema):
-        self.path = path
-        self.avro_schema = avro_schema
-
-    def to_ddl(self):
-        yield 'STORED AS AVRO'
-        yield f"LOCATION '{self.path}'"
-
-        schema = json.dumps(self.avro_schema, indent=2, sort_keys=True)
-        schema = '\n'.join(x.rstrip() for x in schema.splitlines())
-
-        props = {'avro.schema.literal': schema}
-        yield format_tblproperties(props)
-
-
-class ParquetFormat:
-    def __init__(self, path):
-        self.path = path
-
-    def to_ddl(self):
-        yield 'STORED AS PARQUET'
-        yield f"LOCATION '{self.path}'"
-
-
-class CreateTableDelimited(CreateTableWithSchema):
-    def __init__(
-        self,
-        table_name,
-        path,
-        schema,
-        delimiter=None,
-        escapechar=None,
-        lineterminator=None,
-        na_rep=None,
-        external=True,
-        **kwargs,
-    ):
-        table_format = DelimitedFormat(
-            path,
-            delimiter=delimiter,
-            escapechar=escapechar,
-            lineterminator=lineterminator,
-            na_rep=na_rep,
-        )
-        super().__init__(table_name, schema, table_format, external=external, **kwargs)
-
-
-class CreateTableAvro(CreateTable):
-    def __init__(self, table_name, path, avro_schema, external=True, **kwargs):
-        super().__init__(table_name, external=external, **kwargs)
-        self.table_format = AvroFormat(path, avro_schema)
 
+def _get_meta(attr, key):
     @property
-    def _pieces(self):
-        yield '\n'.join(self.table_format.to_ddl())
+    def f(self):
+        data = getattr(self, attr)
+        if isinstance(key, list):
+            result = data
+            for k in key:
+                if k not in result:
+                    raise KeyError(k)
+                result = result[k]
+            return result
+        else:
+            return data[key]
+    return f
 
 
-class LoadData(BaseDDL):
-    """Generate DDL for LOAD DATA command.
+class TableMetadata(object):
 
-    Cannot be cancelled
     """
+    Container for the parsed and wrangled results of DESCRIBE FORMATTED for
+    easier Ibis use (and testing).
+    """
+    def __init__(self, schema, info, storage, partitions=None):
+        self.schema = schema
+        self.info = info
+        self.storage = storage
+        self.partitions = partitions
+
+    def __repr__(self):
+        import pprint
+
+        # Quick and dirty for now
+        buf = StringIO()
+        buf.write(str(type(self)))
+        buf.write('\n')
+
+        data = {
+            'schema': self.schema,
+            'info': self.info,
+            'storage info': self.storage
+        }
+        if self.partitions is not None:
+            data['partition schema'] = self.partitions
 
-    def __init__(
-        self,
-        table_name,
-        path,
-        database=None,
-        partition=None,
-        partition_schema=None,
-        overwrite=False,
-    ):
-        self.table_name = table_name
-        self.database = database
-        self.path = path
-
-        self.partition = partition
-        self.partition_schema = partition_schema
+        pprint.pprint(data, stream=buf)
 
-        self.overwrite = overwrite
+        return buf.getvalue()
 
-    def compile(self):
-        overwrite = 'OVERWRITE ' if self.overwrite else ''
+    @property
+    def is_partitioned(self):
+        return self.partitions is not None
+
+    create_time = _get_meta('info', 'CreateTime')
+    location = _get_meta('info', 'Location')
+    owner = _get_meta('info', 'Owner')
+    num_rows = _get_meta('info', ['Table Parameters', 'numRows'])
+    hive_format = _get_meta('storage', 'InputFormat')
+
+    tbl_properties = _get_meta('info', 'Table Parameters')
+    serde_properties = _get_meta('storage', 'Desc Params')
+
+
+class TableInfo(object):
+    pass
 
-        if self.partition is not None:
-            partition = '\n' + format_partition(self.partition, self.partition_schema)
-        else:
-            partition = ''
 
-        scoped_name = self._get_scoped_name(self.table_name, self.database)
-        return "LOAD DATA INPATH '{}' {}INTO TABLE {}{}".format(
-            self.path, overwrite, scoped_name, partition
-        )
-
-
-class PartitionProperties(AlterTable):
-    def __init__(
-        self,
-        table,
-        partition,
-        partition_schema,
-        location=None,
-        format=None,
-        tbl_properties=None,
-        serde_properties=None,
-    ):
-        super().__init__(
-            table,
-            location=location,
-            format=format,
-            tbl_properties=tbl_properties,
-            serde_properties=serde_properties,
-        )
-        self.partition = partition
-        self.partition_schema = partition_schema
-
-    def _compile(self, cmd, property_prefix=''):
-        part = format_partition(self.partition, self.partition_schema)
-        if cmd:
-            part = f'{cmd} {part}'
-
-        props = self._format_properties(property_prefix)
-        action = f'{self.table} {part}{props}'
-        return self._wrap_command(action)
-
-
-class AddPartition(PartitionProperties):
-    def __init__(self, table, partition, partition_schema, location=None):
-        super().__init__(table, partition, partition_schema, location=location)
-
-    def compile(self):
-        return self._compile('ADD')
-
-
-class AlterPartition(PartitionProperties):
-    def compile(self):
-        return self._compile('', 'SET ')
-
-
-class DropPartition(PartitionProperties):
-    def __init__(self, table, partition, partition_schema):
-        super().__init__(table, partition, partition_schema)
-
-    def compile(self):
-        return self._compile('DROP')
-
-
-class CacheTable(BaseDDL):
-    def __init__(self, table_name, database=None, pool='default'):
-        self.table_name = table_name
-        self.database = database
-        self.pool = pool
-
-    def compile(self):
-        scoped_name = self._get_scoped_name(self.table_name, self.database)
-        return f"ALTER TABLE {scoped_name} SET CACHED IN '{self.pool}'"
-
-
-class CreateFunction(BaseDDL):
-    _object_type = 'FUNCTION'
-
-    def __init__(self, func, name=None, database=None):
-        self.func = func
-        self.name = name or func.name
-        self.database = database
-
-    def _impala_signature(self):
-        scoped_name = self._get_scoped_name(self.name, self.database)
-        input_sig = _impala_input_signature(self.func.inputs)
-        output_sig = type_to_sql_string(self.func.output)
-
-        return f'{scoped_name}({input_sig}) returns {output_sig}'
-
-
-class CreateUDF(CreateFunction):
-    def compile(self):
-        create_decl = 'CREATE FUNCTION'
-        impala_sig = self._impala_signature()
-        param_line = "location '{}' symbol='{}'".format(
-            self.func.lib_path, self.func.so_symbol
-        )
-        return ' '.join([create_decl, impala_sig, param_line])
-
-
-class CreateUDA(CreateFunction):
-    def compile(self):
-        create_decl = 'CREATE AGGREGATE FUNCTION'
-        impala_sig = self._impala_signature()
-        tokens = [f"location '{self.func.lib_path}'"]
-
-        fn_names = (
-            'init_fn',
-            'update_fn',
-            'merge_fn',
-            'serialize_fn',
-            'finalize_fn',
-        )
-
-        for fn in fn_names:
-            value = getattr(self.func, fn)
-            if value is not None:
-                tokens.append(f"{fn}='{value}'")
-
-        return ' '.join([create_decl, impala_sig]) + ' ' + '\n'.join(tokens)
-
-
-class DropFunction(DropFunction):
-    def _impala_signature(self):
-        full_name = self._get_scoped_name(self.name, self.database)
-        input_sig = _impala_input_signature(self.inputs)
-        return f'{full_name}({input_sig})'
-
-
-class ListFunction(BaseDDL):
-    def __init__(self, database, like=None, aggregate=False):
-        self.database = database
-        self.like = like
-        self.aggregate = aggregate
-
-    def compile(self):
-        statement = 'SHOW '
-        if self.aggregate:
-            statement += 'AGGREGATE '
-        statement += f'FUNCTIONS IN {self.database}'
-        if self.like:
-            statement += f" LIKE '{self.like}'"
-        return statement
-
-
-def _impala_input_signature(inputs):
-    # TODO: varargs '{}...'.format(val)
-    return ', '.join(map(type_to_sql_string, inputs))
+class TableStorageInfo(object):
+    pass
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/metadata.py` & `ibis-framework-v0.6.0/ibis/impala/tests/test_partition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,253 @@
-from __future__ import annotations
-
 # Copyright 2014 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from io import StringIO
 
+from posixpath import join as pjoin
+import pytest
+
+from pandas.util.testing import assert_frame_equal
+import pandas as pd
 
-def parse_metadata(descr_table):
-    parser = MetadataParser(descr_table)
-    return parser.parse()
-
-
-def _noop(tup):
-    return None
-
-
-def _item_converter(i):
-    def _get_item(converter=None):
-        def _converter(tup):
-            result = tup[i]
-            if converter is not None:
-                result = converter(result)
-            return result
-
-        return _converter
-
-    return _get_item
-
-
-_get_type = _item_converter(1)
-_get_comment = _item_converter(2)
-
-
-def _try_timestamp(x):
-    import pandas as pd
-
-    try:
-        ts = pd.Timestamp(x, tz='UTC')
-        return ts.to_pydatetime().replace(tzinfo=None)
-    except (ValueError, TypeError):
-        return x
-
-
-def _try_unix_timestamp(x):
-    try:
-        value = int(x)
-    except (ValueError, TypeError):
-        return x
-    else:
-        import pandas as pd
-
-        return (
-            pd.Timestamp.fromtimestamp(value, tz="UTC")
-            .tz_localize(None)
-            .to_pydatetime()
-        )
-
-
-def _try_boolean(x):
-    try:
-        x = x.lower()
-        if x in ('true', 'yes'):
-            return True
-        elif x in ('false', 'no'):
-            return False
-        return x
-    except (ValueError, TypeError):
-        return x
-
-
-def _try_int(x):
-    try:
-        return int(x)
-    except (ValueError, TypeError):
-        return x
-
-
-class MetadataParser:
-    """A simple state machine to parse the results of `DESCRIBE FORMATTED`."""
-
-    def __init__(self, table):
-        self.table = table
-        self.tuples = list(self.table.itertuples(index=False))
-
-    def _reset(self):
-        self.pos = 0
-        self.schema = None
-        self.partitions = None
-        self.info = None
-        self.storage = None
-
-    def _next_tuple(self):
-        if self.pos == len(self.tuples):
-            raise StopIteration
-
-        result = self.tuples[self.pos]
-        self.pos += 1
-        return result
-
-    def parse(self):
-        self._reset()
-        self._parse()
-
-        return TableMetadata(
-            self.schema, self.info, self.storage, partitions=self.partitions
-        )
-
-    def _parse(self):
-        self.schema = self._parse_schema()
-
-        next_section = self._next_tuple()
-        if 'partition' in next_section[0].lower():
-            self._parse_partitions()
-        else:
-            self._parse_info()
-
-    def _parse_partitions(self):
-        self.partitions = self._parse_schema()
-
-        next_section = self._next_tuple()
-        if 'table information' not in next_section[0].lower():
-            raise ValueError('Table information not present')
-
-        self._parse_info()
-
-    def _parse_schema(self):
-        tup = self._next_tuple()
-        if 'col_name' not in tup[0]:
-            raise ValueError(
-                'DESCRIBE FORMATTED did not return '
-                'the expected results: {}'.format(tup)
-            )
-        self._next_tuple()
-
-        # Use for both main schema and partition schema (if any)
-        schema = []
-        while True:
-            tup = self._next_tuple()
-            if not tup[0].strip():
-                break
-            schema.append((tup[0], tup[1]))
-
-        return schema
-
-    def _parse_info(self):
-        self.info = {}
-        while True:
-            tup = self._next_tuple()
-            orig_key = tup[0].strip(':')
-            key = _clean_param_name(tup[0])
-
-            if not key or key.startswith('#'):
-                # section is done
-                break
-
-            if key == 'table parameters':
-                self._parse_table_parameters()
-            elif key in self._info_cleaners:
-                result = self._info_cleaners[key](tup)
-                self.info[orig_key] = result
+from ibis.compat import unittest
+from ibis.impala.compat import ImpylaError
+from ibis.impala.tests.common import ImpalaE2E
+from ibis.tests.util import assert_equal
+import ibis
+import ibis.util as util
+
+
+def _tmp_name():
+    return 'tmp_partition_{0}'.format(util.guid())
+
+
+class TestPartitioning(ImpalaE2E, unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        ImpalaE2E.setup_e2e(cls)
+
+        df = pd.DataFrame({'year': [2009, 2009, 2009, 2010, 2010, 2010],
+                           'month': [1, 2, 3, 1, 2, 3],
+                           'value': [1, 2, 3, 4, 5, 6]})
+        df = pd.concat([df] * 10, ignore_index=True)
+        df['id'] = df.index.values
+
+        cls.df = df
+        cls.db = cls.con.database(cls.tmp_db)
+        cls.pd_name = _tmp_name()
+        cls.db.create_table(cls.pd_name, df,
+                            location=cls._temp_location())
+
+    @classmethod
+    def _temp_location(cls):
+        return cls._create_777_tmp_dir()
+
+    def test_is_partitioned(self):
+        schema = ibis.schema([('foo', 'string'),
+                              ('year', 'int32'),
+                              ('month', 'int16')])
+        name = _tmp_name()
+        self.db.create_table(name, schema=schema,
+                             partition=['year', 'month'],
+                             location=self._temp_location())
+        assert self.db.table(name).is_partitioned
+
+    @pytest.mark.superuser
+    def test_create_table_with_partition_column(self):
+        schema = ibis.schema([('year', 'int32'),
+                              ('month', 'int8'),
+                              ('day', 'int8'),
+                              ('value', 'double')])
+
+        name = _tmp_name()
+        self.con.create_table(name, schema=schema,
+                              database=self.tmp_db,
+                              partition=['year', 'month'],
+                              location=self._temp_location())
+        self.temp_tables.append(name)
+
+        # the partition column get put at the end of the table
+        ex_schema = ibis.schema([('day', 'int8'),
+                                 ('value', 'double'),
+                                 ('year', 'int32'),
+                                 ('month', 'int8')])
+        table_schema = self.con.get_schema(name, database=self.tmp_db)
+        assert_equal(table_schema, ex_schema)
+
+        partition_schema = self.db.table(name).partition_schema()
+
+        expected = ibis.schema([('year', 'int32'),
+                                ('month', 'int8')])
+        assert_equal(partition_schema, expected)
+
+    @pytest.mark.superuser
+    def test_create_partitioned_separate_schema(self):
+        schema = ibis.schema([('day', 'int8'),
+                              ('value', 'double')])
+        part_schema = ibis.schema([('year', 'int32'),
+                                   ('month', 'int8')])
+
+        name = _tmp_name()
+        self.con.create_table(name, schema=schema, partition=part_schema,
+                              location=self._temp_location())
+        self.temp_tables.append(name)
+
+        # the partition column get put at the end of the table
+        ex_schema = ibis.schema([('day', 'int8'),
+                                 ('value', 'double'),
+                                 ('year', 'int32'),
+                                 ('month', 'int8')])
+        table_schema = self.con.get_schema(name)
+        assert_equal(table_schema, ex_schema)
+
+        partition_schema = self.con.table(name).partition_schema()
+        assert_equal(partition_schema, part_schema)
+
+    @pytest.mark.superuser
+    def test_unpartitioned_table_get_schema(self):
+        tname = 'functional_alltypes'
+        with self.assertRaises(ImpylaError):
+            self.con.table(tname).partition_schema()
+
+    @pytest.mark.superuser
+    def test_insert_select_partitioned_table(self):
+        df = self.df
+
+        unpart_t = self.db.table(self.pd_name)
+        part_keys = ['year', 'month']
+        part_t = self._create_partitioned_table(unpart_t.schema(),
+                                                part_keys)
+        unique_keys = df[part_keys].drop_duplicates()
+
+        for i, (year, month) in enumerate(unique_keys.itertuples(index=False)):
+            select_stmt = unpart_t[(unpart_t.year == year) &
+                                   (unpart_t.month == month)]
+
+            # test both styles of insert
+            if i:
+                part = {'year': year, 'month': month}
             else:
-                self.info[orig_key] = tup[1]
+                part = [year, month]
+            part_t.insert(select_stmt, partition=part)
 
-        if 'storage information' not in key:
-            raise ValueError('Storage information not present')
+        self._verify_partitioned_table(part_t, df, unique_keys)
 
-        self._parse_storage_info()
+    @pytest.mark.superuser
+    def test_insert_overwrite_partition(self):
+        pass
 
-    _info_cleaners = {
-        'database': _get_type(),
-        'owner': _get_type(),
-        'createtime': _get_type(_try_timestamp),
-        'lastaccesstime': _get_type(_try_timestamp),
-        'protect mode': _get_type(),
-        'retention': _get_type(_try_int),
-        'location': _get_type(),
-        'table type': _get_type(),
-    }
-
-    def _parse_table_parameters(self):
-        params = self._parse_nested_params(self._table_param_cleaners)
-        self.info['Table Parameters'] = params
-
-    _table_param_cleaners = {
-        'external': _try_boolean,
-        'column_stats_accurate': _try_boolean,
-        'numfiles': _try_int,
-        'totalsize': _try_int,
-        'stats_generated_via_stats_task': _try_boolean,
-        'numrows': _try_int,
-        'transient_lastddltime': _try_unix_timestamp,
-    }
-
-    def _parse_storage_info(self):
-        self.storage = {}
-        while True:
-            # end of the road
-            try:
-                tup = self._next_tuple()
-            except StopIteration:
-                break
-
-            orig_key = tup[0].strip(':')
-            key = _clean_param_name(tup[0])
-
-            if not key or key.startswith('#'):
-                # section is done
-                break
-
-            if key == 'storage desc params':
-                self._parse_storage_desc_params()
-            elif key in self._storage_cleaners:
-                result = self._storage_cleaners[key](tup)
-                self.storage[orig_key] = result
-            else:
-                self.storage[orig_key] = tup[1]
+    @pytest.mark.superuser
+    def test_dynamic_partitioning(self):
+        pass
 
-    _storage_cleaners = {
-        'compressed': _get_type(_try_boolean),
-        'num buckets': _get_type(_try_int),
-    }
-
-    def _parse_storage_desc_params(self):
-        params = self._parse_nested_params(self._storage_param_cleaners)
-        self.storage['Desc Params'] = params
-
-    _storage_param_cleaners = {}
-
-    def _parse_nested_params(self, cleaners):
-        import pandas as pd
-
-        params = {}
-        while True:
-            try:
-                tup = self._next_tuple()
-            except StopIteration:
-                break
-            if pd.isnull(tup[1]):
-                break
-
-            key, value = tup[1:]
-
-            if key.lower() in cleaners:
-                cleaner = cleaners[key.lower()]
-                value = cleaner(value)
-            params[key] = value
-
-        return params
-
-
-def _clean_param_name(x):
-    return x.strip().strip(':').lower()
-
-
-def _get_meta(attr, key):
-    @property
-    def f(self):
-        data = getattr(self, attr)
-        if isinstance(key, list):
-            result = data
-            for k in key:
-                if k not in result:
-                    raise KeyError(k)
-                result = result[k]
-            return result
-        else:
-            return data[key]
-
-    return f
-
-
-class TableMetadata:
-    """Container for the parsed and wrangled results of `DESCRIBE FORMATTED`."""
-
-    def __init__(self, schema, info, storage, partitions=None):
-        self.schema = schema
-        self.info = info
-        self.storage = storage
-        self.partitions = partitions
-
-    def __repr__(self):
-        import pprint
-
-        # Quick and dirty for now
-        buf = StringIO()
-        buf.write(str(type(self)))
-        buf.write('\n')
-
-        data = {
-            'schema': self.schema,
-            'info': self.info,
-            'storage info': self.storage,
-        }
-        if self.partitions is not None:
-            data['partition schema'] = self.partitions
+    @pytest.mark.superuser
+    def test_add_drop_partition(self):
+        schema = ibis.schema([('foo', 'string'),
+                              ('year', 'int32'),
+                              ('month', 'int16')])
+        name = _tmp_name()
+        tmp_dir = self._temp_location()
+        self.db.create_table(name, schema=schema,
+                             partition=['year', 'month'],
+                             location=tmp_dir)
+
+        table = self.db.table(name)
+
+        part = {'year': 2007, 'month': 4}
+
+        path = '/tmp/tmp-{0}'.format(util.guid())
+        table.add_partition(part, location=path)
 
-        pprint.pprint(data, stream=buf)  # noqa: T203
+        assert len(table.partitions()) == 2
 
-        return buf.getvalue()
+        table.drop_partition(part)
 
-    @property
-    def is_partitioned(self):
-        return self.partitions is not None
+        assert len(table.partitions()) == 1
 
-    create_time = _get_meta('info', 'CreateTime')
-    location = _get_meta('info', 'Location')
-    owner = _get_meta('info', 'Owner')
-    num_rows = _get_meta('info', ['Table Parameters', 'numRows'])
-    hive_format = _get_meta('storage', 'InputFormat')
+    @pytest.mark.superuser
+    def test_set_partition_location(self):
+        pass
 
-    tbl_properties = _get_meta('info', 'Table Parameters')
-    serde_properties = _get_meta('storage', 'Desc Params')
+    @pytest.mark.superuser
+    def test_load_data_partition(self):
+        df = self.df
 
+        unpart_t = self.db.table(self.pd_name)
+        part_keys = ['year', 'month']
+        part_t = self._create_partitioned_table(unpart_t.schema(),
+                                                part_keys)
 
-class TableInfo:
-    pass
+        # trim the runtime of this test
+        df = df[df.month == 1].reset_index(drop=True)
 
+        unique_keys = df[part_keys].drop_duplicates()
+
+        hdfs_dir = pjoin(self.tmp_dir, 'load-data-partition')
+
+        df2 = df.drop(['year', 'month'], axis='columns')
+
+        csv_props = {
+            'serialization.format': ',',
+            'field.delim': ','
+        }
+
+        for i, (year, month) in enumerate(unique_keys.itertuples(index=False)):
+            chunk = df2[(df.year == year) & (df.month == month)]
+            chunk_path = pjoin(hdfs_dir, '{0}.csv'.format(i))
+
+            self.con.write_dataframe(chunk, chunk_path)
+
+            # test both styles of insert
+            if i:
+                part = {'year': year, 'month': month}
+            else:
+                part = [year, month]
 
-class TableStorageInfo:
-    pass
+            part_t.add_partition(part)
+            part_t.alter_partition(part, format='text',
+                                   serde_properties=csv_props)
+            part_t.load_data(chunk_path, partition=part)
+
+        self.hdfs.rmdir(hdfs_dir)
+        self._verify_partitioned_table(part_t, df, unique_keys)
+
+    def _verify_partitioned_table(self, part_t, df, unique_keys):
+        result = (part_t.execute()
+                  .sort_index(by='id')
+                  .reset_index(drop=True)
+                  [df.columns])
+
+        assert_frame_equal(result, df)
+
+        parts = part_t.partitions()
+
+        # allow for the total line
+        assert len(parts) == (len(unique_keys) + 1)
+
+    def _create_partitioned_table(self, schema, part_keys):
+        part_name = _tmp_name()
+
+        self.db.create_table(part_name,
+                             schema=schema,
+                             partition=part_keys,
+                             location=self._temp_location())
+        self.temp_tables.append(part_name)
+        return self.db.table(part_name)
+
+    @pytest.mark.superuser
+    def test_drop_partition(self):
+        pass
+
+    @pytest.mark.superuser
+    def test_repartition_automated(self):
+        pass
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/tests/conftest.py` & `ibis-framework-v0.6.0/scripts/test_data_admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,551 +1,517 @@
-from __future__ import annotations
+#! /usr/bin/env python
+# Copyright 2015 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import ast
-import collections
-import concurrent.futures
-import contextlib
-import itertools
 import os
-import subprocess
-from pathlib import Path
-from typing import Any, Iterator
+import shutil
+import tempfile
+import os.path as osp
+from os.path import join as pjoin
+from subprocess import check_call
 
-import pytest
+from click import group, option
 
 import ibis
-import ibis.expr.types as ir
-from ibis import options, util
-from ibis.backends.base import BaseBackend
-from ibis.backends.conftest import TEST_TABLES, _random_identifier
-from ibis.backends.impala.compiler import ImpalaCompiler, ImpalaExprTranslator
-from ibis.backends.tests.base import BackendTest, RoundAwayFromZero, UnorderedComparator
-from ibis.backends.tests.data import win
-from ibis.tests.expr.mocks import MockBackend
-
-
-class TestConf(UnorderedComparator, BackendTest, RoundAwayFromZero):
-    supports_arrays = True
-    supports_arrays_outside_of_select = False
-    check_dtype = False
-    supports_divide_by_zero = True
-    returned_timestamp_unit = 's'
-    supports_structs = False
-    supports_json = False
-
-    @staticmethod
-    def _load_data(data_dir: Path, script_dir: Path, **_: Any) -> None:
-        """Load test data into an Impala backend instance.
-
-        Parameters
-        ----------
-        data_dir
-            Location of test data
-        script_dir
-            Location of scripts defining schemas
-        """
-        fsspec = pytest.importorskip("fsspec")
-        fs = fsspec.filesystem("file")
-
-        data_files = {
-            data_file
-            for data_file in fs.find(data_dir)
-            # ignore sqlite databases and markdown files
-            if not data_file.endswith((".db", ".md"))
-            # ignore files in the test data .git directory
-            if (
-                # ignore .git
-                os.path.relpath(data_file, data_dir).split(os.sep, 1)[0]
-                != ".git"
-            )
-        }
-
-        # without setting the pool size
-        # connections are dropped from the urllib3
-        # connection pool when the number of workers exceeds this value.
-        # this doesn't appear to be configurable through fsspec
-        URLLIB_DEFAULT_POOL_SIZE = 10
-
-        env = IbisTestEnv()
-        with contextlib.closing(
-            ibis.impala.connect(
-                host=env.impala_host,
-                port=env.impala_port,
-                hdfs_client=fsspec.filesystem(
-                    env.hdfs_protocol,
-                    host=env.nn_host,
-                    port=env.hdfs_port,
-                    user=env.hdfs_user,
-                ),
-                pool_size=URLLIB_DEFAULT_POOL_SIZE,
-            )
-        ) as con, concurrent.futures.ThreadPoolExecutor(
-            max_workers=int(
-                os.environ.get("IBIS_DATA_MAX_WORKERS", URLLIB_DEFAULT_POOL_SIZE)
-            )
-        ) as executor:
-            hdfs = con.hdfs
-            tasks = {
-                # make the database
-                executor.submit(impala_create_test_database, con, env),
-                # build and upload UDFs
-                *itertools.starmap(
-                    executor.submit,
-                    impala_build_and_upload_udfs(hdfs, env, fs=fs),
-                ),
-                # upload data files
-                *(
-                    executor.submit(
-                        hdfs_make_dir_and_put_file,
-                        hdfs,
-                        data_file,
-                        os.path.join(
-                            env.test_data_dir,
-                            os.path.relpath(data_file, data_dir),
-                        ),
-                    )
-                    for data_file in data_files
-                ),
-            }
-
-            for future in concurrent.futures.as_completed(tasks):
-                future.result()
-
-            # create the tables and compute stats
-            for future in concurrent.futures.as_completed(
-                executor.submit(table_future.result().compute_stats)
-                for table_future in concurrent.futures.as_completed(
-                    impala_create_tables(con, env, executor=executor)
-                )
-            ):
-                future.result()
-
-    @staticmethod
-    def connect(
-        data_directory: Path,
-        database: str
-        | None = os.environ.get("IBIS_TEST_DATA_DB", "ibis_testing"),  # noqa: B008
-        with_hdfs: bool = True,
-    ):
-        fsspec = pytest.importorskip("fsspec")
-
-        env = IbisTestEnv()
-        return ibis.impala.connect(
-            host=env.impala_host,
-            port=env.impala_port,
-            auth_mechanism=env.auth_mechanism,
-            hdfs_client=fsspec.filesystem(
-                env.hdfs_protocol,
-                host=env.nn_host,
-                port=env.hdfs_port,
-                user=env.hdfs_user,
-            )
-            if with_hdfs
-            else None,
-            database=database,
-        )
-
-    def _get_original_column_names(self, tablename: str) -> list[str]:
-        return list(TEST_TABLES[tablename].names)
-
-    def _get_renamed_table(self, tablename: str) -> ir.Table:
-        t = self.connection.table(tablename)
-        original_names = self._get_original_column_names(tablename)
-        return t.relabel(dict(zip(t.columns, original_names)))
-
-    @property
-    def batting(self) -> ir.Table:
-        return self._get_renamed_table("batting")
-
-    @property
-    def awards_players(self) -> ir.Table:
-        return self._get_renamed_table("awards_players")
-
-
-class IbisTestEnv:
-    def __init__(self):
-        if options.impala is None:
-            ibis.backends.impala.Backend.register_options()
-
-    @property
-    def impala_host(self):
-        return os.environ.get('IBIS_TEST_IMPALA_HOST', 'localhost')
-
-    @property
-    def impala_port(self):
-        return int(os.environ.get('IBIS_TEST_IMPALA_PORT', "21050"))
-
-    @property
-    def tmp_db(self):
-        options.impala.temp_db = tmp_db = os.environ.get(
-            'IBIS_TEST_TMP_DB', 'ibis_testing_tmp_db'
-        )
-        return tmp_db
-
-    @property
-    def tmp_dir(self):
-        options.impala.temp_hdfs_path = tmp_dir = os.environ.get(
-            'IBIS_TEST_TMP_HDFS_DIR', f'/tmp/__ibis_test_{util.guid()}'
-        )
-        return tmp_dir
-
-    @property
-    def test_data_db(self):
-        return os.environ.get('IBIS_TEST_DATA_DB', 'ibis_testing')
-
-    @property
-    def test_data_dir(self):
-        return os.environ.get('IBIS_TEST_DATA_HDFS_DIR', '/__ibis/ibis-testing-data')
-
-    @property
-    def nn_host(self):
-        return os.environ.get('IBIS_TEST_NN_HOST', 'localhost')
-
-    @property
-    def hdfs_port(self):
-        return int(os.environ.get('IBIS_TEST_HDFS_PORT', 50070))
-
-    @property
-    def hdfs_superuser(self):
-        return os.environ.get('IBIS_TEST_HDFS_SUPERUSER', 'hdfs')
-
-    @property
-    def use_codegen(self):
-        return ast.literal_eval(
-            os.environ.get('IBIS_TEST_USE_CODEGEN', 'False').lower().capitalize()
-        )
-
-    @property
-    def auth_mechanism(self):
-        return os.environ.get('IBIS_TEST_AUTH_MECH', 'NOSASL')
-
-    @property
-    def hdfs_user(self):
-        return os.environ.get('IBIS_TEST_HDFS_USER', 'hdfs')
-
-    @property
-    def hdfs_protocol(self):
-        return os.environ.get("IBIS_TEST_HDFS_PROTOCOL", "webhdfs")
-
-
-@pytest.fixture(scope="session")
-def env():
-    return IbisTestEnv()
-
-
-@pytest.fixture(scope="session")
-def tmp_dir(env):
-    options.impala.temp_hdfs_path = tmp_dir = env.tmp_dir
-    return tmp_dir
-
-
-@pytest.fixture(scope="session")
-def test_data_db(env):
-    return env.test_data_db
-
-
-@pytest.fixture(scope="session")
-def test_data_dir(env):
-    return env.test_data_dir
-
-
-@pytest.fixture(scope="session")
-def hdfs(env, tmp_dir):
-    fsspec = pytest.importorskip("fsspec")
-    client = fsspec.filesystem(
-        env.hdfs_protocol,
-        host=env.nn_host,
-        port=env.hdfs_port,
-        user=env.hdfs_user,
-    )
-
-    if not client.exists(tmp_dir):
-        client.mkdir(tmp_dir)
-    return client
-
-
-@pytest.fixture(scope="session")
-def backend(tmp_path_factory, data_directory, script_directory, worker_id):
-    return TestConf.load_data(
-        data_directory,
-        script_directory,
-        tmp_path_factory,
-        worker_id,
-    )
-
-
-@pytest.fixture(scope="module")
-def con_no_hdfs(env, data_directory, backend):
-    con = backend.connect(data_directory, with_hdfs=False)
-    con.disable_codegen(disabled=not env.use_codegen)
-    assert con.get_options()['DISABLE_CODEGEN'] == str(int(not env.use_codegen))
-    try:
-        yield con
-    finally:
-        con.close()
-
-
-@pytest.fixture(scope="module")
-def con(env, data_directory, backend):
-    con = backend.connect(data_directory)
-    con.disable_codegen(disabled=not env.use_codegen)
-    assert con.get_options()['DISABLE_CODEGEN'] == str(int(not env.use_codegen))
-    try:
-        yield con
-    finally:
-        con.close()
-
-
-@pytest.fixture
-def tmp_db(env, con, test_data_db):
-    impala = pytest.importorskip("impala")
-
-    tmp_db = env.tmp_db
-
-    if tmp_db not in con.list_databases():
-        con.create_database(tmp_db)
-    try:
-        yield tmp_db
-    finally:
-        with contextlib.suppress(impala.error.HiveServer2Error):
-            # The database can be dropped by another process during tear down
-            # in the middle of dropping this one if tests are running in
-            # parallel.
-            #
-            # We only care that it gets dropped before all tests are finished
-            # running.
-            con.drop_database(tmp_db, force=True)
-
-
-@pytest.fixture(scope="module")
-def con_no_db(env, data_directory, backend):
-    con = backend.connect(data_directory, database=None)
-    if not env.use_codegen:
-        con.disable_codegen()
-    assert con.get_options()['DISABLE_CODEGEN'] == '1'
-    try:
-        yield con
-    finally:
-        con.close()
-
-
-@pytest.fixture(scope="module")
-def alltypes(con):
-    return con.table("functional_alltypes")
-
-
-@pytest.fixture(scope="module")
-def alltypes_df(alltypes):
-    return alltypes.execute()
-
-
-@pytest.fixture
-def temp_database(con, test_data_db):
-    name = _random_identifier('database')
-    con.create_database(name)
-    try:
-        yield name
-    finally:
-        con.drop_database(name, force=True)
-
-
-@pytest.fixture
-def temp_table(con):
-    name = _random_identifier('table')
-    try:
-        yield name
-    finally:
-        assert name in con.list_tables(), name
-        con.drop_table(name)
-
-
-@pytest.fixture
-def temp_table_db(con, temp_database):
-    name = _random_identifier('table')
-    try:
-        yield temp_database, name
-    finally:
-        assert name in con.list_tables(database=temp_database), name
-        con.drop_table(name, database=temp_database)
-
-
-@pytest.fixture
-def temp_view(con):
-    name = _random_identifier('view')
-    try:
-        yield name
-    finally:
-        assert name in con.list_tables(), name
-        con.drop_view(name)
-
-
-@pytest.fixture
-def temp_parquet_table_schema():
-    return ibis.schema([('id', 'int32'), ('name', 'string'), ('files', 'int32')])
-
-
-@pytest.fixture
-def temp_parquet_table(con, tmp_db, temp_parquet_table_schema):
-    name = util.guid()
-    db = con.database(tmp_db)
-    db.create_table(name, schema=temp_parquet_table_schema, format='parquet')
-    try:
-        yield db[name]
-    finally:
-        db.client.drop_table(name, database=tmp_db)
-
-
-@pytest.fixture
-def temp_parquet_table2(con, tmp_db, temp_parquet_table_schema):
-    name = util.guid()
-    db = con.database(tmp_db)
-    db.create_table(name, schema=temp_parquet_table_schema, format='parquet')
-    try:
-        yield db[name]
-    finally:
-        db.client.drop_table(name, database=tmp_db)
-
+from ibis.compat import BytesIO
+from ibis.common import IbisError
+from ibis.impala.tests.common import IbisTestEnv
+from ibis.util import guid
+
+import numpy as np
+
+import pandas as pd
+import pandas.util.testing as tm
+
+ENV = IbisTestEnv()
+IBIS_TEST_DATA_S3_BUCKET = 'ibis-resources'
+IBIS_TEST_DATA_LOCAL_DIR = 'ibis-testing-data'
+
+TARBALL_NAME = 'ibis-testing-data.tar.gz'
+IBIS_TEST_DATA_TARBALL = 'testing/{0}'.format(TARBALL_NAME)
+
+
+IBIS_TEST_AWS_KEY_ID = os.environ.get('IBIS_TEST_AWS_KEY_ID')
+IBIS_TEST_AWS_SECRET = os.environ.get('IBIS_TEST_AWS_SECRET')
+
+
+def make_ibis_client():
+    hc = ibis.hdfs_connect(host=ENV.nn_host, port=ENV.webhdfs_port,
+                           auth_mechanism=ENV.auth_mechanism,
+                           verify=(ENV.auth_mechanism
+                                   not in ['GSSAPI', 'LDAP']))
+    if ENV.auth_mechanism in ['GSSAPI', 'LDAP']:
+        print("Warning: ignoring invalid Certificate Authority errors")
+    return ibis.impala.connect(host=ENV.impala_host, port=ENV.impala_port,
+                               auth_mechanism=ENV.auth_mechanism,
+                               hdfs_client=hc)
+
+
+def can_write_to_hdfs(con):
+    test_path = pjoin(ENV.test_data_dir, ibis.util.guid())
+    test_file = BytesIO(ibis.util.guid().encode('utf-8'))
+    try:
+        con.hdfs.put(test_path, test_file)
+        con.hdfs.rm(test_path)
+        return True
+    except:
+        return False
+
+
+def can_build_udfs():
+    try:
+        check_call('which cmake', shell=True)
+    except:
+        print('Could not find cmake on PATH')
+        return False
+    try:
+        check_call('which make', shell=True)
+    except:
+        print('Could not find make on PATH')
+        return False
+    try:
+        check_call('which clang++', shell=True)
+    except:
+        print('Could not find LLVM on PATH; if IBIS_TEST_LLVM_CONFIG is set, '
+              'try setting PATH="$($IBIS_TEST_LLVM_CONFIG --bindir):$PATH"')
+        return False
+    return True
+
+
+def is_data_loaded(con):
+    if not con.hdfs.exists(ENV.test_data_dir):
+        return False
+    if not con.exists_database(ENV.test_data_db):
+        return False
+    return True
+
+
+def is_udf_loaded(con):
+    bitcode_dir = pjoin(ENV.test_data_dir, 'udf')
+    if con.hdfs.exists(bitcode_dir):
+        return True
+    return False
+
+
+def dnload_ibis_test_data_from_s3(local_path):
+    url = 'https://{0}.s3.amazonaws.com/{1}'.format(
+        IBIS_TEST_DATA_S3_BUCKET, IBIS_TEST_DATA_TARBALL)
+    cmd = 'cd {0} && wget -q {1} && tar -xzf {2}'.format(
+        local_path, url, TARBALL_NAME)
+    check_call(cmd, shell=True)
+    data_dir = pjoin(local_path, IBIS_TEST_DATA_LOCAL_DIR)
+    print('Downloaded {0} and unpacked it to {1}'.format(url, data_dir))
+    return data_dir
+
+
+def upload_ibis_test_data_to_hdfs(con, data_path):
+    hdfs = con.hdfs
+    if hdfs.exists(ENV.test_data_dir):
+        hdfs.rmdir(ENV.test_data_dir)
+    hdfs.put(ENV.test_data_dir, data_path, verbose=True)
+
+
+def create_test_database(con):
+    if con.exists_database(ENV.test_data_db):
+        con.drop_database(ENV.test_data_db, force=True)
+    con.create_database(ENV.test_data_db)
+    print('Created database {0}'.format(ENV.test_data_db))
+
+
+def create_parquet_tables(con):
+    parquet_files = con.hdfs.ls(pjoin(ENV.test_data_dir, 'parquet'))
+    schemas = {
+        'functional_alltypes': ibis.schema(
+            [('id', 'int32'),
+             ('bool_col', 'boolean'),
+             ('tinyint_col', 'int8'),
+             ('smallint_col', 'int16'),
+             ('int_col', 'int32'),
+             ('bigint_col', 'int64'),
+             ('float_col', 'float'),
+             ('double_col', 'double'),
+             ('date_string_col', 'string'),
+             ('string_col', 'string'),
+             ('timestamp_col', 'timestamp'),
+             ('year', 'int32'),
+             ('month', 'int32')]),
+        'tpch_region': ibis.schema(
+            [('r_regionkey', 'int16'),
+             ('r_name', 'string'),
+             ('r_comment', 'string')])}
+    tables = []
+    for table_name in parquet_files:
+        print('Creating {0}'.format(table_name))
+        # if no schema infer!
+        schema = schemas.get(table_name)
+        path = pjoin(ENV.test_data_dir, 'parquet', table_name)
+        table = con.parquet_file(path, schema=schema, name=table_name,
+                                 database=ENV.test_data_db, persist=True)
+        tables.append(table)
+    return tables
+
+
+def create_avro_tables(con):
+    avro_files = con.hdfs.ls(pjoin(ENV.test_data_dir, 'avro'))
+    schemas = {
+        'tpch_region_avro': {
+            'type': 'record',
+            'name': 'a',
+            'fields': [
+                {'name': 'R_REGIONKEY', 'type': ['null', 'int']},
+                {'name': 'R_NAME', 'type': ['null', 'string']},
+                {'name': 'R_COMMENT', 'type': ['null', 'string']}]}}
+    tables = []
+    for table_name in avro_files:
+        print('Creating {0}'.format(table_name))
+        schema = schemas[table_name]
+        path = pjoin(ENV.test_data_dir, 'avro', table_name)
+        table = con.avro_file(path, schema, name=table_name,
+                              database=ENV.test_data_db, persist=True)
+        tables.append(table)
+    return tables
+
+
+def build_udfs():
+    print('Building UDFs')
+    ibis_home_dir = osp.dirname(osp.dirname(osp.abspath(__file__)))
+    udf_dir = pjoin(ibis_home_dir, 'testing', 'udf')
+    check_call('cmake . && make', shell=True, cwd=udf_dir)
+
+
+def upload_udfs(con):
+    ibis_home_dir = osp.dirname(osp.dirname(osp.abspath(__file__)))
+    build_dir = pjoin(ibis_home_dir, 'testing', 'udf', 'build')
+    bitcode_dir = pjoin(ENV.test_data_dir, 'udf')
+    print('Uploading UDFs to {0}'.format(bitcode_dir))
+    if con.hdfs.exists(bitcode_dir):
+        con.hdfs.rmdir(bitcode_dir)
+    con.hdfs.put(bitcode_dir, build_dir, verbose=True)
+
+
+def scrape_parquet_files(tmp_db, con):
+    to_scrape = [('tpch', x) for x in con.list_tables(database='tpch')]
+    to_scrape.append(('functional', 'alltypes'))
+    for db, tname in to_scrape:
+        table = con.table(tname, database=db)
+        new_name = '{0}_{1}'.format(db, tname)
+        print('Creating {0}'.format(new_name))
+        con.create_table(new_name, table, database=tmp_db)
+
+
+def download_parquet_files(con, tmp_db_hdfs_path):
+    parquet_path = pjoin(IBIS_TEST_DATA_LOCAL_DIR, 'parquet')
+    print("Downloading {0}".format(parquet_path))
+    con.hdfs.get(tmp_db_hdfs_path, parquet_path)
+
+
+def generate_sqlite_db(con):
+    from sqlalchemy import create_engine
+
+    path = pjoin(IBIS_TEST_DATA_LOCAL_DIR, 'ibis_testing.db')
+    csv_path = guid()
+
+    engine = create_engine('sqlite:///{0}'.format(path))
+
+    generate_sql_csv_sources(csv_path, con.database('ibis_testing'))
+    make_sqlite_testing_db(csv_path, engine)
+    shutil.rmtree(csv_path)
+
+
+def download_avro_files(con):
+    avro_hdfs_path = '/test-warehouse/tpch.region_avro'
+    avro_local_path = pjoin(IBIS_TEST_DATA_LOCAL_DIR, 'avro')
+    os.mkdir(avro_local_path)
+    print("Downloading {0}".format(avro_hdfs_path))
+    con.hdfs.get(avro_hdfs_path, pjoin(avro_local_path, 'tpch_region_avro'))
+
+
+def generate_csv_files():
+    N = 10
+    nfiles = 10
+    df = pd.DataFrame({'foo': [tm.rands(10) for _ in xrange(N)],
+                       'bar': np.random.randn(N),
+                       'baz': np.random.randint(0, 100, size=N)},
+                      columns=['foo', 'bar', 'baz'])
+    csv_base = pjoin(IBIS_TEST_DATA_LOCAL_DIR, 'csv')
+    os.mkdir(csv_base)
+    for i in xrange(nfiles):
+        csv_path = pjoin(csv_base, '{0}.csv'.format(i))
+        print('Writing {0}'.format(csv_path))
+        df.to_csv(csv_path, index=False, header=False)
+
+
+def copy_tarball_to_versioned_backup(bucket):
+    key = bucket.get_key(IBIS_TEST_DATA_TARBALL)
+    if key:
+        names = [k.name for k in bucket.list(prefix=IBIS_TEST_DATA_TARBALL)]
+        names.remove(IBIS_TEST_DATA_TARBALL)
+        # get the highest number for this key name
+        last = sorted([int(names.split('.')[-1]) for name in names])[-1]
+        next_key = '{0}.{1}'.format(IBIS_TEST_DATA_TARBALL, last + 1)
+        key.copy(IBIS_TEST_DATA_S3_BUCKET, next_key)
+        key.delete()
+    assert bucket.get_key(IBIS_TEST_DATA_TARBALL) is None
+
+
+_sql_tpch_tables = ['tpch_lineitem', 'tpch_customer',
+                    'tpch_region', 'tpch_nation', 'tpch_orders']
+
+_sql_tables = ['functional_alltypes']
+
+
+def _project_tpch_lineitem(t):
+    return t['l_orderkey',
+             'l_partkey',
+             'l_suppkey',
+             'l_linenumber',
+             t.l_quantity.cast('double'),
+             t.l_extendedprice.cast('double'),
+             t.l_discount.cast('double'),
+             t.l_tax.cast('double'),
+             'l_returnflag',
+             'l_linestatus',
+             'l_shipdate',
+             'l_commitdate',
+             'l_receiptdate',
+             'l_shipinstruct',
+             'l_shipmode']
+
+
+def _project_tpch_orders(t):
+    return t['o_orderkey',
+             'o_custkey',
+             'o_orderstatus',
+             t.o_totalprice.cast('double'),
+             'o_orderdate',
+             'o_orderpriority',
+             'o_clerk',
+             'o_shippriority']
+
+
+def _project_tpch_customer(t):
+    return t['c_custkey',
+             'c_name',
+             'c_nationkey',
+             'c_phone',
+             'c_acctbal',
+             'c_mktsegment']
+
+
+_projectors = {
+    'tpch_customer': _project_tpch_customer,
+    'tpch_lineitem': _project_tpch_lineitem,
+    'tpch_orders': _project_tpch_orders,
+}
 
-@pytest.fixture(scope="session")
-def mockcon():
-    return MockBackend()
-
-
-@pytest.fixture(scope="module")
-def kudu_table(con, test_data_db):
-    name = 'kudu_backed_table'
-    con.raw_sql(
-        f"""\
-CREATE TABLE {test_data_db}.{name} (
-  a STRING,
-  PRIMARY KEY(a)
-)
-PARTITION BY HASH PARTITIONS 2
-STORED AS KUDU
-TBLPROPERTIES (
-  'kudu.master_addresses' = 'kudu',
-  'kudu.num_tablet_replicas' = '1'
-)"""
-    )
-    try:
-        yield con.table(name)
-    finally:
-        con.drop_table(name, database=test_data_db)
 
+def generate_sql_csv_sources(output_path, db):
+    ibis.options.sql.default_limit = None
 
-def translate(expr, context=None, named=False):
-    if context is None:
-        context = ImpalaCompiler.make_context()
-    translator = ImpalaExprTranslator(expr.op(), context=context, named=named)
-    return translator.get_result()
-
-
-def impala_build_and_upload_udfs(hdfs, env, *, fs):
-    IBIS_HOME = Path(__file__).absolute().parents[4]
-    cwd = str(IBIS_HOME / "ci" / "udf")
-    subprocess.run(["cmake", ".", "-G", "Ninja"], cwd=cwd)
-    subprocess.run(["ninja"], cwd=cwd)
-    build_dir = IBIS_HOME / "ci" / "udf" / "build"
-    bitcode_dir = os.path.join(env.test_data_dir, "udf")
-
-    hdfs.mkdir(bitcode_dir, create_parents=True)
-
-    for file in fs.find(build_dir):
-        bitcode_path = os.path.join(bitcode_dir, os.path.relpath(file, build_dir))
-        yield hdfs.put_file, file, bitcode_path
-
-
-def hdfs_make_dir_and_put_file(fs, src, target):
-    fs.mkdir(os.path.dirname(target), create_parents=True)
-    fs.put_file(src, target)
-
-
-def impala_create_test_database(con, env):
-    con.drop_database(env.test_data_db, force=True)
-    con.create_database(env.test_data_db)
-    con.create_table(
-        'alltypes',
-        schema=ibis.schema(
-            [
-                ('a', 'int8'),
-                ('b', 'int16'),
-                ('c', 'int32'),
-                ('d', 'int64'),
-                ('e', 'float'),
-                ('f', 'double'),
-                ('g', 'string'),
-                ('h', 'boolean'),
-                ('i', 'timestamp'),
-            ]
-        ),
-        database=env.test_data_db,
-    )
-    con.create_table(
-        "win",
-        schema=ibis.schema(dict(g="string", x="int64", y="int64")),
-        database=env.test_data_db,
-    )
-    con.table("win", database=env.test_data_db).insert(win, overwrite=True)
-
-
-PARQUET_SCHEMAS = {
-    "functional_alltypes": ibis.schema(
-        {
-            name: dtype
-            for name, dtype in TEST_TABLES["functional_alltypes"].items()
-            if name not in {"index", "Unnamed: 0"}
-        }
-    ),
-    "tpch_region": ibis.schema(
-        [
-            ("r_regionkey", "int16"),
-            ("r_name", "string"),
-            ("r_comment", "string"),
-        ]
-    ),
-}
+    if not osp.exists(output_path):
+        os.mkdir(output_path)
 
-PARQUET_SCHEMAS.update(
-    (table, schema)
-    for table, schema in TEST_TABLES.items()
-    if table != "functional_alltypes"
-)
-
-AVRO_SCHEMAS = {
-    "tpch_region_avro": {
-        "type": "record",
-        "name": "a",
-        "fields": [
-            {"name": "R_REGIONKEY", "type": ["null", "int"]},
-            {"name": "R_NAME", "type": ["null", "string"]},
-            {"name": "R_COMMENT", "type": ["null", "string"]},
-        ],
-    }
-}
+    for name in _sql_tables:
+        print(name)
+        table = db[name]
+
+        if name in _projectors:
+            table = _projectors[name](table)
+
+        df = table.execute()
+        path = osp.join(output_path, name)
+        df.to_csv('{0}.csv'.format(path), na_rep='\\N')
+
+
+def make_sqlite_testing_db(csv_dir, con):
+    for name in _sql_tables:
+        print(name)
+        path = osp.join(csv_dir, '{0}.csv'.format(name))
+        df = pd.read_csv(path, na_values=['\\N'])
+        pd.io.sql.to_sql(df, name, con, chunksize=10000)
+
+
+# ==========================================
+
+
+@group(context_settings={'help_option_names': ['-h', '--help']})
+def main():
+    """Manage test data for Ibis"""
+    pass
+
+
+@main.command()
+def printenv():
+    """Print current IbisTestEnv"""
+    print(str(ENV))
+
+
+@main.command()
+@option('--create-tarball', is_flag=True,
+        help="Create a gzipped tarball")
+@option('--push-to-s3', is_flag=True,
+        help="Also push the tarball to s3://ibis-test-resources")
+def create(create_tarball, push_to_s3):
+    """Create Ibis test data"""
+    print(str(ENV))
+
+    con = make_ibis_client()
+
+    # verify some assumptions before proceeding
+    if push_to_s3 and not create_tarball:
+        raise IbisError(
+            "Must specify --create-tarball if specifying --push-to-s3")
+    if osp.exists(IBIS_TEST_DATA_LOCAL_DIR):
+        raise IbisError(
+            'Local dir {0} already exists; please remove it first'.format(
+                IBIS_TEST_DATA_LOCAL_DIR))
+    if not con.exists_database('tpch'):
+        raise IbisError('`tpch` database does not exist')
+    if not con.hdfs.exists('/test-warehouse/tpch.region_avro'):
+        raise IbisError(
+            'HDFS dir /test-warehouse/tpch.region_avro does not exist')
+
+    # generate tmp identifiers
+    tmp_db_hdfs_path = pjoin(ENV.tmp_dir, guid())
+    tmp_db = guid()
+    os.mkdir(IBIS_TEST_DATA_LOCAL_DIR)
+    try:
+        # create the tmp data locally
+        con.create_database(tmp_db, path=tmp_db_hdfs_path)
+        print('Created database {0} at {1}'.format(tmp_db, tmp_db_hdfs_path))
+
+        # create the local data set
+        scrape_parquet_files(tmp_db, con)
+        download_parquet_files(con, tmp_db_hdfs_path)
+        download_avro_files(con)
+        generate_csv_files()
+        generate_sqlite_db(con)
+    finally:
+        con.drop_database(tmp_db, force=True)
+        assert not con.hdfs.exists(tmp_db_hdfs_path)
+
+    if create_tarball:
+        check_call('tar -zc {0} > {1}'
+                   .format(IBIS_TEST_DATA_LOCAL_DIR, TARBALL_NAME),
+                   shell=True)
+
+    if push_to_s3:
+        import boto
+        s3_conn = boto.connect_s3(IBIS_TEST_AWS_KEY_ID,
+                                  IBIS_TEST_AWS_SECRET)
+        bucket = s3_conn.get_bucket(IBIS_TEST_DATA_S3_BUCKET)
+        # copy_tarball_to_versioned_backup(bucket)
+        key = bucket.new_key(IBIS_TEST_DATA_TARBALL)
+        print('Upload tarball to S3')
+        key.set_contents_from_filename(TARBALL_NAME, replace=True)
+
+
+@main.command()
+@option('--data/--no-data', default=True, help='Load (skip) ibis testing data')
+@option('--udf/--no-udf', default=True, help='Build/upload (skip) test UDFs')
+@option('--data-dir',
+        help='Path to testing data; dnloads data from S3 if unset')
+@option('--overwrite', is_flag=True, help='Forces overwriting of data/UDFs')
+def load(data, udf, data_dir, overwrite):
+    """Load Ibis test data and build/upload UDFs"""
+    print(str(ENV))
+
+    con = make_ibis_client()
+
+    # validate our environment before performing possibly expensive operations
+    if not can_write_to_hdfs(con):
+        raise IbisError('Failed to write to HDFS; check your settings')
+    if udf and not can_build_udfs():
+        raise IbisError('Build environment does not support building UDFs')
+
+    # load the data files
+    if data:
+        already_loaded = is_data_loaded(con)
+        print('Attempting to load Ibis test data (--data)')
+        if already_loaded and not overwrite:
+            print('Data is already loaded and not overwriting; moving on')
+        else:
+            if already_loaded:
+                print('Data is already loaded; attempting to overwrite')
+            tmp_dir = tempfile.mkdtemp(prefix='__ibis_tmp_')
+            try:
+                if not data_dir:
+                    print('Did not specify a local dir with the test data, so '
+                          'downloading it from S3')
+                    data_dir = dnload_ibis_test_data_from_s3(tmp_dir)
+                print('Uploading to HDFS')
+                upload_ibis_test_data_to_hdfs(con, data_dir)
+                print('Creating Ibis test data database')
+                create_test_database(con)
+                parquet_tables = create_parquet_tables(con)
+                avro_tables = create_avro_tables(con)
+                for table in parquet_tables + avro_tables:
+                    print('Computing stats for {0}'.format(table.op().name))
+                    table.compute_stats()
+
+                # sqlite database
+                sqlite_src = osp.join(data_dir, 'ibis_testing.db')
+                shutil.copy(sqlite_src, '.')
+            finally:
+                shutil.rmtree(tmp_dir)
+    else:
+        print('Skipping Ibis test data load (--no-data)')
+
+    # build and upload the UDFs
+    if udf:
+        already_loaded = is_udf_loaded(con)
+        print('Attempting to build and load test UDFs')
+        if already_loaded and not overwrite:
+            print('UDFs already loaded and not overwriting; moving on')
+        else:
+            if already_loaded:
+                print('UDFs already loaded; attempting to overwrite')
+            print('Building UDFs')
+            build_udfs()
+            print('Uploading UDFs')
+            upload_udfs(con)
+    else:
+        print('Skipping UDF build/load (--no-udf)')
+
+
+@main.command()
+@option('--test-data', is_flag=True,
+        help='Cleanup Ibis test data, test database, and also the test UDFs '
+             'if they are stored in the test data directory/database')
+@option('--udfs', is_flag=True, help='Cleanup Ibis test UDFs only')
+@option('--tmp-data', is_flag=True,
+        help='Cleanup Ibis temporary HDFS directory')
+@option('--tmp-db', is_flag=True, help='Cleanup Ibis temporary database')
+def cleanup(test_data, udfs, tmp_data, tmp_db):
+    """Cleanup Ibis test data and UDFs"""
+    print(str(ENV))
+
+    con = make_ibis_client()
+
+    if udfs:
+        # this comes before test_data bc the latter clobbers this too
+        con.hdfs.rmdir(pjoin(ENV.test_data_dir, 'udf'))
+
+    if test_data:
+        con.drop_database(ENV.test_data_db, force=True)
+        con.hdfs.rmdir(ENV.test_data_dir)
+
+    if tmp_data:
+        con.hdfs.rmdir(ENV.tmp_dir)
 
-ALL_SCHEMAS = collections.ChainMap(PARQUET_SCHEMAS, AVRO_SCHEMAS)
+    if tmp_db:
+        con.drop_database(ENV.tmp_db, force=True)
 
 
-def impala_create_tables(
-    con: BaseBackend,
-    env: IbisTestEnv,
-    *,
-    executor: concurrent.futures.Executor,
-) -> Iterator[concurrent.futures.Future]:
-    test_data_dir = env.test_data_dir
-    avro_files = [
-        (con.avro_file, os.path.join(test_data_dir, 'avro', path))
-        for path in con.hdfs.ls(os.path.join(test_data_dir, 'avro'))
-    ]
-    parquet_files = [
-        (con.parquet_file, os.path.join(test_data_dir, 'parquet', path))
-        for path in con.hdfs.ls(os.path.join(test_data_dir, 'parquet'))
-    ]
-    for method, path in itertools.chain(parquet_files, avro_files):
-        yield executor.submit(
-            method,
-            path,
-            ALL_SCHEMAS.get(os.path.basename(path)),
-            name=os.path.basename(path),
-            database=env.test_data_db,
-            persist=True,
-        )
+if __name__ == '__main__':
+    main()
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/tests/test_ddl.py` & `ibis-framework-v0.6.0/ibis/impala/tests/test_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,404 +1,336 @@
-from posixpath import join as pjoin
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import pytest
+import pandas as pd
 
-import ibis
-import ibis.common.exceptions as com
-import ibis.expr.datatypes as dt
-import ibis.expr.types as ir
-from ibis import util
-from ibis.backends.base.sql.ddl import fully_qualified_re
+from ibis.compat import unittest
+from ibis.impala.tests.common import IbisTestEnv, ImpalaE2E, connect_test
 from ibis.tests.util import assert_equal
+import ibis
 
-pytest.importorskip("impala")
-from ibis.backends.impala.compat import HS2Error  # noqa: E402
-
-
-def test_create_exists_view(con, temp_view):
-    tmp_name = temp_view
-    assert tmp_name not in con.list_tables()
-
-    t1 = con.table('functional_alltypes').group_by('string_col').size()
-    t2 = con.create_view(tmp_name, t1)
-
-    assert tmp_name in con.list_tables()
-    # just check it works for now
-    assert t2.execute() is not None
-
-
-def test_drop_non_empty_database(con, alltypes, temp_table_db):
-    temp_database, temp_table = temp_table_db
-    con.create_table(temp_table, alltypes, database=temp_database)
-    assert temp_table in con.list_tables(database=temp_database)
-
-    with pytest.raises(com.IntegrityError):
-        con.drop_database(temp_database)
-
-
-@pytest.mark.hdfs
-def test_create_database_with_location(con, tmp_dir, hdfs):
-    base = pjoin(tmp_dir, util.guid())
-    name = f'__ibis_test_{util.guid()}'
-    tmp_path = pjoin(base, name)
-
-    con.create_database(name, path=tmp_path)
-    try:
-        assert hdfs.exists(base)
-    finally:
-        try:
-            con.drop_database(name)
-        finally:
-            hdfs.rm(base, recursive=True)
-
-
-@pytest.mark.hdfs
-def test_create_table_with_location_execute(
-    con, hdfs, tmp_dir, alltypes, test_data_db, temp_table
-):
-    base = pjoin(tmp_dir, util.guid())
-    name = f'test_{util.guid()}'
-    tmp_path = pjoin(base, name)
-
-    expr = alltypes
-    table_name = temp_table
-
-    con.create_table(table_name, obj=expr, location=tmp_path, database=test_data_db)
-    assert hdfs.exists(tmp_path)
-
-
-def test_drop_table_not_exist(con):
-    non_existent_table = f'ibis_table_{util.guid()}'
-    with pytest.raises(Exception):
-        con.drop_table(non_existent_table)
-    con.drop_table(non_existent_table, force=True)
-
-
-def test_truncate_table(con, alltypes, temp_table):
-    expr = alltypes.limit(1)
-
-    table_name = temp_table
-    con.create_table(table_name, obj=expr)
-
-    try:
-        con.truncate_table(table_name)
-    except HS2Error as e:
-        if 'AnalysisException' in e.args[0]:
-            pytest.skip('TRUNCATE not available in this version of Impala')
-
-    t = con.table(table_name)
-    nrows = t.count().execute()
-    assert not nrows
-
+import ibis.common as com
+import ibis.config as config
+import ibis.expr.types as ir
+import ibis.util as util
 
-def test_truncate_table_expression(con, alltypes, temp_table):
-    expr = alltypes.limit(1)
 
-    table_name = temp_table
-    con.create_table(table_name, obj=expr)
-    t = con.table(table_name)
-    t.truncate()
-    nrows = t.count().execute()
-    assert not nrows
+def approx_equal(a, b, eps):
+    assert abs(a - b) < eps
 
 
-def test_ctas_from_table_expr(con, alltypes, temp_table_db):
-    expr = alltypes
-    db, table_name = temp_table_db
+ENV = IbisTestEnv()
 
-    con.create_table(table_name, expr, database=db)
 
+class TestImpalaClient(ImpalaE2E, unittest.TestCase):
 
-def test_create_empty_table(con, temp_table):
-    schema = ibis.schema(
-        [
-            ('a', 'string'),
-            ('b', 'timestamp'),
-            ('c', 'decimal(12, 8)'),
-            ('d', 'double'),
+    def test_execute_exprs_default_backend(self):
+        cases = [
+            (ibis.literal(2), 2)
         ]
-    )
-
-    table_name = temp_table
-    con.create_table(table_name, schema=schema)
-
-    result_schema = con.get_schema(table_name)
-    assert_equal(result_schema, schema)
-
-    assert con.table(table_name).execute().empty
-
-
-def test_insert_table(con, alltypes, temp_table, test_data_db):
-    expr = alltypes
-    table_name = temp_table
-    db = test_data_db
-
-    con.create_table(table_name, expr.limit(0), database=db)
-
-    con.insert(table_name, expr.limit(10), database=db)
-
-    # check using ImpalaTable.insert
-    t = con.table(table_name, database=db)
-    t.insert(expr.limit(10))
-
-    sz = t.count()
-    assert sz.execute() == 20
-
-    # Overwrite and verify only 10 rows now
-    t.insert(expr.limit(10), overwrite=True)
-    assert sz.execute() == 10
-
-
-def test_insert_validate_types(con, alltypes, test_data_db, temp_table):
-    # GH #235
-    table_name = temp_table
-    db = test_data_db
-
-    expr = alltypes
-    con.create_table(
-        table_name,
-        schema=expr['tinyint_col', 'int_col', 'string_col'].schema(),
-        database=db,
-    )
-
-    t = con.table(table_name, database=db)
-
-    to_insert = expr[
-        expr.tinyint_col, expr.smallint_col.name('int_col'), expr.string_col
-    ]
-    t.insert(to_insert.limit(10))
-
-    to_insert = expr[
-        expr.tinyint_col,
-        expr.smallint_col.cast('int32').name('int_col'),
-        expr.string_col,
-    ]
-    t.insert(to_insert.limit(10))
-
-    to_insert = expr[expr.tinyint_col, expr.bigint_col.name('int_col'), expr.string_col]
-
-    limit_expr = to_insert.limit(10)
-    with pytest.raises(com.IbisError):
-        t.insert(limit_expr)
-
 
-def test_compute_stats(con):
-    t = con.table('functional_alltypes')
-
-    t.compute_stats()
-    t.compute_stats(incremental=True)
-
-    con.compute_stats('functional_alltypes')
-
-
-@pytest.fixture
-def created_view(con, alltypes):
-    name = util.guid()
-    expr = alltypes.limit(10)
-    con.create_view(name, expr)
-    return name
-
-
-def test_drop_view(con, alltypes, created_view):
-    con.drop_view(created_view)
-    assert created_view not in con.list_tables()
-
-
-def test_rename_table(con, temp_database):
-    tmp_db = temp_database
-
-    orig_name = 'tmp_rename_test'
-    con.create_table(orig_name, con.table('tpch_region'))
-    table = con.table(orig_name)
-
-    old_name = table.name
-
-    new_name = 'rename_test'
-    renamed = table.rename(new_name, database=tmp_db)
-    renamed.execute()
-
-    t = con.table(new_name, database=tmp_db)
-    assert_equal(renamed, t)
-
-    assert table.name == old_name
-
-
-@pytest.fixture
-def path_uuid():
-    return f'change-location-{util.guid()}'
-
-
-@pytest.fixture
-def table(con, tmp_db, tmp_dir, path_uuid):
-    table_name = f'table_{util.guid()}'
-    fake_path = pjoin(tmp_dir, path_uuid)
-    schema = ibis.schema([('foo', 'string'), ('bar', 'int64')])
-    con.create_table(
-        table_name,
-        database=tmp_db,
-        schema=schema,
-        format='parquet',
-        external=True,
-        location=fake_path,
-    )
-    try:
-        yield con.table(table_name, database=tmp_db)
-    finally:
-        con.drop_table(table_name, database=tmp_db)
-
-
-def test_change_location(con, table, tmp_dir, path_uuid):
-    old_loc = table.metadata().location
-
-    new_path = pjoin(tmp_dir, 'new-path')
-    table.alter(location=new_path)
-
-    new_loc = table.metadata().location
-    assert new_loc == old_loc.replace(path_uuid, 'new-path')
-
-
-def test_change_properties(con, table):
-    props = {'foo': '1', 'bar': '2'}
-
-    table.alter(tbl_properties=props)
-    tbl_props = table.metadata().tbl_properties
-    for k, v in props.items():
-        assert v == tbl_props[k]
-
-    table.alter(serde_properties=props)
-    serde_props = table.metadata().serde_properties
-    for k, v in props.items():
-        assert v == serde_props[k]
-
-
-def test_change_format(con, table):
-    table.alter(format='avro')
-
-    meta = table.metadata()
-    assert 'Avro' in meta.hive_format
-
-
-def test_query_avro(con, test_data_dir, tmp_db):
-    hdfs_path = pjoin(test_data_dir, 'avro/tpch_region_avro')
-
-    avro_schema = {
-        "fields": [
-            {"type": ["int", "null"], "name": "R_REGIONKEY"},
-            {"type": ["string", "null"], "name": "R_NAME"},
-            {"type": ["string", "null"], "name": "R_COMMENT"},
-        ],
-        "type": "record",
-        "name": "a",
-    }
-
-    table = con.avro_file(hdfs_path, avro_schema, database=tmp_db)
-
-    qualified_name = table.op().name
-    _, name, _ = fully_qualified_re.match(qualified_name).groups()
-
-    # table exists
-    assert name in con.list_tables(database=tmp_db)
-
-    expr = table.r_name.value_counts()
-    expr.execute()
-
-    assert table.count().execute() == 5
-
-    df = table.execute()
-    assert len(df) == 5
-
-
-def test_create_table_reserved_identifier(con):
-    table_name = 'distinct'
-    expr = con.table('functional_alltypes')
-    expected = expr.count().execute()
-    con.create_table(table_name, expr)
-    try:
-        result = con.table(table_name).count().execute()
-    except Exception:
-        raise
-    else:
+        ibis.options.default_backend = None
+        client = connect_test(ENV, with_hdfs=False)
+        assert ibis.options.default_backend is client
+
+        for expr, expected in cases:
+            result = expr.execute()
+            assert result == expected
+
+    def test_raise_ibis_error_no_hdfs(self):
+        # #299
+        client = connect_test(ENV, with_hdfs=False)
+        self.assertRaises(com.IbisError, getattr, client, 'hdfs')
+
+    def test_get_table_ref(self):
+        table = self.db.functional_alltypes
+        assert isinstance(table, ir.TableExpr)
+
+        table = self.db['functional_alltypes']
+        assert isinstance(table, ir.TableExpr)
+
+    def test_run_sql(self):
+        query = """SELECT li.*
+FROM {0}.tpch_lineitem li
+""".format(self.test_data_db)
+        table = self.con.sql(query)
+
+        li = self.con.table('tpch_lineitem')
+        assert isinstance(table, ir.TableExpr)
+        assert_equal(table.schema(), li.schema())
+
+        expr = table.limit(10)
+        result = expr.execute()
+        assert len(result) == 10
+
+    def test_sql_with_limit(self):
+        query = """\
+SELECT *
+FROM functional_alltypes
+LIMIT 10"""
+        table = self.con.sql(query)
+        ex_schema = self.con.get_schema('functional_alltypes')
+        assert_equal(table.schema(), ex_schema)
+
+    def test_raw_sql(self):
+        query = 'SELECT * from functional_alltypes limit 10'
+        cur = self.con.raw_sql(query, results=True)
+        rows = cur.fetchall()
+        cur.release()
+        assert len(rows) == 10
+
+    def test_explain(self):
+        t = self.con.table('functional_alltypes')
+        expr = t.group_by('string_col').size()
+        result = self.con.explain(expr)
+        assert isinstance(result, str)
+
+    def test_get_schema(self):
+        t = self.con.table('tpch_lineitem')
+        schema = self.con.get_schema('tpch_lineitem',
+                                     database=self.test_data_db)
+        assert_equal(t.schema(), schema)
+
+    def test_result_as_dataframe(self):
+        expr = self.alltypes.limit(10)
+
+        ex_names = expr.schema().names
+        result = self.con.execute(expr)
+
+        assert isinstance(result, pd.DataFrame)
+        assert list(result.columns) == ex_names
+        assert len(result) == 10
+
+    def test_adapt_scalar_array_results(self):
+        table = self.alltypes
+
+        expr = table.double_col.sum()
+        result = self.con.execute(expr)
+        assert isinstance(result, float)
+
+        with config.option_context('interactive', True):
+            result2 = expr.execute()
+            assert isinstance(result2, float)
+
+        expr = (table.group_by('string_col')
+                .aggregate([table.count().name('count')])
+                .string_col)
+
+        result = self.con.execute(expr)
+        assert isinstance(result, pd.Series)
+
+    def test_interactive_repr_call_failure(self):
+        t = self.con.table('tpch_lineitem').limit(100000)
+
+        t = t[t, t.l_receiptdate.cast('timestamp').name('date')]
+
+        keys = [t.date.year().name('year'), 'l_linestatus']
+        filt = t.l_linestatus.isin(['F'])
+        expr = (t[filt]
+                .group_by(keys)
+                .aggregate(t.l_extendedprice.mean().name('avg_px')))
+
+        w2 = ibis.trailing_window(9, group_by=expr.l_linestatus,
+                                  order_by=expr.year)
+
+        metric = expr['avg_px'].mean().over(w2)
+        enriched = expr[expr, metric]
+        with config.option_context('interactive', True):
+            repr(enriched)
+
+    def test_array_default_limit(self):
+        t = self.alltypes
+
+        result = self.con.execute(t.float_col, limit=100)
+        assert len(result) == 100
+
+    def test_limit_overrides_expr(self):
+        # #418
+        t = self.alltypes
+        result = self.con.execute(t.limit(10), limit=5)
+        assert len(result) == 5
+
+    def test_limit_equals_none_no_limit(self):
+        t = self.alltypes
+
+        with config.option_context('sql.default_limit', 10):
+            result = t.execute(limit=None)
+            assert len(result) > 10
+
+    def test_verbose_log_queries(self):
+        queries = []
+
+        def logger(x):
+            queries.append(x)
+
+        with config.option_context('verbose', True):
+            with config.option_context('verbose_log', logger):
+                self.con.table('tpch_orders', database=self.test_data_db)
+
+        assert len(queries) == 1
+        expected = 'DESCRIBE {0}.`tpch_orders`'.format(self.test_data_db)
+        assert queries[0] == expected
+
+    def test_sql_query_limits(self):
+        table = self.con.table('tpch_nation', database=self.test_data_db)
+        with config.option_context('sql.default_limit', 100000):
+            # table has 25 rows
+            assert len(table.execute()) == 25
+            # comply with limit arg for TableExpr
+            assert len(table.execute(limit=10)) == 10
+            # state hasn't changed
+            assert len(table.execute()) == 25
+            # non-TableExpr ignores default_limit
+            assert table.count().execute() == 25
+            # non-TableExpr doesn't observe limit arg
+            assert table.count().execute(limit=10) == 25
+        with config.option_context('sql.default_limit', 20):
+            # TableExpr observes default limit setting
+            assert len(table.execute()) == 20
+            # explicit limit= overrides default
+            assert len(table.execute(limit=15)) == 15
+            assert len(table.execute(limit=23)) == 23
+            # non-TableExpr ignores default_limit
+            assert table.count().execute() == 25
+            # non-TableExpr doesn't observe limit arg
+            assert table.count().execute(limit=10) == 25
+        # eliminating default_limit doesn't break anything
+        with config.option_context('sql.default_limit', None):
+            assert len(table.execute()) == 25
+            assert len(table.execute(limit=15)) == 15
+            assert len(table.execute(limit=10000)) == 25
+            assert table.count().execute() == 25
+            assert table.count().execute(limit=10) == 25
+
+    def test_expr_compile_verify(self):
+        table = self.db.functional_alltypes
+        expr = table.double_col.sum()
+
+        assert isinstance(expr.compile(), str)
+        assert expr.verify()
+
+    def test_api_compile_verify(self):
+        t = self.db.functional_alltypes
+
+        s = t.string_col
+
+        supported = s.lower()
+        unsupported = s.replace('foo', 'bar')
+
+        assert ibis.impala.verify(supported)
+        assert not ibis.impala.verify(unsupported)
+
+    def test_database_repr(self):
+        assert self.test_data_db in repr(self.db)
+
+    def test_database_drop(self):
+        tmp_name = '__ibis_test_{0}'.format(util.guid())
+        self.con.create_database(tmp_name)
+
+        db = self.con.database(tmp_name)
+        self.temp_databases.append(tmp_name)
+        db.drop()
+        assert not self.con.exists_database(tmp_name)
+
+    def test_database_default_current_database(self):
+        db = self.con.database()
+        assert db.name == self.con.current_database
+
+    def test_namespace(self):
+        ns = self.db.namespace('tpch_')
+
+        assert 'tpch_' in repr(ns)
+
+        table = ns.lineitem
+        expected = self.db.tpch_lineitem
+        attrs = dir(ns)
+        assert 'lineitem' in attrs
+        assert 'functional_alltypes' not in attrs
+
+        assert_equal(table, expected)
+
+    def test_close_drops_temp_tables(self):
+        from posixpath import join as pjoin
+
+        hdfs_path = pjoin(self.test_data_dir, 'parquet/tpch_region')
+
+        client = connect_test(ENV)
+        table = client.parquet_file(hdfs_path)
+
+        name = table.op().name
+        assert self.con.exists_table(name) is True
+        client.close()
+
+        assert not self.con.exists_table(name)
+
+    def test_execute_async_simple(self):
+        t = self.db.functional_alltypes
+        expr = t.double_col.sum()
+
+        q = expr.execute(async=True)
+        result = q.get_result()
+        expected = expr.execute()
         assert result == expected
-    finally:
-        con.drop_table(table_name)
-
-
-def test_query_delimited_file_directory(con, test_data_dir, tmp_db):
-    hdfs_path = pjoin(test_data_dir, 'csv')
-
-    schema = ibis.schema([('foo', 'string'), ('bar', 'double'), ('baz', 'int8')])
-    name = 'delimited_table_test1'
-    table = con.delimited_file(
-        hdfs_path, schema, name=name, database=tmp_db, delimiter=','
-    )
-
-    expr = (
-        table[table.bar > 0]
-        .group_by('foo')
-        .aggregate(
-            [
-                table.bar.sum().name('sum(bar)'),
-                table.baz.sum().name('mean(baz)'),
-            ]
-        )
-    )
-    assert expr.execute() is not None
-
-
-@pytest.fixture
-def temp_char_table(con):
-    name = "testing_varchar_support"
-    con.raw_sql(
-        f"""\
-CREATE TABLE IF NOT EXISTS {name} (
-  group1 VARCHAR(10),
-  group2 CHAR(10)
-)"""
-    )
-    try:
-        yield con.table(name)
-    finally:
-        try:
-            assert name in con.list_tables(), name
-        finally:
-            con.drop_table(name, force=True)
-
-
-def test_varchar_char_support(temp_char_table):
-    assert isinstance(temp_char_table['group1'], ir.StringValue)
-    assert isinstance(temp_char_table['group2'], ir.StringValue)
-
-
-def test_temp_table_concurrency(con, test_data_dir):
-    import concurrent.futures
-    import multiprocessing
-
-    def limit(con, hdfs_path, offset):
-        t = con.parquet_file(hdfs_path)
-        return t.order_by(t.r_regionkey).limit(1, offset=offset).execute()
-
-    nthreads = multiprocessing.cpu_count()
-    hdfs_path = pjoin(test_data_dir, 'parquet/tpch_region')
-
-    num_rows = int(con.parquet_file(hdfs_path).count().execute())
-    with concurrent.futures.ThreadPoolExecutor(max_workers=nthreads) as e:
-        futures = [
-            e.submit(limit, con, hdfs_path, offset=offset % (num_rows - 1) + 1)
-            for offset in range(nthreads)
-        ]
-        results = [
-            future.result() for future in concurrent.futures.as_completed(futures)
-        ]
-    assert all(map(len, results))
 
+    def test_query_cancel(self):
+        import time
+        t = self.db.functional_alltypes
+
+        t2 = t.union(t).union(t)
+
+        # WM: this query takes about 90 seconds to execute for me locally, so
+        # I'm eyeballing an acceptable time frame for the cancel to work
+        expr = t2.join(t2).count()
+
+        start = time.clock()
+        q = expr.execute(async=True)
+        q.cancel()
+        end = time.clock()
+        elapsed = end - start
+        assert elapsed < 5
+
+        assert q.is_finished()
+
+    def test_set_compression_codec(self):
+        old_opts = self.con.get_options()
+        assert old_opts['COMPRESSION_CODEC'].upper() == 'NONE'
+
+        self.con.set_compression_codec('snappy')
+        opts = self.con.get_options()
+        assert opts['COMPRESSION_CODEC'].upper() == 'SNAPPY'
+
+        self.con.set_compression_codec(None)
+        opts = self.con.get_options()
+        assert opts['COMPRESSION_CODEC'].upper() == 'NONE'
+
+    def test_disable_codegen(self):
+        self.con.disable_codegen(False)
+        opts = self.con.get_options()
+        assert opts['DISABLE_CODEGEN'] == '0'
+
+        self.con.disable_codegen()
+        opts = self.con.get_options()
+        assert opts['DISABLE_CODEGEN'] == '1'
+
+        impala_con = self.con.con
+        cur1 = impala_con.execute('SET')
+        cur2 = impala_con.execute('SET')
 
-def test_access_kudu_table(kudu_table):
-    assert kudu_table.columns == ['a']
-    assert kudu_table['a'].type() == dt.string
+        opts1 = dict(cur1.fetchall())
+        cur1.release()
 
+        opts2 = dict(cur2.fetchall())
+        cur2.release()
 
-def test_kudu_property_raises_useful_error(con):
-    with pytest.raises(
-        NotImplementedError,
-        match="kudu support using kudu-python",
-    ):
-        con.kudu  # noqa: B018
+        assert opts1['DISABLE_CODEGEN'] == '1'
+        assert opts2['DISABLE_CODEGEN'] == '1'
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/tests/test_udf.py` & `ibis-framework-v0.6.0/ibis/impala/tests/test_udf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,690 +1,502 @@
-from decimal import Decimal
-from posixpath import join as pjoin
+# Copyright 2015 Cloudera Inc
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import numpy as np
-import pandas as pd
+from posixpath import join as pjoin
 import pytest
 
 import ibis
-import ibis.backends.impala as api
-import ibis.common.exceptions as com
-import ibis.expr.datatypes as dt
+
 import ibis.expr.types as ir
-from ibis import util
-from ibis.backends.impala import ddl
-from ibis.common.exceptions import IbisTypeError
-from ibis.expr import rules
-
-pytest.importorskip("impala")
-
-
-@pytest.fixture(scope="module")
-def table(mockcon):
-    return mockcon.table("functional_alltypes")
-
-
-@pytest.fixture
-def i8(table):
-    return table.tinyint_col
-
-
-@pytest.fixture
-def i16(table):
-    return table.smallint_col
-
-
-@pytest.fixture
-def i32(table):
-    return table.int_col
-
-
-@pytest.fixture
-def i64(table):
-    return table.bigint_col
-
-
-@pytest.fixture
-def d(table):
-    return table.double_col
-
-
-@pytest.fixture
-def f(table):
-    return table.float_col
-
-
-@pytest.fixture
-def s(table):
-    return table.string_col
-
-
-@pytest.fixture
-def b(table):
-    return table.bool_col
-
-
-@pytest.fixture
-def t(table):
-    return table.timestamp_col
-
-
-@pytest.fixture
-def tpch_customer(con):
-    return con.table("tpch_customer")
-
-
-@pytest.fixture
-def dec(tpch_customer):
-    return tpch_customer.c_acctbal
-
-
-@pytest.fixture
-def all_cols(i8, i16, i32, i64, d, f, dec, s, b, t):
-    return [
-        i8,
-        i16,
-        i32,
-        i64,
-        d,
-        f,
-        dec,
-        s,
-        b,
-        t,
-    ]
-
-
-def test_sql_generation(snapshot):
-    func = api.scalar_function(['string'], 'string', name='Tester')
-    func.register('identity', 'udf_testing')
-
-    result = func('hello world')
-    snapshot.assert_match(ibis.impala.compile(result), "out.sql")
-
-
-def test_sql_generation_from_infoclass(snapshot):
-    func = api.wrap_udf('test.so', ['string'], 'string', 'info_test')
-    repr(func)
-
-    func.register('info_test', 'udf_testing')
-    result = func('hello world').name('tmp')
-    snapshot.assert_match(ibis.impala.compile(result), "out.sql")
-
-
-@pytest.mark.parametrize(
-    ("ty", "value", "column"),
-    [
-        pytest.param('boolean', True, "bool_col", id="boolean"),
-        pytest.param('int8', 1, "tinyint_col", id="int8"),
-        pytest.param('int16', 1, "smallint_col", id="int16"),
-        pytest.param('int32', 1, "int_col", id="int32"),
-        pytest.param('int64', 1, "bigint_col", id="int64"),
-        pytest.param('float', 1.0, "float_col", id="float"),
-        pytest.param('double', 1.0, "double_col", id="double"),
-        pytest.param('string', '1', "string_col", id="string"),
-        pytest.param(
-            'timestamp',
-            ibis.timestamp('1961-04-10'),
-            "timestamp_col",
-            id="timestamp",
-        ),
-    ],
-)
-def test_udf_primitive_output_types(ty, value, column, table):
-    func = _register_udf([ty], ty, 'test')
-
-    ibis_type = dt.validate_type(ty)
-
-    expr = func(value)
-    assert type(expr) == ibis_type.scalar
-
-    expr = func(table[column])
-    assert type(expr) == ibis_type.column
-
-
-@pytest.mark.parametrize(
-    ("ty", "value"),
-    [
-        pytest.param('boolean', True, id="boolean"),
-        pytest.param('int8', 1, id="int8"),
-        pytest.param('int16', 1, id="int16"),
-        pytest.param('int32', 1, id="int32"),
-        pytest.param('int64', 1, id="int64"),
-        pytest.param('float', 1.0, id="float"),
-        pytest.param('double', 1.0, id="double"),
-        pytest.param('string', '1', id="string"),
-        pytest.param(
-            'timestamp',
-            ibis.timestamp('1961-04-10'),
-            id="timestamp",
-        ),
-    ],
-)
-def test_uda_primitive_output_types(ty, value):
-    func = _register_uda([ty], ty, 'test')
-
-    ibis_type = dt.validate_type(ty)
-
-    expr1 = func(value)
-    assert isinstance(expr1, ibis_type.scalar)
-
-    expr2 = func(value)
-    assert isinstance(expr2, ibis_type.scalar)
-
-
-def test_decimal(dec):
-    func = _register_udf(['decimal(12, 2)'], 'decimal(12, 2)', 'test')
-    expr = func(1.0)
-    assert type(expr) == ir.DecimalScalar
-    expr = func(dec)
-    assert type(expr) == ir.DecimalColumn
-
-
-@pytest.mark.parametrize(
-    ("ty", "valid_cast_indexer"),
-    [
-        pytest.param("decimal(12, 2)", slice(7), id="decimal"),
-        pytest.param("double", slice(6), id="double"),
-        pytest.param("float", slice(6), id="float"),
-        pytest.param("int16", slice(2), id="int16"),
-        pytest.param("int32", slice(3), id="int32"),
-        pytest.param("int64", slice(4), id="int64"),
-        pytest.param("int8", slice(1), id="int8"),
-    ],
-)
-def test_udf_valid_typecasting(ty, valid_cast_indexer, all_cols):
-    func = _register_udf([ty], 'int32', 'typecast')
-
-    for expr in all_cols[valid_cast_indexer]:
-        func(expr)
-
-
-@pytest.mark.parametrize(
-    ("ty", "valid_cast_indexer"),
-    [
-        pytest.param("boolean", slice(8), id="boolean_first_8"),
-        pytest.param("boolean", slice(9, None), id="boolean_9_onwards"),
-        pytest.param("decimal", slice(7, None), id="decimal"),
-        pytest.param("double", slice(-3, None), id="double"),
-        pytest.param("float", slice(-3, None), id="float"),
-        pytest.param("int16", slice(2, None), id="int16"),
-        pytest.param("int32", slice(3, None), id="int32"),
-        pytest.param("int64", slice(4, None), id="int64"),
-        pytest.param("int8", slice(1, None), id="int8"),
-        pytest.param("string", slice(7), id="string_first_7"),
-        pytest.param("string", slice(8, None), id="string_8_onwards"),
-        pytest.param("timestamp", slice(-1), id="timestamp"),
-    ],
-)
-def test_udf_invalid_typecasting(ty, valid_cast_indexer, all_cols):
-    func = _register_udf([ty], 'int32', 'typecast')
-
-    for expr in all_cols[valid_cast_indexer]:
-        with pytest.raises(IbisTypeError):
-            func(expr)
-
-
-def test_mult_args(i32, d, s, b, t):
-    func = _register_udf(
-        ['int32', 'double', 'string', 'boolean', 'timestamp'],
-        'int64',
-        'mult_types',
-    )
-
-    expr = func(i32, d, s, b, t)
-    assert issubclass(type(expr), ir.Column)
-
-    expr = func(1, 1.0, 'a', True, ibis.timestamp('1961-04-10'))
-    assert issubclass(type(expr), ir.Scalar)
-
-
-def _register_udf(inputs, output, name):
-    func = api.scalar_function(inputs, output, name=name)
-    func.register(name, 'ibis_testing')
-    return func
-
-
-def _register_uda(inputs, output, name):
-    func = api.aggregate_function(inputs, output, name=name)
-    func.register(name, 'ibis_testing')
-    return func
-
-
-@pytest.fixture
-def udfcon(con):
-    con.disable_codegen(False)
-    try:
-        yield con
-    finally:
-        con.disable_codegen(True)
-
-
-@pytest.fixture
-def alltypes(udfcon):
-    return udfcon.table('functional_alltypes')
-
-
-@pytest.fixture
-def udf_ll(udfcon, test_data_dir):
-    return pjoin(test_data_dir, 'udf/udf-sample.ll')
-
-
-@pytest.fixture
-def uda_ll(udfcon, test_data_dir):
-    return pjoin(test_data_dir, 'udf/uda-sample.ll')
-
-
-@pytest.fixture
-def uda_so(udfcon, test_data_dir):
-    return pjoin(test_data_dir, 'udf/libudasample.so')
-
-
-@pytest.mark.parametrize(
-    ('typ', 'lit_val', 'col_name'),
-    [
-        pytest.param('boolean', True, 'bool_col', id="boolean"),
-        pytest.param('int8', ibis.literal(5), 'tinyint_col', id="int8"),
-        pytest.param(
-            'int16',
-            ibis.literal(2**10),
-            'smallint_col',
-            id="int16",
-        ),
-        pytest.param('int32', ibis.literal(2**17), 'int_col', id="int16"),
-        pytest.param('int64', ibis.literal(2**33), 'bigint_col', id="int64"),
-        pytest.param('float', ibis.literal(3.14), 'float_col', id="float"),
-        pytest.param('double', ibis.literal(3.14), 'double_col', id="double"),
-        pytest.param(
-            'string',
-            ibis.literal('ibis'),
-            'string_col',
-            id="string",
-        ),
-        pytest.param(
-            'timestamp',
-            ibis.timestamp('1961-04-10'),
-            'timestamp_col',
-            id="timestamp",
-        ),
-    ],
-)
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_identity_primitive_types(
-    udfcon, alltypes, test_data_db, udf_ll, typ, lit_val, col_name
-):
-    col_val = alltypes[col_name]
-    identity_func_testing(udf_ll, udfcon, test_data_db, typ, lit_val, col_val)
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_decimal_fail(udfcon, test_data_db, udf_ll):
-    col = udfcon.table('tpch_customer').c_acctbal
-    literal = ibis.literal(1).cast('decimal(12,2)')
-    name = '__tmp_udf_' + util.guid()
-
-    func = udf_creation_to_op(
-        udf_ll,
-        udfcon,
-        test_data_db,
-        name,
-        'Identity',
-        ['decimal(12,2)'],
-        'decimal(12,2)',
-    )
-
-    expr = func(literal)
-    assert issubclass(type(expr), ir.Scalar)
-    result = udfcon.execute(expr)
-    assert result == Decimal(1)
-
-    expr = func(col)
-    assert issubclass(type(expr), ir.Column)
-    udfcon.execute(expr)
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_mixed_inputs(udfcon, alltypes, test_data_db, udf_ll):
-    name = 'two_args'
-    symbol = 'TwoArgs'
-    inputs = ['int32', 'int32']
-    output = 'int32'
-    func = udf_creation_to_op(
-        udf_ll, udfcon, test_data_db, name, symbol, inputs, output
-    )
-
-    expr = func(alltypes.int_col, 1)
-    assert issubclass(type(expr), ir.Column)
-    udfcon.execute(expr)
-
-    expr = func(1, alltypes.int_col)
-    assert issubclass(type(expr), ir.Column)
-    udfcon.execute(expr)
-
-    expr = func(alltypes.int_col, alltypes.tinyint_col)
-    udfcon.execute(expr)
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_implicit_typecasting(udfcon, alltypes, test_data_db, udf_ll):
-    col = alltypes.tinyint_col
-    literal = ibis.literal(1000)
-    identity_func_testing(udf_ll, udfcon, test_data_db, 'int32', literal, col)
-
-
-def identity_func_testing(udf_ll, udfcon, test_data_db, datatype, literal, column):
-    inputs = [datatype]
-    name = '__tmp_udf_' + util.guid()
-    func = udf_creation_to_op(
-        udf_ll, udfcon, test_data_db, name, 'Identity', inputs, datatype
-    )
-
-    expr = func(literal)
-    assert issubclass(type(expr), ir.Scalar)
-    result = udfcon.execute(expr)
-    # Hacky
-    if datatype == 'timestamp':
-        assert type(result) == pd.Timestamp
-    else:
-        lop = literal.op()
-        if isinstance(lop, ir.Literal):
-            np.testing.assert_allclose(lop.value, 5)
-        else:
-            np.testing.assert_allclose(result, udfcon.execute(literal), 5)
 
-    expr = func(column)
-    assert issubclass(type(expr), ir.Column)
-    udfcon.execute(expr)
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_mult_type_args(udfcon, alltypes, test_data_db, udf_ll):
-    symbol = 'AlmostAllTypes'
-    name = 'most_types'
-    inputs = [
-        'string',
-        'boolean',
-        'int8',
-        'int16',
-        'int32',
-        'int64',
-        'float',
-        'double',
-    ]
-    output = 'int32'
-
-    func = udf_creation_to_op(
-        udf_ll, udfcon, test_data_db, name, symbol, inputs, output
-    )
-
-    expr = func('a', True, 1, 1, 1, 1, 1.0, 1.0)
-    result = udfcon.execute(expr)
-    assert result == 8
-
-    table = alltypes
-    expr = func(
-        table.string_col,
-        table.bool_col,
-        table.tinyint_col,
-        table.tinyint_col,
-        table.smallint_col,
-        table.smallint_col,
-        1.0,
-        1.0,
-    )
-    udfcon.execute(expr)
-
-
-def test_all_type_args(udfcon, test_data_db, udf_ll):
-    pytest.skip('failing test, to be fixed later')
-
-    symbol = 'AllTypes'
-    name = 'all_types'
-    inputs = [
-        'string',
-        'boolean',
-        'int8',
-        'int16',
-        'int32',
-        'int64',
-        'float',
-        'double',
-        'decimal',
-    ]
-    output = 'int32'
-
-    func = udf_creation_to_op(
-        udf_ll, udfcon, test_data_db, name, symbol, inputs, output
-    )
-    expr = func('a', True, 1, 1, 1, 1, 1.0, 1.0, 1.0)
-    result = udfcon.execute(expr)
-    assert result == 9
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_udf_varargs(udfcon, alltypes, udf_ll, test_data_db):
-    t = alltypes
-
-    name = f'add_numbers_{util.guid()[:4]}'
-
-    input_sig = rules.varargs(rules.double)
-    func = api.wrap_udf(udf_ll, input_sig, 'double', 'AddNumbers', name=name)
-    func.register(name, test_data_db)
-    udfcon.create_function(func, database=test_data_db)
-
-    expr = func(t.double_col, t.double_col)
-    expr.execute()
-
-
-def test_drop_udf_not_exists(udfcon):
-    random_name = util.guid()
-    with pytest.raises(Exception):
-        udfcon.drop_udf(random_name)
-
-
-def test_drop_uda_not_exists(udfcon):
-    random_name = util.guid()
-    with pytest.raises(Exception):
-        udfcon.drop_uda(random_name)
-
-
-def udf_creation_to_op(udf_ll, udfcon, test_data_db, name, symbol, inputs, output):
-    func = api.wrap_udf(udf_ll, inputs, output, symbol, name)
-
-    udfcon.create_function(func, database=test_data_db)
-
-    func.register(name, test_data_db)
-
-    assert udfcon.exists_udf(name, test_data_db)
-    return func
-
-
-def test_ll_uda_not_supported(uda_ll):
-    # LLVM IR UDAs are not supported as of Impala 2.2
-    with pytest.raises(com.IbisError):
-        conforming_wrapper(uda_ll, ['double'], 'double', 'Variance')
-
-
-def conforming_wrapper(where, inputs, output, prefix, serialize=True, name=None):
-    kwds = {'name': name}
-    if serialize:
-        kwds['serialize_fn'] = f'{prefix}Serialize'
-    return api.wrap_uda(
-        where,
-        inputs,
-        output,
-        f'{prefix}Update',
-        init_fn=f'{prefix}Init',
-        merge_fn=f'{prefix}Merge',
-        finalize_fn=f'{prefix}Finalize',
-        **kwds,
-    )
-
-
-@pytest.fixture
-def wrapped_count_uda(uda_so):
-    name = f'user_count_{util.guid()}'
-    return api.wrap_uda(uda_so, ['int32'], 'int64', 'CountUpdate', name=name)
-
-
-def test_count_uda(udfcon, alltypes, test_data_db, wrapped_count_uda):
-    func = wrapped_count_uda
-    func.register(func.name, test_data_db)
-    udfcon.create_function(func, database=test_data_db)
-
-    # it works!
-    func(alltypes.int_col).execute()
-
-
-def test_list_udas(udfcon, temp_database, wrapped_count_uda):
-    func = wrapped_count_uda
-    db = temp_database
-    udfcon.create_function(func, database=db)
-
-    funcs = udfcon.list_udas(database=db)
-
-    f = funcs[0]
-    assert f.name == func.name
-    assert f.inputs == func.inputs
-    assert f.output == func.output
-
-
-@pytest.mark.xfail(
-    reason='Unknown reason. xfailing to restore the CI for udf tests. #2358'
-)
-def test_drop_database_with_udfs_and_udas(udfcon, temp_database, wrapped_count_uda):
-    uda1 = wrapped_count_uda
-
-    udf1 = api.wrap_udf(
-        udf_ll,
-        ['boolean'],
-        'boolean',
-        'Identity',
-        f'udf_{util.guid()}',
-    )
-
-    db = temp_database
-
-    udfcon.create_database(db)
-
-    udfcon.create_function(uda1, database=db)
-    udfcon.create_function(udf1, database=db)
-    # drop happens in test tear down
-
-
-@pytest.fixture
-def inputs():
-    return ["string", "string"]
-
-
-@pytest.fixture
-def output():
-    return "int64"
-
-
-@pytest.fixture
-def name():
-    return "test_name"
-
-
-def test_create_udf(inputs, output, name, snapshot):
-    func = api.wrap_udf(
-        '/foo/bar.so',
-        inputs,
-        output,
-        so_symbol='testFunc',
-        name=name,
-    )
-    stmt = ddl.CreateUDF(func)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_create_udf_type_conversions(output, name, snapshot):
-    inputs = ['string', 'int8', 'int16', 'int32']
-    func = api.wrap_udf(
-        '/foo/bar.so',
-        inputs,
-        output,
-        so_symbol='testFunc',
-        name=name,
-    )
-    stmt = ddl.CreateUDF(func)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_delete_udf_simple(name, inputs, snapshot):
-    stmt = ddl.DropFunction(name, inputs)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_delete_udf_if_exists(name, inputs, snapshot):
-    stmt = ddl.DropFunction(name, inputs, must_exist=False)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_delete_udf_aggregate(name, inputs, snapshot):
-    stmt = ddl.DropFunction(name, inputs, aggregate=True)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_delete_udf_db(name, inputs, snapshot):
-    stmt = ddl.DropFunction(name, inputs, database='test')
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-@pytest.mark.parametrize("ser", [True, False])
-def test_create_uda(name, inputs, output, ser, snapshot):
-    func = api.wrap_uda(
-        '/foo/bar.so',
-        inputs,
-        output,
-        update_fn='Update',
-        init_fn='Init',
-        merge_fn='Merge',
-        finalize_fn='Finalize',
-        serialize_fn='Serialize' if ser else None,
-    )
-    stmt = ddl.CreateUDA(func, name=name, database='bar')
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_list_udf(snapshot):
-    stmt = ddl.ListFunction('test')
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_list_udfs_like(snapshot):
-    stmt = ddl.ListFunction('test', like='identity')
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_list_udafs(snapshot):
-    stmt = ddl.ListFunction('test', aggregate=True)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
-
-
-def test_list_udafs_like(snapshot):
-    stmt = ddl.ListFunction('test', like='identity', aggregate=True)
-    result = stmt.compile()
-    snapshot.assert_match(result, "out.sql")
+from ibis.impala import ddl
+import ibis.impala as api
+
+from ibis.common import IbisTypeError
+from ibis.compat import unittest, Decimal
+from ibis.expr.datatypes import validate_type
+from ibis.expr.tests.mocks import MockConnection
+from ibis.impala.tests.common import ImpalaE2E
+import ibis.expr.rules as rules
+import ibis.common as com
+import ibis.util as util
+
+
+class TestWrapping(unittest.TestCase):
+
+    def setUp(self):
+        self.con = MockConnection()
+        self.table = self.con.table('functional_alltypes')
+
+        self.i8 = self.table.tinyint_col
+        self.i16 = self.table.smallint_col
+        self.i32 = self.table.int_col
+        self.i64 = self.table.bigint_col
+        self.d = self.table.double_col
+        self.f = self.table.float_col
+        self.s = self.table.string_col
+        self.b = self.table.bool_col
+        self.t = self.table.timestamp_col
+        self.dec = self.con.table('tpch_customer').c_acctbal
+        self.all_cols = [self.i8, self.i16, self.i32, self.i64, self.d,
+                         self.f, self.dec, self.s, self.b, self.t]
+
+    def test_sql_generation(self):
+        func = api.scalar_function(['string'], 'string', name='Tester')
+        func.register('identity', 'udf_testing')
+
+        result = func('hello world')
+        assert result == "SELECT udf_testing.identity('hello world')"
+
+    def test_sql_generation_from_infoclass(self):
+        func = api.wrap_udf('test.so', ['string'], 'string', 'info_test')
+        repr(func)
+
+        func.register('info_test', 'udf_testing')
+        result = func('hello world')
+        assert result == "SELECT udf_testing.info_test('hello world')"
+
+    def test_udf_primitive_output_types(self):
+        types = [
+            ('boolean', True, self.b),
+            ('int8', 1, self.i8),
+            ('int16', 1, self.i16),
+            ('int32', 1, self.i32),
+            ('int64', 1, self.i64),
+            ('float', 1.0, self.f),
+            ('double', 1.0, self.d),
+            ('string', '1', self.s),
+            ('timestamp', ibis.timestamp('1961-04-10'), self.t)
+        ]
+        for t, sv, av in types:
+            func = self._register_udf([t], t, 'test')
+
+            ibis_type = validate_type(t)
+
+            expr = func(sv)
+            assert type(expr) == ibis_type.scalar_type()
+            expr = func(av)
+            assert type(expr) == ibis_type.array_type()
+
+    def test_uda_primitive_output_types(self):
+        types = [
+            ('boolean', True, self.b),
+            ('int8', 1, self.i8),
+            ('int16', 1, self.i16),
+            ('int32', 1, self.i32),
+            ('int64', 1, self.i64),
+            ('float', 1.0, self.f),
+            ('double', 1.0, self.d),
+            ('string', '1', self.s),
+            ('timestamp', ibis.timestamp('1961-04-10'), self.t)
+        ]
+        for t, sv, av in types:
+            func = self._register_uda([t], t, 'test')
+
+            ibis_type = validate_type(t)
+
+            expr1 = func(sv)
+            expr2 = func(sv)
+            assert isinstance(expr1, ibis_type.scalar_type())
+            assert isinstance(expr2, ibis_type.scalar_type())
+
+    def test_decimal(self):
+        func = self._register_udf(['decimal(9,0)'], 'decimal(9,0)', 'test')
+        expr = func(1.0)
+        assert type(expr) == ir.DecimalScalar
+        expr = func(self.dec)
+        assert type(expr) == ir.DecimalArray
+
+    def test_udf_invalid_typecasting(self):
+        cases = [
+            ('int8', self.all_cols[:1], self.all_cols[1:]),
+            ('int16', self.all_cols[:2], self.all_cols[2:]),
+            ('int32', self.all_cols[:3], self.all_cols[3:]),
+            ('int64', self.all_cols[:4], self.all_cols[4:]),
+            ('boolean', [], self.all_cols[:8] + self.all_cols[9:]),
+
+            # allowing double here for now
+            ('float', self.all_cols[:4], [self.s, self.b, self.t, self.dec]),
+
+            ('double', self.all_cols[:4], [self.s, self.b, self.t, self.dec]),
+            ('string', [], self.all_cols[:7] + self.all_cols[8:]),
+            ('timestamp', [], self.all_cols[:-1]),
+            ('decimal', [], self.all_cols[:4] + self.all_cols[7:])
+        ]
+
+        for t, valid_casts, invalid_casts in cases:
+            func = self._register_udf([t], 'int32', 'typecast')
+
+            for expr in valid_casts:
+                func(expr)
+
+            for expr in invalid_casts:
+                self.assertRaises(IbisTypeError, func, expr)
+
+    def test_mult_args(self):
+        func = self._register_udf(['int32', 'double', 'string',
+                                   'boolean', 'timestamp'],
+                                  'int64', 'mult_types')
+
+        expr = func(self.i32, self.d, self.s, self.b, self.t)
+        assert issubclass(type(expr), ir.ArrayExpr)
+
+        expr = func(1, 1.0, 'a', True, ibis.timestamp('1961-04-10'))
+        assert issubclass(type(expr), ir.ScalarExpr)
+
+    def _register_udf(self, inputs, output, name):
+        func = api.scalar_function(inputs, output, name=name)
+        func.register(name, 'ibis_testing')
+        return func
+
+    def _register_uda(self, inputs, output, name):
+        func = api.aggregate_function(inputs, output, name=name)
+        func.register(name, 'ibis_testing')
+        return func
+
+
+class TestUDFE2E(ImpalaE2E, unittest.TestCase):
+
+    def setUp(self):
+        super(TestUDFE2E, self).setUp()
+        self.udf_ll = pjoin(self.test_data_dir, 'udf/udf-sample.ll')
+        self.uda_ll = pjoin(self.test_data_dir, 'udf/uda-sample.ll')
+        self.uda_so = pjoin(self.test_data_dir, 'udf/libudasample.so')
+
+    @pytest.mark.udf
+    def test_identity_primitive_types(self):
+        cases = [
+            ('boolean', True, self.alltypes.bool_col),
+            ('int8', 5, self.alltypes.tinyint_col),
+            ('int16', 2**10, self.alltypes.smallint_col),
+            ('int32', 2**17, self.alltypes.int_col),
+            ('int64', 2**33, self.alltypes.bigint_col),
+            ('float', 3.14, self.alltypes.float_col),
+            ('double', 3.14, self.alltypes.double_col),
+            ('string', 'ibis', self.alltypes.string_col),
+            ('timestamp', ibis.timestamp('1961-04-10'),
+             self.alltypes.timestamp_col),
+        ]
+
+        for t, lit_val, array_val in cases:
+            if not isinstance(lit_val, ir.Expr):
+                lit_val = ibis.literal(lit_val)
+            self._identity_func_testing(t, lit_val, array_val)
+
+    @pytest.mark.udf
+    def test_decimal(self):
+        col = self.con.table('tpch_customer').c_acctbal
+        literal = ibis.literal(1).cast('decimal(12,2)')
+        name = '__tmp_udf_' + util.guid()
+        func = self._udf_creation_to_op(name, 'Identity',
+                                        ['decimal(12,2)'],
+                                        'decimal(12,2)')
+
+        expr = func(literal)
+        assert issubclass(type(expr), ir.ScalarExpr)
+        result = self.con.execute(expr)
+        assert result == Decimal(1)
+
+        expr = func(col)
+        assert issubclass(type(expr), ir.ArrayExpr)
+        self.con.execute(expr)
+
+    @pytest.mark.udf
+    def test_mixed_inputs(self):
+        name = 'two_args'
+        symbol = 'TwoArgs'
+        inputs = ['int32', 'int32']
+        output = 'int32'
+        func = self._udf_creation_to_op(name, symbol, inputs, output)
+
+        expr = func(self.alltypes.int_col, 1)
+        assert issubclass(type(expr), ir.ArrayExpr)
+        self.con.execute(expr)
+
+        expr = func(1, self.alltypes.int_col)
+        assert issubclass(type(expr), ir.ArrayExpr)
+        self.con.execute(expr)
+
+        expr = func(self.alltypes.int_col, self.alltypes.tinyint_col)
+        self.con.execute(expr)
+
+    @pytest.mark.udf
+    def test_implicit_typecasting(self):
+        col = self.alltypes.tinyint_col
+        literal = ibis.literal(1000)
+        self._identity_func_testing('int32', literal, col)
+
+    def _identity_func_testing(self, datatype, literal, column):
+        inputs = [datatype]
+        name = '__tmp_udf_' + util.guid()
+        func = self._udf_creation_to_op(name, 'Identity', inputs, datatype)
+
+        expr = func(literal)
+        assert issubclass(type(expr), ir.ScalarExpr)
+        result = self.con.execute(expr)
+        # Hacky
+        if datatype is 'timestamp':
+            import pandas as pd
+            assert type(result) == pd.tslib.Timestamp
+        else:
+            lop = literal.op()
+            if isinstance(lop, ir.Literal):
+                self.assertAlmostEqual(result, lop.value, 5)
+            else:
+                self.assertAlmostEqual(result, self.con.execute(literal), 5)
+
+        expr = func(column)
+        assert issubclass(type(expr), ir.ArrayExpr)
+        self.con.execute(expr)
+
+    @pytest.mark.udf
+    def test_mult_type_args(self):
+        symbol = 'AlmostAllTypes'
+        name = 'most_types'
+        inputs = ['string', 'boolean', 'int8', 'int16', 'int32',
+                  'int64', 'float', 'double']
+        output = 'int32'
+
+        func = self._udf_creation_to_op(name, symbol, inputs, output)
+
+        expr = func('a', True, 1, 1, 1, 1, 1.0, 1.0)
+        result = self.con.execute(expr)
+        assert result == 8
+
+        table = self.alltypes
+        expr = func(table.string_col, table.bool_col, table.tinyint_col,
+                    table.tinyint_col, table.smallint_col,
+                    table.smallint_col, 1.0, 1.0)
+        self.con.execute(expr)
+
+    def test_all_type_args(self):
+        pytest.skip('failing test, to be fixed later')
+
+        symbol = 'AllTypes'
+        name = 'all_types'
+        inputs = ['string', 'boolean', 'int8', 'int16', 'int32',
+                  'int64', 'float', 'double', 'decimal']
+        output = 'int32'
+
+        func = self._udf_creation_to_op(name, symbol, inputs, output)
+        expr = func('a', True, 1, 1, 1, 1, 1.0, 1.0, 1.0)
+        result = self.con.execute(expr)
+        assert result == 9
+
+    @pytest.mark.udf
+    def test_udf_varargs(self):
+        t = self.alltypes
+
+        name = 'add_numbers_{0}'.format(util.guid()[:4])
+
+        input_sig = rules.varargs(rules.double)
+        func = api.wrap_udf(self.udf_ll, input_sig, 'double', 'AddNumbers',
+                            name=name)
+        func.register(name, self.test_data_db)
+        self.con.create_function(func, database=self.test_data_db)
+
+        expr = func(t.double_col, t.double_col)
+        expr.execute()
+
+    def test_drop_udf_not_exists(self):
+        random_name = util.guid()
+        self.assertRaises(Exception, self.con.drop_udf, random_name)
+
+    def test_drop_uda_not_exists(self):
+        random_name = util.guid()
+        self.assertRaises(Exception, self.con.drop_uda, random_name)
+
+    def _udf_creation_to_op(self, name, symbol, inputs, output):
+        func = api.wrap_udf(self.udf_ll, inputs, output, symbol, name)
+
+        self.temp_udfs.append((name, inputs))
+
+        self.con.create_function(func, database=self.test_data_db)
+
+        func.register(name, self.test_data_db)
+
+        assert self.con.exists_udf(name, self.test_data_db)
+        return func
+
+    def test_ll_uda_not_supported(self):
+        # LLVM IR UDAs are not supported as of Impala 2.2
+        with self.assertRaises(com.IbisError):
+            self._conforming_wrapper(self.uda_ll, ['double'], 'double',
+                                     'Variance')
+
+    def _conforming_wrapper(self, where, inputs, output, prefix,
+                            serialize=True, name=None):
+        kwds = {
+            'name': name
+        }
+        if serialize:
+            kwds['serialize_fn'] = '{0}Serialize'.format(prefix)
+        return api.wrap_uda(where, inputs, output, '{0}Update'.format(prefix),
+                            init_fn='{0}Init'.format(prefix),
+                            merge_fn='{0}Merge'.format(prefix),
+                            finalize_fn='{0}Finalize'.format(prefix),
+                            **kwds)
+
+    @pytest.mark.udf
+    def test_count_uda(self):
+        func = self._wrap_count_uda()
+        func.register(func.name, self.test_data_db)
+        self.con.create_function(func, database=self.test_data_db)
+
+        # it works!
+        func(self.alltypes.int_col).execute()
+        self.temp_udas.append((func.name, ['int32']))
+
+    @pytest.mark.udf
+    def test_list_udas(self):
+        db = '__ibis_tmp_{0}'.format(util.guid())
+        self.con.create_database(db)
+        self.temp_databases.append(db)
+
+        func = self._wrap_count_uda()
+        self.con.create_function(func, database=db)
+
+        funcs = self.con.list_udas(database=db)
+
+        f = funcs[0]
+        assert f.name == func.name
+        assert f.inputs == func.inputs
+        assert f.output == func.output
+
+    @pytest.mark.udf
+    def test_drop_database_with_udfs_and_udas(self):
+        uda1 = self._wrap_count_uda()
+        uda2 = self._wrap_count_uda()
+
+        udf1 = api.wrap_udf(self.udf_ll, ['boolean'], 'boolean', 'Identity',
+                            'udf_{0}'.format(util.guid()))
+
+        db = '__ibis_tmp_{0}'.format(util.guid())
+
+        self.con.create_database(db)
+
+        self.con.create_function(uda1, database=db)
+        self.con.create_function(uda2, database=db)
+
+        self.con.create_function(udf1, database=db)
+
+        self.con.drop_database(db, force=True)
+
+        assert not self.con.exists_database(db)
+
+    def _wrap_count_uda(self, name=None):
+        if name is None:
+            name = 'user_count_{0}'.format(util.guid())
+        func = api.wrap_uda(self.uda_so, ['int32'], 'int64',
+                            'CountUpdate', name=name)
+        return func
+
+
+class TestUDFDDL(unittest.TestCase):
+
+    def setUp(self):
+        self.con = MockConnection()
+        self.name = 'test_name'
+        self.inputs = ['string', 'string']
+        self.output = 'int64'
+
+    def test_create_udf(self):
+        stmt = ddl.CreateFunction('/foo/bar.so', 'testFunc', self.inputs,
+                                  self.output, self.name)
+        result = stmt.compile()
+        expected = ("CREATE FUNCTION `test_name`(string, string) "
+                    "returns bigint "
+                    "location '/foo/bar.so' symbol='testFunc'")
+        assert result == expected
+
+    def test_create_udf_type_conversions(self):
+        stmt = ddl.CreateFunction('/foo/bar.so', 'testFunc',
+                                  ['string', 'int8', 'int16', 'int32'],
+                                  self.output, self.name)
+        result = stmt.compile()
+        expected = ("CREATE FUNCTION `test_name`(string, tinyint, "
+                    "smallint, int) returns bigint "
+                    "location '/foo/bar.so' symbol='testFunc'")
+        assert result == expected
+
+    def test_delete_udf_simple(self):
+        stmt = ddl.DropFunction(self.name, self.inputs)
+        result = stmt.compile()
+        expected = "DROP FUNCTION `test_name`(string, string)"
+        assert result == expected
+
+    def test_delete_udf_if_exists(self):
+        stmt = ddl.DropFunction(self.name, self.inputs, must_exist=False)
+        result = stmt.compile()
+        expected = "DROP FUNCTION IF EXISTS `test_name`(string, string)"
+        assert result == expected
+
+    def test_delete_udf_aggregate(self):
+        stmt = ddl.DropFunction(self.name, self.inputs, aggregate=True)
+        result = stmt.compile()
+        expected = "DROP AGGREGATE FUNCTION `test_name`(string, string)"
+        assert result == expected
+
+    def test_delete_udf_db(self):
+        stmt = ddl.DropFunction(self.name, self.inputs, database='test')
+        result = stmt.compile()
+        expected = "DROP FUNCTION test.`test_name`(string, string)"
+        assert result == expected
+
+    def test_create_uda(self):
+        def make_ex(serialize=False):
+            if serialize:
+                serialize = "\nserialize_fn='Serialize'"
+            else:
+                serialize = ""
+            return (("CREATE AGGREGATE FUNCTION "
+                     "bar.`test_name`(string, string)"
+                     " returns bigint location '/foo/bar.so'"
+                     "\ninit_fn='Init'"
+                     "\nupdate_fn='Update'"
+                     "\nmerge_fn='Merge'") +
+                    serialize +
+                    ("\nfinalize_fn='Finalize'"))
+
+        for ser in [True, False]:
+            stmt = ddl.CreateAggregateFunction('/foo/bar.so', self.inputs,
+                                               self.output, 'Update', 'Init',
+                                               'Merge',
+                                               'Serialize' if ser else None,
+                                               'Finalize', self.name, 'bar')
+            result = stmt.compile()
+            expected = make_ex(ser)
+            assert result == expected
+
+    def test_list_udf(self):
+        stmt = ddl.ListFunction('test')
+        result = stmt.compile()
+        expected = 'SHOW FUNCTIONS IN test'
+        assert result == expected
+
+    def test_list_udfs_like(self):
+        stmt = ddl.ListFunction('test', like='identity')
+        result = stmt.compile()
+        expected = "SHOW FUNCTIONS IN test LIKE 'identity'"
+        assert result == expected
+
+    def test_list_udafs(self):
+        stmt = ddl.ListFunction('test', aggregate=True)
+        result = stmt.compile()
+        expected = 'SHOW AGGREGATE FUNCTIONS IN test'
+        assert result == expected
+
+    def test_list_udafs_like(self):
+        stmt = ddl.ListFunction('test', like='identity', aggregate=True)
+        result = stmt.compile()
+        expected = "SHOW AGGREGATE FUNCTIONS IN test LIKE 'identity'"
+        assert result == expected
```

### Comparing `ibis_framework-5.1.0/ibis/backends/impala/udf.py` & `ibis-framework-v0.6.0/ibis/impala/udf.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,84 +7,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import annotations
+from ibis.expr.datatypes import validate_type
+import ibis.expr.datatypes as _dt
+import ibis.expr.operations as _ops
+import ibis.expr.rules as rules
+import ibis.impala.compiler as comp
+import ibis.common as com
+import ibis.util as util
 
-import abc
-import re
 
-import ibis.common.exceptions as com
-import ibis.expr.datatypes as dt
-import ibis.expr.operations as ops
-import ibis.expr.rules as rlz
-import ibis.udf.validate as v
-from ibis import util
-from ibis.backends.base.sql.registry import fixed_arity, sql_type_names
-from ibis.backends.impala.compiler import ImpalaExprTranslator
-
-__all__ = [
-    'add_operation',
-    'scalar_function',
-    'aggregate_function',
-    'wrap_udf',
-    'wrap_uda',
-]
+__all__ = ['add_operation', 'scalar_function', 'aggregate_function',
+           'wrap_udf', 'wrap_uda']
 
 
-class Function(metaclass=abc.ABCMeta):
-    def __init__(self, inputs, output, name):
-        self.inputs = tuple(map(dt.dtype, inputs))
-        self.output = dt.dtype(output)
-        self.name = name or util.guid()
-        self._klass = self._create_operation_class()
+class Function(object):
 
-    @abc.abstractmethod
-    def _create_operation_class(self):
-        pass
+    def __init__(self, inputs, output, name):
+        self.inputs = inputs
+        self.output = output
+        self.name = name
+
+        (self.input_type,
+         self.output_type) = self._type_signature(inputs, output)
+        self._klass = self._create_operation(name)
+
+    def _create_operation(self, name):
+        class_name = self._get_class_name(name)
+        return _create_operation_class(class_name, self.input_type,
+                                       self.output_type)
 
     def __repr__(self):
         klass = type(self).__name__
-        return f'{klass}({self.name}, {self.inputs!r}, {self.output!r})'
+        return ('{0}({1}, {2!r}, {3!r})'
+                .format(klass, self.name, self.inputs, self.output))
 
     def __call__(self, *args):
         return self._klass(*args).to_expr()
 
-    def register(self, name: str, database: str) -> None:
-        """Register the given operation.
+    def register(self, name, database):
+        """
+        Registers the given operation within the Ibis SQL translation
+        toolchain. Can also use add_operation API
 
         Parameters
         ----------
-        name
-            Used in issuing statements to SQL engine
-        database
-            Database the relevant operator is registered to
+        name: used in issuing statements to SQL engine
+        database: database the relevant operator is registered to
         """
         add_operation(self._klass, name, database)
 
 
 class ScalarFunction(Function):
-    def _create_operation_class(self):
-        fields = {f'_{i}': rlz.value(dtype) for i, dtype in enumerate(self.inputs)}
-        fields['output_dtype'] = self.output
-        fields['output_shape'] = rlz.shape_like('args')
-        return type(f"UDF_{self.name}", (ops.Value,), fields)
+
+    def _get_class_name(self, name):
+        if name is None:
+            name = util.guid()
+        return 'UDF_{0}'.format(name)
+
+    def _type_signature(self, inputs, output):
+        input_type = _to_input_sig(inputs)
+        output = validate_type(output)
+        output_type = rules.shape_like_flatargs(output)
+        return input_type, output_type
 
 
 class AggregateFunction(Function):
-    def _create_operation_class(self):
-        fields = {f'_{i}': rlz.value(dtype) for i, dtype in enumerate(self.inputs)}
-        fields['output_dtype'] = self.output
-        return type(f"UDA_{self.name}", (ops.Reduction,), fields)
+
+    def _create_operation(self, name):
+        klass = Function._create_operation(self, name)
+        klass._reduction = True
+        return klass
+
+    def _get_class_name(self, name):
+        if name is None:
+            name = util.guid()
+        return 'UDA_{0}'.format(name)
+
+    def _type_signature(self, inputs, output):
+        input_type = _to_input_sig(inputs)
+        output = validate_type(output)
+        output_type = rules.scalar_output(output)
+        return input_type, output_type
 
 
-class ImpalaFunction:
+class ImpalaFunction(object):
+
     def __init__(self, name=None, lib_path=None):
         self.lib_path = lib_path
         self.name = name or util.guid()
 
         if lib_path is not None:
             self._check_library()
 
@@ -94,18 +109,19 @@
             raise ValueError('Invalid file type. Must be .so or .ll ')
 
     def hash(self):
         raise NotImplementedError
 
 
 class ImpalaUDF(ScalarFunction, ImpalaFunction):
-    """Feel free to customize my __doc__ or wrap in a nicer user API."""
-
-    def __init__(self, inputs, output, so_symbol=None, lib_path=None, name=None):
-        v.validate_output_type(output)
+    """
+    Feel free to customize my __doc__ or wrap in a nicer user API
+    """
+    def __init__(self, inputs, output, so_symbol=None, lib_path=None,
+                 name=None):
         self.so_symbol = so_symbol
         ImpalaFunction.__init__(self, name=name, lib_path=lib_path)
         ScalarFunction.__init__(self, inputs, output, name=self.name)
 
     def hash(self):
         # TODO: revisit this later
         # from hashlib import sha1
@@ -114,222 +130,196 @@
         #     val += in_type.name()
 
         # return sha1(val).hexdigest()
         pass
 
 
 class ImpalaUDA(AggregateFunction, ImpalaFunction):
-    def __init__(
-        self,
-        inputs,
-        output,
-        update_fn=None,
-        init_fn=None,
-        merge_fn=None,
-        finalize_fn=None,
-        serialize_fn=None,
-        lib_path=None,
-        name=None,
-    ):
+
+    def __init__(self, inputs, output, update_fn=None, init_fn=None,
+                 merge_fn=None, finalize_fn=None, serialize_fn=None,
+                 lib_path=None, name=None):
         self.init_fn = init_fn
         self.update_fn = update_fn
         self.merge_fn = merge_fn
         self.finalize_fn = finalize_fn
         self.serialize_fn = serialize_fn
 
-        v.validate_output_type(output)
-
         ImpalaFunction.__init__(self, name=name, lib_path=lib_path)
         AggregateFunction.__init__(self, inputs, output, name=self.name)
 
     def _check_library(self):
         suffix = self.lib_path[-3:]
         if suffix == '.ll':
             raise com.IbisInputError('LLVM IR UDAs are not yet supported')
         elif suffix != '.so':
             raise ValueError('Invalid file type. Must be .so')
 
 
-def wrap_uda(
-    hdfs_file: str,
-    inputs: str,
-    output: str,
-    update_fn: str,
-    init_fn: str | None = None,
-    merge_fn: str | None = None,
-    finalize_fn: str | None = None,
-    serialize_fn: str | None = None,
-    name: str | None = None,
-):
-    """Creates a callable aggregation function object.
-
-    Must be created in Impala to be used.
+def wrap_uda(hdfs_file, inputs, output, update_fn, init_fn=None,
+             merge_fn=None, finalize_fn=None, serialize_fn=None,
+             close_fn=None, name=None):
+    """
+    Creates a callable aggregation function object. Must be created in Impala
+    to be used
 
     Parameters
     ----------
-    hdfs_file
-        .so file that contains relevant UDA
-    inputs
-        list of strings denoting ibis datatypes
-    output
-        string denoting ibis datatype
-    update_fn
-        Library symbol name for update function
-    init_fn
-        Library symbol name for initialization function
-    merge_fn
-        Library symbol name for merge function
-    finalize_fn
-        Library symbol name for finalize function
-    serialize_fn
-        Library symbol name for serialize UDA API function. Not required for all
-        UDAs.
-    name
-        Used internally to track function
+    hdfs_file: .so file that contains relevant UDA
+    inputs: list of strings denoting ibis datatypes
+    output: string denoting ibis datatype
+    update_fn: string
+      Library symbol name for update function
+    init_fn: string, optional
+      Library symbol name for initialization function
+    merge_fn: string, optional
+      Library symbol name for merge function
+    finalize_fn: string, optional
+      Library symbol name for finalize function
+    serialize_fn : string, optional
+      Library symbol name for serialize UDA API function. Not required for all
+      UDAs; see documentation for more.
+    close_fn : string, optional
+    name: string, optional
+      Used internally to track function
 
     Returns
     -------
     container : UDA object
     """
-    return ImpalaUDA(
-        inputs,
-        output,
-        update_fn,
-        init_fn,
-        merge_fn,
-        finalize_fn,
-        serialize_fn=serialize_fn,
-        name=name,
-        lib_path=hdfs_file,
-    )
+    func = ImpalaUDA(inputs, output, update_fn, init_fn,
+                     merge_fn, finalize_fn,
+                     serialize_fn=serialize_fn,
+                     name=name, lib_path=hdfs_file)
+    return func
 
 
 def wrap_udf(hdfs_file, inputs, output, so_symbol, name=None):
-    """Creates a callable scalar function object.
-
-    Must be created in Impala to be used.
+    """
+    Creates a callable scalar function object. Must be created in Impala to be
+    used
 
     Parameters
     ----------
-    hdfs_file
-        .so file that contains relevant UDF
-    inputs
-        Input types to UDF
-    output
-        Ibis data type
-    so_symbol
-        C++ function name for relevant UDF
-    name
-        Used internally to track function
+    hdfs_file: .so file that contains relevant UDF
+    inputs: list of strings or TypeSignature
+      Input types to UDF
+    output: string
+      Ibis data type
+    so_symbol: string, C++ function name for relevant UDF
+    name: string (optional). Used internally to track function
+
+    Returns
+    -------
+    container : UDF object
     """
-    func = ImpalaUDF(inputs, output, so_symbol, name=name, lib_path=hdfs_file)
+    func = ImpalaUDF(inputs, output, so_symbol, name=name,
+                     lib_path=hdfs_file)
     return func
 
 
 def scalar_function(inputs, output, name=None):
-    """Creates an operator class that can be passed to add_operation().
+    """
+    Creates an operator class that can be passed to add_operation()
 
-    Parameters
-    ----------
-    inputs
-        Ibis data type names
-    output
-        Ibis data type
-    name
-        Used internally to track function
+    Parameters:
+    inputs: list of strings
+      Ibis data type names
+    output: string
+      Ibis data type
+    name: string, optional
+      Used internally to track function
+
+    Returns
+    -------
+    klass, user_api : class, function
     """
     return ScalarFunction(inputs, output, name=name)
 
 
 def aggregate_function(inputs, output, name=None):
-    """Creates an operator class that can be passed to add_operation().
+    """
+    Creates an operator class that can be passed to add_operation()
 
-    Parameters
-    ----------
+    Parameters:
     inputs: list of strings
       Ibis data type names
     output: string
       Ibis data type
     name: string, optional
         Used internally to track function
+
+    Returns
+    -------
+    klass, user_api : class, function
     """
     return AggregateFunction(inputs, output, name=name)
 
 
+def _to_input_sig(inputs):
+    if isinstance(inputs, rules.TypeSignature):
+        return inputs
+    else:
+        in_type = [validate_type(x) for x in inputs]
+        return rules.TypeSignature([rules.value_typed_as(x)
+                                    for x in in_type])
+
+
+def _create_operation_class(name, input_type, output_type):
+    func_dict = {
+        'input_type': input_type,
+        'output_type': output_type,
+    }
+    klass = type(name, (_ops.ValueOp,), func_dict)
+    return klass
+
+
 def add_operation(op, func_name, db):
-    """Registers the given operation within the Ibis SQL translation toolchain.
+    """
+    Registers the given operation within the Ibis SQL translation toolchain
 
     Parameters
     ----------
-    op
-        operator class
-    func_name
-        used in issuing statements to SQL engine
-    db
-        database the relevant operator is registered to
-    """
-    full_name = f'{db}.{func_name}'
-    # TODO
-    # if op.input_type is rlz.listof:
-    #     translator = comp.varargs(full_name)
-    # else:
-    arity = len(op.__signature__.parameters)
-    translator = fixed_arity(full_name, arity)
-
-    ImpalaExprTranslator._registry[op] = translator
-
-
-def parse_type(t):
-    t = t.lower()
-    if t in _impala_to_ibis_type:
-        return _impala_to_ibis_type[t]
-    elif 'varchar' in t or 'char' in t:
-        return 'string'
-    elif 'decimal' in t:
-        result = dt.dtype(t)
-        if result:
-            return t
-        else:
-            return ValueError(t)
+    op: operator class
+    name: used in issuing statements to SQL engine
+    database: database the relevant operator is registered to
+    """
+    full_name = '{0}.{1}'.format(db, func_name)
+    if isinstance(op.input_type, rules.VarArgs):
+        translator = comp.varargs(full_name)
     else:
-        raise Exception(t)
-
+        arity = len(op.input_type.types)
+        translator = comp.fixed_arity(full_name, arity)
 
-_VARCHAR_RE = re.compile(r'varchar\((\d+)\)')
-
-
-def _parse_varchar(t):
-    m = _VARCHAR_RE.match(t)
-    if m:
-        return 'string'
-    return None
+    comp._operation_registry[op] = translator
 
 
 def _impala_type_to_ibis(tval):
     if tval in _impala_to_ibis_type:
         return _impala_to_ibis_type[tval]
     return tval
 
 
 def _ibis_string_to_impala(tval):
-    if tval in sql_type_names:
-        return sql_type_names[tval]
-    result = dt.validate_type(tval)
-    return repr(result) if result else None
+    from ibis.impala.compiler import _sql_type_names
+
+    if tval in _sql_type_names:
+        return _sql_type_names[tval]
+    result = _dt._parse_decimal(tval)
+    if result:
+        return repr(result)
 
 
 _impala_to_ibis_type = {
     'boolean': 'boolean',
     'tinyint': 'int8',
     'smallint': 'int16',
     'int': 'int32',
     'bigint': 'int64',
-    'float': 'float32',
-    'double': 'float64',
+    'float': 'float',
+    'double': 'double',
     'string': 'string',
     'varchar': 'string',
     'char': 'string',
     'timestamp': 'timestamp',
-    'decimal': 'decimal',
-    'date': 'date',
-    'void': 'null',
+    'decimal': 'decimal'
 }
```

### Comparing `ibis_framework-5.1.0/ibis/backends/pandas/__init__.py` & `ibis-framework-v0.6.0/ibis/expr/format.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,310 +1,254 @@
-from __future__ import annotations
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import importlib
-from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Mapping, MutableMapping
+import ibis.util as util
 
-import pandas as pd
-
-import ibis.common.exceptions as com
-import ibis.config
-import ibis.expr.operations as ops
-import ibis.expr.schema as sch
 import ibis.expr.types as ir
-from ibis import util
-from ibis.backends.base import BaseBackend
-from ibis.backends.pandas.client import (
-    PandasDatabase,
-    PandasTable,
-    ibis_schema_to_pandas,
-)
-
-if TYPE_CHECKING:
-    import pyarrow as pa
-
-
-class BasePandasBackend(BaseBackend):
-    """Base class for backends based on pandas."""
-
-    name = "pandas"
-    backend_table_type = pd.DataFrame
-
-    class Options(ibis.config.Config):
-        enable_trace: bool = False
-
-    def do_connect(
-        self,
-        dictionary: MutableMapping[str, pd.DataFrame] | None = None,
-    ) -> None:
-        """Construct a client from a dictionary of pandas DataFrames.
-
-        Parameters
-        ----------
-        dictionary
-            An optional mapping of string table names to pandas DataFrames.
-
-        Examples
-        --------
-        >>> import ibis
-        >>> ibis.pandas.connect({"t": pd.DataFrame({"a": [1, 2, 3]})})
-        <ibis.backends.pandas.Backend at 0x...>
-        """
-        # register dispatchers
-        from ibis.backends.pandas import execution, udf  # noqa: F401
-
-        self.dictionary = dictionary or {}
-        self.schemas: MutableMapping[str, sch.Schema] = {}
-
-    def from_dataframe(
-        self,
-        df: pd.DataFrame,
-        name: str = 'df',
-        client: BasePandasBackend | None = None,
-    ) -> ir.Table:
-        """Construct an ibis table from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df
-            A pandas DataFrame
-        name
-            The name of the pandas DataFrame
-        client
-            Client dictionary will be mutated with the name of the DataFrame,
-            if not provided a new client is created
-
-        Returns
-        -------
-        Table
-            A table expression
-        """
-        if client is None:
-            return self.connect({name: df}).table(name)
-        client.dictionary[name] = df
-        return client.table(name)
-
-    @property
-    def version(self) -> str:
-        return pd.__version__
-
-    @property
-    def current_database(self):
-        raise NotImplementedError('pandas backend does not support databases')
-
-    def list_databases(self, like=None):
-        raise NotImplementedError('pandas backend does not support databases')
-
-    def list_tables(self, like=None, database=None):
-        return self._filter_with_like(list(self.dictionary.keys()), like)
-
-    def table(self, name: str, schema: sch.Schema = None):
-        df = self.dictionary[name]
-        schema = sch.infer(df, schema=schema or self.schemas.get(name, None))
-        return self.table_class(name, schema, self).to_expr()
-
-    def database(self, name=None):
-        return self.database_class(name, self)
-
-    @util.deprecated(
-        as_of="5.0", removed_in="6.0", instead="Use create_table(overwrite=True)"
-    )
-    def load_data(self, table_name, obj, **kwargs):
-        # kwargs is a catch all for any options required by other backends.
-        self.dictionary[table_name] = obj
-
-    def get_schema(self, table_name, database=None):
-        schemas = self.schemas
-        try:
-            schema = schemas[table_name]
-        except KeyError:
-            schemas[table_name] = schema = sch.infer(self.dictionary[table_name])
-        return schema
-
-    def compile(self, expr, *args, **kwargs):
-        return expr
-
-    def create_table(
-        self,
-        name: str,
-        obj: pd.DataFrame | ir.Table | None = None,
-        *,
-        schema: sch.Schema | None = None,
-        database: str | None = None,
-        temp: bool | None = None,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        """Create a table."""
-        if temp:
-            com.IbisError(
-                "Passing `temp=True` to the Pandas backend create_table method has no "
-                "effect: all tables are in memory and temporary."
-            )
-        if database:
-            com.IbisError(
-                "Passing `database` to the Pandas backend create_table method has no "
-                "effect: Pandas cannot set a database."
-            )
-        if obj is None and schema is None:
-            raise com.IbisError("The schema or obj parameter is required")
-
-        if obj is not None:
-            if not self._supports_conversion(obj):
-                raise com.BackendConversionError(
-                    f"Unable to convert {obj.__class__} object "
-                    f"to backend type: {self.__class__.backend_table_type}"
-                )
-            df = self._convert_object(obj)
-        else:
-            pandas_schema = self._convert_schema(schema)
-            dtypes = dict(pandas_schema)
-            df = self._from_pandas(pd.DataFrame(columns=dtypes.keys()).astype(dtypes))
-
-        if name in self.dictionary and not overwrite:
-            raise com.IbisError(f"Cannot overwrite existing table `{name}`")
-
-        self.dictionary[name] = df
-
-        if schema is not None:
-            self.schemas[name] = schema
-        return self.table(name)
-
-    def create_view(
-        self,
-        name: str,
-        obj: ir.Table,
-        *,
-        database: str | None = None,
-        overwrite: bool = False,
-    ) -> ir.Table:
-        return self.create_table(
-            name, obj=obj, temp=None, database=database, overwrite=overwrite
-        )
-
-    def drop_view(self, name: str, *, force: bool = False) -> None:
-        self.drop_table(name, force=force)
-
-    def drop_table(self, name: str, *, force: bool = False) -> None:
-        if not force and name in self.dictionary:
-            raise com.IbisError(
-                "Cannot drop existing table. Call drop_table with force=True to drop existing table."
-            )
-        del self.dictionary[name]
-
-    @classmethod
-    def _supports_conversion(cls, obj: Any) -> bool:
-        return True
-
-    @staticmethod
-    def _convert_schema(schema: sch.Schema):
-        return ibis_schema_to_pandas(schema)
-
-    @staticmethod
-    def _from_pandas(df: pd.DataFrame) -> pd.DataFrame:
-        return df
-
-    @classmethod
-    def _convert_object(cls, obj: Any) -> Any:
-        return cls.backend_table_type(obj)
-
-    @classmethod
-    @lru_cache
-    def _get_operations(cls):
-        backend = f"ibis.backends.{cls.name}"
-
-        execution = importlib.import_module(f"{backend}.execution")
-        execute_node = execution.execute_node
-
-        # import UDF to pick up AnalyticVectorizedUDF and others
-        importlib.import_module(f"{backend}.udf")
-
-        dispatch = importlib.import_module(f"{backend}.dispatch")
-        pre_execute = dispatch.pre_execute
-
-        return frozenset(
-            op
-            for op, *_ in execute_node.funcs.keys() | pre_execute.funcs.keys()
-            if issubclass(op, ops.Value)
-        )
-
-    @classmethod
-    def has_operation(cls, operation: type[ops.Value]) -> bool:
-        # Pandas doesn't support geospatial ops, but the dispatcher implements
-        # a common base class that makes it appear that it does. Explicitly
-        # exclude these operations.
-        if issubclass(operation, (ops.GeoSpatialUnOp, ops.GeoSpatialBinOp)):
-            return False
-        op_classes = cls._get_operations()
-        return operation in op_classes or any(
-            issubclass(operation, op_impl) for op_impl in op_classes
-        )
-
-    def _clean_up_cached_table(self, op):
-        del self.dictionary[op.name]
-
-
-class Backend(BasePandasBackend):
-    name = 'pandas'
-    database_class = PandasDatabase
-    table_class = PandasTable
-
-    def to_pyarrow(
-        self,
-        expr: ir.Expr,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        **kwargs: Any,
-    ) -> pa.Table:
-        pa = self._import_pyarrow()
-        output = self.execute(expr, params=params, limit=limit)
-
-        if isinstance(output, pd.DataFrame):
-            return pa.Table.from_pandas(output)
-        elif isinstance(output, pd.Series):
-            return pa.Array.from_pandas(output)
-        else:
-            return pa.scalar(output)
+import ibis.expr.operations as ops
 
-    def to_pyarrow_batches(
-        self,
-        expr: ir.Expr,
-        *,
-        params: Mapping[ir.Scalar, Any] | None = None,
-        limit: int | str | None = None,
-        chunk_size: int = 1000000,
-        **kwargs: Any,
-    ) -> pa.ipc.RecordBatchReader:
-        pa = self._import_pyarrow()
-        pa_table = self.to_pyarrow(expr, params=params, limit=limit)
-        return pa.RecordBatchReader.from_batches(
-            pa_table.schema, pa_table.to_batches(max_chunksize=chunk_size)
-        )
-
-    def execute(self, query, params=None, limit='default', **kwargs):
-        from ibis.backends.pandas.core import execute_and_reset
-
-        if limit != 'default' and limit is not None:
-            raise ValueError(
-                'limit parameter to execute is not yet implemented in the '
-                'pandas backend'
-            )
-
-        if not isinstance(query, ir.Expr):
-            raise TypeError(
-                "`query` has type {!r}, expected ibis.expr.types.Expr".format(
-                    type(query).__name__
-                )
-            )
 
-        node = query.op()
+class FormatMemo(object):
+    # A little sanity hack to simplify the below
 
-        if params is None:
-            params = {}
+    def __init__(self):
+        from collections import defaultdict
+        self.formatted = {}
+        self.aliases = {}
+        self.ops = {}
+        self.counts = defaultdict(lambda: 0)
+        self._repr_memo = {}
+
+    def __contains__(self, obj):
+        return self._key(obj) in self.formatted
+
+    def _key(self, obj):
+        memo_key = id(obj)
+        if memo_key in self._repr_memo:
+            return self._repr_memo[memo_key]
+        result = self._format(obj)
+        self._repr_memo[memo_key] = result
+
+        return result
+
+    def _format(self, obj):
+        return obj._repr(memo=self._repr_memo)
+
+    def observe(self, obj, formatter=lambda x: x._repr()):
+        key = self._key(obj)
+        if key not in self.formatted:
+            self.aliases[key] = 'ref_%d' % len(self.formatted)
+            self.formatted[key] = formatter(obj)
+            self.ops[key] = obj
+
+        self.counts[key] += 1
+
+    def count(self, obj):
+        return self.counts[self._key(obj)]
+
+    def get_alias(self, obj):
+        return self.aliases[self._key(obj)]
+
+    def get_formatted(self, obj):
+        return self.formatted[self._key(obj)]
+
+
+class ExprFormatter(object):
+
+    """
+    For creating a nice tree-like representation of an expression graph for
+    displaying in the console.
+
+    TODO: detect reused DAG nodes and do not display redundant information
+    """
+
+    def __init__(self, expr, indent_size=2, base_level=0, memo=None,
+                 memoize=True):
+        self.expr = expr
+        self.indent_size = indent_size
+        self.base_level = base_level
+
+        self.memoize = memoize
+
+        # For tracking "extracted" objects, like tables, that we don't want to
+        # print out more than once, and simply alias in the expression tree
+        self.memo = memo or FormatMemo()
+
+    def get_result(self):
+        what = self.expr.op()
+
+        if self.memoize:
+            self._memoize_tables()
+
+        if isinstance(what, ir.TableNode) and what.has_schema():
+            # This should also catch aggregations
+            if not self.memoize and what in self.memo:
+                text = 'Table: %s' % self.memo.get_alias(what)
+            elif isinstance(what, ops.PhysicalTable):
+                text = self._format_table(what)
+            else:
+                # Any other node type
+                text = self._format_node(what)
+        elif isinstance(what, ops.TableColumn):
+            text = self._format_column(self.expr)
+        elif isinstance(what, ir.Node):
+            text = self._format_node(what)
+        elif isinstance(what, ops.Literal):
+            text = 'Literal[%s] %s' % (self._get_type_display(),
+                                       str(what.value))
+
+        if isinstance(self.expr, ir.ValueExpr) and self.expr._name is not None:
+            text = '{0} = {1}'.format(self.expr.get_name(), text)
+
+        if self.memoize:
+            alias_to_text = [(self.memo.aliases[x],
+                              self.memo.formatted[x],
+                              self.memo.ops[x])
+                             for x in self.memo.formatted]
+            alias_to_text.sort()
+
+            # A hack to suppress printing out of a ref that is the result of
+            # the top level expression
+            refs = [x + '\n' + y
+                    for x, y, op in alias_to_text
+                    if not op.equals(what)]
+
+            text = '\n\n'.join(refs + [text])
+
+        return self._indent(text, self.base_level)
+
+    def _memoize_tables(self):
+        table_memo_ops = (ops.Aggregation, ops.Filter,
+                          ops.Projection, ops.SelfReference)
+
+        def walk(expr):
+            op = expr.op()
+
+            def visit(arg):
+                if isinstance(arg, list):
+                    [visit(x) for x in arg]
+                elif isinstance(arg, ir.Expr):
+                    walk(arg)
+
+            if isinstance(op, ops.PhysicalTable):
+                self.memo.observe(op, self._format_table)
+            elif isinstance(op, ir.Node):
+                visit(op.args)
+                if isinstance(op, table_memo_ops):
+                    self.memo.observe(op, self._format_node)
+            elif isinstance(op, ir.TableNode) and op.has_schema():
+                self.memo.observe(op, self._format_table)
+
+        walk(self.expr)
+
+    def _indent(self, text, indents=1):
+        return util.indent(text, self.indent_size * indents)
+
+    def _format_table(self, table):
+        # format the schema
+        rows = ['name: {0!s}\nschema:'.format(table.name)]
+        rows.extend(['  %s : %s' % tup for tup in
+                     zip(table.schema.names, table.schema.types)])
+        opname = type(table).__name__
+        type_display = self._get_type_display(table)
+        opline = '%s[%s]' % (opname, type_display)
+        return '{0}\n{1}'.format(opline, self._indent('\n'.join(rows)))
+
+    def _format_column(self, expr):
+        # HACK: if column is pulled from a Filter of another table, this parent
+        # will not be found in the memo
+        col = expr.op()
+        parent_op = col.parent().op()
+        if parent_op in self.memo:
+            table_formatted = self.memo.get_alias(parent_op)
         else:
-            params = {
-                k.op() if isinstance(k, ir.Expr) else k: v for k, v in params.items()
-            }
-
-        return execute_and_reset(node, params=params, **kwargs)
-
-    def _load_into_cache(self, name, expr):
-        self.create_table(name, expr.execute())
+            table_formatted = '\n' + self._indent(self._format_node(parent_op))
+        type_display = self._get_type_display(self.expr)
+        return ("Column[{0}] '{1}' from table {2}"
+                .format(type_display, col.name, table_formatted))
+
+    def _format_node(self, op):
+        formatted_args = []
+
+        def visit(what, extra_indents=0):
+            if isinstance(what, ir.Expr):
+                result = self._format_subexpr(what)
+            else:
+                result = self._indent(str(what))
+
+            if extra_indents > 0:
+                result = util.indent(result, self.indent_size)
+
+            formatted_args.append(result)
+
+        arg_names = getattr(op, '_arg_names', None)
+
+        if arg_names is None:
+            for arg in op.args:
+                if isinstance(arg, list):
+                    for x in arg:
+                        visit(x)
+                else:
+                    visit(arg)
+        else:
+            for arg, name in zip(op.args, arg_names):
+                if name is not None:
+                    name = self._indent('{0}:'.format(name))
+                if isinstance(arg, list):
+                    if name is not None and len(arg) > 0:
+                        formatted_args.append(name)
+                        indents = 1
+                    else:
+                        indents = 0
+                    for x in arg:
+                        visit(x, extra_indents=indents)
+                else:
+                    if name is not None:
+                        formatted_args.append(name)
+                        indents = 1
+                    else:
+                        indents = 0
+                    visit(arg, extra_indents=indents)
+
+        opname = type(op).__name__
+        type_display = self._get_type_display(op)
+        opline = '%s[%s]' % (opname, type_display)
+
+        return '\n'.join([opline] + formatted_args)
+
+    def _format_subexpr(self, expr):
+        formatter = ExprFormatter(expr, base_level=1, memo=self.memo,
+                                  memoize=False)
+        return formatter.get_result()
+
+    def _get_type_display(self, expr=None):
+        if expr is None:
+            expr = self.expr
+
+        if isinstance(expr, ir.Node):
+            expr = expr.to_expr()
+
+        if isinstance(expr, ir.TableExpr):
+            return 'table'
+        elif isinstance(expr, ir.ArrayExpr):
+            return 'array(%s)' % expr.type()
+        elif isinstance(expr, ir.SortExpr):
+            return 'array-sort'
+        elif isinstance(expr, (ir.ScalarExpr, ir.AnalyticExpr)):
+            return '%s' % expr.type()
+        elif isinstance(expr, ir.ExprList):
+            list_args = [self._get_type_display(arg)
+                         for arg in expr.op().args]
+            return ', '.join(list_args)
+        else:
+            raise NotImplementedError
```

### Comparing `ibis_framework-5.1.0/ibis/backends/pandas/client.py` & `ibis-framework-v0.6.0/ibis/impala/pandas_interop.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,247 +1,209 @@
-"""The pandas client implementation."""
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from __future__ import annotations
 
-import json
-import warnings
-from typing import TYPE_CHECKING
-from uuid import UUID
+from posixpath import join as pjoin
+import os
 
-import numpy as np
+import pandas.core.common as pdcom
 import pandas as pd
-import toolz
-from dateutil.parser import parse as date_parse
-from pandas.api.types import CategoricalDtype, DatetimeTZDtype
-
-import ibis.expr.datatypes as dt
-import ibis.expr.operations as ops
-import ibis.expr.schema as sch
-from ibis import util
-from ibis.backends.base import Database
-from ibis.expr.operations.relations import TableProxy
-
-_ibis_dtypes = toolz.valmap(
-    np.dtype,
-    {
-        dt.Boolean: np.bool_,
-        dt.Null: np.object_,
-        dt.Array: np.object_,
-        dt.String: np.object_,
-        dt.Binary: np.object_,
-        dt.Date: 'datetime64[ns]',
-        dt.Time: 'timedelta64[ns]',
-        dt.Timestamp: 'datetime64[ns]',
-        dt.Int8: np.int8,
-        dt.Int16: np.int16,
-        dt.Int32: np.int32,
-        dt.Int64: np.int64,
-        dt.UInt8: np.uint8,
-        dt.UInt16: np.uint16,
-        dt.UInt32: np.uint32,
-        dt.UInt64: np.uint64,
-        dt.Float16: np.float16,
-        dt.Float32: np.float32,
-        dt.Float64: np.float64,
-        dt.Decimal: np.object_,
-        dt.Struct: np.object_,
-    },
-)
-
-if TYPE_CHECKING:
-    import pyarrow as pa
-
-
-@dt.dtype.register(DatetimeTZDtype)
-def from_pandas_tzdtype(value):
-    return dt.Timestamp(timezone=str(value.tz))
-
-
-@dt.dtype.register(CategoricalDtype)
-def from_pandas_categorical(_):
-    return dt.String()
-
-
-@dt.dtype.register(pd.core.dtypes.base.ExtensionDtype)
-def from_pandas_extension_dtype(t):
-    return getattr(dt, t.__class__.__name__.replace("Dtype", "").lower())
-
-
-try:
-    _arrow_dtype_class = pd.ArrowDtype
-except AttributeError:
-    warnings.warn(
-        f"The `ArrowDtype` class is not available in pandas {pd.__version__}. "
-        "Install pandas >= 1.5.0 for interop with pandas and arrow dtype support"
-    )
-else:
-
-    @dt.dtype.register(_arrow_dtype_class)
-    def from_pandas_arrow_extension_dtype(t):
-        import ibis.backends.pyarrow.datatypes as _  # noqa: F401
-
-        return dt.dtype(t.pyarrow_dtype)
-
-
-@sch.schema.register(pd.Series)
-def schema_from_series(s):
-    return sch.schema(tuple(s.items()))
-
-
-@sch.infer.register(pd.DataFrame)
-def infer_pandas_schema(df: pd.DataFrame, schema=None):
-    schema = schema if schema is not None else {}
 
-    pairs = []
-    for column_name in df.dtypes.keys():
-        if not isinstance(column_name, str):
-            raise TypeError('Column names must be strings to use the pandas backend')
-
-        if column_name in schema:
-            ibis_dtype = dt.dtype(schema[column_name])
-        else:
-            ibis_dtype = dt.infer(df[column_name]).value_type
-
-        pairs.append((column_name, ibis_dtype))
+import ibis.common as com
 
-    return sch.schema(pairs)
+from ibis.config import options
+from ibis.util import log
+import ibis.compat as compat
+import ibis.expr.datatypes as itypes
+import ibis.util as util
 
 
-def ibis_dtype_to_pandas(ibis_dtype: dt.DataType):
-    """Convert ibis dtype to the pandas / numpy alternative."""
-    assert isinstance(ibis_dtype, dt.DataType)
-
-    if ibis_dtype.is_timestamp() and ibis_dtype.timezone:
-        return DatetimeTZDtype('ns', ibis_dtype.timezone)
-    elif ibis_dtype.is_interval():
-        return np.dtype(f'timedelta64[{ibis_dtype.unit}]')
-    else:
-        return _ibis_dtypes.get(type(ibis_dtype), np.dtype(np.object_))
-
+# ----------------------------------------------------------------------
+# pandas integration
 
-def ibis_schema_to_pandas(schema):
-    return list(zip(schema.names, map(ibis_dtype_to_pandas, schema.types)))
 
+def pandas_col_to_ibis_type(col):
+    import numpy as np
+    dty = col.dtype
 
-@sch.convert.register(DatetimeTZDtype, dt.Timestamp, pd.Series)
-def convert_datetimetz_to_timestamp(_, out_dtype, column):
-    output_timezone = out_dtype.timezone
-    if output_timezone is not None:
-        return column.dt.tz_convert(output_timezone)
+    # datetime types
+    if pdcom.is_datetime64_dtype(dty):
+        if pdcom.is_datetime64_ns_dtype(dty):
+            return 'timestamp'
+        else:
+            raise com.IbisTypeError("Column {0} has dtype {1}, which is "
+                                    "datetime64-like but does "
+                                    "not use nanosecond units"
+                                    .format(col.name, dty))
+    if pdcom.is_timedelta64_dtype(dty):
+        print("Warning: encoding a timedelta64 as an int64")
+        return 'int64'
+
+    if pdcom.is_categorical_dtype(dty):
+        return itypes.Category(len(col.cat.categories))
+
+    if pdcom.is_bool_dtype(dty):
+        return 'boolean'
+
+    # simple numerical types
+    if issubclass(dty.type, np.int8):
+        return 'int8'
+    if issubclass(dty.type, np.int16):
+        return 'int16'
+    if issubclass(dty.type, np.int32):
+        return 'int32'
+    if issubclass(dty.type, np.int64):
+        return 'int64'
+    if issubclass(dty.type, np.float32):
+        return 'float'
+    if issubclass(dty.type, np.float64):
+        return 'double'
+    if issubclass(dty.type, np.uint8):
+        return 'int16'
+    if issubclass(dty.type, np.uint16):
+        return 'int32'
+    if issubclass(dty.type, np.uint32):
+        return 'int64'
+    if issubclass(dty.type, np.uint64):
+        raise com.IbisTypeError("Column {0} is an unsigned int64"
+                                .format(col.name))
+
+    if pdcom.is_object_dtype(dty):
+        return _infer_object_dtype(col)
+
+    raise com.IbisTypeError("Column {0} is dtype {1}".format(col.name, dty))
+
+
+def _infer_object_dtype(arr):
+    # TODO: accelerate with Cython/C
+
+    BOOLEAN, STRING = 0, 1
+    state = BOOLEAN
+
+    avalues = arr.values if isinstance(arr, pd.Series) else arr
+    nulls = pd.isnull(avalues)
+
+    if nulls.any():
+        for i in compat.range(len(avalues)):
+            if state == BOOLEAN:
+                if not nulls[i] and not pdcom.is_bool(avalues[i]):
+                    state = STRING
+            elif state == STRING:
+                break
+        if state == BOOLEAN:
+            return 'boolean'
+        elif state == STRING:
+            return 'string'
     else:
-        return column.dt.tz_localize(None)
+        return pd.lib.infer_dtype(avalues)
 
 
-@sch.convert.register(np.dtype, dt.Interval, pd.Series)
-def convert_any_to_interval(_, out_dtype, column):
-    return column.values.astype(out_dtype.to_pandas())
+class DataFrameWriter(object):
 
+    """
+    Interface class for writing pandas objects to Impala tables
 
-@sch.convert.register(np.dtype, dt.String, pd.Series)
-def convert_any_to_string(_, out_dtype, column):
-    result = column.astype(out_dtype.to_pandas(), errors='ignore')
-    return result
+    Class takes ownership of any temporary data written to HDFS
+    """
+    def __init__(self, client, df, path=None):
+        self.client = client
+        self.hdfs = client.hdfs
 
+        self.df = df
 
-@sch.convert.register(np.dtype, dt.UUID, pd.Series)
-def convert_any_to_uuid(_, out_dtype, column):
-    return column.map(lambda v: v if isinstance(v, UUID) else UUID(v))
+        self.temp_hdfs_dirs = []
 
+    def write_temp_csv(self):
+        temp_hdfs_dir = pjoin(options.impala.temp_hdfs_path,
+                              'pandas_{0}'.format(util.guid()))
+        self.hdfs.mkdir(temp_hdfs_dir)
 
-@sch.convert.register(np.dtype, dt.Boolean, pd.Series)
-def convert_boolean_to_series(in_dtype, out_dtype, column):
-    # XXX: this is a workaround until #1595 can be addressed
-    in_dtype_type = in_dtype.type
-    out_dtype_type = out_dtype.to_pandas().type
-    if column.empty:
-        return column.astype(out_dtype_type)
-    elif in_dtype_type != np.object_ and in_dtype_type != out_dtype_type:
-        return column.map(lambda value: pd.NA if pd.isna(value) else bool(value))
-    return column
+        # Keep track of the temporary HDFS file
+        self.temp_hdfs_dirs.append(temp_hdfs_dir)
 
+        # Write the file to HDFS
+        hdfs_path = pjoin(temp_hdfs_dir, '0.csv')
 
-@sch.convert.register(DatetimeTZDtype, dt.Date, pd.Series)
-def convert_timestamp_to_date(in_dtype, out_dtype, column):
-    if in_dtype.tz is not None:
-        column = column.dt.tz_convert("UTC").dt.tz_localize(None)
-    return column.astype(out_dtype.to_pandas(), errors='ignore').dt.normalize()
+        self.write_csv(hdfs_path)
 
+        return temp_hdfs_dir
 
-@sch.convert.register(object, dt.DataType, pd.Series)
-def convert_any_to_any(_, out_dtype, column):
-    try:
-        return column.astype(out_dtype.to_pandas())
-    except Exception:  # noqa: BLE001
-        return column
+    def write_csv(self, path):
+        import csv
 
+        tmp_path = 'tmp_{0}.csv'.format(util.guid())
+        f = open(tmp_path, 'w+')
 
-@sch.convert.register(np.dtype, dt.Timestamp, pd.Series)
-def convert_any_to_timestamp(_, out_dtype, column):
-    try:
-        return column.astype(out_dtype.to_pandas())
-    except pd.errors.OutOfBoundsDatetime:
-        try:
-            return column.map(date_parse)
-        except TypeError:
-            return column
-    except TypeError:
-        column = pd.to_datetime(column)
-        timezone = out_dtype.timezone
         try:
-            return column.dt.tz_convert(timezone)
-        except TypeError:
-            return column.dt.tz_localize(timezone)
-
-
-@sch.convert.register(object, dt.Struct, pd.Series)
-def convert_struct_to_dict(_, out_dtype, column):
-    def convert_element(values, names=out_dtype.names):
-        if values is None or isinstance(values, dict) or pd.isna(values):
-            return values
-        return dict(zip(names, values))
-
-    return column.map(convert_element)
-
-
-@sch.convert.register(np.dtype, dt.Array, pd.Series)
-def convert_array_to_series(in_dtype, out_dtype, column):
-    return column.map(lambda x: list(x) if util.is_iterable(x) else x)
+            # Write the DataFrame to the temporary file path
+            if options.verbose:
+                log('Writing DataFrame to temporary file')
+
+            self.df.to_csv(f, header=False, index=False,
+                           sep=',',
+                           quoting=csv.QUOTE_NONE,
+                           escapechar='\\',
+                           na_rep='#NULL')
+            f.seek(0)
+
+            if options.verbose:
+                log('Writing CSV to: {0}'.format(path))
+
+            self.hdfs.put(path, f)
+        finally:
+            f.close()
+            try:
+                os.remove(tmp_path)
+            except os.error:
+                pass
+
+        return path
+
+    def get_schema(self):
+        # define a temporary table using delimited data
+        return pandas_to_ibis_schema(self.df)
+
+    def delimited_table(self, csv_dir, name=None, database=None):
+        temp_delimited_name = 'ibis_tmp_pandas_{0}'.format(util.guid())
+        schema = self.get_schema()
+
+        return self.client.delimited_file(csv_dir, schema,
+                                          name=temp_delimited_name,
+                                          database=database,
+                                          delimiter=',',
+                                          na_rep='#NULL',
+                                          escapechar='\\\\',
+                                          external=True,
+                                          persist=False)
 
-
-@sch.convert.register(np.dtype, dt.Map, pd.Series)
-def convert_map_to_series(in_dtype, out_dtype, column):
-    return column.map(lambda x: dict(x) if util.is_iterable(x) else x)
-
-
-@sch.convert.register(np.dtype, dt.JSON, pd.Series)
-def convert_json_to_series(in_, out, col: pd.Series):
-    def try_json(x):
-        if x is None:
-            return x
+    def __del__(self):
         try:
-            return json.loads(x)
-        except (TypeError, json.JSONDecodeError):
-            return x
-
-    return pd.Series(list(map(try_json, col)), dtype="object")
-
-
-class DataFrameProxy(TableProxy):
-    __slots__ = ()
-
-    def to_frame(self) -> pd.DataFrame:
-        return self._data
+            self.cleanup()
+        except com.IbisError:
+            pass
+
+    def cleanup(self):
+        for path in self.temp_hdfs_dirs:
+            self.hdfs.rmdir(path)
+        self.temp_hdfs_dirs = []
+        self.csv_dir = None
 
-    def to_pyarrow(self, schema: sch.Schema) -> pa.Table:
-        import pyarrow as pa
 
-        from ibis.backends.pyarrow.datatypes import ibis_to_pyarrow_schema
-
-        return pa.Table.from_pandas(self._data, schema=ibis_to_pyarrow_schema(schema))
-
-
-class PandasTable(ops.DatabaseTable):
-    pass
-
-
-class PandasDatabase(Database):
-    pass
+def pandas_to_ibis_schema(frame):
+    from ibis.expr.api import schema
+    # no analog for decimal in pandas
+    pairs = []
+    for col_name in frame:
+        ibis_type = pandas_col_to_ibis_type(frame[col_name])
+        pairs.append((col_name, ibis_type))
+    return schema(pairs)
```

### Comparing `ibis_framework-5.1.0/ibis/backends/tests/base.py` & `ibis-framework-v0.6.0/ibis/expr/groupby.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,256 +1,230 @@
-from __future__ import annotations
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import abc
-import concurrent.futures
-import inspect
-import subprocess
-from pathlib import Path
-from typing import Any, Mapping, NamedTuple
-
-import numpy as np
-import pandas as pd
-import pandas.testing as tm
-import pytest
-from filelock import FileLock
+# User API for grouped data operations
 
+import ibis.expr.analysis as L
+import ibis.expr.operations as ops
 import ibis.expr.types as ir
+import ibis.expr.window as _window
+import ibis.util as util
 
 
-# TODO: Merge into BackendTest, #2564
-class RoundingConvention:
-    @staticmethod
-    @abc.abstractmethod
-    def round(series: pd.Series, decimals: int = 0) -> pd.Series:
-        """Round a series to `decimals` number of decimal values."""
-
-
-# TODO: Merge into BackendTest, #2564
-class RoundAwayFromZero(RoundingConvention):
-    @staticmethod
-    def round(series: pd.Series, decimals: int = 0) -> pd.Series:
-        if not decimals:
-            return (-(np.sign(series)) * np.ceil(-(series.abs()) - 0.5)).astype(
-                np.int64
-            )
-        return series.round(decimals=decimals)
-
-
-# TODO: Merge into BackendTest, #2564
-class RoundHalfToEven(RoundingConvention):
-    @staticmethod
-    def round(series: pd.Series, decimals: int = 0) -> pd.Series:
-        result = series.round(decimals=decimals)
-        return result if decimals else result.astype(np.int64)
-
-
-# TODO: Merge into BackendTest, #2564
-class UnorderedComparator:
-    @classmethod
-    def assert_series_equal(
-        cls, left: pd.Series, right: pd.Series, *args: Any, **kwargs: Any
-    ) -> None:
-        left = left.sort_values().reset_index(drop=True)
-        right = right.sort_values().reset_index(drop=True)
-        return super().assert_series_equal(left, right, *args, **kwargs)
-
-    @classmethod
-    def assert_frame_equal(
-        cls, left: pd.DataFrame, right: pd.DataFrame, *args: Any, **kwargs: Any
-    ) -> None:
-        columns = list(set(left.columns) & set(right.columns))
-        left = left.sort_values(by=columns)
-        right = right.sort_values(by=columns)
-        return super().assert_frame_equal(left, right, *args, **kwargs)
-
-
-class BackendTest(abc.ABC):
-    check_dtype = True
-    check_names = True
-    supports_arrays = True
-    supports_arrays_outside_of_select = supports_arrays
-    supports_window_operations = True
-    additional_skipped_operations = frozenset()
-    supports_divide_by_zero = False
-    returned_timestamp_unit = 'us'
-    supported_to_timestamp_units = {'s', 'ms', 'us'}
-    supports_floating_modulus = True
-    native_bool = True
-    supports_structs = True
-    supports_json = True
-    supports_map = False  # basically nothing does except trino and snowflake
-    reduction_tolerance = 1e-7
-
-    @staticmethod
-    def format_table(name: str) -> str:
-        return name
-
-    def __init__(self, data_directory: Path) -> None:
-        self.connection = self.connect(data_directory)
-        self.data_directory = data_directory
-
-    def __str__(self):
-        return f'<BackendTest {self.name()}>'
-
-    @classmethod
-    def name(cls) -> str:
-        backend_tests_path = inspect.getmodule(cls).__file__
-        return Path(backend_tests_path).resolve().parent.parent.name
-
-    @staticmethod
-    @abc.abstractmethod
-    def connect(data_directory: Path):
-        """Return a connection with data loaded from `data_directory`."""
-
-    @staticmethod
-    def _load_data(  # noqa: B027
-        data_directory: Path, script_directory: Path, **kwargs: Any
-    ) -> None:
-        """Load test data into a backend.
-
-        Default implementation is a no-op.
-        """
-
-    @classmethod
-    def load_data(
-        cls, data_dir: Path, script_dir: Path, tmpdir: Path, worker_id: str, **kw: Any
-    ) -> None:
-        """Load testdata from `data_directory` into the backend using scripts
-        in `script_directory`."""
-        # handling for multi-processes pytest
-
-        # get the temp directory shared by all workers
-        root_tmp_dir = tmpdir.getbasetemp()
-        if worker_id != "master":
-            root_tmp_dir = root_tmp_dir.parent
-
-        fn = root_tmp_dir / f"lockfile_{cls.name()}"
-        with FileLock(f"{fn}.lock"):
-            if not fn.exists():
-                cls.preload(data_dir)
-                cls._load_data(data_dir, script_dir, **kw)
-                fn.touch()
-        return cls(data_dir)
-
-    @classmethod
-    def preload(cls, data_dir: Path):  # noqa: B027
-        """Code to execute before loading data."""
-
-    @classmethod
-    def assert_series_equal(
-        cls, left: pd.Series, right: pd.Series, *args: Any, **kwargs: Any
-    ) -> None:
-        kwargs.setdefault('check_dtype', cls.check_dtype)
-        kwargs.setdefault('check_names', cls.check_names)
-        tm.assert_series_equal(left, right, *args, **kwargs)
-
-    @classmethod
-    def assert_frame_equal(
-        cls, left: pd.DataFrame, right: pd.DataFrame, *args: Any, **kwargs: Any
-    ) -> None:
-        left = left.reset_index(drop=True)
-        right = right.reset_index(drop=True)
-        tm.assert_frame_equal(left, right, *args, **kwargs)
-
-    @staticmethod
-    def default_series_rename(series: pd.Series, name: str = 'tmp') -> pd.Series:
-        return series.rename(name)
-
-    @property
-    def functional_alltypes(self) -> ir.Table:
-        t = self.connection.table('functional_alltypes')
-        if not self.native_bool:
-            return t.mutate(bool_col=t.bool_col == 1)
-        return t
-
-    @property
-    def batting(self) -> ir.Table:
-        return self.connection.table('batting')
-
-    @property
-    def awards_players(self) -> ir.Table:
-        return self.connection.table('awards_players')
-
-    @property
-    def diamonds(self) -> ir.Table:
-        return self.connection.table('diamonds')
-
-    @property
-    def geo(self) -> ir.Table | None:
-        if 'geo' in self.connection.list_tables():
-            return self.connection.table('geo')
-        return None
-
-    @property
-    def struct(self) -> ir.Table | None:
-        if self.supports_structs:
-            return self.connection.table("struct")
-        else:
-            pytest.xfail(f"{self.name()} backend does not support struct types")
+def _resolve_exprs(table, exprs):
+    exprs = util.promote_list(exprs)
+    return table._resolve(exprs)
+
+
+class GroupedTableExpr(object):
+
+    """
+    Helper intermediate construct
+    """
+
+    def __init__(self, table, by, having=None, order_by=None, window=None):
+        self.table = table
+        self.by = _resolve_exprs(table, by)
+        self._order_by = order_by or []
+        self._having = having or []
+        self._window = window
+
+    def __getitem__(self, args):
+        # Shortcut for projection with window functions
+        return self.projection(list(args))
 
-    @property
-    def array_types(self) -> ir.Table | None:
-        if self.supports_arrays:
-            return self.connection.table("array_types")
+    def __getattr__(self, attr):
+        if hasattr(self.table, attr):
+            return self._column_wrapper(attr)
+
+        raise AttributeError("GroupBy has no attribute %r" % attr)
+
+    def _column_wrapper(self, attr):
+        col = self.table[attr]
+        if isinstance(col, ir.NumericValue):
+            return GroupedNumbers(col, self)
         else:
-            pytest.xfail(f"{self.name()} backend does not support array types")
+            return GroupedArray(col, self)
+
+    def aggregate(self, metrics=None, **kwds):
+        return self.table.aggregate(metrics, by=self.by,
+                                    having=self._having, **kwds)
 
-    @property
-    def json_t(self) -> ir.Table | None:
-        from ibis import _
+    def having(self, expr):
+        """
+        Add a post-aggregation result filter (like the having argument in
+        `aggregate`), for composability with the group_by API
+
+        Parameters
+        ----------
 
-        if self.supports_json:
-            return self.connection.table("json_t").mutate(js=_.js.cast("json"))
+        Returns
+        -------
+        grouped : GroupedTableExpr
+        """
+        exprs = util.promote_list(expr)
+        new_having = self._having + exprs
+        return GroupedTableExpr(self.table, self.by, having=new_having,
+                                order_by=self._order_by,
+                                window=self._window)
+
+    def order_by(self, expr):
+        """
+        Expressions to use for ordering data for a window function
+        computation. Ignored in aggregations.
+
+        Parameters
+        ----------
+        expr : value expression or list of value expressions
+
+        Returns
+        -------
+        grouped : GroupedTableExpr
+        """
+        exprs = util.promote_list(expr)
+        new_order = self._order_by + exprs
+        return GroupedTableExpr(self.table, self.by, having=self._having,
+                                order_by=new_order,
+                                window=self._window)
+
+    def mutate(self, exprs=None, **kwds):
+        """
+        Returns a table projection with analytic / window functions
+        applied. Any arguments can be functions.
+
+        Parameters
+        ----------
+        exprs : list, default None
+        kwds : key=value pairs
+
+        Examples
+        --------
+        >>> expr = (table
+                    .group_by('foo')
+                    .order_by(ibis.desc('bar'))
+                    .mutate(qux=lambda x: x.baz.lag(),
+                            qux2=table.baz.lead()))
+
+        Returns
+        -------
+        mutated : TableExpr
+        """
+        if exprs is None:
+            exprs = []
         else:
-            pytest.xfail(f"{self.name()} backend does not support json types")
+            exprs = util.promote_list(exprs)
+
+        kwd_names = list(kwds.keys())
+        kwd_values = list(kwds.values())
+        kwd_values = self.table._resolve(kwd_values)
+
+        for k, v in sorted(zip(kwd_names, kwd_values)):
+            exprs.append(v.name(k))
+
+        return self.projection([self.table] + exprs)
 
-    @property
-    def map(self) -> ir.Table | None:
-        if self.supports_map:
-            return self.connection.table("map")
+    def projection(self, exprs):
+        """
+        Like mutate, but do not include existing table columns
+        """
+        w = self._get_window()
+        windowed_exprs = []
+        exprs = self.table._resolve(exprs)
+        for expr in exprs:
+            expr = L.windowize_function(expr, w=w)
+            windowed_exprs.append(expr)
+        return self.table.projection(windowed_exprs)
+
+    def _get_window(self):
+        if self._window is None:
+            groups = self.by
+            sorts = self._order_by
+            preceding, following = None, None
         else:
-            pytest.xfail(f"{self.name()} backend does not support map types")
+            w = self._window
+            groups = w.group_by + self.by
+            sorts = w.order_by + self._order_by
+            preceding, following = w.preceding, w.following
+
+        sorts = [ops.to_sort_key(self.table, k) for k in sorts]
+
+        return _window.window(preceding=preceding, following=following,
+                              group_by=groups, order_by=sorts)
+
+    def over(self, window):
+        """
+        Add a window clause to be applied to downstream analytic expressions
+        """
+        return GroupedTableExpr(self.table, self.by, having=self._having,
+                                order_by=self._order_by,
+                                window=window)
+
+    def count(self, metric_name='count'):
+        """
+        Convenience function for computing the group sizes (number of rows per
+        group) given a grouped table.
+
+        Parameters
+        ----------
+        metric_name : string, default 'count'
+          Name to use for the row count metric
+
+        Returns
+        -------
+        aggregated : TableExpr
+          The aggregated table
+        """
+        metric = self.table.count().name(metric_name)
+        return self.table.aggregate([metric], by=self.by)
+
+    size = count
+
+
+def _group_agg_dispatch(name):
+    def wrapper(self, *args, **kwargs):
+        f = getattr(self.arr, name)
+        metric = f(*args, **kwargs)
+        alias = '{0}({1})'.format(name, self.arr.get_name())
+        return self.parent.aggregate(metric.name(alias))
+
+    wrapper.__name__ = name
+    return wrapper
+
+
+class GroupedArray(object):
+
+    def __init__(self, arr, parent):
+        self.arr = arr
+        self.parent = parent
+
+    count = _group_agg_dispatch('count')
+    size = count
+    min = _group_agg_dispatch('min')
+    max = _group_agg_dispatch('max')
+    approx_nunique = _group_agg_dispatch('approx_nunique')
+    approx_median = _group_agg_dispatch('approx_median')
+    group_concat = _group_agg_dispatch('group_concat')
+
+    def summary(self, exact_nunique=False):
+        metric = self.arr.summary(exact_nunique=exact_nunique)
+        return self.parent.aggregate(metric)
+
+
+class GroupedNumbers(GroupedArray):
+
+    mean = _group_agg_dispatch('mean')
+    sum = _group_agg_dispatch('sum')
 
-    @property
-    def win(self) -> ir.Table | None:
-        return self.connection.table("win")
-
-    @property
-    def api(self):
-        return self.connection
-
-    def make_context(self, params: Mapping[ir.Value, Any] | None = None):
-        return self.api.compiler.make_context(params=params)
-
-
-class ServiceSpec(NamedTuple):
-    name: str
-    data_volume: str
-    files: list[Path]
-
-
-class ServiceBackendTest(BackendTest):
-    @classmethod
-    @abc.abstractmethod
-    def service_spec(data_dir: Path) -> ServiceSpec:
-        ...
-
-    @classmethod
-    def preload(cls, data_dir: Path):
-        spec = cls.service_spec(data_dir)
-        service = spec.name
-        data_volume = spec.data_volume
-        with concurrent.futures.ThreadPoolExecutor() as e:
-            for fut in concurrent.futures.as_completed(
-                e.submit(
-                    subprocess.check_call,
-                    [
-                        "docker",
-                        "compose",
-                        "cp",
-                        str(path),
-                        f"{service}:{data_volume}/{path.name}",
-                    ],
-                )
-                for path in spec.files
-            ):
-                fut.result()
+    def summary(self, exact_nunique=False):
+        metric = self.arr.summary(exact_nunique=exact_nunique)
+        return self.parent.aggregate(metric)
```

### Comparing `ibis_framework-5.1.0/ibis/expr/analysis.py` & `ibis-framework-v0.6.0/ibis/cloudpickle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,859 +1,874 @@
-from __future__ import annotations
+"""
+This class is defined to override standard pickle functionality
 
-import functools
-import operator
-from collections import defaultdict
-from typing import Iterable, Iterator, Mapping
-
-import toolz
+The goals of it follow:
+-Serialize lambdas and nested functions to compiled byte code
+-Deal with main module correctly
+-Deal with other non-serializable objects
+
+It does not include an unpickler, as standard python unpickling suffices.
+
+This module was extracted from the `cloud` package, developed by `PiCloud, Inc.
+<http://www.picloud.com>`_, and as modified for Apache Spark (licensed under
+ASL 2.0).
+
+Copyright (c) 2012, Regents of the University of California.
+Copyright (c) 2009 `PiCloud, Inc. <http://www.picloud.com>`_.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions
+are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of the University of California, Berkeley nor the
+      names of its contributors may be used to endorse or promote
+      products derived from this software without specific prior written
+      permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+"""
 
-import ibis.common.graph as g
-import ibis.expr.operations as ops
-import ibis.expr.operations.relations as rels
-import ibis.expr.types as ir
-from ibis import util
-from ibis.common.exceptions import IbisTypeError, IntegrityError
-
-# ---------------------------------------------------------------------
-# Some expression metaprogramming / graph transformations to support
-# compilation later
-
-
-def sub_for(node: ops.Node, substitutions: Mapping[ops.node, ops.Node]) -> ops.Node:
-    """Substitute operations in `node` with nodes in `substitutions`.
-
-    Parameters
-    ----------
-    node
-        An Ibis operation
-    substitutions
-        A mapping from node to node. If any subnode of `node` is equal to any
-        of the keys in `substitutions`, the value for that key will replace the
-        corresponding node in `node`.
-
-    Returns
-    -------
-    Node
-        An Ibis expression
-    """
-    assert isinstance(node, ops.Node), type(node)
+# flake8: noqa
 
-    def fn(node):
-        try:
-            return substitutions[node]
-        except KeyError:
-            if isinstance(node, ops.TableNode):
-                return g.halt
-            return g.proceed
-
-    return substitute(fn, node)
-
-
-def sub_immediate_parents(op: ops.Node, table: ops.TableNode) -> ops.Node:
-    """Replace immediate parent tables in `op` with `table`."""
-    return sub_for(op, {base: table for base in find_immediate_parent_tables(op)})
-
-
-class ScalarAggregate:
-    def __init__(self, expr):
-        assert isinstance(expr, ir.Expr)
-        self.expr = expr
-        self.tables = []
-
-    def get_result(self):
-        expr = self.expr
-        subbed_expr = self._visit(expr)
-
-        table = self.tables[0]
-        for other in self.tables[1:]:
-            table = table.cross_join(other)
-
-        return table.select(subbed_expr)
-
-    def _visit(self, expr):
-        assert isinstance(expr, ir.Expr), type(expr)
-
-        if is_scalar_reduction(expr.op()) and not has_multiple_bases(expr.op()):
-            # An aggregation unit
-            if not expr.has_name():
-                expr = expr.name('tmp')
-            agg_expr = reduction_to_aggregation(expr.op())
-            self.tables.append(agg_expr)
-            return agg_expr[expr.get_name()]
-        elif not isinstance(expr, ir.Expr):
-            return expr
-
-        node = expr.op()
-        # TODO(kszucs): use the substitute() utility instead
-        new_args = (
-            self._visit(arg.to_expr()) if isinstance(arg, ops.Node) else arg
-            for arg in node.args
-        )
-        new_node = node.__class__(*new_args)
-        new_expr = new_node.to_expr()
+from copy_reg import _extension_registry
+from functools import partial
 
-        if expr.has_name():
-            new_expr = new_expr.name(name=expr.get_name())
-
-        return new_expr
+import dis
+import itertools
+import operator
+import os
+import pickle
+import struct
+import sys
+import traceback
+import types
+
+import logging
+cloudLog = logging.getLogger("Cloud.Transport")
+
+#relevant opcodes
+STORE_GLOBAL = chr(dis.opname.index('STORE_GLOBAL'))
+DELETE_GLOBAL = chr(dis.opname.index('DELETE_GLOBAL'))
+LOAD_GLOBAL = chr(dis.opname.index('LOAD_GLOBAL'))
+GLOBAL_OPS = [STORE_GLOBAL, DELETE_GLOBAL, LOAD_GLOBAL]
+
+HAVE_ARGUMENT = chr(dis.HAVE_ARGUMENT)
+EXTENDED_ARG = chr(dis.EXTENDED_ARG)
+
+
+try:
+    from cStringIO import StringIO
+except ImportError:
+    from StringIO import StringIO
+
+# These helper functions were copied from PiCloud's util module.
+def islambda(func):
+    return getattr(func,'func_name') == '<lambda>'
+
+def xrange_params(xrangeobj):
+    """Returns a 3 element tuple describing the xrange start, step, and len
+    respectively
+
+    Note: Only guarentees that elements of xrange are the same. parameters may
+    be different.
+    e.g. xrange(1,1) is interpretted as xrange(0,0); both behave the same
+    though w/ iteration
+    """
 
+    xrange_len = len(xrangeobj)
+    if not xrange_len: #empty
+        return (0,1,0)
+    start = xrangeobj[0]
+    if xrange_len == 1: #one element
+        return start, 1, 1
+    return (start, xrangeobj[1] - xrangeobj[0], xrange_len)
+
+#debug variables intended for developer use:
+printSerialization = False
+printMemoization = False
+
+useForcedImports = True #Should I use forced imports for tracking?
 
-def has_multiple_bases(node):
-    assert isinstance(node, ops.Node), type(node)
-    return len(find_immediate_parent_tables(node)) > 1
-
-
-def reduction_to_aggregation(node):
-    tables = find_immediate_parent_tables(node)
-
-    # TODO(kszucs): avoid the expression roundtrip
-    node = ops.Alias(node, node.name)
-    expr = node.to_expr()
-    if len(tables) == 1:
-        (table,) = tables
-        agg = table.to_expr().aggregate([expr])
-    else:
-        agg = ScalarAggregate(expr).get_result()
-
-    return agg
-
-
-def find_immediate_parent_tables(input_node, keep_input=True):
-    """Find every first occurrence of a `ir.Table` object in `input_node`.
-
-    This function does not traverse into `Table` objects. For example, the
-    underlying `PhysicalTable` of a `Selection` will not be yielded.
-
-    Parameters
-    ----------
-    input_node
-        Input node
-    keep_input
-        Whether to keep the input when traversing
-
-    Yields
-    ------
-    ir.Expr
-        Parent table expression
-
-    Examples
-    --------
-    >>> import ibis, toolz
-    >>> t = ibis.table([('a', 'int64')], name='t')
-    >>> expr = t.mutate(foo=t.a + 1)
-    >>> result, = find_immediate_parent_tables(expr.op())
-    >>> result.equals(expr.op())
-    True
-    >>> result, = find_immediate_parent_tables(expr.op(), keep_input=False)
-    >>> result.equals(t.op())
-    True
-    """
-    assert all(isinstance(arg, ops.Node) for arg in util.promote_list(input_node))
 
-    def finder(node):
-        if isinstance(node, ops.TableNode):
-            if keep_input or node != input_node:
-                return g.halt, node
-            else:
-                return g.proceed, None
 
-        # HACK: special case ops.Contains to only consider the needle's base
-        # table, since that's the only expression that matters for determining
-        # cardinality
-        elif isinstance(node, ops.Contains):
-            return [node.value], None
-        else:
-            return g.proceed, None
-
-    return list(toolz.unique(g.traverse(finder, input_node)))
-
-
-def substitute(fn, node):
-    """Substitute expressions with other expressions."""
-
-    assert isinstance(node, ops.Node), type(node)
-
-    result = fn(node)
-    if result is g.halt:
-        return node
-    elif result is not g.proceed:
-        assert isinstance(result, ops.Node), type(result)
-        return result
-
-    new_args = []
-    for arg in node.args:
-        if isinstance(arg, tuple):
-            arg = tuple(
-                substitute(fn, x) if isinstance(arg, ops.Node) else x for x in arg
-            )
-        elif isinstance(arg, ops.Node):
-            arg = substitute(fn, arg)
-        new_args.append(arg)
+class CloudPickler(pickle.Pickler):
+
+    dispatch = pickle.Pickler.dispatch.copy()
+    savedForceImports = False
+
+    def __init__(self, file, protocol=None, min_size_to_save= 0):
+        pickle.Pickler.__init__(self,file,protocol)
+        self.modules = set() #set of modules needed to depickle
+        self.globals_ref = {}  # map ids to dictionary. used to ensure that functions can share global env
+
+    def dump(self, obj):
+        # note: not thread safe
+        # minimal side-effects, so not fixing
+        recurse_limit = 3000
+        base_recurse = sys.getrecursionlimit()
+        if base_recurse < recurse_limit:
+            sys.setrecursionlimit(recurse_limit)
+        self.inject_addons()
+        try:
+            return pickle.Pickler.dump(self, obj)
+        except RuntimeError as e:
+            if 'recursion' in e.args[0]:
+                msg = """Could not pickle object as excessively deep recursion required.
+                Try _fast_serialization=2 or contact PiCloud support"""
+                raise pickle.PicklingError(msg)
+        finally:
+            new_recurse = sys.getrecursionlimit()
+            if new_recurse == recurse_limit:
+                sys.setrecursionlimit(base_recurse)
+
+    def save_buffer(self, obj):
+        """Fallback to save_string"""
+        pickle.Pickler.save_string(self,str(obj))
+    dispatch[buffer] = save_buffer
+
+    #block broken objects
+    def save_unsupported(self, obj, pack=None):
+        raise pickle.PicklingError("Cannot pickle objects of type %s" % type(obj))
+    dispatch[types.GeneratorType] = save_unsupported
 
+    #python2.6+ supports slice pickling. some py2.5 extensions might as well.  We just test it
     try:
-        return node.__class__(*new_args)
-    except TypeError:
-        return node
-
-
-def substitute_parents(node):
-    """Rewrite `node` by replacing table nodes that commute."""
-    assert isinstance(node, ops.Node), type(node)
-
-    def fn(node):
-        if isinstance(node, ops.Selection):
-            # stop substituting child nodes
-            return g.halt
-        elif isinstance(node, ops.TableColumn):
-            # For table column references, in the event that we're on top of a
-            # projection, we need to check whether the ref comes from the base
-            # table schema or is a derived field. If we've projected out of
-            # something other than a physical table, then lifting should not
-            # occur
-            table = node.table
-
-            if isinstance(table, ops.Selection):
-                for val in table.selections:
-                    if isinstance(val, ops.PhysicalTable) and node.name in val.schema:
-                        return ops.TableColumn(val, node.name)
-
-        # keep looking for nodes to substitute
-        return g.proceed
-
-    return substitute(fn, node)
-
-
-def substitute_unbound(node):
-    """Rewrite `node` by replacing table expressions with an equivalent unbound table."""
-    assert isinstance(node, ops.Node), type(node)
-
-    def fn(node, _, *args, **kwargs):
-        if isinstance(node, ops.DatabaseTable):
-            return ops.UnboundTable(name=node.name, schema=node.schema)
-        else:
-            return node.__class__(*args, **kwargs)
-
-    return node.substitute(fn)
-
-
-def get_mutation_exprs(exprs: list[ir.Expr], table: ir.Table) -> list[ir.Expr | None]:
-    """Return the exprs to use to instantiate the mutation."""
-    # The below logic computes the mutation node exprs by splitting the
-    # assignment exprs into two disjoint sets:
-    # 1) overwriting_cols_to_expr, which maps a column name to its expr
-    # if the expr contains a column that overwrites an existing table column.
-    # All keys in this dict are columns in the original table that are being
-    # overwritten by an assignment expr.
-    # 2) non_overwriting_exprs, which is a list of all exprs that do not do
-    # any overwriting. That is, if an expr is in this list, then its column
-    # name does not exist in the original table.
-    # Given these two data structures, we can compute the mutation node exprs
-    # based on whether any columns are being overwritten.
-    overwriting_cols_to_expr: dict[str, ir.Expr | None] = {}
-    non_overwriting_exprs: list[ir.Expr] = []
-    table_schema = table.schema()
-    for expr in exprs:
-        expr_contains_overwrite = False
-        if isinstance(expr, ir.Value) and expr.get_name() in table_schema:
-            overwriting_cols_to_expr[expr.get_name()] = expr
-            expr_contains_overwrite = True
-
-        if not expr_contains_overwrite:
-            non_overwriting_exprs.append(expr)
-
-    columns = table.columns
-    if overwriting_cols_to_expr:
-        return [
-            overwriting_cols_to_expr.get(column, table[column])
-            for column in columns
-            if overwriting_cols_to_expr.get(column, table[column]) is not None
-        ] + non_overwriting_exprs
-
-    table_expr: ir.Expr = table
-    return [table_expr] + exprs
-
-
-def apply_filter(op, predicates):
-    # This will attempt predicate pushdown in the cases where we can do it
-    # easily and safely, to make both cleaner SQL and fewer referential errors
-    # for users
-    if not predicates:
-        return op
-
-    if isinstance(op, ops.Selection):
-        return pushdown_selection_filters(op, predicates)
-    elif isinstance(op, ops.Aggregation):
-        return pushdown_aggregation_filters(op, predicates)
-    else:
-        return ops.Selection(op, [], predicates)
-
-
-def pushdown_selection_filters(op, predicates):
-    default = ops.Selection(op, selections=[], predicates=predicates)
-
-    # We can't push down filters on Unnest or Window because they
-    # change the shape and potential values of the data.
-    if any(
-        isinstance(
-            sel.arg if isinstance(sel, ops.Alias) else sel,
-            (ops.Unnest, ops.Window),
-        )
-        for sel in op.selections
-    ):
-        return default
-
-    # if any of the filter predicates have the parent expression among
-    # their roots, then pushdown (at least of that predicate) is not
-    # possible
-
-    # It's not unusual for the filter to reference the projection
-    # itself. If a predicate can be pushed down, in this case we must
-    # rewrite replacing the table refs with the roots internal to the
-    # projection we are referencing
-    #
-    # Assuming that the fields referenced by the filter predicate originate
-    # below the projection, we need to rewrite the predicate referencing
-    # the parent tables in the join being projected
-
-    # Potential fusion opportunity. The predicates may need to be
-    # rewritten in terms of the child table. This prevents the broken
-    # ref issue (described in more detail in #59)
-    try:
-        simplified_predicates = tuple(
-            sub_for(predicate, {op: op.table})
-            if not is_reduction(predicate)
-            else predicate
-            for predicate in predicates
-        )
-    except IntegrityError:
-        return default
+        slice(0,1).__reduce__()
+    except TypeError: #can't pickle -
+        dispatch[slice] = save_unsupported
+
+    #itertools objects do not pickle!
+    for v in itertools.__dict__.values():
+        if type(v) is type:
+            dispatch[v] = save_unsupported
+
+
+    def save_dict(self, obj):
+        """hack fix
+        If the dict is a global, deal with it in a special way
+        """
+        #print 'saving', obj
+        if obj is __builtins__:
+            self.save_reduce(_get_module_builtins, (), obj=obj)
+        else:
+            pickle.Pickler.save_dict(self, obj)
+    dispatch[pickle.DictionaryType] = save_dict
 
-    if not shares_all_roots(simplified_predicates, op.table):
-        return default
 
-    # find spuriously simplified predicates
-    for predicate in simplified_predicates:
-        # find columns in the predicate
-        depends_on = predicate.find((ops.TableColumn, ops.Literal))
-        for projection in op.selections:
-            if not isinstance(projection, (ops.TableColumn, ops.Literal)):
-                # if the projection's table columns overlap with columns
-                # used in the predicate then we return immediately
-                #
-                # this means that we were too aggressive during simplification
-                # example: t.mutate(a=_.a + 1).filter(_.a > 1)
-                if projection.find((ops.TableColumn, ops.Literal)) & depends_on:
-                    return default
-
-    return ops.Selection(
-        op.table,
-        selections=op.selections,
-        predicates=op.predicates + simplified_predicates,
-        sort_keys=op.sort_keys,
-    )
-
-
-def pushdown_aggregation_filters(op, predicates):
-    # Potential fusion opportunity
-    # GH1344: We can't sub in things with correlated subqueries
-    simplified_predicates = tuple(
-        # Originally this line tried substituting op.table in for expr, but
-        # that is too aggressive in the presence of filters that occur
-        # after aggregations.
-        #
-        # See https://github.com/ibis-project/ibis/pull/3341 for details
-        sub_for(predicate, {op.table: op}) if not is_reduction(predicate) else predicate
-        for predicate in predicates
-    )
-
-    if shares_all_roots(simplified_predicates, op.table):
-        return ops.Aggregation(
-            op.table,
-            op.metrics,
-            by=op.by,
-            having=op.having,
-            predicates=op.predicates + simplified_predicates,
-            sort_keys=op.sort_keys,
+    def save_module(self, obj, pack=struct.pack):
+        """
+        Save a module as an import
+        """
+        #print 'try save import', obj.__name__
+        self.modules.add(obj)
+        self.save_reduce(subimport,(obj.__name__,), obj=obj)
+    dispatch[types.ModuleType] = save_module    #new type
+
+    def save_codeobject(self, obj, pack=struct.pack):
+        """
+        Save a code object
+        """
+        #print 'try to save codeobj: ', obj
+        args = (
+            obj.co_argcount, obj.co_nlocals, obj.co_stacksize, obj.co_flags, obj.co_code,
+            obj.co_consts, obj.co_names, obj.co_varnames, obj.co_filename, obj.co_name,
+            obj.co_firstlineno, obj.co_lnotab, obj.co_freevars, obj.co_cellvars
         )
-    else:
-        return ops.Selection(op, [], predicates)
+        self.save_reduce(types.CodeType, args, obj=obj)
+    dispatch[types.CodeType] = save_codeobject    #new type
 
+    def save_function(self, obj, name=None, pack=struct.pack):
+        """ Registered with the dispatch to handle all function types.
 
-# TODO(kszucs): use ibis.expr.analysis.substitute instead
-def propagate_down_window(func: ops.Value, frame: ops.WindowFrame):
-    import ibis.expr.operations as ops
-
-    clean_args = []
-    for arg in func.args:
-        if isinstance(arg, ops.Value) and not isinstance(func, ops.WindowFunction):
-            arg = propagate_down_window(arg, frame)
-            if isinstance(arg, ops.Analytic):
-                arg = ops.WindowFunction(arg, frame)
-        clean_args.append(arg)
-
-    return type(func)(*clean_args)
-
-
-# TODO(kszucs): rewrite to receive and return an ops.Node
-def windowize_function(expr, frame):
-    assert isinstance(expr, ir.Expr), type(expr)
-    assert isinstance(frame, ops.WindowFrame)
-
-    def _windowize(op, frame):
-        if isinstance(op, ops.WindowFunction):
-            walked_child = _walk(op.func, frame)
-            walked = walked_child.to_expr().over(op.frame).op()
-        elif isinstance(op, ops.Value):
-            walked = _walk(op, frame)
-        else:
-            walked = op
-
-        if isinstance(walked, (ops.Analytic, ops.Reduction)):
-            return op.to_expr().over(frame).op()
-        elif isinstance(walked, ops.WindowFunction):
-            if frame is not None:
-                frame = walked.frame.copy(
-                    group_by=frame.group_by + walked.frame.group_by,
-                    order_by=frame.order_by + walked.frame.order_by,
-                )
-                return walked.to_expr().over(frame).op()
-            else:
-                return walked
+        Determines what kind of function obj is (e.g. lambda, defined at
+        interactive prompt, etc) and handles the pickling appropriately.
+        """
+        write = self.write
+
+        name = obj.__name__
+        modname = pickle.whichmodule(obj, name)
+        #print 'which gives %s %s %s' % (modname, obj, name)
+        try:
+            themodule = sys.modules[modname]
+        except KeyError: # eval'd items such as namedtuple give invalid items for their function __module__
+            modname = '__main__'
+
+        if modname == '__main__':
+            themodule = None
+
+        if themodule:
+            self.modules.add(themodule)
+            if getattr(themodule, name, None) is obj:
+                return self.save_global(obj, name)
+
+        # if func is lambda, def'ed at prompt, is in main, or is nested, then
+        # we'll pickle the actual function object rather than simply saving a
+        # reference (as is done in default pickler), via save_function_tuple.
+        if islambda(obj) or obj.func_code.co_filename == '<stdin>' or themodule is None:
+            #Force server to import modules that have been imported in main
+            modList = None
+            if themodule is None and not self.savedForceImports:
+                mainmod = sys.modules['__main__']
+                if useForcedImports and hasattr(mainmod,'___pyc_forcedImports__'):
+                    modList = list(mainmod.___pyc_forcedImports__)
+                self.savedForceImports = True
+            self.save_function_tuple(obj, modList)
+            return
+        else:   # func is nested
+            klass = getattr(themodule, name, None)
+            if klass is None or klass is not obj:
+                self.save_function_tuple(obj, [themodule])
+                return
+
+        if obj.__dict__:
+            # essentially save_reduce, but workaround needed to avoid recursion
+            self.save(_restore_attr)
+            write(pickle.MARK + pickle.GLOBAL + modname + '\n' + name + '\n')
+            self.memoize(obj)
+            self.save(obj.__dict__)
+            write(pickle.TUPLE + pickle.REDUCE)
         else:
-            return walked
-
-    def _walk(op, frame):
-        # TODO(kszucs): rewrite to use the substitute utility
-        windowed_args = []
-        for arg in op.args:
-            if isinstance(arg, ops.Value):
-                arg = _windowize(arg, frame)
-            elif isinstance(arg, tuple):
-                arg = tuple(_windowize(x, frame) for x in arg)
-
-            windowed_args.append(arg)
-
-        return type(op)(*windowed_args)
-
-    return _windowize(expr.op(), frame).to_expr()
-
-
-def simplify_aggregation(agg):
-    def _pushdown(nodes):
-        subbed = []
-        for node in nodes:
-            subbed.append(sub_for(node, {agg.table: agg.table.table}))
-
-        # TODO(kszucs): perhaps this validation could be omitted
-        if subbed:
-            valid = shares_all_roots(subbed, agg.table.table)
-        else:
-            valid = True
-
-        return valid, subbed
-
-    if isinstance(agg.table, ops.Selection) and not agg.table.selections:
-        metrics_valid, lowered_metrics = _pushdown(agg.metrics)
-        by_valid, lowered_by = _pushdown(agg.by)
-        having_valid, lowered_having = _pushdown(agg.having)
-
-        if metrics_valid and by_valid and having_valid:
-            valid_lowered_sort_keys = frozenset(lowered_metrics).union(lowered_by)
-            return ops.Aggregation(
-                agg.table.table,
-                lowered_metrics,
-                by=lowered_by,
-                having=lowered_having,
-                predicates=agg.table.predicates,
-                # only the sort keys that exist as grouping keys or metrics can
-                # be included
-                sort_keys=[
-                    key
-                    for key in agg.table.sort_keys
-                    if key.expr in valid_lowered_sort_keys
-                ],
-            )
-
-    return agg
-
-
-class Projector:
-    """Analysis and validation of projection operation.
-
-    This pass tries to take advantage of projection fusion opportunities where
-    they exist, i.e. combining compatible projections together rather than
-    nesting them.
+            write(pickle.GLOBAL + modname + '\n' + name + '\n')
+            self.memoize(obj)
+    dispatch[types.FunctionType] = save_function
+
+    def save_function_tuple(self, func, forced_imports):
+        """  Pickles an actual func object.
+
+        A func comprises: code, globals, defaults, closure, and dict.  We
+        extract and save these, injecting reducing functions at certain points
+        to recreate the func object.  Keep in mind that some of these pieces
+        can contain a ref to the func itself.  Thus, a naive save on these
+        pieces could trigger an infinite loop of save's.  To get around that,
+        we first create a skeleton func object using just the code (this is
+        safe, since this won't contain a ref to the func), and memoize it as
+        soon as it's created.  The other stuff can then be filled in later.
+        """
+        save = self.save
+        write = self.write
+
+        # save the modules (if any)
+        if forced_imports:
+            write(pickle.MARK)
+            save(_modules_to_main)
+            #print 'forced imports are', forced_imports
+
+            forced_names = map(lambda m: m.__name__, forced_imports)
+            save((forced_names,))
+
+            #save((forced_imports,))
+            write(pickle.REDUCE)
+            write(pickle.POP_MARK)
+
+        code, f_globals, defaults, closure, dct, base_globals = self.extract_func_data(func)
+
+        save(_fill_function)  # skeleton function updater
+        write(pickle.MARK)    # beginning of tuple that _fill_function expects
+
+        # create a skeleton function object and memoize it
+        save(_make_skel_func)
+        save((code, closure, base_globals))
+        write(pickle.REDUCE)
+        self.memoize(func)
+
+        # save the rest of the func data needed by _fill_function
+        save(f_globals)
+        save(defaults)
+        save(dct)
+        write(pickle.TUPLE)
+        write(pickle.REDUCE)  # applies _fill_function on the tuple
+
+    @staticmethod
+    def extract_code_globals(co):
+        """
+        Find all globals names read or written to by codeblock co
+        """
+        code = co.co_code
+        names = co.co_names
+        out_names = set()
+
+        n = len(code)
+        i = 0
+        extended_arg = 0
+        while i < n:
+            op = code[i]
+
+            i = i+1
+            if op >= HAVE_ARGUMENT:
+                oparg = ord(code[i]) + ord(code[i+1])*256 + extended_arg
+                extended_arg = 0
+                i = i+2
+                if op == EXTENDED_ARG:
+                    extended_arg = oparg*65536
+                if op in GLOBAL_OPS:
+                    out_names.add(names[oparg])
+        #print 'extracted', out_names, ' from ', names
+
+        if co.co_consts:   # see if nested function have any global refs
+            for const in co.co_consts:
+                if type(const) is types.CodeType:
+                    out_names |= CloudPickler.extract_code_globals(const)
+
+        return out_names
+
+    def extract_func_data(self, func):
+        """
+        Turn the function into a tuple of data necessary to recreate it:
+            code, globals, defaults, closure, dict
+        """
+        code = func.func_code
+
+        # extract all global ref's
+        func_global_refs = CloudPickler.extract_code_globals(code)
+
+        # process all variables referenced by global environment
+        f_globals = {}
+        for var in func_global_refs:
+            #Some names, such as class functions are not global - we don't need them
+            if func.func_globals.has_key(var):
+                f_globals[var] = func.func_globals[var]
 
-    Translation / evaluation later will not attempt to do any further fusion /
-    simplification.
-    """
-
-    def __init__(self, parent, proj_exprs):
-        # TODO(kszucs): rewrite projector to work with operations exclusively
-        proj_exprs = util.promote_list(proj_exprs)
-        self.parent = parent
-        self.input_exprs = proj_exprs
-        self.resolved_exprs = [parent._ensure_expr(e) for e in proj_exprs]
-
-        default_frame = ops.RowsWindowFrame(table=parent)
-        self.clean_exprs = [
-            windowize_function(expr, frame=default_frame)
-            for expr in self.resolved_exprs
-        ]
-
-    def get_result(self):
-        roots = find_immediate_parent_tables(self.parent.op())
-        first_root = roots[0]
-
-        if len(roots) == 1 and isinstance(first_root, ops.Selection):
-            fused_op = self.try_fusion(first_root)
-            if fused_op is not None:
-                return fused_op
-
-        return ops.Selection(self.parent, self.clean_exprs)
-
-    def try_fusion(self, root):
-        assert self.parent.op() == root
-
-        root_table = root.table
-        root_table_expr = root_table.to_expr()
-        roots = find_immediate_parent_tables(root_table)
-        fused_exprs = []
-        clean_exprs = self.clean_exprs
+        # defaults requires no processing
+        defaults = func.func_defaults
 
-        if not isinstance(root_table, ops.Join):
+        def get_contents(cell):
             try:
-                resolved = [
-                    root_table_expr._ensure_expr(expr) for expr in self.input_exprs
-                ]
-            except (AttributeError, IbisTypeError):
-                resolved = clean_exprs
-            else:
-                # if any expressions aren't exactly equivalent then don't try
-                # to fuse them
-                if any(
-                    not res_root_root.equals(res_root)
-                    for res_root_root, res_root in zip(resolved, clean_exprs)
-                ):
-                    return None
-        else:
-            # joins cannot be used to resolve expressions, but we still may be
-            # able to fuse columns from a projection off of a join. In that
-            # case, use the projection's input expressions as the columns with
-            # which to attempt fusion
-            resolved = clean_exprs
-
-        root_selections = root.selections
-        parent_op = self.parent.op()
-        for val in resolved:
-            # a * projection
-            if isinstance(val, ir.Table) and (
-                parent_op.equals(val.op())
-                # gross we share the same table root. Better way to
-                # detect?
-                or len(roots) == 1
-                and find_immediate_parent_tables(val.op())[0] == roots[0]
-            ):
-                have_root = False
-                for root_sel in root_selections:
-                    # Don't add the * projection twice
-                    if root_sel.equals(root_table):
-                        fused_exprs.append(root_table)
-                        have_root = True
-                        continue
-                    fused_exprs.append(root_sel)
-
-                # This was a filter, so implicitly a select *
-                if not have_root and not root_selections:
-                    fused_exprs = [root_table, *fused_exprs]
-            elif shares_all_roots(val.op(), root_table):
-                fused_exprs.append(val)
-            else:
-                return None
-
-        return ops.Selection(
-            root_table,
-            fused_exprs,
-            predicates=root.predicates,
-            sort_keys=root.sort_keys,
-        )
-
-
-def find_first_base_table(node):
-    def predicate(node):
-        if isinstance(node, ops.TableNode):
-            return g.halt, node
-        else:
-            return g.proceed, None
+                return cell.cell_contents
+            except ValueError as e: #cell is empty error on not yet assigned
+                raise pickle.PicklingError('Function to be pickled has free variables that are referenced before assignment in enclosing scope')
 
-    try:
-        return next(g.traverse(predicate, node))
-    except StopIteration:
-        return None
-
-
-def _find_projections(node):
-    if isinstance(node, ops.Selection):
-        # remove predicates and sort_keys, so that child tables are considered
-        # equivalent even if their predicates and sort_keys are not
-        return g.proceed, node._projection
-    elif isinstance(node, ops.SelfReference):
-        return g.proceed, node
-    elif isinstance(node, ops.Join):
-        return g.proceed, None
-    elif isinstance(node, ops.TableNode):
-        return g.halt, node
-    elif isinstance(node, ops.Contains):
-        return [node.value], None
-    else:
-        return g.proceed, None
-
-
-def shares_all_roots(exprs, parents):
-    # unique table dependencies of exprs and parents
-    exprs_deps = set(g.traverse(_find_projections, exprs))
-    parents_deps = set(g.traverse(_find_projections, parents))
-    return exprs_deps <= parents_deps
-
-
-def shares_some_roots(exprs, parents):
-    # unique table dependencies of exprs and parents
-    exprs_deps = set(g.traverse(_find_projections, exprs))
-    parents_deps = set(g.traverse(_find_projections, parents))
-    # Also return True if exprs has no roots (e.g. literal-only expressions)
-    return bool(exprs_deps & parents_deps) or not exprs_deps
-
-
-def flatten_predicate(node):
-    """Yield the expressions corresponding to the `And` nodes of a predicate.
-
-    Examples
-    --------
-    >>> import ibis
-    >>> t = ibis.table([('a', 'int64'), ('b', 'string')], name='t')
-    >>> filt = (t.a == 1) & (t.b == 'foo')
-    >>> predicates = flatten_predicate(filt.op())
-    >>> len(predicates)
-    2
-    >>> predicates[0].to_expr().name("left")
-    r0 := UnboundTable: t
-      a int64
-      b string
-    left: r0.a == 1
-    >>> predicates[1].to_expr().name("right")
-    r0 := UnboundTable: t
-      a int64
-      b string
-    right: r0.b == 'foo'
-    """
 
-    def predicate(node):
-        if isinstance(node, ops.And):
-            return g.proceed, None
+        # process closure
+        if func.func_closure:
+            closure = map(get_contents, func.func_closure)
         else:
-            return g.halt, node
+            closure = []
 
-    return list(g.traverse(predicate, node))
+        # save the dict
+        dct = func.func_dict
 
+        if printSerialization:
+            outvars = ['code: ' + str(code) ]
+            outvars.append('globals: ' + str(f_globals))
+            outvars.append('defaults: ' + str(defaults))
+            outvars.append('closure: ' + str(closure))
+            print('function {0} is extracted to: {1}'.format(
+                func, ', '.join(outvars)))
+
+        base_globals = self.globals_ref.get(id(func.func_globals), {})
+        self.globals_ref[id(func.func_globals)] = base_globals
+
+        return (code, f_globals, defaults, closure, dct, base_globals)
+
+    def save_builtin_function(self, obj):
+        if obj.__module__ is "__builtin__":
+            return self.save_global(obj)
+        return self.save_function(obj)
+    dispatch[types.BuiltinFunctionType] = save_builtin_function
+
+    def save_global(self, obj, name=None, pack=struct.pack):
+        write = self.write
+        memo = self.memo
+
+        if name is None:
+            name = obj.__name__
+
+        modname = getattr(obj, "__module__", None)
+        if modname is None:
+            modname = pickle.whichmodule(obj, name)
 
-def is_analytic(node):
-    def predicate(node):
-        if isinstance(node, (ops.Reduction, ops.Analytic)):
-            return g.halt, True
+        try:
+            __import__(modname)
+            themodule = sys.modules[modname]
+        except (ImportError, KeyError, AttributeError):  #should never occur
+            raise pickle.PicklingError(
+                "Can't pickle %r: Module %s cannot be found" %
+                (obj, modname))
+
+        if modname == '__main__':
+            themodule = None
+
+        if themodule:
+            self.modules.add(themodule)
+
+        sendRef = True
+        typ = type(obj)
+        #print 'saving', obj, typ
+        try:
+            try: #Deal with case when getattribute fails with exceptions
+                klass = getattr(themodule, name)
+            except (AttributeError):
+                if modname == '__builtin__':  #new.* are misrepeported
+                    modname = 'new'
+                    __import__(modname)
+                    themodule = sys.modules[modname]
+                    try:
+                        klass = getattr(themodule, name)
+                    except AttributeError as a:
+                        # print themodule, name, obj, type(obj)
+                        raise pickle.PicklingError("Can't pickle builtin %s" % obj)
+                else:
+                    raise
+
+        except (ImportError, KeyError, AttributeError):
+            if typ == types.TypeType or typ == types.ClassType:
+                sendRef = False
+            else: #we can't deal with this
+                raise
         else:
-            return g.proceed, None
-
-    return any(g.traverse(predicate, node))
-
-
-def is_reduction(node):
-    """Check whether an expression contains a reduction or not.
-
-    Aggregations yield typed scalar expressions, since the result of an
-    aggregation is a single value. When creating an table expression
-    containing a GROUP BY equivalent, we need to be able to easily check
-    that we are looking at the result of an aggregation.
-
-    As an example, the expression we are looking at might be something
-    like: foo.sum().log10() + bar.sum().log10()
-
-    We examine the operator DAG in the expression to determine if there
-    are aggregations present.
-
-    A bound aggregation referencing a separate table is a "false
-    aggregation" in a GROUP BY-type expression and should be treated a
-    literal, and must be computed as a separate query and stored in a
-    temporary variable (or joined, for bound aggregations with keys)
-    """
-
-    def predicate(node):
-        if isinstance(node, ops.Reduction):
-            return g.halt, True
-        elif isinstance(node, ops.TableNode):
-            # don't go below any table nodes
-            return g.halt, None
+            if klass is not obj and (typ == types.TypeType or typ == types.ClassType):
+                sendRef = False
+        if not sendRef:
+            #note: Third party types might crash this - add better checks!
+            d = dict(obj.__dict__) #copy dict proxy to a dict
+            if not isinstance(d.get('__dict__', None), property): # don't extract dict that are properties
+                d.pop('__dict__',None)
+            d.pop('__weakref__',None)
+
+            # hack as __new__ is stored differently in the __dict__
+            new_override = d.get('__new__', None)
+            if new_override:
+                d['__new__'] = obj.__new__
+
+            self.save_reduce(type(obj),(obj.__name__,obj.__bases__,
+                                   d),obj=obj)
+            #print 'internal reduce dask %s %s'  % (obj, d)
+            return
+
+        if self.proto >= 2:
+            code = _extension_registry.get((modname, name))
+            if code:
+                assert code > 0
+                if code <= 0xff:
+                    write(pickle.EXT1 + chr(code))
+                elif code <= 0xffff:
+                    write("%c%c%c" % (pickle.EXT2, code&0xff, code>>8))
+                else:
+                    write(pickle.EXT4 + pack("<i", code))
+                return
+
+        write(pickle.GLOBAL + modname + '\n' + name + '\n')
+        self.memoize(obj)
+    dispatch[types.ClassType] = save_global
+    dispatch[types.TypeType] = save_global
+
+    def save_instancemethod(self, obj):
+        #Memoization rarely is ever useful due to python bounding
+        self.save_reduce(types.MethodType, (obj.im_func, obj.im_self,obj.im_class), obj=obj)
+    dispatch[types.MethodType] = save_instancemethod
+
+    def save_inst_logic(self, obj):
+        """Inner logic to save instance. Based off pickle.save_inst
+        Supports __transient__"""
+        cls = obj.__class__
+
+        memo  = self.memo
+        write = self.write
+        save  = self.save
+
+        if hasattr(obj, '__getinitargs__'):
+            args = obj.__getinitargs__()
+            len(args) # XXX Assert it's a sequence
+            pickle._keep_alive(args, memo)
         else:
-            return g.proceed, None
-
-    return any(g.traverse(predicate, node))
-
-
-def is_scalar_reduction(node):
-    assert isinstance(node, ops.Node), type(node)
-    return node.output_shape.is_scalar() and is_reduction(node)
-
-
-_ANY_OP_MAPPING = {
-    ops.Any: ops.UnresolvedExistsSubquery,
-    ops.NotAny: ops.UnresolvedNotExistsSubquery,
-}
+            args = ()
 
+        write(pickle.MARK)
 
-def find_predicates(node, flatten=True):
-    # TODO(kszucs): consider to remove flatten argument and compose with
-    # flatten_predicates instead
-    def predicate(node):
-        assert isinstance(node, ops.Node), type(node)
-        if isinstance(node, ops.Value) and node.output_dtype.is_boolean():
-            if flatten and isinstance(node, ops.And):
-                return g.proceed, None
-            else:
-                return g.halt, node
-        return g.proceed, None
-
-    return list(g.traverse(predicate, node))
-
-
-def find_subqueries(node: ops.Node, min_dependents=1) -> tuple[ops.Node, ...]:
-    subquery_dependents = defaultdict(set)
-    for n in filter(None, util.promote_list(node)):
-        dependents = g.Graph.from_dfs(n).invert()
-        for u, vs in dependents.toposort().items():
-            # count the number of table-node dependents on the current node
-            # but only if the current node is a selection or aggregation
-            if isinstance(u, (rels.Projection, rels.Aggregation, rels.Limit)):
-                subquery_dependents[u].update(vs)
-
-    return tuple(
-        node
-        for node, dependents in reversed(subquery_dependents.items())
-        if len(dependents) >= min_dependents
-    )
-
-
-# TODO(kszucs): move to types/logical.py
-def _make_any(
-    expr,
-    any_op_class: type[ops.Any] | type[ops.NotAny],
-    *,
-    where: ir.BooleanValue | None = None,
-):
-    assert isinstance(expr, ir.Expr), type(expr)
-
-    tables = find_immediate_parent_tables(expr.op())
-    predicates = find_predicates(expr.op(), flatten=True)
-
-    if len(tables) > 1:
-        op = _ANY_OP_MAPPING[any_op_class](
-            tables=[t.to_expr() for t in tables],
-            predicates=predicates,
-        )
-    else:
-        op = any_op_class(expr, where=where)
-    return op.to_expr()
-
-
-# TODO(kszucs): use substitute instead
-@functools.singledispatch
-def _rewrite_filter(op, **kwargs):
-    raise NotImplementedError(type(op))
-
+        if self.bin:
+            save(cls)
+            for arg in args:
+                save(arg)
+            write(pickle.OBJ)
+        else:
+            for arg in args:
+                save(arg)
+            write(pickle.INST + cls.__module__ + '\n' + cls.__name__ + '\n')
 
-@_rewrite_filter.register(ops.Reduction)
-def _rewrite_filter_reduction(op, name: str | None = None, **kwargs):
-    """Turn a reduction inside of a filter into an aggregate."""
-    # TODO: what about reductions that reference a join that isn't visible at
-    # this level? Means we probably have the wrong design, but will have to
-    # revisit when it becomes a problem.
+        self.memoize(obj)
 
-    if name is not None:
-        op = ops.Alias(op, name=name)
-    aggregation = reduction_to_aggregation(op)
-    return ops.TableArrayView(aggregation)
+        try:
+            getstate = obj.__getstate__
+        except AttributeError:
+            stuff = obj.__dict__
+            #remove items if transient
+            if hasattr(obj, '__transient__'):
+                transient = obj.__transient__
+                stuff = stuff.copy()
+                for k in list(stuff.keys()):
+                    if k in transient:
+                        del stuff[k]
+        else:
+            stuff = getstate()
+            pickle._keep_alive(stuff, memo)
+        save(stuff)
+        write(pickle.BUILD)
 
 
-@_rewrite_filter.register(ops.Any)
-@_rewrite_filter.register(ops.TableColumn)
-@_rewrite_filter.register(ops.Literal)
-@_rewrite_filter.register(ops.ExistsSubquery)
-@_rewrite_filter.register(ops.NotExistsSubquery)
-@_rewrite_filter.register(ops.WindowFunction)
-def _rewrite_filter_subqueries(op, **kwargs):
-    """Don't rewrite any of these operations in filters."""
-    return op
+    def save_inst(self, obj):
+        # Hack to detect PIL Image instances without importing Imaging
+        # PIL can be loaded with multiple names, so we don't check sys.modules for it
+        if hasattr(obj,'im') and hasattr(obj,'palette') and 'Image' in obj.__module__:
+            self.save_image(obj)
+        else:
+            self.save_inst_logic(obj)
+    dispatch[types.InstanceType] = save_inst
 
+    def save_property(self, obj):
+        # properties not correctly saved in python
+        self.save_reduce(property, (obj.fget, obj.fset, obj.fdel, obj.__doc__), obj=obj)
+    dispatch[property] = save_property
+
+    def save_itemgetter(self, obj):
+        """itemgetter serializer (needed for namedtuple support)"""
+        class Dummy:
+            def __getitem__(self, item):
+                return item
+        items = obj(Dummy())
+        if not isinstance(items, tuple):
+            items = (items, )
+        return self.save_reduce(operator.itemgetter, items)
+
+    if type(operator.itemgetter) is type:
+        dispatch[operator.itemgetter] = save_itemgetter
+
+    def save_attrgetter(self, obj):
+        """attrgetter serializer"""
+        class Dummy(object):
+            def __init__(self, attrs, index=None):
+                self.attrs = attrs
+                self.index = index
+            def __getattribute__(self, item):
+                attrs = object.__getattribute__(self, "attrs")
+                index = object.__getattribute__(self, "index")
+                if index is None:
+                    index = len(attrs)
+                    attrs.append(item)
+                else:
+                    attrs[index] = ".".join([attrs[index], item])
+                return type(self)(attrs, index)
+        attrs = []
+        obj(Dummy(attrs))
+        return self.save_reduce(operator.attrgetter, tuple(attrs))
+
+    if type(operator.attrgetter) is type:
+        dispatch[operator.attrgetter] = save_attrgetter
+
+    def save_reduce(self, func, args, state=None,
+                    listitems=None, dictitems=None, obj=None):
+        """Modified to support __transient__ on new objects
+        Change only affects protocol level 2 (which is always used by PiCloud"""
+        # Assert that args is a tuple or None
+        if not isinstance(args, types.TupleType):
+            raise pickle.PicklingError("args from reduce() should be a tuple")
+
+        # Assert that func is callable
+        if not hasattr(func, '__call__'):
+            raise pickle.PicklingError("func from reduce should be callable")
+
+        save = self.save
+        write = self.write
+
+        # Protocol 2 special case: if func's name is __newobj__, use NEWOBJ
+        if self.proto >= 2 and getattr(func, "__name__", "") == "__newobj__":
+            #Added fix to allow transient
+            cls = args[0]
+            if not hasattr(cls, "__new__"):
+                raise pickle.PicklingError(
+                    "args[0] from __newobj__ args has no __new__")
+            if obj is not None and cls is not obj.__class__:
+                raise pickle.PicklingError(
+                    "args[0] from __newobj__ args has the wrong class")
+            args = args[1:]
+            save(cls)
+
+            #Don't pickle transient entries
+            if hasattr(obj, '__transient__'):
+                transient = obj.__transient__
+                state = state.copy()
+
+                for k in list(state.keys()):
+                    if k in transient:
+                        del state[k]
 
-@_rewrite_filter.register(ops.Alias)
-def _rewrite_filter_alias(op, name: str | None = None, **kwargs):
-    """Rewrite filters on aliases."""
-    return _rewrite_filter(
-        op.arg,
-        name=name if name is not None else op.name,
-        **kwargs,
-    )
+            save(args)
+            write(pickle.NEWOBJ)
+        else:
+            save(func)
+            save(args)
+            write(pickle.REDUCE)
+
+        if obj is not None:
+            self.memoize(obj)
+
+        # More new special cases (that work with older protocols as
+        # well): when __reduce__ returns a tuple with 4 or 5 items,
+        # the 4th and 5th item should be iterators that provide list
+        # items and dict items (as (key, value) tuples), or None.
+
+        if listitems is not None:
+            self._batch_appends(listitems)
+
+        if dictitems is not None:
+            self._batch_setitems(dictitems)
+
+        if state is not None:
+            #print 'obj %s has state %s' % (obj, state)
+            save(state)
+            write(pickle.BUILD)
+
+
+    def save_xrange(self, obj):
+        """Save an xrange object in python 2.5
+        Python 2.6 supports this natively
+        """
+        range_params = xrange_params(obj)
+        self.save_reduce(_build_xrange,range_params)
 
+    #python2.6+ supports xrange pickling. some py2.5 extensions might as well.  We just test it
+    try:
+        xrange(0).__reduce__()
+    except TypeError: #can't pickle -- use PiCloud pickler
+        dispatch[xrange] = save_xrange
+
+    def save_partial(self, obj):
+        """Partial objects do not serialize correctly in python2.x -- this fixes the bugs"""
+        self.save_reduce(_genpartial, (obj.func, obj.args, obj.keywords))
+
+    if sys.version_info < (2,7): #2.7 supports partial pickling
+        dispatch[partial] = save_partial
+
+
+    def save_file(self, obj):
+        """Save a file"""
+        import StringIO as pystringIO #we can't use cStringIO as it lacks the name attribute
+
+        if not hasattr(obj, 'name') or  not hasattr(obj, 'mode'):
+            raise pickle.PicklingError("Cannot pickle files that do not map to an actual file")
+        if obj is sys.stdout:
+            return self.save_reduce(getattr, (sys,'stdout'), obj=obj)
+        if obj is sys.stderr:
+            return self.save_reduce(getattr, (sys,'stderr'), obj=obj)
+        if obj is sys.stdin:
+            raise pickle.PicklingError("Cannot pickle standard input")
+        if  hasattr(obj, 'isatty') and obj.isatty():
+            raise pickle.PicklingError("Cannot pickle files that map to tty objects")
+        if 'r' not in obj.mode:
+            raise pickle.PicklingError("Cannot pickle files that are not opened for reading")
+        name = obj.name
+        try:
+            fsize = os.stat(name).st_size
+        except OSError:
+            raise pickle.PicklingError("Cannot pickle file %s as it cannot be stat" % name)
+
+        if obj.closed:
+            #create an empty closed string io
+            retval = pystringIO.StringIO("")
+            retval.close()
+        elif not fsize: #empty file
+            retval = pystringIO.StringIO("")
+            try:
+                tmpfile = file(name)
+                tst = tmpfile.read(1)
+            except IOError:
+                raise pickle.PicklingError("Cannot pickle file %s as it cannot be read" % name)
+            tmpfile.close()
+            if tst != '':
+                raise pickle.PicklingError("Cannot pickle file %s as it does not appear to map to a physical, real file" % name)
+        else:
+            try:
+                tmpfile = file(name)
+                contents = tmpfile.read()
+                tmpfile.close()
+            except IOError:
+                raise pickle.PicklingError("Cannot pickle file %s as it cannot be read" % name)
+            retval = pystringIO.StringIO(contents)
+            curloc = obj.tell()
+            retval.seek(curloc)
+
+        retval.name = name
+        self.save(retval)  #save stringIO
+        self.memoize(obj)
+
+    dispatch[file] = save_file
+    """Special functions for Add-on libraries"""
+
+    def inject_numpy(self):
+        numpy = sys.modules.get('numpy')
+        if not numpy or not hasattr(numpy, 'ufunc'):
+            return
+        self.dispatch[numpy.ufunc] = self.__class__.save_ufunc
+
+    numpy_tst_mods = ['numpy', 'scipy.special']
+    def save_ufunc(self, obj):
+        """Hack function for saving numpy ufunc objects"""
+        name = obj.__name__
+        for tst_mod_name in self.numpy_tst_mods:
+            tst_mod = sys.modules.get(tst_mod_name, None)
+            if tst_mod:
+                if name in tst_mod.__dict__:
+                    self.save_reduce(_getobject, (tst_mod_name, name))
+                    return
+        raise pickle.PicklingError('cannot save %s. Cannot resolve what module it is defined in' % str(obj))
+
+    def inject_email(self):
+        """Block email LazyImporters from being saved"""
+        email = sys.modules.get('email')
+        if not email:
+            return
+        self.dispatch[email.LazyImporter] = self.__class__.save_unsupported
+
+    def inject_addons(self):
+        """Plug in system. Register additional pickling functions if modules already loaded"""
+        self.inject_numpy()
+        self.inject_email()
+
+    """Python Imaging Library"""
+    def save_image(self, obj):
+        if not obj.im and obj.fp and 'r' in obj.fp.mode and obj.fp.name \
+            and not obj.fp.closed and (not hasattr(obj, 'isatty') or not obj.isatty()):
+            #if image not loaded yet -- lazy load
+            self.save_reduce(_lazyloadImage,(obj.fp,), obj=obj)
+        else:
+            #image is loaded - just transmit it over
+            self.save_reduce(_generateImage, (obj.size, obj.mode, obj.tostring()), obj=obj)
 
-@_rewrite_filter.register(ops.Value)
-def _rewrite_filter_value(op, **kwargs):
-    """Recursively apply filter rewriting on operations."""
+    """
+    def memoize(self, obj):
+        pickle.Pickler.memoize(self, obj)
+        if printMemoization:
+            print 'memoizing ' + str(obj)
+    """
 
-    visited = [
-        _rewrite_filter(arg, **kwargs) if isinstance(arg, ops.Node) else arg
-        for arg in op.args
-    ]
-    if all(map(operator.is_, visited, op.args)):
-        return op
 
-    return op.__class__(*visited)
 
+# Shorthands for legacy support
 
-@_rewrite_filter.register(tuple)
-def _rewrite_filter_value_list(op, **kwargs):
-    visited = [
-        _rewrite_filter(arg, **kwargs) if isinstance(arg, ops.Node) else arg
-        for arg in op.args
-    ]
+def dump(obj, file, protocol=2):
+    CloudPickler(file, protocol).dump(obj)
 
-    if all(map(operator.is_, visited, op.args)):
-        return op
+def dumps(obj, protocol=2):
+    file = StringIO()
 
-    return op.__class__(*visited)
+    cp = CloudPickler(file,protocol)
+    cp.dump(obj)
 
+    #print 'cloud dumped', str(obj), str(cp.modules)
 
-def find_memtables(node: ops.Node) -> Iterator[ops.InMemoryTable]:
-    """Find all in-memory tables in `node`."""
+    return file.getvalue()
 
-    def finder(node):
-        return g.proceed, node if isinstance(node, ops.InMemoryTable) else None
 
-    return g.traverse(finder, node, filter=ops.Node)
+#hack for __import__ not working as desired
+def subimport(name):
+    __import__(name)
+    return sys.modules[name]
 
+# restores function attributes
+def _restore_attr(obj, attr):
+    for key, val in attr.items():
+        setattr(obj, key, val)
+    return obj
 
-def find_toplevel_unnest_children(nodes: Iterable[ops.Node]) -> Iterator[ops.Table]:
-    def finder(node):
-        return (
-            isinstance(node, ops.Value),
-            find_first_base_table(node) if isinstance(node, ops.Unnest) else None,
-        )
+def _get_module_builtins():
+    return pickle.__builtins__
 
-    return g.traverse(finder, nodes, filter=ops.Node)
+def print_exec(stream):
+    ei = sys.exc_info()
+    traceback.print_exception(ei[0], ei[1], ei[2], None, stream)
 
+def _modules_to_main(modList):
+    """Force every module in modList to be placed into main"""
+    if not modList:
+        return
 
-def find_toplevel_aggs(nodes: Iterable[ops.Node]) -> Iterator[ops.Table]:
-    def finder(node):
-        return (
-            isinstance(node, ops.Value),
-            node if isinstance(node, ops.Reduction) else None,
-        )
+    main = sys.modules['__main__']
+    for modname in modList:
+        if type(modname) is str:
+            try:
+                mod = __import__(modname)
+            except Exception as i: #catch all...
+                sys.stderr.write('warning: could not import %s\n.  Your function may unexpectedly error due to this import failing; \
+A version mismatch is likely.  Specific error was:\n' % modname)
+                print_exec(sys.stderr)
+            else:
+                setattr(main,mod.__name__, mod)
+        else:
+            #REVERSE COMPATIBILITY FOR CLOUD CLIENT 1.5 (WITH EPD)
+            #In old version actual module was sent
+            setattr(main,modname.__name__, modname)
+
+#object generators:
+def _build_xrange(start, step, len):
+    """Built xrange explicitly"""
+    return xrange(start, start + step*len, step)
+
+def _genpartial(func, args, kwds):
+    if not args:
+        args = ()
+    if not kwds:
+        kwds = {}
+    return partial(func, *args, **kwds)
+
+def _fill_function(func, globals, defaults, dict):
+    """ Fills in the rest of function data into the skeleton function object
+        that were created via _make_skel_func().
+         """
+    func.func_globals.update(globals)
+    func.func_defaults = defaults
+    func.func_dict = dict
+
+    return func
+
+def _make_cell(value):
+    return (lambda: value).func_closure[0]
+
+def _reconstruct_closure(values):
+    return tuple([_make_cell(v) for v in values])
+
+def _make_skel_func(code, closures, base_globals = None):
+    """ Creates a skeleton function object that contains just the provided
+        code and the correct number of cells in func_closure.  All other
+        func attributes (e.g. func_globals) are empty.
+    """
+    closure = _reconstruct_closure(closures) if closures else None
 
-    return g.traverse(finder, nodes, filter=ops.Node)
+    if base_globals is None:
+        base_globals = {}
+    base_globals['__builtins__'] = __builtins__
+
+    return types.FunctionType(code, base_globals,
+                              None, None, closure)
+
+
+"""Constructors for 3rd party libraries
+Note: These can never be renamed due to client compatibility issues"""
+
+def _getobject(modname, attribute):
+    mod = __import__(modname, fromlist=[attribute])
+    return mod.__dict__[attribute]
+
+def _generateImage(size, mode, str_rep):
+    """Generate image from string representation"""
+    import Image
+    i = Image.new(mode, size)
+    i.fromstring(str_rep)
+    return i
+
+def _lazyloadImage(fp):
+    import Image
+    fp.seek(0)  #works in almost any case
+    return Image.open(fp)
```

### Comparing `ibis_framework-5.1.0/ibis/expr/rules.py` & `ibis-framework-v0.6.0/ibis/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,656 +1,725 @@
-from __future__ import annotations
+# This file has been adapted from pandas/core/config.py. pandas 3-clause BSD
+# license. See LICENSES/pandas
+#
+# Further modifications:
+#
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import enum
-import operator
-from itertools import product, starmap
-
-from public import public
-
-import ibis.common.exceptions as com
-import ibis.expr.datatypes as dt
-import ibis.expr.schema as sch
-import ibis.expr.types as ir
-from ibis import util
-from ibis.common.annotations import attribute, optional
-from ibis.common.validators import (
-    bool_,
-    callable_with,  # noqa: F401
-    coerced_to,  # noqa: F401
-    equal_to,  # noqa: F401
-    instance_of,
-    isin,
-    lazy_instance_of,
-    map_to,
-    one_of,
-    option,  # noqa: F401
-    pair_of,  # noqa: F401
-    ref,
-    str_,
-    tuple_of,
-    validator,
-)
-from ibis.expr.deferred import Deferred
-
-
-# TODO(kszucs): consider to rename to datashape
-@public
-class Shape(enum.IntEnum):
-    SCALAR = 0
-    COLUMNAR = 1
-    # TABULAR = 2
-
-    def is_scalar(self):
-        return self is Shape.SCALAR
-
-    def is_columnar(self):
-        return self is Shape.COLUMNAR
-
-
-@public
-def highest_precedence_shape(nodes):
-    return max(node.output_shape for node in nodes)
-
-
-@public
-def highest_precedence_dtype(nodes):
-    """Return the highest precedence type from the passed expressions.
-
-    Also verifies that there are valid implicit casts between any of the types
-    and the selected highest precedence type.
-    This is a thin wrapper around datatypes highest precedence check.
+import re
 
-    Parameters
-    ----------
-    nodes : Iterable[ops.Value]
-      A sequence of Expressions
+from collections import namedtuple
+from contextlib import contextmanager
+import pprint
+import warnings
+import sys
 
-    Returns
-    -------
-    dtype: DataType
-      The highest precedence datatype
-    """
-    return dt.highest_precedence(node.output_dtype for node in nodes)
+from six import StringIO
 
+PY3 = (sys.version_info[0] >= 3)
 
-@public
-def castable(source, target):
-    """Return whether source ir type is implicitly castable to target.
+if PY3:
+    def u(s):
+        return s
+else:
+    def u(s):
+        return unicode(s, "unicode_escape")
 
-    Based on the underlying datatypes and the value in case of Literals
-    """
-    value = getattr(source, 'value', None)
-    return dt.castable(source.output_dtype, target.output_dtype, value=value)
 
+DeprecatedOption = namedtuple('DeprecatedOption', 'key msg rkey removal_ver')
+RegisteredOption = namedtuple(
+    'RegisteredOption', 'key defval doc validator cb')
 
-@public
-def comparable(left, right):
-    return castable(left, right) or castable(right, left)
+_deprecated_options = {}  # holds deprecated option metdata
+_registered_options = {}  # holds registered option metdata
+_global_config = {}  # holds the current values for registered options
+_reserved_keys = ['all']  # keys which have a special meaning
 
 
-class rule(validator):
-    def _erase_expr(self, value):
-        return value.op() if isinstance(value, ir.Expr) else value
+class OptionError(AttributeError, KeyError):
 
-    def __call__(self, *args, **kwargs):
-        args = map(self._erase_expr, args)
-        kwargs = {k: self._erase_expr(v) for k, v in kwargs.items()}
-        result = super().__call__(*args, **kwargs)
-        assert not isinstance(result, ir.Expr)
-        return result
+    """Exception for ibis.options, backwards compatible with KeyError
+    checks"""
 
 
-# ---------------------------------------------------------------------
-# Input type validators / coercion functions
+#
+# User API
 
+def _get_single_key(pat, silent):
+    keys = _select_options(pat)
+    if len(keys) == 0:
+        if not silent:
+            _warn_if_deprecated(pat)
+        raise OptionError('No such keys(s): %r' % pat)
+    if len(keys) > 1:
+        raise OptionError('Pattern matched multiple keys')
+    key = keys[0]
 
-@validator
-def expr_of(inner, value, **kwargs):
-    value = inner(value, **kwargs)
-    return value if isinstance(value, ir.Expr) else value.to_expr()
+    if not silent:
+        _warn_if_deprecated(key)
 
+    key = _translate_key(key)
 
-@rule
-def just(arg):
-    return lambda **_: arg
+    return key
 
 
-@rule
-def sort_key_from(table_ref, key, **kwargs):
-    import ibis.expr.operations as ops
+def _get_option(pat, silent=False):
+    key = _get_single_key(pat, silent)
 
-    is_ascending = {
-        "asc": True,
-        "ascending": True,
-        "desc": False,
-        "descending": False,
-        0: False,
-        1: True,
-        False: False,
-        True: True,
-    }
+    # walk the nested dict
+    root, k = _get_root(key)
+    return root[k]
 
-    if callable(key):
-        key = function_of(table_ref, key, **kwargs)
 
-    if isinstance(key, ops.SortKey):
-        return key
-    elif isinstance(key, tuple):
-        key, order = key
-    else:
-        key, order = key, True
+def _set_option(*args, **kwargs):
+    # must at least 1 arg deal with constraints later
+    nargs = len(args)
+    if not nargs or nargs % 2 != 0:
+        raise ValueError("Must provide an even number of non-keyword "
+                         "arguments")
 
-    if isinstance(key, (str, int)):
-        # Actual str/int keys must refer to columns in the table, we don't want
-        # to fallback to converting them to expressions with ibis.literal
-        key = column_from(table_ref, key, **kwargs)
-    else:
-        key = one_of(
-            (function_of(table_ref), column_from(table_ref), any),
-            key,
-            **kwargs,
-        )
-
-    if isinstance(order, str):
-        order = order.lower()
-    order = map_to(is_ascending, order)
-
-    return ops.SortKey(key, ascending=order)
-
-
-@rule
-def datatype(arg, **kwargs):
-    return dt.dtype(arg)
-
-
-# TODO(kszucs): make type argument the first and mandatory, similarly to the
-# value rule, move out the type inference to `ir.literal()` method
-# TODO(kszucs): may not make sense to support an explicit datatype here, we
-# could do the coercion in the API function ibis.literal()
-@rule
-def literal(dtype, value, **kwargs):
-    import ibis.expr.operations as ops
+    # default to false
+    silent = kwargs.get('silent', False)
 
-    if isinstance(value, ops.Literal):
-        return value
+    for k, v in zip(args[::2], args[1::2]):
+        key = _get_single_key(k, silent)
 
-    try:
-        inferred_dtype = dt.infer(value)
-    except com.InputTypeError:
-        has_inferred = False
-    else:
-        has_inferred = True
+        o = _get_registered_option(key)
+        if o and o.validator:
+            o.validator(v)
 
-    if dtype is None:
-        has_explicit = False
-    else:
-        has_explicit = True
-        # TODO(kszucs): handle class-like dtype definitions here explicitly
-        explicit_dtype = dt.dtype(dtype)
-
-    if has_explicit and has_inferred:
-        try:
-            # ensure type correctness: check that the inferred dtype is
-            # implicitly castable to the explicitly given dtype and value
-            dtype = dt.cast(inferred_dtype, target=explicit_dtype, value=value)
-        except com.IbisTypeError:
-            raise TypeError(f'Value {value!r} cannot be safely coerced to `{dtype}`')
-    elif has_explicit:
-        dtype = explicit_dtype
-    elif has_inferred:
-        dtype = inferred_dtype
+        # walk the nested dict
+        root, k = _get_root(key)
+        root[k] = v
+
+        if o.cb:
+            o.cb(key)
+
+
+def _describe_option(pat='', _print_desc=True):
+
+    keys = _select_options(pat)
+    if len(keys) == 0:
+        raise OptionError('No such keys(s)')
+
+    s = u('')
+    for k in keys:  # filter by pat
+        s += _build_option_description(k)
+
+    if _print_desc:
+        print(s)
     else:
-        raise com.IbisTypeError(
-            'The datatype of value {!r} cannot be inferred, try '
-            'passing it explicitly with the `type` keyword.'.format(value)
-        )
+        return s
 
-    if dtype.is_null():
-        return ops.NullLiteral()
 
-    value = dt.normalize(dtype, value)
-    return ops.Literal(value, dtype=dtype)
+def _reset_option(pat, silent=False):
 
+    keys = _select_options(pat)
 
-@rule
-def value(dtype, arg, **kwargs):
-    """Validates that the given argument is a Value with a particular datatype.
+    if len(keys) == 0:
+        raise OptionError('No such keys(s)')
 
-    Parameters
-    ----------
-    dtype
-        DataType subclass or DataType instance
-    arg
-        If a Python literal is given the validator tries to coerce it to an ibis
-        literal.
-    kwargs
-        Keyword arguments
+    if len(keys) > 1 and len(pat) < 4 and pat != 'all':
+        raise ValueError('You must specify at least 4 characters when '
+                         'resetting multiple keys, use the special keyword '
+                         '"all" to reset all the options to their default '
+                         'value')
 
-    Returns
-    -------
-    ir.Value
-        An ibis value expression with the specified datatype
+    for k in keys:
+        _set_option(k, _registered_options[k].defval, silent=silent)
+
+
+def get_default_val(pat):
+    key = _get_single_key(pat, silent=True)
+    return _get_registered_option(key).defval
+
+
+class DictWrapper(object):
+
+    """ provide attribute-style access to a nested dict
     """
-    import ibis.expr.operations as ops
 
-    if isinstance(arg, Deferred):
-        raise com.IbisTypeError(
-            "Deferred input is not allowed, try passing a lambda function instead. "
-            "For example, instead of writing `f(_.a)` write `lambda t: f(t.a)`"
-        )
-
-    if not isinstance(arg, ops.Value):
-        # coerce python literal to ibis literal
-        arg = literal(None, arg)
-
-    if dtype is None:
-        # no datatype restriction
-        return arg
-    elif isinstance(dtype, type):
-        # dtype class has been specified like dt.Interval or dt.Decimal
-        if not issubclass(dtype, dt.DataType):
-            raise com.IbisTypeError(
-                f"Datatype specification {dtype} is not a subclass dt.DataType"
-            )
-        elif isinstance(arg.output_dtype, dtype):
-            return arg
+    def __init__(self, d, prefix=""):
+        object.__setattr__(self, "d", d)
+        object.__setattr__(self, "prefix", prefix)
+
+    def __repr__(self):
+        buf = StringIO()
+        pprint.pprint(self.d, stream=buf)
+        return buf.getvalue()
+
+    def __setattr__(self, key, val):
+        prefix = object.__getattribute__(self, "prefix")
+        if prefix:
+            prefix += "."
+        prefix += key
+        # you can't set new keys
+        # can you can't overwrite subtrees
+        if key in self.d and not isinstance(self.d[key], dict):
+            _set_option(prefix, val)
         else:
-            raise com.IbisTypeError(
-                f'Given argument with datatype {arg.output_dtype} is not '
-                f'subtype of {dtype}'
-            )
-    elif isinstance(dtype, (dt.DataType, str)):
-        # dtype instance or string has been specified and arg's dtype is
-        # implicitly castable to it, like dt.int8 is castable to dt.int64
-        dtype = dt.dtype(dtype)
-        # retrieve literal values for implicit cast check
-        value = getattr(arg, 'value', None)
-        if dt.castable(arg.output_dtype, dtype, value=value):
-            return arg
+            raise OptionError("You can only set the value of existing options")
+
+    def __getattr__(self, key):
+        prefix = object.__getattribute__(self, "prefix")
+        if prefix:
+            prefix += "."
+        prefix += key
+        v = object.__getattribute__(self, "d")[key]
+        if isinstance(v, dict):
+            return DictWrapper(v, prefix)
         else:
-            raise com.IbisTypeError(
-                f'Given argument with datatype {arg.output_dtype} is not '
-                f'implicitly castable to {dtype}'
-            )
-    else:
-        raise com.IbisTypeError(f'Invalid datatype specification {dtype}')
+            return _get_option(prefix)
 
+    def __dir__(self):
+        return list(self.d.keys())
 
-@rule
-def scalar(inner, arg, **kwargs):
-    arg = inner(arg, **kwargs)
-    if arg.output_shape.is_scalar():
-        return arg
-    else:
-        raise com.IbisTypeError(f"{arg} it not a scalar")
 
+# For user convenience,  we'd like to have the available options described
+# in the docstring. For dev convenience we'd like to generate the docstrings
+# dynamically instead of maintaining them by hand. To this, we use the
+# class below which wraps functions inside a callable, and converts
+# __doc__ into a propery function. The doctsrings below are templates
+# using the py2.6+ advanced formatting syntax to plug in a concise list
+# of options, and option descriptions.
+
+
+class CallableDynamicDoc(object):
+
+    def __init__(self, func, doc_tmpl):
+        self.__doc_tmpl__ = doc_tmpl
+        self.__func__ = func
+
+    def __call__(self, *args, **kwds):
+        return self.__func__(*args, **kwds)
+
+    @property
+    def __doc__(self):
+        opts_desc = _describe_option('all', _print_desc=False)
+        opts_list = pp_options_list(list(_registered_options.keys()))
+        return self.__doc_tmpl__.format(opts_desc=opts_desc,
+                                        opts_list=opts_list)
+
+_get_option_tmpl = """
+get_option(pat)
+Retrieves the value of the specified option.
+Available options:
+{opts_list}
+Parameters
+----------
+pat : str
+    Regexp which should match a single option.
+    Note: partial matches are supported for convenience, but unless you use the
+    full option name (e.g. x.y.z.option_name), your code may break in future
+    versions if new options with similar names are introduced.
+Returns
+-------
+result : the value of the option
+Raises
+------
+OptionError : if no such option exists
+Notes
+-----
+The available options with its descriptions:
+{opts_desc}
+"""
+
+_set_option_tmpl = """
+set_option(pat, value)
+Sets the value of the specified option.
+Available options:
+{opts_list}
+Parameters
+----------
+pat : str
+    Regexp which should match a single option.
+    Note: partial matches are supported for convenience, but unless you use the
+    full option name (e.g. x.y.z.option_name), your code may break in future
+    versions if new options with similar names are introduced.
+value :
+    new value of option.
+Returns
+-------
+None
+Raises
+------
+OptionError if no such option exists
+Notes
+-----
+The available options with its descriptions:
+{opts_desc}
+"""
+
+_describe_option_tmpl = """
+describe_option(pat, _print_desc=False)
+Prints the description for one or more registered options.
+Call with not arguments to get a listing for all registered options.
+Available options:
+{opts_list}
+Parameters
+----------
+pat : str
+    Regexp pattern. All matching keys will have their description displayed.
+_print_desc : bool, default True
+    If True (default) the description(s) will be printed to stdout.
+    Otherwise, the description(s) will be returned as a unicode string
+    (for testing).
+Returns
+-------
+None by default, the description(s) as a unicode string if _print_desc
+is False
+Notes
+-----
+The available options with its descriptions:
+{opts_desc}
+"""
+
+_reset_option_tmpl = """
+reset_option(pat)
+Reset one or more options to their default value.
+Pass "all" as argument to reset all options.
+Available options:
+{opts_list}
+Parameters
+----------
+pat : str/regex
+    If specified only options matching `prefix*` will be reset.
+    Note: partial matches are supported for convenience, but unless you
+    use the full option name (e.g. x.y.z.option_name), your code may break
+    in future versions if new options with similar names are introduced.
+Returns
+-------
+None
+Notes
+-----
+The available options with its descriptions:
+{opts_desc}
+"""
+
+# bind the functions with their docstrings into a Callable
+# and use that as the functions exposed in pd.api
+get_option = CallableDynamicDoc(_get_option, _get_option_tmpl)
+set_option = CallableDynamicDoc(_set_option, _set_option_tmpl)
+reset_option = CallableDynamicDoc(_reset_option, _reset_option_tmpl)
+describe_option = CallableDynamicDoc(_describe_option, _describe_option_tmpl)
+options = DictWrapper(_global_config)
 
-@rule
-def column(inner, arg, **kwargs):
-    arg = inner(arg, **kwargs)
-    if arg.output_shape.is_columnar():
-        return arg
-    else:
-        raise com.IbisTypeError(f"{arg} it not a column")
+#
+# Functions for use by pandas developers, in addition to User - api
 
 
-any = value(None)
-double = value(dt.double)
-string = value(dt.string)
-boolean = value(dt.boolean)
-integer = value(dt.int64)
-decimal = value(dt.Decimal)
-floating = value(dt.float64)
-date = value(dt.date)
-time = value(dt.time)
-timestamp = value(dt.Timestamp)
-temporal = one_of([timestamp, date, time])
-json = value(dt.json)
-
-strict_numeric = one_of([integer, floating, decimal])
-soft_numeric = one_of([integer, floating, decimal, boolean])
-numeric = soft_numeric
-
-set_ = value(dt.Set)
-array = value(dt.Array)
-struct = value(dt.Struct)
-mapping = value(dt.Map)
-
-geospatial = value(dt.GeoSpatial)
-point = value(dt.Point)
-linestring = value(dt.LineString)
-polygon = value(dt.Polygon)
-multilinestring = value(dt.MultiLineString)
-multipoint = value(dt.MultiPoint)
-multipolygon = value(dt.MultiPolygon)
-
-
-@public
-@rule
-def interval(arg, units=None, **kwargs):
-    arg = value(dt.Interval, arg)
-    unit = arg.output_dtype.unit
-    if units is not None and unit not in units:
-        msg = 'Interval unit `{}` is not among the allowed ones {}'
-        raise com.IbisTypeError(msg.format(unit, units))
-    return arg
-
-
-@public
-@rule
-def client(arg, **kwargs):
-    from ibis.backends.base import BaseBackend
-
-    return instance_of(BaseBackend, arg)
-
-
-# ---------------------------------------------------------------------
-# Ouput type functions
-
-
-@public
-def dtype_like(name):
-    @attribute.default
-    def output_dtype(self):
-        args = getattr(self, name)
-        args = args if util.is_iterable(args) else [args]
-        return highest_precedence_dtype(args)
-
-    return output_dtype
-
-
-@public
-def shape_like(name):
-    @attribute.default
-    def output_shape(self):
-        args = getattr(self, name)
-        args = args if util.is_iterable(args) else [args]
-        return highest_precedence_shape(args)
-
-    return output_shape
-
-
-# TODO(kszucs): might just use bounds instead of actual literal values
-# that could simplify interval binop output_type methods
-# TODO(kszucs): pre-generate mapping?
-
-
-def _promote_integral_binop(exprs, op):
-    import ibis.expr.operations as ops
-
-    bounds, dtypes = [], []
-    for arg in exprs:
-        dtypes.append(arg.output_dtype)
-        if isinstance(arg, ops.Literal):
-            bounds.append([arg.value])
-        else:
-            bounds.append(arg.output_dtype.bounds)
+class option_context(object):
 
-    all_unsigned = dtypes and util.all_of(dtypes, dt.UnsignedInteger)
-    # In some cases, the bounding type might be int8, even though neither
-    # of the types are that small. We want to ensure the containing type is
-    # _at least_ as large as the smallest type in the expression.
-    values = starmap(op, product(*bounds))
-    dtypes += [dt.infer(v, prefer_unsigned=all_unsigned) for v in values]
-
-    return dt.highest_precedence(dtypes)
-
-
-def _promote_decimal_binop(args, op):
-    if len(args) != 2:
-        return highest_precedence_dtype(args)
-
-    # TODO: Add support for setting the maximum precision and maximum scale
-    left = args[0].output_dtype
-    right = args[1].output_dtype
-
-    max_prec = 31 if left.precision <= 31 and right.precision <= 31 else 63
-    max_scale = 31
-
-    if op is operator.mul:
-        return dt.Decimal(
-            min(max_prec, left.precision + right.precision),
-            min(max_scale, left.scale + right.scale),
-        )
-    elif op is operator.add or op is operator.sub:
-        return dt.Decimal(
-            min(
-                max_prec,
-                max(
-                    left.precision - left.scale,
-                    right.precision - right.scale,
-                )
-                + max(left.scale, right.scale)
-                + 1,
-            ),
-            max(left.scale, right.scale),
-        )
-    else:
-        return highest_precedence_dtype(args)
+    """
+    Context manager to temporarily set options in the `with` statement context.
+    You need to invoke as ``option_context(pat, val, [(pat, val), ...])``.
+    Examples
+    --------
+    >>> with option_context('display.max_rows', 10, 'display.max_columns', 5):
+            ...
+    """
 
+    def __init__(self, *args):
+        if not (len(args) % 2 == 0 and len(args) >= 2):
+            raise ValueError(
+                'Need to invoke as'
+                'option_context(pat, val, [(pat, val), ...)).'
+            )
 
-@public
-def numeric_like(name, op):
-    @attribute.default
-    def output_dtype(self):
-        args = getattr(self, name)
-        dtypes = [arg.output_dtype for arg in args]
-        if util.all_of(dtypes, dt.Integer):
-            result = _promote_integral_binop(args, op)
-        elif util.all_of(dtypes, dt.Decimal):
-            result = _promote_decimal_binop(args, op)
-        else:
-            result = highest_precedence_dtype(args)
+        self.ops = list(zip(args[::2], args[1::2]))
+
+    def __enter__(self):
+        undo = []
+        for pat, val in self.ops:
+            undo.append((pat, _get_option(pat, silent=True)))
 
-        return result
+        self.undo = undo
 
-    return output_dtype
+        for pat, val in self.ops:
+            _set_option(pat, val, silent=True)
 
+    def __exit__(self, *args):
+        if self.undo:
+            for pat, val in self.undo:
+                _set_option(pat, val, silent=True)
 
-# TODO(kszucs): it could be as simple as rlz.instance_of(ops.TableNode)
-# we have a single test case testing the schema superset condition, not
-# used anywhere else
-@public
-@rule
-def table(arg, schema=None, **kwargs):
-    """A table argument.
 
+def register_option(key, defval, doc='', validator=None, cb=None):
+    """Register an option in the package-wide ibis config object
     Parameters
     ----------
-    arg
-        A table node
-    schema
-        A validator for the table's columns. Only column subset validators are
-        currently supported. Accepts any arguments that `sch.schema` accepts.
-        See the example for usage.
-    kwargs
-        Keyword arguments
-
-    The following op will accept an argument named `'table'`. Note that the
-    `schema` argument specifies rules for columns that are required to be in
-    the table: `time`, `group` and `value1`. These must match the types
-    specified in the column rules. Column `value2` is optional, but if present
-    it must be of the specified type. The table may have extra columns not
-    specified in the schema.
-    """
-    import pandas as pd
-
-    import ibis
-    import ibis.expr.operations as ops
-
-    if isinstance(arg, pd.DataFrame):
-        arg = ibis.memtable(arg).op()
-
-    if not isinstance(arg, ops.TableNode):
-        raise com.IbisTypeError(
-            f'Argument is not a table; got type {type(arg).__name__}'
-        )
-
-    if schema is not None:
-        if arg.schema >= sch.schema(schema):
-            return arg
-
-        raise com.IbisTypeError(
-            f'Argument is not a table with column subset of {schema}'
-        )
-    return arg
-
-
-@public
-@rule
-def column_from(table_ref, column, **kwargs):
-    """A column from a named table.
-
-    This validator accepts columns passed as string, integer, or column
-    expression. In the case of a column expression, this validator
-    checks if the column in the table is equal to the column being
-    passed.
-    """
-    import ibis.expr.operations as ops
-
-    # TODO(kszucs): should avoid converting to TableExpr
-    table = table_ref(**kwargs).to_expr()
-
-    # TODO(kszucs): should avoid converting to a ColumnExpr
-    if isinstance(column, ops.Node):
-        column = column.to_expr()
-
-    column = table._ensure_expr(column)
-
-    if not isinstance(column, ir.Column):
-        raise com.IbisTypeError(
-            f"value must be an int or str or Column, got {type(column).__name__}"
-        )
+    key       - a fully-qualified key, e.g. "x.y.option - z".
+    defval    - the default value of the option
+    doc       - a string description of the option
+    validator - a function of a single argument, should raise `ValueError` if
+                called with a value which is not a legal value for the option.
+    cb        - a function of a single argument "key", which is called
+                immediately after an option value is set/reset. key is
+                the full name of the option.
+    Returns
+    -------
+    Nothing.
+    Raises
+    ------
+    ValueError if `validator` is specified and `defval` is not a valid value.
+    """
+    import tokenize
+    import keyword
+    key = key.lower()
+
+    if key in _registered_options:
+        raise OptionError("Option '%s' has already been registered" % key)
+    if key in _reserved_keys:
+        raise OptionError("Option '%s' is a reserved key" % key)
+
+    # the default value should be legal
+    if validator:
+        validator(defval)
+
+    # walk the nested dict, creating dicts as needed along the path
+    path = key.split('.')
+
+    for k in path:
+        if not bool(re.match('^' + tokenize.Name + '$', k)):
+            raise ValueError("%s is not a valid identifier" % k)
+        if keyword.iskeyword(k):
+            raise ValueError("%s is a python keyword" % k)
+
+    cursor = _global_config
+    for i, p in enumerate(path[:-1]):
+        if not isinstance(cursor, dict):
+            raise OptionError("Path prefix to option '%s' is already an option"
+                              % '.'.join(path[:i]))
+        if p not in cursor:
+            cursor[p] = {}
+        cursor = cursor[p]
+
+    if not isinstance(cursor, dict):
+        raise OptionError("Path prefix to option '%s' is already an option"
+                          % '.'.join(path[:-1]))
+
+    cursor[path[-1]] = defval  # initialize
+
+    # save the option metadata
+    _registered_options[key] = RegisteredOption(key=key, defval=defval,
+                                                doc=doc, validator=validator,
+                                                cb=cb)
 
-    if not column.has_name():
-        raise com.IbisTypeError(f"Passed column {column} has no name")
 
-    maybe_column = column.get_name()
-    try:
-        if column.equals(table[maybe_column]):
-            return column.op()
-        else:
-            raise com.IbisTypeError(f"Passed column is not a column in {type(table)}")
-    except com.IbisError:
-        raise com.IbisTypeError(f"Cannot get column {maybe_column} from {type(table)}")
-
-
-@public
-@rule
-def base_table_of(table_ref, *, this, strict=True):
-    from ibis.expr.analysis import find_first_base_table
-
-    arg = table_ref(this=this)
-    base = find_first_base_table(arg)
-    if strict and base is None:
-        raise com.IbisTypeError(f"`{arg}` doesn't have a base table")
-    return base
-
-
-@public
-@rule
-def function_of(table_ref, fn, *, output_rule=any, this=None):
-    arg = table_ref(this=this).to_expr()
-
-    if util.is_function(fn):
-        arg = fn(arg)
-    elif isinstance(fn, Deferred):
-        arg = fn.resolve(arg)
-    else:
-        raise com.IbisTypeError(
-            'argument `fn` must be a function, lambda or deferred operation'
-        )
+def deprecate_option(key, msg=None, rkey=None, removal_ver=None):
+    """
+    Mark option `key` as deprecated, if code attempts to access this option,
+    a warning will be produced, using `msg` if given, or a default message
+    if not.
+    if `rkey` is given, any access to the key will be re-routed to `rkey`.
+    Neither the existence of `key` nor that if `rkey` is checked. If they
+    do not exist, any subsequence access will fail as usual, after the
+    deprecation warning is given.
+    Parameters
+    ----------
+    key - the name of the option to be deprecated. must be a fully-qualified
+          option name (e.g "x.y.z.rkey").
+    msg - (Optional) a warning message to output when the key is referenced.
+          if no message is given a default message will be emitted.
+    rkey - (Optional) the name of an option to reroute access to.
+           If specified, any referenced `key` will be re-routed to `rkey`
+           including set/get/reset.
+           rkey must be a fully-qualified option name (e.g "x.y.z.rkey").
+           used by the default message if no `msg` is specified.
+    removal_ver - (Optional) specifies the version in which this option will
+                  be removed. used by the default message if no `msg`
+                  is specified.
+    Returns
+    -------
+    Nothing
+    Raises
+    ------
+    OptionError - if key has already been deprecated.
+    """
 
-    return output_rule(arg, this=this)
+    key = key.lower()
 
+    if key in _deprecated_options:
+        raise OptionError("Option '%s' has already been defined as deprecated."
+                          % key)
 
-@public
-@rule
-def reduction(arg, **kwargs):
-    from ibis.expr.analysis import is_reduction
+    _deprecated_options[key] = DeprecatedOption(key, msg, rkey, removal_ver)
 
-    if not is_reduction(arg):
-        raise com.IbisTypeError("`argument` must be a reduction")
 
-    return arg
+#
+# functions internal to the module
+
+def _select_options(pat):
+    """returns a list of keys matching `pat`
+    if pat=="all", returns all registered options
+    """
 
+    # short-circuit for exact key
+    if pat in _registered_options:
+        return [pat]
 
-@public
-@rule
-def analytic(arg, **kwargs):
-    from ibis.expr.analysis import is_analytic
+    # else look through all of them
+    keys = sorted(_registered_options.keys())
+    if pat == 'all':  # reserved key
+        return keys
 
-    if not is_analytic(arg):
-        raise com.IbisInputError('Expression does not contain a valid window operation')
+    return [k for k in keys if re.search(pat, k, re.I)]
 
-    return arg
 
+def _get_root(key):
+    path = key.split('.')
+    cursor = _global_config
+    for p in path[:-1]:
+        cursor = cursor[p]
+    return cursor, path[-1]
 
-@public
-@rule
-def window_boundary(inner, arg, **kwargs):
-    import ibis.expr.operations as ops
 
-    arg = inner(arg, **kwargs)
+def _is_deprecated(key):
+    """ Returns True if the given option has been deprecated """
 
-    if isinstance(arg, ops.WindowBoundary):
-        return arg
-    elif isinstance(arg, ops.Negate):
-        return ops.WindowBoundary(arg.arg, preceding=True)
-    elif isinstance(arg, ops.Literal):
-        new = arg.copy(value=abs(arg.value))
-        return ops.WindowBoundary(new, preceding=arg.value < 0)
-    elif isinstance(arg, ops.Value):
-        return ops.WindowBoundary(arg, preceding=False)
+    key = key.lower()
+    return key in _deprecated_options
+
+
+def _get_deprecated_option(key):
+    """
+    Retrieves the metadata for a deprecated option, if `key` is deprecated.
+    Returns
+    -------
+    DeprecatedOption (namedtuple) if key is deprecated, None otherwise
+    """
+
+    try:
+        d = _deprecated_options[key]
+    except KeyError:
+        return None
     else:
-        raise TypeError(f'Invalid window boundary type: {type(arg)}')
+        return d
 
 
-row_window_boundary = window_boundary(integer)
-range_window_boundary = window_boundary(one_of([numeric, interval]))
+def _get_registered_option(key):
+    """
+    Retrieves the option metadata if `key` is a registered option.
+    Returns
+    -------
+    RegisteredOption (namedtuple) if key is deprecated, None otherwise
+    """
+    return _registered_options.get(key)
 
 
-def _arg_type_error_format(op):
-    from ibis.expr.operations.generic import Literal
+def _translate_key(key):
+    """
+    if key id deprecated and a replacement key defined, will return the
+    replacement key, otherwise returns `key` as - is
+    """
 
-    if isinstance(op, Literal):
-        return f"Literal({op.value}):{op.output_dtype}"
+    d = _get_deprecated_option(key)
+    if d:
+        return d.rkey or key
     else:
-        return f"{op.name}:{op.output_dtype}"
+        return key
 
 
-public(
-    any=any,
-    array=array,
-    bool=bool_,
-    boolean=boolean,
-    date=date,
-    decimal=decimal,
-    double=double,
-    floating=floating,
-    geospatial=geospatial,
-    integer=integer,
-    isin=isin,
-    json=json,
-    lazy_instance_of=lazy_instance_of,
-    linestring=linestring,
-    mapping=mapping,
-    multilinestring=multilinestring,
-    multipoint=multipoint,
-    numeric=numeric,
-    optional=optional,
-    point=point,
-    polygon=polygon,
-    ref=ref,
-    set_=set_,
-    soft_numeric=soft_numeric,
-    str_=str_,
-    strict_numeric=strict_numeric,
-    string=string,
-    struct=struct,
-    temporal=temporal,
-    time=time,
-    timestamp=timestamp,
-    tuple_of=tuple_of,
-    row_window_boundary=row_window_boundary,
-    range_window_boundary=range_window_boundary,
-)
+def _warn_if_deprecated(key):
+    """
+    Checks if `key` is a deprecated option and if so, prints a warning.
+    Returns
+    -------
+    bool - True if `key` is deprecated, False otherwise.
+    """
+
+    d = _get_deprecated_option(key)
+    if d:
+        if d.msg:
+            print(d.msg)
+            warnings.warn(d.msg, DeprecationWarning)
+        else:
+            msg = "'%s' is deprecated" % key
+            if d.removal_ver:
+                msg += ' and will be removed in %s' % d.removal_ver
+            if d.rkey:
+                msg += ", please use '%s' instead." % d.rkey
+            else:
+                msg += ', please refrain from using it.'
+
+            warnings.warn(msg, DeprecationWarning)
+        return True
+    return False
+
+
+def _build_option_description(k):
+    """ Builds a formatted description of a registered option and prints it """
+
+    o = _get_registered_option(k)
+    d = _get_deprecated_option(k)
+
+    s = u('%s ') % k
+
+    if o.doc:
+        s += '\n'.join(o.doc.strip().split('\n'))
+    else:
+        s += 'No description available.'
+
+    if o:
+        s += u('\n    [default: %s] [currently: %s]') % (o.defval,
+                                                         _get_option(k, True))
+
+    if d:
+        s += u('\n    (Deprecated')
+        s += (u(', use `%s` instead.') % d.rkey if d.rkey else '')
+        s += u(')')
+
+    s += '\n\n'
+    return s
+
+
+def pp_options_list(keys, width=80, _print=False):
+    """ Builds a concise listing of available options, grouped by prefix """
+
+    from textwrap import wrap
+    from itertools import groupby
+
+    def pp(name, ks):
+        pfx = ('- ' + name + '.[' if name else '')
+        ls = wrap(', '.join(ks), width, initial_indent=pfx,
+                  subsequent_indent='  ', break_long_words=False)
+        if ls and ls[-1] and name:
+            ls[-1] = ls[-1] + ']'
+        return ls
+
+    ls = []
+    singles = [x for x in sorted(keys) if x.find('.') < 0]
+    if singles:
+        ls += pp('', singles)
+    keys = [x for x in keys if x.find('.') >= 0]
+
+    for k, g in groupby(sorted(keys), lambda x: x[:x.rfind('.')]):
+        ks = [x[len(k) + 1:] for x in list(g)]
+        ls += pp(k, ks)
+    s = '\n'.join(ls)
+    if _print:
+        print(s)
+    else:
+        return s
+
+
+#
+# helpers
+
+
+@contextmanager
+def config_prefix(prefix):
+    """contextmanager for multiple invocations of API  with a common prefix
+    supported API functions: (register / get / set )__option
+    Warning: This is not thread - safe, and won't work properly if you import
+    the API functions into your module using the "from x import y" construct.
+    Example:
+    import ibis.config as cf
+    with cf.config_prefix("display.font"):
+        cf.register_option("color", "red")
+        cf.register_option("size", " 5 pt")
+        cf.set_option(size, " 6 pt")
+        cf.get_option(size)
+        ...
+        etc'
+    will register options "display.font.color", "display.font.size", set the
+    value of "display.font.size"... and so on.
+    """
+
+    # Note: reset_option relies on set_option, and on key directly
+    # it does not fit in to this monkey-patching scheme
+
+    global register_option, get_option, set_option, reset_option
+
+    def wrap(func):
+
+        def inner(key, *args, **kwds):
+            pkey = '%s.%s' % (prefix, key)
+            return func(pkey, *args, **kwds)
+
+        return inner
+
+    _register_option = register_option
+    _get_option = get_option
+    _set_option = set_option
+    set_option = wrap(set_option)
+    get_option = wrap(get_option)
+    register_option = wrap(register_option)
+    yield None
+    set_option = _set_option
+    get_option = _get_option
+    register_option = _register_option
+
+
+# These factories and methods are handy for use as the validator
+# arg in register_option
+
+def is_type_factory(_type):
+    """
+    Parameters
+    ----------
+    `_type` - a type to be compared against (e.g. type(x) == `_type`)
+    Returns
+    -------
+    validator - a function of a single argument x , which returns the
+                True if type(x) is equal to `_type`
+    """
+
+    def inner(x):
+        if type(x) != _type:
+            raise ValueError("Value must have type '%s'" % str(_type))
+
+    return inner
+
+
+def is_instance_factory(_type):
+    """
+    Parameters
+    ----------
+    `_type` - the type to be checked against
+    Returns
+    -------
+    validator - a function of a single argument x , which returns the
+                True if x is an instance of `_type`
+    """
+    if isinstance(_type, (tuple, list)):
+        _type = tuple(_type)
+        type_repr = "|".join(map(str, _type))
+    else:
+        type_repr = "'%s'" % _type
+
+    def inner(x):
+        if not isinstance(x, _type):
+            raise ValueError("Value must be an instance of %s" % type_repr)
+
+    return inner
+
+
+def is_one_of_factory(legal_values):
+    def inner(x):
+        if x not in legal_values:
+            pp_values = map(str, legal_values)
+            raise ValueError("Value must be one of %s"
+                             % str("|".join(pp_values)))
+
+    return inner
+
+# common type validators, for convenience
+# usage: register_option(... , validator = is_int)
+is_int = is_type_factory(int)
+is_bool = is_type_factory(bool)
+is_float = is_type_factory(float)
+is_str = is_type_factory(str)
+# is_unicode = is_type_factory(compat.text_type)
+is_text = is_instance_factory((str, bytes))
```

### Comparing `ibis_framework-5.1.0/ibis/expr/types/generic.py` & `ibis-framework-v0.6.0/ibis/impala/compiler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1224 +1,1315 @@
-from __future__ import annotations
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from typing import TYPE_CHECKING, Any, Iterable, Literal, Sequence
-
-from public import public
+from six import StringIO
+import datetime
 
 import ibis
-import ibis.common.exceptions as com
+import ibis.expr.analysis as L
 import ibis.expr.datatypes as dt
+import ibis.expr.types as ir
 import ibis.expr.operations as ops
-from ibis import util
-from ibis.common.grounds import Singleton
-from ibis.expr.types.core import Expr, _binop, _FixedTextJupyterMixin
-
-if TYPE_CHECKING:
-    import pandas as pd
-
-    import ibis.expr.types as ir
-
-
-@public
-class Value(Expr):
-    """Base class for a data generating expression having a known type."""
-
-    def name(self, name):
-        """Rename an expression to `name`.
-
-        Parameters
-        ----------
-        name
-            The new name of the expression
-
-        Returns
-        -------
-        Value
-            `self` with name `name`
-
-        Examples
-        --------
-        >>> import ibis
-        >>> t = ibis.table(dict(a="int64"), name="t")
-        >>> t.a.name("b")
-        r0 := UnboundTable: t
-          a int64
-        b: r0.a
+import ibis.expr.temporal as tempo
+
+import ibis.sql.compiler as comp
+import ibis.sql.transforms as transforms
+
+import ibis.impala.identifiers as identifiers
+
+import ibis.common as com
+import ibis.util as util
+
+
+def build_ast(expr, context=None):
+    builder = ImpalaQueryBuilder(expr, context=context)
+    return builder.get_result()
+
+
+def _get_query(expr, context):
+    ast = build_ast(expr, context)
+    query = ast.queries[0]
+
+    return query
+
+
+def to_sql(expr, context=None):
+    query = _get_query(expr, context)
+    return query.compile()
+
+
+# ----------------------------------------------------------------------
+# Select compilation
+
+class ImpalaSelectBuilder(comp.SelectBuilder):
+
+    @property
+    def _select_class(self):
+        return ImpalaSelect
+
+
+class ImpalaQueryBuilder(comp.QueryBuilder):
+
+    select_builder = ImpalaSelectBuilder
+
+    @property
+    def _make_context(self):
+        return ImpalaContext
+
+    @property
+    def _union_class(self):
+        return ImpalaUnion
+
+
+class ImpalaContext(comp.QueryContext):
+
+    def _to_sql(self, expr, ctx):
+        return to_sql(expr, context=ctx)
+
+
+class ImpalaSelect(comp.Select):
+
+    """
+    A SELECT statement which, after execution, might yield back to the user a
+    table, array/list, or scalar value, depending on the expression that
+    generated it
+    """
+
+    def compile(self):
+        """
+        This method isn't yet idempotent; calling multiple times may yield
+        unexpected results
         """
-        # TODO(kszucs): shouldn't do simplification here, but rather later
-        # when simplifying the whole operation tree
-        # the expression's name is idendical to the new one
-        if self.has_name() and self.get_name() == name:
-            return self
-
-        if isinstance(self.op(), ops.Alias):
-            # only keep a single alias operation
-            op = ops.Alias(arg=self.op().arg, name=name)
+        # Can't tell if this is a hack or not. Revisit later
+        self.context.set_query(self)
+
+        # If any subqueries, translate them and add to beginning of query as
+        # part of the WITH section
+        with_frag = self.format_subqueries()
+
+        # SELECT
+        select_frag = self.format_select_set()
+
+        # FROM, JOIN, UNION
+        from_frag = self.format_table_set()
+
+        # WHERE
+        where_frag = self.format_where()
+
+        # GROUP BY and HAVING
+        groupby_frag = self.format_group_by()
+
+        # ORDER BY and LIMIT
+        order_frag = self.format_postamble()
+
+        # Glue together the query fragments and return
+        query = _join_not_none('\n', [with_frag, select_frag, from_frag,
+                                      where_frag, groupby_frag, order_frag])
+
+        return query
+
+    def format_subqueries(self):
+        if len(self.subqueries) == 0:
+            return
+
+        context = self.context
+
+        buf = StringIO()
+        buf.write('WITH ')
+
+        for i, expr in enumerate(self.subqueries):
+            if i > 0:
+                buf.write(',\n')
+            formatted = util.indent(context.get_compiled_expr(expr), 2)
+            alias = context.get_ref(expr)
+            buf.write('{0} AS (\n{1}\n)'.format(alias, formatted))
+
+        return buf.getvalue()
+
+    def format_select_set(self):
+        # TODO:
+        context = self.context
+        formatted = []
+        for expr in self.select_set:
+            if isinstance(expr, ir.ValueExpr):
+                expr_str = self._translate(expr, named=True)
+            elif isinstance(expr, ir.TableExpr):
+                # A * selection, possibly prefixed
+                if context.need_aliases():
+                    alias = context.get_ref(expr)
+
+                    # materialized join will not have an alias. see #491
+                    expr_str = '{0}.*'.format(alias) if alias else '*'
+                else:
+                    expr_str = '*'
+            formatted.append(expr_str)
+
+        buf = StringIO()
+        line_length = 0
+        max_length = 70
+        tokens = 0
+        for i, val in enumerate(formatted):
+            # always line-break for multi-line expressions
+            if val.count('\n'):
+                if i:
+                    buf.write(',')
+                buf.write('\n')
+                indented = util.indent(val, self.indent)
+                buf.write(indented)
+
+                # set length of last line
+                line_length = len(indented.split('\n')[-1])
+                tokens = 1
+            elif (tokens > 0 and line_length and
+                  len(val) + line_length > max_length):
+                # There is an expr, and adding this new one will make the line
+                # too long
+                buf.write(',\n       ') if i else buf.write('\n')
+                buf.write(val)
+                line_length = len(val) + 7
+                tokens = 1
+            else:
+                if i:
+                    buf.write(',')
+                buf.write(' ')
+                buf.write(val)
+                tokens += 1
+                line_length += len(val) + 2
+
+        if self.distinct:
+            select_key = 'SELECT DISTINCT'
         else:
-            op = ops.Alias(arg=self, name=name)
+            select_key = 'SELECT'
 
-        return op.to_expr()
+        return '{0}{1}'.format(select_key, buf.getvalue())
 
-    # TODO(kszucs): should rename to dtype
-    def type(self) -> dt.DataType:
-        """Return the [DataType] of this expression."""
-        return self.op().output_dtype
-
-    def hash(self, how: str = "fnv") -> ir.IntegerValue:
-        """Compute an integer hash value.
-
-        Parameters
-        ----------
-        how
-            Hash algorithm to use
-
-        Returns
-        -------
-        IntegerValue
-            The hash value of `self`
-        """
-        return ops.Hash(self, how).to_expr()
+    def format_table_set(self):
+        if self.table_set is None:
+            return None
+
+        fragment = 'FROM '
+
+        helper = _TableSetFormatter(self, self.table_set)
+        fragment += helper.get_result()
+
+        return fragment
+
+    def format_group_by(self):
+        if not len(self.group_by):
+            # There is no aggregation, nothing to see here
+            return None
+
+        lines = []
+        if len(self.group_by) > 0:
+            clause = 'GROUP BY {0}'.format(', '.join([
+                str(x + 1) for x in self.group_by]))
+            lines.append(clause)
+
+        if len(self.having) > 0:
+            trans_exprs = []
+            for expr in self.having:
+                translated = self._translate(expr)
+                trans_exprs.append(translated)
+            lines.append('HAVING {0}'.format(' AND '.join(trans_exprs)))
+
+        return '\n'.join(lines)
+
+    def format_where(self):
+        if len(self.where) == 0:
+            return None
+
+        buf = StringIO()
+        buf.write('WHERE ')
+        fmt_preds = [self._translate(pred, permit_subquery=True)
+                     for pred in self.where]
+        conj = ' AND\n{0}'.format(' ' * 6)
+        buf.write(conj.join(fmt_preds))
+        return buf.getvalue()
+
+    def format_postamble(self):
+        buf = StringIO()
+        lines = 0
+
+        if len(self.order_by) > 0:
+            buf.write('ORDER BY ')
+            formatted = []
+            for expr in self.order_by:
+                key = expr.op()
+                translated = self._translate(key.expr)
+                if not key.ascending:
+                    translated += ' DESC'
+                formatted.append(translated)
+            buf.write(', '.join(formatted))
+            lines += 1
+
+        if self.limit is not None:
+            if lines:
+                buf.write('\n')
+            n, offset = self.limit['n'], self.limit['offset']
+            buf.write('LIMIT {0}'.format(n))
+            if offset is not None and offset != 0:
+                buf.write(' OFFSET {0}'.format(offset))
+            lines += 1
+
+        if not lines:
+            return None
+
+        return buf.getvalue()
+
+    @property
+    def translator(self):
+        return ImpalaExprTranslator
+
+
+def _join_not_none(sep, pieces):
+    pieces = [x for x in pieces if x is not None]
+    return sep.join(pieces)
+
+
+class _TableSetFormatter(comp.TableSetFormatter):
+
+    def get_result(self):
+        # Got to unravel the join stack; the nesting order could be
+        # arbitrary, so we do a depth first search and push the join tokens
+        # and predicates onto a flat list, then format them
+        op = self.expr.op()
 
-    def cast(self, target_type: dt.DataType) -> Value:
-        """Cast expression to indicated data type.
+        if isinstance(op, ops.Join):
+            self._walk_join_tree(op)
+        else:
+            self.join_tables.append(self._format_table(self.expr))
 
-        Parameters
-        ----------
-        target_type
-            Type to cast to
-
-        Returns
-        -------
-        Value
-            Casted expression
-        """
-        op = ops.Cast(self, to=target_type)
+        # TODO: Now actually format the things
+        buf = StringIO()
+        buf.write(self.join_tables[0])
+        for jtype, table, preds in zip(self.join_types, self.join_tables[1:],
+                                       self.join_predicates):
+            buf.write('\n')
+            buf.write(util.indent('{0} {1}'.format(jtype, table), self.indent))
+
+            if len(preds):
+                buf.write('\n')
+                fmt_preds = [self._translate(pred) for pred in preds]
+                conj = ' AND\n{0}'.format(' ' * 3)
+                fmt_preds = util.indent('ON ' + conj.join(fmt_preds),
+                                        self.indent * 2)
+                buf.write(fmt_preds)
+
+        return buf.getvalue()
+
+    _join_names = {
+        ops.InnerJoin: 'INNER JOIN',
+        ops.LeftJoin: 'LEFT OUTER JOIN',
+        ops.RightJoin: 'RIGHT OUTER JOIN',
+        ops.OuterJoin: 'FULL OUTER JOIN',
+        ops.LeftAntiJoin: 'LEFT ANTI JOIN',
+        ops.LeftSemiJoin: 'LEFT SEMI JOIN',
+        ops.CrossJoin: 'CROSS JOIN'
+    }
+
+    def _get_join_type(self, op):
+        jname = self._join_names[type(op)]
+
+        # Impala requires this
+        if len(op.predicates) == 0:
+            jname = self._join_names[ops.CrossJoin]
+
+        return jname
+
+    def _format_table(self, expr):
+        # TODO: This could probably go in a class and be significantly nicer
+        ctx = self.context
+
+        ref_expr = expr
+        op = ref_op = expr.op()
+        if isinstance(op, ops.SelfReference):
+            ref_expr = op.table
+            ref_op = ref_expr.op()
+
+        if isinstance(ref_op, ops.PhysicalTable):
+            name = ref_op.name
+            if name is None:
+                raise com.RelationError('Table did not have a name: {0!r}'
+                                        .format(expr))
+            result = quote_identifier(name)
+            is_subquery = False
+        else:
+            # A subquery
+            if ctx.is_extracted(ref_expr):
+                # Was put elsewhere, e.g. WITH block, we just need to grab its
+                # alias
+                alias = ctx.get_ref(expr)
 
-        if op.to == self.type():
-            # noop case if passed type is the same
-            return self
-
-        if op.to.is_geospatial():
-            from_geotype = self.type().geotype or 'geometry'
-            to_geotype = op.to.geotype
-            if from_geotype == to_geotype:
-                return self
-
-        return op.to_expr()
-
-    def coalesce(self, *args: Value) -> Value:
-        """Return the first non-null value from `args`.
-
-        Parameters
-        ----------
-        args
-            Arguments from which to choose the first non-null value
-
-        Returns
-        -------
-        Value
-            Coalesced expression
-
-        Examples
-        --------
-        >>> import ibis
-        >>> ibis.coalesce(None, 4, 5).name("x")
-        x: Coalesce(...)
-        """
-        return ops.Coalesce((self, *args)).to_expr()
+                # HACK: self-references have to be treated more carefully here
+                if isinstance(op, ops.SelfReference):
+                    return '{0} {1}'.format(ctx.get_ref(ref_expr), alias)
+                else:
+                    return alias
 
-    def greatest(self, *args: ir.Value) -> ir.Value:
-        """Compute the largest value among the supplied arguments.
+            subquery = ctx.get_compiled_expr(expr)
+            result = '(\n{0}\n)'.format(util.indent(subquery, self.indent))
+            is_subquery = True
 
-        Parameters
-        ----------
-        args
-            Arguments to choose from
-
-        Returns
-        -------
-        Value
-            Maximum of the passed arguments
-        """
-        return ops.Greatest((self, *args)).to_expr()
+        if is_subquery or ctx.need_aliases():
+            result += ' {0}'.format(ctx.get_ref(expr))
 
-    def least(self, *args: ir.Value) -> ir.Value:
-        """Compute the smallest value among the supplied arguments.
+        return result
 
-        Parameters
-        ----------
-        args
-            Arguments to choose from
-
-        Returns
-        -------
-        Value
-            Minimum of the passed arguments
-        """
-        return ops.Least((self, *args)).to_expr()
 
-    def typeof(self) -> ir.StringValue:
-        """Return the data type of the expression.
+class ImpalaUnion(comp.Union):
 
-        The values of the returned strings are necessarily backend dependent.
+    def compile(self):
+        context = self.context
 
-        Returns
-        -------
-        StringValue
-            A string indicating the type of the value
-        """
-        return ops.TypeOf(self).to_expr()
+        if self.distinct:
+            union_keyword = 'UNION'
+        else:
+            union_keyword = 'UNION ALL'
 
-    def fillna(self, fill_value: Scalar) -> Value:
-        """Replace any null values with the indicated fill value.
+        left_set = context.get_compiled_expr(self.left)
+        right_set = context.get_compiled_expr(self.right)
 
-        Parameters
-        ----------
-        fill_value
-            Value with which to replace `NA` values in `self`
-
-        Examples
-        --------
-        >>> import ibis
-        >>> ibis.options.interactive = True
-        >>> t = ibis.examples.penguins.fetch()
-        >>> t.sex
-        ┏━━━━━━━━┓
-        ┃ sex    ┃
-        ┡━━━━━━━━┩
-        │ string │
-        ├────────┤
-        │ male   │
-        │ female │
-        │ female │
-        │ NULL   │
-        │ female │
-        │ male   │
-        │ female │
-        │ male   │
-        │ NULL   │
-        │ NULL   │
-        │ …      │
-        └────────┘
-        >>> t.sex.fillna("unrecorded").name("sex")
-        ┏━━━━━━━━━━━━┓
-        ┃ sex        ┃
-        ┡━━━━━━━━━━━━┩
-        │ string     │
-        ├────────────┤
-        │ male       │
-        │ female     │
-        │ female     │
-        │ unrecorded │
-        │ female     │
-        │ male       │
-        │ female     │
-        │ male       │
-        │ unrecorded │
-        │ unrecorded │
-        │ …          │
-        └────────────┘
-
-        Returns
-        -------
-        Value
-            `self` filled with `fill_value` where it is `NA`
-        """
-        return ops.IfNull(self, fill_value).to_expr()
+        query = '{0}\n{1}\n{2}'.format(left_set, union_keyword, right_set)
+        return query
 
-    def nullif(self, null_if_expr: Value) -> Value:
-        """Set values to null if they equal the values `null_if_expr`.
 
-        Commonly use to avoid divide-by-zero problems by replacing zero with
-        `NULL` in the divisor.
+# ---------------------------------------------------------------------
+# Scalar and array expression formatting
 
-        Parameters
-        ----------
-        null_if_expr
-            Expression indicating what values should be NULL
-
-        Returns
-        -------
-        Value
-            Value expression
-        """
-        return ops.NullIf(self, null_if_expr).to_expr()
+_sql_type_names = {
+    'int8': 'tinyint',
+    'int16': 'smallint',
+    'int32': 'int',
+    'int64': 'bigint',
+    'float': 'float',
+    'double': 'double',
+    'string': 'string',
+    'boolean': 'boolean',
+    'timestamp': 'timestamp',
+    'decimal': 'decimal',
+}
 
-    def between(
-        self,
-        lower: Value,
-        upper: Value,
-    ) -> ir.BooleanValue:
-        """Check if this expression is between `lower` and `upper`, inclusive.
-
-        Parameters
-        ----------
-        lower
-            Lower bound
-        upper
-            Upper bound
-
-        Returns
-        -------
-        BooleanValue
-            Expression indicating membership in the provided range
-        """
-        return ops.Between(self, lower, upper).to_expr()
 
-    def isin(self, values: Value | Sequence[Value]) -> ir.BooleanValue:
-        """Check whether this expression's values are in `values`.
+def _cast(translator, expr):
+    op = expr.op()
+    arg, target_type = op.args
+    arg_formatted = translator.translate(arg)
 
-        Parameters
-        ----------
-        values
-            Values or expression to check for membership
-
-        Returns
-        -------
-        BooleanValue
-            Expression indicating membership
-
-        Examples
-        --------
-        Check whether a column's values are contained in a sequence
-
-        >>> import ibis
-        >>> table = ibis.table(dict(string_col='string'), name="t")
-        >>> table.string_col.isin(['foo', 'bar', 'baz'])
-        r0 := UnboundTable: t
-          string_col string
-        Contains(string_col): Contains(...)
-
-        Check whether a column's values are contained in another table's column
-
-        >>> table2 = ibis.table(dict(other_string_col='string'), name="t2")
-        >>> table.string_col.isin(table2.other_string_col)
-        r0 := UnboundTable: t
-          string_col string
-        r1 := UnboundTable: t2
-          other_string_col string
-        Contains(string_col, other_string_col): Contains(...)
-        """
-        return ops.Contains(self, values).to_expr()
+    if isinstance(arg, ir.CategoryValue) and target_type == 'int32':
+        return arg_formatted
+    else:
+        sql_type = _type_to_sql_string(target_type)
+        return 'CAST({0!s} AS {1!s})'.format(arg_formatted, sql_type)
 
-    def notin(self, values: Value | Sequence[Value]) -> ir.BooleanValue:
-        """Check whether this expression's values are not in `values`.
 
-        Parameters
-        ----------
-        values
-            Values or expression to check for lack of membership
-
-        Returns
-        -------
-        BooleanValue
-            Whether `self`'s values are not contained in `values`
-        """
-        return ops.NotContains(self, values).to_expr()
+def _type_to_sql_string(tval):
+    if isinstance(tval, dt.Decimal):
+        return 'decimal({0},{1})'.format(tval.precision, tval.scale)
+    else:
+        return _sql_type_names[tval.name()]
 
-    def substitute(
-        self,
-        value: Value | dict,
-        replacement: Value | None = None,
-        else_: Value | None = None,
-    ):
-        """Replace values given in `values` with `replacement`.
-
-        This is similar to the pandas `replace` method.
-
-        Parameters
-        ----------
-        value
-            Expression or dict.
-        replacement
-            If an expression is passed to value, this must be
-            passed.
-        else_
-            If an original value does not match `value`, then `else_` is used.
-            The default of `None` means leave the original value unchanged.
-
-        Returns
-        -------
-        Value
-            Replaced values
-        """
-        expr = self.case()
-        if isinstance(value, dict):
-            for k, v in sorted(value.items()):
-                expr = expr.when(k, v)
+
+def _between(translator, expr):
+    op = expr.op()
+    comp, lower, upper = [translator.translate(x) for x in op.args]
+    return '{0!s} BETWEEN {1!s} AND {2!s}'.format(comp, lower, upper)
+
+
+def _is_null(translator, expr):
+    formatted_arg = translator.translate(expr.op().args[0])
+    return '{0!s} IS NULL'.format(formatted_arg)
+
+
+def _not_null(translator, expr):
+    formatted_arg = translator.translate(expr.op().args[0])
+    return '{0!s} IS NOT NULL'.format(formatted_arg)
+
+
+_cumulative_to_reduction = {
+    ops.CumulativeSum: ops.Sum,
+    ops.CumulativeMin: ops.Min,
+    ops.CumulativeMax: ops.Max,
+    ops.CumulativeMean: ops.Mean,
+    ops.CumulativeAny: ops.Any,
+    ops.CumulativeAll: ops.All,
+}
+
+
+def _cumulative_to_window(translator, expr, window):
+    win = ibis.cumulative_window()
+    win = (win.group_by(window._group_by)
+           .order_by(window._order_by))
+
+    op = expr.op()
+
+    klass = _cumulative_to_reduction[type(op)]
+    new_op = klass(*op.args)
+    new_expr = expr._factory(new_op, name=expr._name)
+
+    if type(new_op) in translator._rewrites:
+        new_expr = translator._rewrites[type(new_op)](new_expr)
+
+    new_expr = L.windowize_function(new_expr, win)
+    return new_expr
+
+
+def _window(translator, expr):
+    op = expr.op()
+
+    arg, window = op.args
+    window_op = arg.op()
+
+    _require_order_by = (ops.Lag,
+                         ops.Lead,
+                         ops.DenseRank,
+                         ops.MinRank,
+                         ops.FirstValue,
+                         ops.LastValue)
+
+    _unsupported_reductions = (
+        ops.CMSMedian,
+        ops.GroupConcat,
+        ops.HLLCardinality,
+    )
+
+    if isinstance(window_op, _unsupported_reductions):
+        raise com.TranslationError('{0!s} is not supported in '
+                                   'window functions'
+                                   .format(type(window_op)))
+
+    if isinstance(window_op, ops.CumulativeOp):
+        arg = _cumulative_to_window(translator, arg, window)
+        return translator.translate(arg)
+
+    # Some analytic functions need to have the expression of interest in
+    # the ORDER BY part of the window clause
+    if (isinstance(window_op, _require_order_by) and
+            len(window._order_by) == 0):
+        window = window.order_by(window_op.args[0])
+
+    window_formatted = _format_window(translator, window)
+
+    arg_formatted = translator.translate(arg)
+    result = '{0} {1}'.format(arg_formatted, window_formatted)
+
+    if type(window_op) in _expr_transforms:
+        return _expr_transforms[type(window_op)](result)
+    else:
+        return result
+
+
+def _format_window(translator, window):
+    components = []
+
+    if len(window._group_by) > 0:
+        partition_args = [translator.translate(x)
+                          for x in window._group_by]
+        components.append('PARTITION BY {0}'.format(', '.join(partition_args)))
+
+    if len(window._order_by) > 0:
+        order_args = []
+        for expr in window._order_by:
+            key = expr.op()
+            translated = translator.translate(key.expr)
+            if not key.ascending:
+                translated += ' DESC'
+            order_args.append(translated)
+
+        components.append('ORDER BY {0}'.format(', '.join(order_args)))
+
+    p, f = window.preceding, window.following
+
+    def _prec(p):
+        return '{0} PRECEDING'.format(p) if p > 0 else 'CURRENT ROW'
+
+    def _foll(f):
+        return '{0} FOLLOWING'.format(f) if f > 0 else 'CURRENT ROW'
+
+    if p is not None and f is not None:
+        frame = ('ROWS BETWEEN {0} AND {1}'
+                 .format(_prec(p), _foll(f)))
+    elif p is not None:
+        if isinstance(p, tuple):
+            start, end = p
+            frame = ('ROWS BETWEEN {0} AND {1}'
+                     .format(_prec(start), _prec(end)))
         else:
-            expr = expr.when(value, replacement)
+            kind = 'ROWS' if p > 0 else 'RANGE'
+            frame = ('{0} BETWEEN {1} AND UNBOUNDED FOLLOWING'
+                     .format(kind, _prec(p)))
+    elif f is not None:
+        if isinstance(f, tuple):
+            start, end = f
+            frame = ('ROWS BETWEEN {0} AND {1}'
+                     .format(_foll(start), _foll(end)))
+        else:
+            kind = 'ROWS' if f > 0 else 'RANGE'
+            frame = ('{0} BETWEEN UNBOUNDED PRECEDING AND {1}'
+                     .format(kind, _foll(f)))
+    else:
+        # no-op, default is full sample
+        frame = None
 
-        return expr.else_(else_ if else_ is not None else self).end()
+    if frame is not None:
+        components.append(frame)
 
-    def over(
-        self,
-        window=None,
-        *,
-        rows=None,
-        range=None,
-        group_by=None,
-        order_by=None,
-    ) -> Value:
-        """Construct a window expression.
-
-        Parameters
-        ----------
-        window
-            Window specification
-        rows
-            Whether to use the `ROWS` window clause
-        range
-            Whether to use the `RANGE` window clause
-        group_by
-            Grouping key
-        order_by
-            Ordering key
-
-        Returns
-        -------
-        Value
-            A window function expression
-        """
-        import ibis.expr.analysis as an
-        import ibis.expr.builders as bl
-        import ibis.expr.deferred as de
-
-        if window is None:
-            window = ibis.window(
-                rows=rows,
-                range=range,
-                group_by=group_by,
-                order_by=order_by,
-            )
-
-        def bind(table):
-            frame = window.bind(table)
-            return ops.WindowFunction(self, frame).to_expr()
-
-        op = self.op()
-        if isinstance(op, ops.Alias):
-            return op.arg.to_expr().over(window).name(op.name)
-        elif isinstance(op, ops.WindowFunction):
-            return op.func.to_expr().over(window)
-        elif isinstance(window, bl.WindowBuilder):
-            if table := an.find_first_base_table(self.op()):
-                return bind(table)
+    return 'OVER ({0})'.format(' '.join(components))
+
+
+def _shift_like(name):
+
+    def formatter(translator, expr):
+        op = expr.op()
+        arg, offset, default = op.args
+
+        arg_formatted = translator.translate(arg)
+
+        if default is not None:
+            if offset is None:
+                offset_formatted = '1'
             else:
-                return de.Deferred(bind)
+                offset_formatted = translator.translate(offset)
+
+            default_formatted = translator.translate(default)
+
+            return '{0}({1}, {2}, {3})'.format(name, arg_formatted,
+                                               offset_formatted,
+                                               default_formatted)
+        elif offset is not None:
+            offset_formatted = translator.translate(offset)
+            return '{0}({1}, {2})'.format(name, arg_formatted,
+                                          offset_formatted)
         else:
-            return ops.WindowFunction(self, window).to_expr()
+            return '{0}({1})'.format(name, arg_formatted)
 
-    def isnull(self) -> ir.BooleanValue:
-        """Return whether this expression is NULL."""
-        return ops.IsNull(self).to_expr()
-
-    def notnull(self) -> ir.BooleanValue:
-        """Return whether this expression is not NULL."""
-        return ops.NotNull(self).to_expr()
-
-    def case(self):
-        """Create a SimpleCaseBuilder to chain multiple if-else statements.
-
-        Add new search expressions with the `.when()` method. These must be
-        comparable with this column expression. Conclude by calling `.end()`
-
-        Returns
-        -------
-        SimpleCaseBuilder
-            A case builder
-
-        Examples
-        --------
-        >>> import ibis
-        >>> t = ibis.table([('string_col', 'string')], name='t')
-        >>> expr = t.string_col
-        >>> case_expr = (expr.case()
-        ...              .when('a', 'an a')
-        ...              .when('b', 'a b')
-        ...              .else_('null or (not a and not b)')
-        ...              .end())
-        >>> case_expr
-        r0 := UnboundTable: t
-          string_col string
-        SimpleCase(...)
-        """
-        import ibis.expr.builders as bl
+    return formatter
 
-        return bl.SimpleCaseBuilder(self.op())
 
-    def cases(
-        self,
-        case_result_pairs: Iterable[tuple[ir.BooleanValue, Value]],
-        default: Value | None = None,
-    ) -> Value:
-        """Create a case expression in one shot.
-
-        Parameters
-        ----------
-        case_result_pairs
-            Conditional-result pairs
-        default
-            Value to return if none of the case conditions are true
-
-        Returns
-        -------
-        Value
-            Value expression
-        """
-        builder = self.case()
-        for case, result in case_result_pairs:
-            builder = builder.when(case, result)
-        return builder.else_(default).end()
-
-    def collect(self, where: ir.BooleanValue | None = None) -> ir.ArrayScalar:
-        """Aggregate this expression's elements into an array.
-
-        This function is called `array_agg`, `list_agg`, or `list` in other systems.
-
-        Parameters
-        ----------
-        where
-            Filter to apply before aggregation
-
-        Returns
-        -------
-        ArrayScalar
-            Collected array
-
-        Examples
-        --------
-        Basic collect usage
-
-        >>> import ibis
-        >>> ibis.options.interactive = True
-        >>> t = ibis.memtable({"key": list("aaabb"), "value": [1, 2, 3, 4, 5]})
-        >>> t
-        ┏━━━━━━━━┳━━━━━━━┓
-        ┃ key    ┃ value ┃
-        ┡━━━━━━━━╇━━━━━━━┩
-        │ string │ int64 │
-        ├────────┼───────┤
-        │ a      │     1 │
-        │ a      │     2 │
-        │ a      │     3 │
-        │ b      │     4 │
-        │ b      │     5 │
-        └────────┴───────┘
-        >>> t.value.collect()
-        [1, 2, 3, 4, 5]
-        >>> type(t.value.collect())
-        <class 'ibis.expr.types.arrays.ArrayScalar'>
-
-        Collect elements per group
-
-        >>> t.group_by("key").agg(v=lambda t: t.value.collect())
-        ┏━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┓
-        ┃ key    ┃ v                    ┃
-        ┡━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━┩
-        │ string │ array<int64>         │
-        ├────────┼──────────────────────┤
-        │ a      │ [1, 2, ... +1]       │
-        │ b      │ [4, 5]               │
-        └────────┴──────────────────────┘
-
-        Collect elements per group using a filter
-
-        >>> t.group_by("key").agg(v=lambda t: t.value.collect(where=t.value > 1))
-        ┏━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┓
-        ┃ key    ┃ v                    ┃
-        ┡━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━┩
-        │ string │ array<int64>         │
-        ├────────┼──────────────────────┤
-        │ a      │ [2, 3]               │
-        │ b      │ [4, 5]               │
-        └────────┴──────────────────────┘
-        """
-        return ops.ArrayCollect(self, where=where).to_expr()
+def _nth_value(translator, expr):
+    op = expr.op()
+    arg, rank = op.args
 
-    def identical_to(self, other: Value) -> ir.BooleanValue:
-        """Return whether this expression is identical to other.
+    arg_formatted = translator.translate(arg)
+    rank_formatted = translator.translate(rank - 1)
 
-        Corresponds to `IS NOT DISTINCT FROM` in SQL.
+    return 'first_value(lag({0}, {1}))'.format(arg_formatted,
+                                               rank_formatted)
 
-        Parameters
-        ----------
-        other
-            Expression to compare to
-
-        Returns
-        -------
-        BooleanValue
-            Whether this expression is not distinct from `other`
-        """
-        try:
-            return ops.IdenticalTo(self, other).to_expr()
-        except (com.IbisTypeError, NotImplementedError):
-            return NotImplemented
-
-    def group_concat(
-        self,
-        sep: str = ",",
-        where: ir.BooleanValue | None = None,
-    ) -> ir.StringScalar:
-        """Concatenate values using the indicated separator to produce a string.
-
-        Parameters
-        ----------
-        sep
-            Separator will be used to join strings
-        where
-            Filter expression
-
-        Returns
-        -------
-        StringScalar
-            Concatenated string expression
-        """
-        return ops.GroupConcat(self, sep=sep, where=where).to_expr()
 
-    def __hash__(self) -> int:
-        return super().__hash__()
+def _negate(translator, expr):
+    arg = expr.op().args[0]
+    formatted_arg = translator.translate(arg)
+    if isinstance(expr, ir.BooleanValue):
+        return 'NOT {0!s}'.format(formatted_arg)
+    else:
+        if _needs_parens(arg):
+            formatted_arg = _parenthesize(formatted_arg)
+        return '-{0!s}'.format(formatted_arg)
 
-    def __eq__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.Equals, self, other)
 
-    def __ne__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.NotEquals, self, other)
+def _parenthesize(what):
+    return '({0!s})'.format(what)
 
-    def __ge__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.GreaterEqual, self, other)
 
-    def __gt__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.Greater, self, other)
+def unary(func_name):
+    return fixed_arity(func_name, 1)
 
-    def __le__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.LessEqual, self, other)
 
-    def __lt__(self, other: Value) -> ir.BooleanValue:
-        return _binop(ops.Less, self, other)
+def _reduction_format(translator, func_name, arg, where):
+    if where is not None:
+        case = where.ifelse(arg, ibis.NA)
+        arg = translator.translate(case)
+    else:
+        arg = translator.translate(arg)
 
-    def asc(self) -> ir.Value:
-        """Sort an expression ascending."""
-        return ops.SortKey(self, ascending=True).to_expr()
+    return '{0!s}({1!s})'.format(func_name, arg)
 
-    def desc(self) -> ir.Value:
-        """Sort an expression descending."""
-        return ops.SortKey(self, ascending=False).to_expr()
 
-    def as_table(self) -> ir.Table:
-        """Promote the expression to a table.
+def _reduction(func_name):
+    def formatter(translator, expr):
+        op = expr.op()
 
-        Returns
-        -------
-        Table
-            A table expression
+        # HACK: support trailing arguments
+        arg, where = op.args[:2]
 
-        Examples
-        --------
-        >>> t = ibis.table(dict(a="str"), name="t")
-        >>> expr = t.a.length().name("len").as_table()
-        >>> expected = t.select(len=t.a.length())
-        >>> expr.equals(expected)
-        True
-        """
-        from ibis.expr.analysis import find_immediate_parent_tables
+        return _reduction_format(translator, func_name, arg, where)
+    return formatter
 
-        roots = find_immediate_parent_tables(self.op())
-        if len(roots) > 1:
-            raise com.RelationError(
-                f'Cannot convert {type(self)} expression '
-                'involving multiple base table references '
-                'to a projection'
-            )
-        table = roots[0].to_expr()
-        return table.select(self)
-
-    def to_pandas(self, **kwargs) -> pd.Series:
-        """Convert a column expression to a pandas Series or scalar object.
-
-        Parameters
-        ----------
-        kwargs
-            Same as keyword arguments to [`execute`][ibis.expr.types.core.Expr.execute]
-        """
-        return self.execute(**kwargs)
 
+def _variance_like(func_name):
+    func_names = {
+        'sample': func_name,
+        'pop': '{0}_pop'.format(func_name)
+    }
 
-@public
-class Scalar(Value):
-    def __rich_console__(self, console, options):
-        from rich.text import Text
-
-        if not ibis.options.interactive:
-            return console.render(Text(self._repr()), options=options)
-        return console.render(repr(self.execute()), options=options)
-
-    def as_table(self) -> ir.Table:
-        """Promote the scalar expression to a table.
-
-        Returns
-        -------
-        Table
-            A table expression
-
-        Examples
-        --------
-        Promote an aggregation to a table
-
-        >>> import ibis
-        >>> import ibis.expr.types as ir
-        >>> t = ibis.table(dict(a="str"), name="t")
-        >>> expr = t.a.length().sum().name("len").as_table()
-        >>> isinstance(expr, ir.Table)
-        True
-
-        Promote a literal value to a table
-
-        >>> import ibis.expr.types as ir
-        >>> lit = ibis.literal(1).name("a").as_table()
-        >>> isinstance(lit, ir.Table)
-        True
-        """
-        from ibis.expr.analysis import (
-            find_first_base_table,
-            is_scalar_reduction,
-            reduction_to_aggregation,
-        )
-
-        op = self.op()
-        if is_scalar_reduction(op):
-            return reduction_to_aggregation(op)
-
-        table = find_first_base_table(op)
-        if table is not None:
-            agg = ops.Aggregation(table=table, metrics=(op,))
-        else:
-            agg = ops.DummyTable(values=(op,))
-        return agg.to_expr()
+    def formatter(translator, expr):
+        arg, where, how = expr.op().args
+        return _reduction_format(translator, func_names[how], arg, where)
+    return formatter
 
-    def _repr_html_(self) -> str | None:
-        return None
 
+def fixed_arity(func_name, arity):
 
-@public
-class Column(Value, _FixedTextJupyterMixin):
-    # Higher than numpy & dask objects
-    __array_priority__ = 20
+    def formatter(translator, expr):
+        op = expr.op()
+        if arity != len(op.args):
+            raise com.IbisError('incorrect number of args')
+        return _format_call(translator, func_name, *op.args)
 
-    __array_ufunc__ = None
+    return formatter
 
-    def __array__(self, dtype=None):
-        return self.execute().__array__(dtype)
 
-    def __rich_console__(self, console, options):
-        named = self.name(self.op().name)
-        projection = named.as_table()
-        return console.render(projection, options=options)
+def _ifnull_workaround(translator, expr):
+    op = expr.op()
+    a, b = op.args
 
-    def approx_nunique(
-        self,
-        where: ir.BooleanValue | None = None,
-    ) -> ir.IntegerScalar:
-        """Return the approximate number of distinct elements in `self`.
+    # work around per #345, #360
+    if (isinstance(a, ir.DecimalValue) and
+            isinstance(b, ir.IntegerValue)):
+        b = b.cast(a.type())
 
-        !!! info "The result may or may not be exact"
+    return _format_call(translator, 'isnull', a, b)
 
-            Whether the result is an approximation depends on the backend.
 
-            !!! warning "Do not depend on the results being exact"
+def _format_call(translator, func, *args):
+    formatted_args = []
+    for arg in args:
+        fmt_arg = translator.translate(arg)
+        formatted_args.append(fmt_arg)
 
-        Parameters
-        ----------
-        where
-            Filter in values when `where` is `True`
+    return '{0!s}({1!s})'.format(func, ', '.join(formatted_args))
 
-        Returns
-        -------
-        Scalar
-            An approximate count of the distinct elements of `self`
-        """
-        return ops.ApproxCountDistinct(self, where).to_expr()
 
-    def approx_median(
-        self,
-        where: ir.BooleanValue | None = None,
-    ) -> Scalar:
-        """Return an approximate of the median of `self`.
+def _binary_infix_op(infix_sym):
+    def formatter(translator, expr):
+        op = expr.op()
 
-        !!! info "The result may or may not be exact"
+        left, right = op.args
 
-            Whether the result is an approximation depends on the backend.
+        left_arg = translator.translate(left)
+        right_arg = translator.translate(right)
 
-            !!! warning "Do not depend on the results being exact"
+        if _needs_parens(left):
+            left_arg = _parenthesize(left_arg)
 
-        Parameters
-        ----------
-        where
-            Filter in values when `where` is `True`
+        if _needs_parens(right):
+            right_arg = _parenthesize(right_arg)
 
-        Returns
-        -------
-        Scalar
-            An approximation of the median of `self`
-        """
-        return ops.ApproxMedian(self, where).to_expr()
+        return '{0!s} {1!s} {2!s}'.format(left_arg, infix_sym, right_arg)
+    return formatter
 
-    def mode(self, where: ir.BooleanValue | None = None) -> Scalar:
-        """Return the mode of a column."""
-        return ops.Mode(self, where).to_expr()
-
-    def max(self, where: ir.BooleanValue | None = None) -> Scalar:
-        """Return the maximum of a column."""
-        return ops.Max(self, where).to_expr()
-
-    def min(self, where: ir.BooleanValue | None = None) -> Scalar:
-        """Return the minimum of a column."""
-        return ops.Min(self, where).to_expr()
-
-    def argmax(self, key: ir.Value, where: ir.BooleanValue | None = None) -> Scalar:
-        """Return the value of `self` that maximizes `key`."""
-        return ops.ArgMax(self, key=key, where=where).to_expr()
-
-    def argmin(self, key: ir.Value, where: ir.BooleanValue | None = None) -> Scalar:
-        """Return the value of `self` that minimizes `key`."""
-        return ops.ArgMin(self, key=key, where=where).to_expr()
-
-    def nunique(self, where: ir.BooleanValue | None = None) -> ir.IntegerScalar:
-        """Compute the number of distinct rows in an expression.
-
-        Parameters
-        ----------
-        where
-            Filter expression
-
-        Returns
-        -------
-        IntegerScalar
-            Number of distinct elements in an expression
-        """
-        return ops.CountDistinct(self, where).to_expr()
 
-    def topk(
-        self,
-        k: int,
-        by: ir.Value | None = None,
-    ) -> ir.TopK:
-        """Return a "top k" expression.
-
-        Parameters
-        ----------
-        k
-            Return this number of rows
-        by
-            An expression. Defaults to `count`.
-
-        Returns
-        -------
-        TableExpr
-            A top-k expression
-        """
+def _xor(translator, expr):
+    op = expr.op()
 
-        from ibis.expr.analysis import find_first_base_table
+    left_arg = translator.translate(op.left)
+    right_arg = translator.translate(op.right)
 
-        arg_table = find_first_base_table(self.op()).to_expr()
+    if _needs_parens(op.left):
+        left_arg = _parenthesize(left_arg)
 
-        if by is None:
-            by = self.count().name("count")
+    if _needs_parens(op.right):
+        right_arg = _parenthesize(right_arg)
 
-        if callable(by):
-            by = by(arg_table)
-            by_table = arg_table
-        elif isinstance(by, Value):
-            by_table = find_first_base_table(by.op()).to_expr()
-        else:
-            raise com.IbisTypeError(f"Invalid `by` argument with type {type(by)}")
+    return ('{0} AND NOT {1}'
+            .format('({0} {1} {2})'.format(left_arg, 'OR', right_arg),
+                    '({0} {1} {2})'.format(left_arg, 'AND', right_arg)))
 
-        assert by.op().name != self.op().name
 
-        if not arg_table.equals(by_table):
-            raise com.IbisError('Cross-table TopK; must provide a parent joined table')
+def _name_expr(formatted_expr, quoted_name):
+    return '{0!s} AS {1!s}'.format(formatted_expr, quoted_name)
 
-        return (
-            arg_table.aggregate(by, by=[self])
-            .order_by(ibis.desc(by.get_name()))
-            .limit(k)
-        )
-
-    @util.deprecated(
-        instead="Reach out at https://github.com/ibis-project/ibis if you'd like this API to remain.",
-        as_of="5.0",
-        removed_in="6.0",
-    )
-    def summary(
-        self,
-        exact_nunique: bool = False,
-        prefix: str = "",
-        suffix: str = "",
-    ) -> list[ir.NumericScalar]:
-        """Compute a set of summary metrics.
-
-        Parameters
-        ----------
-        exact_nunique
-            Compute the exact number of distinct values. Typically slower if
-            `True`.
-        prefix
-            String prefix for metric names
-        suffix
-            String suffix for metric names
-
-        Returns
-        -------
-        list[NumericScalar]
-            Metrics list
-        """
-        if exact_nunique:
-            unique_metric = self.nunique()
-        else:
-            unique_metric = self.approx_nunique()
-        unique_metric = unique_metric.name("uniques")
 
-        metrics = [
-            self.count().name("count"),
-            self.isnull().sum().name('nulls'),
-            unique_metric,
-        ]
-        metrics = [m.name(f"{prefix}{m.get_name()}{suffix}") for m in metrics]
-
-        return metrics
-
-    def arbitrary(
-        self,
-        where: ir.BooleanValue | None = None,
-        how: Literal["first", "last", "heavy"] = "first",
-    ) -> Scalar:
-        """Select an arbitrary value in a column.
-
-        Parameters
-        ----------
-        where
-            A filter expression
-        how
-            The method to use for selecting the element.
-
-            * `"first"`: Select the first non-`NULL` element
-            * `"last"`: Select the last non-`NULL` element
-            * `"heavy"`: Select a frequently occurring value using the heavy
-              hitters algorithm. `"heavy"` is only supported by Clickhouse
-              backend.
-
-        Returns
-        -------
-        Scalar
-            An expression
-        """
-        return ops.Arbitrary(self, how=how, where=where).to_expr()
+def _needs_parens(op):
+    if isinstance(op, ir.Expr):
+        op = op.op()
+    op_klass = type(op)
+    # function calls don't need parens
+    return (op_klass in _binary_infix_ops or
+            op_klass in [ops.Negate])
 
-    def count(self, where: ir.BooleanValue | None = None) -> ir.IntegerScalar:
-        """Compute the number of rows in an expression.
 
-        Parameters
-        ----------
-        where
-            Filter expression
-
-        Returns
-        -------
-        IntegerScalar
-            Number of elements in an expression
-        """
-        return ops.Count(self, where).to_expr()
+def _need_parenthesize_args(op):
+    if isinstance(op, ir.Expr):
+        op = op.op()
+    op_klass = type(op)
+    return (op_klass in _binary_infix_ops or
+            op_klass in [ops.Negate])
 
-    def value_counts(self) -> ir.Table:
-        """Compute a frequency table.
 
-        Returns
-        -------
-        Table
-            Frequency table expression
-
-        Examples
-        --------
-        >>> import ibis
-        >>> ibis.options.interactive = True
-        >>> t = ibis.memtable({"chars": char} for char in "aabcddd")
-        >>> t
-        ┏━━━━━━━━┓
-        ┃ chars  ┃
-        ┡━━━━━━━━┩
-        │ string │
-        ├────────┤
-        │ a      │
-        │ a      │
-        │ b      │
-        │ c      │
-        │ d      │
-        │ d      │
-        │ d      │
-        └────────┘
-        >>> t.chars.value_counts()
-        ┏━━━━━━━━┳━━━━━━━━━━━━━┓
-        ┃ chars  ┃ chars_count ┃
-        ┡━━━━━━━━╇━━━━━━━━━━━━━┩
-        │ string │ int64       │
-        ├────────┼─────────────┤
-        │ a      │           2 │
-        │ b      │           1 │
-        │ c      │           1 │
-        │ d      │           3 │
-        └────────┴─────────────┘
-        """
-        from ibis.expr.analysis import find_first_base_table
+def _boolean_literal_format(expr):
+    value = expr.op().value
+    return 'TRUE' if value else 'FALSE'
 
-        name = self.get_name()
-        return (
-            find_first_base_table(self.op())
-            .to_expr()
-            .select(self)
-            .group_by(name)
-            .agg(**{f"{name}_count": lambda t: t.count()})
-        )
 
-    def first(self) -> Column:
-        """Return the first value of a column.
+def _number_literal_format(expr):
+    value = expr.op().value
+    return repr(value)
 
-        Equivalent to SQL's `FIRST_VALUE` window function.
-        """
-        return ops.FirstValue(self).to_expr()
 
-    def last(self) -> Column:
-        """Return the last value of a column.
+def _string_literal_format(expr):
+    value = expr.op().value
+    return "'{0!s}'".format(value.replace("'", "\\'"))
 
-        Equivalent to SQL's `LAST_VALUE` window function.
-        """
-        return ops.LastValue(self).to_expr()
 
-    def rank(self) -> ir.IntegerColumn:
-        """Compute position of first element within each equal-value group in sorted order.
+def _timestamp_literal_format(expr):
+    value = expr.op().value
+    if isinstance(value, datetime.datetime):
+        if value.microsecond != 0:
+            raise ValueError(value)
+        value = value.strftime('%Y-%m-%d %H:%M:%S')
 
-        Equivalent to SQL's `RANK()` window function.
+    return "'{0!s}'".format(value)
 
-        Examples
-        --------
-        values   ranks
-        1        0
-        1        0
-        2        2
-        2        2
-        2        2
-        3        5
-
-        Returns
-        -------
-        Int64Column
-            The min rank
-        """
-        return ops.MinRank(self).to_expr()
 
-    def dense_rank(self) -> ir.IntegerColumn:
-        """Position of first element within each group of equal values.
+def quote_identifier(name, quotechar='`', force=False):
+    if force or name.count(' ') or name in identifiers.impala_identifiers:
+        return '{0}{1}{0}'.format(quotechar, name)
+    else:
+        return name
 
-        Values are returned in sorted order and duplicate values are ignored.
 
-        Equivalent to SQL's `DENSE_RANK()`.
+class CaseFormatter(object):
 
-        Examples
-        --------
-        values   ranks
-        1        0
-        1        0
-        2        1
-        2        1
-        2        1
-        3        2
-
-        Returns
-        -------
-        IntegerColumn
-            The rank
-        """
-        return ops.DenseRank(self).to_expr()
+    def __init__(self, translator, base, cases, results, default):
+        self.translator = translator
+        self.base = base
+        self.cases = cases
+        self.results = results
+        self.default = default
 
-    def percent_rank(self) -> Column:
-        """Return the relative rank of the values in the column."""
-        return ops.PercentRank(self).to_expr()
-
-    def cume_dist(self) -> Column:
-        """Return the cumulative distribution over a window."""
-        return ops.CumeDist(self).to_expr()
-
-    def cummin(self) -> Column:
-        """Return the cumulative min over a window."""
-        return ops.CumulativeMin(self).to_expr()
-
-    def cummax(self) -> Column:
-        """Return the cumulative max over a window."""
-        return ops.CumulativeMax(self).to_expr()
-
-    def lag(
-        self,
-        offset: int | ir.IntegerValue | None = None,
-        default: Value | None = None,
-    ) -> Column:
-        """Return the row located at `offset` rows **before** the current row.
-
-        Parameters
-        ----------
-        offset
-            Index of row to select
-        default
-            Value used if no row exists at `offset`
-        """
-        return ops.Lag(self, offset, default).to_expr()
+        # HACK
+        self.indent = 2
+        self.multiline = len(cases) > 1
+        self.buf = StringIO()
 
-    def lead(
-        self,
-        offset: int | ir.IntegerValue | None = None,
-        default: Value | None = None,
-    ) -> Column:
-        """Return the row located at `offset` rows **after** the current row.
-
-        Parameters
-        ----------
-        offset
-            Index of row to select
-        default
-            Value used if no row exists at `offset`
-        """
-        return ops.Lead(self, offset, default).to_expr()
+    def _trans(self, expr):
+        return self.translator.translate(expr)
 
-    def ntile(self, buckets: int | ir.IntegerValue) -> ir.IntegerColumn:
-        """Return the integer number of a partitioning of the column values.
+    def get_result(self):
+        self.buf.seek(0)
 
-        Parameters
-        ----------
-        buckets
-            Number of buckets to partition into
-        """
-        return ops.NTile(self, buckets).to_expr()
+        self.buf.write('CASE')
+        if self.base is not None:
+            base_str = self._trans(self.base)
+            self.buf.write(' {0}'.format(base_str))
 
-    def nth(self, n: int | ir.IntegerValue) -> Column:
-        """Return the `n`th value (0-indexed) over a window.
+        for case, result in zip(self.cases, self.results):
+            self._next_case()
+            case_str = self._trans(case)
+            result_str = self._trans(result)
+            self.buf.write('WHEN {0} THEN {1}'.format(case_str, result_str))
 
-        `.nth(0)` is equivalent to `.first()`. Negative will result in `NULL`.
-        If the value of `n` is greater than the number of rows in the window,
-        `NULL` will be returned.
-
-        Parameters
-        ----------
-        n
-            Desired rank value
-
-        Returns
-        -------
-        Column
-            The nth value over a window
-        """
-        return ops.NthValue(self, n).to_expr()
+        if self.default is not None:
+            self._next_case()
+            default_str = self._trans(self.default)
+            self.buf.write('ELSE {0}'.format(default_str))
 
+        if self.multiline:
+            self.buf.write('\nEND')
+        else:
+            self.buf.write(' END')
 
-@public
-class UnknownValue(Value):
-    pass
+        return self.buf.getvalue()
 
+    def _next_case(self):
+        if self.multiline:
+            self.buf.write('\n{0}'.format(' ' * self.indent))
+        else:
+            self.buf.write(' ')
 
-@public
-class UnknownScalar(Scalar):
-    pass
 
+def _simple_case(translator, expr):
+    op = expr.op()
+    formatter = CaseFormatter(translator, op.base, op.cases, op.results,
+                              op.default)
+    return formatter.get_result()
 
-@public
-class UnknownColumn(Column):
-    pass
 
+def _searched_case(translator, expr):
+    op = expr.op()
+    formatter = CaseFormatter(translator, None, op.cases, op.results,
+                              op.default)
+    return formatter.get_result()
 
-@public
-class NullValue(Value):
-    pass
 
+def _table_array_view(translator, expr):
+    ctx = translator.context
+    table = expr.op().table
+    query = ctx.get_compiled_expr(table)
+    return '(\n{0}\n)'.format(util.indent(query, ctx.indent))
 
-@public
-class NullScalar(Scalar, NullValue, Singleton):
-    pass
 
+# ---------------------------------------------------------------------
+# Timestamp arithmetic and other functions
 
-@public
-class NullColumn(Column, NullValue):
-    pass
+def _timestamp_delta(translator, expr):
+    op = expr.op()
+    arg, offset = op.args
+    formatted_arg = translator.translate(arg)
+    return _timestamp_format_offset(offset, formatted_arg)
 
 
-@public
-def null():
-    """Create a NULL/NA scalar."""
-    return ops.NullLiteral().to_expr()
+_impala_delta_functions = {
+    tempo.Year: 'years_add',
+    tempo.Month: 'months_add',
+    tempo.Week: 'weeks_add',
+    tempo.Day: 'days_add',
+    tempo.Hour: 'hours_add',
+    tempo.Minute: 'minutes_add',
+    tempo.Second: 'seconds_add',
+    tempo.Millisecond: 'milliseconds_add',
+    tempo.Microsecond: 'microseconds_add',
+    tempo.Nanosecond: 'nanoseconds_add'
+}
 
 
-@public
-def literal(value: Any, type: dt.DataType | str | None = None) -> Scalar:
-    """Create a scalar expression from a Python value.
+def _timestamp_format_offset(offset, arg):
+    f = _impala_delta_functions[type(offset)]
+    return '{0}({1}, {2})'.format(f, arg, offset.n)
 
-    !!! tip "Use specific functions for arrays, structs and maps"
 
-        Ibis supports literal construction of arrays using the following
-        functions:
+# ---------------------------------------------------------------------
+# Semi/anti-join supports
 
-        1. [`ibis.array`][ibis.array]
-        1. [`ibis.struct`][ibis.struct]
-        1. [`ibis.map`][ibis.map]
 
-        Constructing these types using `literal` will be deprecated in a future
-        release.
+def _exists_subquery(translator, expr):
+    op = expr.op()
+    ctx = translator.context
 
-    Parameters
-    ----------
-    value
-        A Python value
-    type
-        An instance of [`DataType`][ibis.expr.datatypes.DataType] or a string
-        indicating the ibis type of `value`. This parameter can be used
-        in cases where ibis's type inference isn't sufficient for discovering
-        the type of `value`.
+    expr = (op.foreign_table
+            .filter(op.predicates)
+            .projection([ir.literal(1).name(ir.unnamed)]))
 
-    Returns
-    -------
-    Scalar
-        An expression representing a literal value
+    subquery = ctx.get_compiled_expr(expr)
 
-    Examples
-    --------
-    Construct an integer literal
+    if isinstance(op, transforms.ExistsSubquery):
+        key = 'EXISTS'
+    elif isinstance(op, transforms.NotExistsSubquery):
+        key = 'NOT EXISTS'
+    else:
+        raise NotImplementedError
 
-    >>> import ibis
-    >>> x = ibis.literal(42)
-    >>> x.type()
-    Int8(nullable=True)
+    return '{0} (\n{1}\n)'.format(key, util.indent(subquery, ctx.indent))
 
-    Construct a `float64` literal from an `int`
 
-    >>> y = ibis.literal(42, type='double')
-    >>> y.type()
-    Float64(nullable=True)
+def _table_column(translator, expr):
+    op = expr.op()
+    field_name = op.name
+    quoted_name = quote_identifier(field_name, force=True)
 
-    Ibis checks for invalid types
+    table = op.table
+    ctx = translator.context
 
-    >>> ibis.literal('foobar', type='int64')  # doctest: +ELLIPSIS
-    Traceback (most recent call last):
-      ...
-    TypeError: Value 'foobar' cannot be safely coerced to int64
-    """
-    import ibis.expr.rules as rlz
+    # If the column does not originate from the table set in the current SELECT
+    # context, we should format as a subquery
+    if translator.permit_subquery and ctx.is_foreign_expr(table):
+        proj_expr = table.projection([field_name]).to_array()
+        return _table_array_view(translator, proj_expr)
+
+    if ctx.need_aliases():
+        alias = ctx.get_ref(table)
+        if alias is not None:
+            quoted_name = '{0}.{1}'.format(alias, quoted_name)
+
+    return quoted_name
+
+
+def _extract_field(sql_attr):
+    def extract_field_formatter(translator, expr):
+        op = expr.op()
+        arg = translator.translate(op.args[0])
 
-    if isinstance(value, Expr):
-        value = value.op()
+        # This is pre-2.0 Impala-style, which did not used to support the
+        # SQL-99 format extract($FIELD from expr)
+        return "extract({0!s}, '{1!s}')".format(arg, sql_attr)
+    return extract_field_formatter
 
-    return rlz.literal(type, value).to_expr()
 
+def _truncate(translator, expr):
+    op = expr.op()
 
-public(
-    ValueExpr=Value,
-    ScalarExpr=Scalar,
-    ColumnExpr=Column,
-    AnyValue=Value,
-    AnyScalar=Scalar,
-    AnyColumn=Column,
-)
+    arg = translator.translate(op.args[0])
+
+    _impala_unit_names = {
+        'M': 'MONTH',
+        'D': 'J',
+        'J': 'D',
+        'H': 'HH'
+    }
+
+    unit = op.args[1]
+    unit = _impala_unit_names.get(unit, unit)
+
+    return "trunc({0!s}, '{1!s}')".format(arg, unit)
+
+
+def _timestamp_from_unix(translator, expr):
+    op = expr.op()
+
+    val, unit = op.args
+
+    if unit == 'ms':
+        val = (val / 1000).cast('int32')
+    elif unit == 'us':
+        val = (val / 1000000).cast('int32')
+
+    arg = _from_unixtime(translator, val)
+    return 'CAST({0} AS timestamp)'.format(arg)
+
+
+def _from_unixtime(translator, expr):
+    arg = translator.translate(expr)
+    return 'from_unixtime({0}, "yyyy-MM-dd HH:mm:ss")'.format(arg)
+
+
+def varargs(func_name):
+    def varargs_formatter(translator, expr):
+        op = expr.op()
+        return _format_call(translator, func_name, *op.args)
+    return varargs_formatter
+
+
+def _substring(translator, expr):
+    op = expr.op()
+    arg, start, length = op.args
+    arg_formatted = translator.translate(arg)
+    start_formatted = translator.translate(start)
+
+    # Impala is 1-indexed
+    if length is None or isinstance(length.op(), ir.Literal):
+        lvalue = length.op().value if length else None
+        if lvalue:
+            return 'substr({0}, {1} + 1, {2})'.format(arg_formatted,
+                                                      start_formatted,
+                                                      lvalue)
+        else:
+            return 'substr({0}, {1} + 1)'.format(arg_formatted,
+                                                 start_formatted)
+    else:
+        length_formatted = translator.translate(length)
+        return 'substr({0}, {1} + 1, {2})'.format(arg_formatted,
+                                                  start_formatted,
+                                                  length_formatted)
+
+
+def _string_find(translator, expr):
+    op = expr.op()
+    arg, substr, start, _ = op.args
+    arg_formatted = translator.translate(arg)
+    substr_formatted = translator.translate(substr)
+
+    if start and not isinstance(start.op(), ir.Literal):
+        start_fmt = translator.translate(start)
+        return 'locate({0}, {1}, {2} + 1) - 1'.format(substr_formatted,
+                                                      arg_formatted,
+                                                      start_fmt)
+    elif start and start.op().value:
+        sval = start.op().value
+        return 'locate({0}, {1}, {2}) - 1'.format(substr_formatted,
+                                                  arg_formatted,
+                                                  sval + 1)
+    else:
+        return 'locate({0}, {1}) - 1'.format(substr_formatted, arg_formatted)
+
+
+def _string_join(translator, expr):
+    op = expr.op()
+    arg, strings = op.args
+    return _format_call(translator, 'concat_ws', arg, *strings)
+
+
+def _parse_url(translator, expr):
+    op = expr.op()
+
+    arg, extract, key = op.args
+    arg_formatted = translator.translate(arg)
+
+    if key is None:
+        return "parse_url({0}, '{1}')".format(arg_formatted, extract)
+    else:
+        key_fmt = translator.translate(key)
+        return "parse_url({0}, '{1}', {2})".format(arg_formatted,
+                                                   extract, key_fmt)
+
+
+def _find_in_set(translator, expr):
+    op = expr.op()
+
+    arg, str_list = op.args
+    arg_formatted = translator.translate(arg)
+    str_formatted = ','.join([x._arg.value for x in str_list])
+    return "find_in_set({0}, '{1}') - 1".format(arg_formatted, str_formatted)
+
+
+def _round(translator, expr):
+    op = expr.op()
+    arg, digits = op.args
+
+    arg_formatted = translator.translate(arg)
+
+    if digits is not None:
+        digits_formatted = translator.translate(digits)
+        return 'round({0}, {1})'.format(arg_formatted,
+                                        digits_formatted)
+    else:
+        return 'round({0})'.format(arg_formatted)
+
+
+def _hash(translator, expr):
+    op = expr.op()
+    arg, how = op.args
+
+    arg_formatted = translator.translate(arg)
+
+    if how == 'fnv':
+        return 'fnv_hash({0})'.format(arg_formatted)
+    else:
+        raise NotImplementedError(how)
+
+
+def _log(translator, expr):
+    op = expr.op()
+    arg, base = op.args
+    arg_formatted = translator.translate(arg)
+
+    if base is None:
+        return 'ln({0})'.format(arg_formatted)
+    else:
+        return 'log({0}, {1})'.format(arg_formatted,
+                                      translator.translate(base))
+
+
+def _count_distinct(translator, expr):
+    op = expr.op()
+    arg_formatted = translator.translate(op.args[0])
+    return 'COUNT(DISTINCT {0})'.format(arg_formatted)
+
+
+def _literal(translator, expr):
+    if isinstance(expr, ir.BooleanValue):
+        typeclass = 'boolean'
+    elif isinstance(expr, ir.StringValue):
+        typeclass = 'string'
+    elif isinstance(expr, ir.NumericValue):
+        typeclass = 'number'
+    elif isinstance(expr, ir.TimestampValue):
+        typeclass = 'timestamp'
+    else:
+        raise NotImplementedError
+
+    return _literal_formatters[typeclass](expr)
+
+
+def _null_literal(translator, expr):
+    return 'NULL'
+
+
+_literal_formatters = {
+    'boolean': _boolean_literal_format,
+    'number': _number_literal_format,
+    'string': _string_literal_format,
+    'timestamp': _timestamp_literal_format
+}
+
+
+def _value_list(translator, expr):
+    op = expr.op()
+    formatted = [translator.translate(x) for x in op.values]
+    return '({0})'.format(', '.join(formatted))
+
+
+_subtract_one = '{0} - 1'.format
+
+
+_expr_transforms = {
+    ops.RowNumber: _subtract_one,
+    ops.DenseRank: _subtract_one,
+    ops.MinRank: _subtract_one,
+}
+
+
+_binary_infix_ops = {
+    # Binary operations
+    ops.Add: _binary_infix_op('+'),
+    ops.Subtract: _binary_infix_op('-'),
+    ops.Multiply: _binary_infix_op('*'),
+    ops.Divide: _binary_infix_op('/'),
+    ops.Power: fixed_arity('pow', 2),
+    ops.Modulus: _binary_infix_op('%'),
+
+    # Comparisons
+    ops.Equals: _binary_infix_op('='),
+    ops.NotEquals: _binary_infix_op('!='),
+    ops.GreaterEqual: _binary_infix_op('>='),
+    ops.Greater: _binary_infix_op('>'),
+    ops.LessEqual: _binary_infix_op('<='),
+    ops.Less: _binary_infix_op('<'),
+
+    # Boolean comparisons
+    ops.And: _binary_infix_op('AND'),
+    ops.Or: _binary_infix_op('OR'),
+    ops.Xor: _xor,
+}
+
+
+_operation_registry = {
+    # Unary operations
+    ops.NotNull: _not_null,
+    ops.IsNull: _is_null,
+    ops.Negate: _negate,
+
+    ops.IfNull: _ifnull_workaround,
+    ops.NullIf: fixed_arity('nullif', 2),
+
+    ops.ZeroIfNull: unary('zeroifnull'),
+    ops.NullIfZero: unary('nullifzero'),
+
+    ops.Abs: unary('abs'),
+    ops.BaseConvert: fixed_arity('conv', 3),
+    ops.Ceil: unary('ceil'),
+    ops.Floor: unary('floor'),
+    ops.Exp: unary('exp'),
+    ops.Round: _round,
+
+    ops.Sign: unary('sign'),
+    ops.Sqrt: unary('sqrt'),
+
+    ops.Hash: _hash,
+
+    ops.Log: _log,
+    ops.Ln: unary('ln'),
+    ops.Log2: unary('log2'),
+    ops.Log10: unary('log10'),
+
+    ops.DecimalPrecision: unary('precision'),
+    ops.DecimalScale: unary('scale'),
+
+    # Unary aggregates
+    ops.CMSMedian: _reduction('appx_median'),
+    ops.HLLCardinality: _reduction('ndv'),
+    ops.Mean: _reduction('avg'),
+    ops.Sum: _reduction('sum'),
+    ops.Max: _reduction('max'),
+    ops.Min: _reduction('min'),
+
+    ops.StandardDev: _variance_like('stddev'),
+    ops.Variance: _variance_like('variance'),
+
+    ops.GroupConcat: fixed_arity('group_concat', 2),
+
+    ops.Count: _reduction('count'),
+    ops.CountDistinct: _count_distinct,
+
+    # string operations
+    ops.StringLength: unary('length'),
+    ops.StringAscii: unary('ascii'),
+    ops.Lowercase: unary('lower'),
+    ops.Uppercase: unary('upper'),
+    ops.Reverse: unary('reverse'),
+    ops.Strip: unary('trim'),
+    ops.LStrip: unary('ltrim'),
+    ops.RStrip: unary('rtrim'),
+    ops.Capitalize: unary('initcap'),
+    ops.Substring: _substring,
+    ops.StrRight: fixed_arity('strright', 2),
+    ops.Repeat: fixed_arity('repeat', 2),
+    ops.StringFind: _string_find,
+    ops.Translate: fixed_arity('translate', 3),
+    ops.FindInSet: _find_in_set,
+    ops.LPad: fixed_arity('lpad', 3),
+    ops.RPad: fixed_arity('rpad', 3),
+    ops.StringJoin: _string_join,
+    ops.StringSQLLike: _binary_infix_op('LIKE'),
+    ops.RegexSearch: _binary_infix_op('RLIKE'),
+    ops.RegexExtract: fixed_arity('regexp_extract', 3),
+    ops.RegexReplace: fixed_arity('regexp_replace', 3),
+    ops.ParseURL: _parse_url,
+
+    # Timestamp operations
+    ops.TimestampNow: lambda *args: 'now()',
+    ops.ExtractYear: _extract_field('year'),
+    ops.ExtractMonth: _extract_field('month'),
+    ops.ExtractDay: _extract_field('day'),
+    ops.ExtractHour: _extract_field('hour'),
+    ops.ExtractMinute: _extract_field('minute'),
+    ops.ExtractSecond: _extract_field('second'),
+    ops.ExtractMillisecond: _extract_field('millisecond'),
+    ops.Truncate: _truncate,
+
+    # Other operations
+    ops.E: lambda *args: 'e()',
+
+    ir.Literal: _literal,
+    ir.NullLiteral: _null_literal,
+
+    ir.ValueList: _value_list,
+
+    ops.Cast: _cast,
+
+    ops.Coalesce: varargs('coalesce'),
+    ops.Greatest: varargs('greatest'),
+    ops.Least: varargs('least'),
+
+    ops.Where: fixed_arity('if', 3),
+
+    ops.Between: _between,
+    ops.Contains: _binary_infix_op('IN'),
+    ops.NotContains: _binary_infix_op('NOT IN'),
+
+    ops.SimpleCase: _simple_case,
+    ops.SearchedCase: _searched_case,
+
+    ops.TableColumn: _table_column,
+
+    ops.TableArrayView: _table_array_view,
+
+    ops.TimestampDelta: _timestamp_delta,
+    ops.TimestampFromUNIX: _timestamp_from_unix,
+
+    transforms.ExistsSubquery: _exists_subquery,
+    transforms.NotExistsSubquery: _exists_subquery,
+
+    # RowNumber, and rank functions starts with 0 in Ibis-land
+    ops.RowNumber: lambda *args: 'row_number()',
+    ops.DenseRank: lambda *args: 'dense_rank()',
+    ops.MinRank: lambda *args: 'rank()',
+
+    ops.FirstValue: unary('first_value'),
+    ops.LastValue: unary('last_value'),
+    ops.NthValue: _nth_value,
+    ops.Lag: _shift_like('lag'),
+    ops.Lead: _shift_like('lead'),
+    ops.WindowOp: _window
+}
+
+_operation_registry.update(_binary_infix_ops)
+
+
+class ImpalaExprTranslator(comp.ExprTranslator):
+
+    _registry = _operation_registry
+    _context_class = ImpalaContext
+
+    def name(self, translated, name, force=True):
+        return _name_expr(translated,
+                          quote_identifier(name, force=force))
+
+compiles = ImpalaExprTranslator.compiles
+rewrites = ImpalaExprTranslator.rewrites
+
+
+@rewrites(ops.FloorDivide)
+def _floor_divide(expr):
+    left, right = expr.op().args
+    return left.div(right).floor()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ibis_framework-5.1.0/ibis/tests/__init__.py` & `ibis-framework-v0.6.0/ibis/tests/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 # Copyright 2015 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ibis_framework-5.1.0/ibis/tests/expr/test_analysis.py` & `ibis-framework-v0.6.0/ibis/expr/tests/test_analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,305 +1,269 @@
-import pytest
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import ibis
-import ibis.common.exceptions as com
-import ibis.expr.analysis as an
+
+from ibis.compat import unittest
+from ibis.expr.tests.mocks import BasicTestCase
+import ibis.expr.analysis as L
 import ibis.expr.operations as ops
+import ibis.common as com
+
 from ibis.tests.util import assert_equal
 
-# TODO: test is_reduction
-# TODO: test is_scalar_reduction
 
 # Place to collect esoteric expression analysis bugs and tests
 
 
-def test_rewrite_join_projection_without_other_ops(con):
-    # See #790, predicate pushdown in joins not supported
-
-    # Star schema with fact table
-    table = con.table('star1')
-    table2 = con.table('star2')
-    table3 = con.table('star3')
-
-    filtered = table[table['f'] > 0]
-
-    pred1 = table['foo_id'] == table2['foo_id']
-    pred2 = filtered['bar_id'] == table3['bar_id']
-
-    j1 = filtered.left_join(table2, [pred1])
-    j2 = j1.inner_join(table3, [pred2])
-
-    # Project out the desired fields
-    view = j2[[filtered, table2['value1'], table3['value2']]]
-
-    # Construct the thing we expect to obtain
-    ex_pred2 = table['bar_id'] == table3['bar_id']
-    ex_expr = table.left_join(table2, [pred1]).inner_join(table3, [ex_pred2])
-
-    rewritten_proj = an.substitute_parents(view.op())
-
-    assert not rewritten_proj.table.equals(ex_expr.op())
-
-
-def test_multiple_join_deeper_reference():
-    # Join predicates down the chain might reference one or more root
-    # tables in the hierarchy.
-    table1 = ibis.table({'key1': 'string', 'key2': 'string', 'value1': 'double'})
-    table2 = ibis.table({'key3': 'string', 'value2': 'double'})
-    table3 = ibis.table({'key4': 'string', 'value3': 'double'})
-
-    joined = table1.inner_join(table2, [table1['key1'] == table2['key3']])
-    joined2 = joined.inner_join(table3, [table1['key2'] == table3['key4']])
-
-    # it works, what more should we test here?
-    repr(joined2)
-
-
-def test_filter_on_projected_field(con):
-    # See #173. Impala and other SQL engines do not allow filtering on a
-    # just-created alias in a projection
-    region = con.table('tpch_region')
-    nation = con.table('tpch_nation')
-    customer = con.table('tpch_customer')
-    orders = con.table('tpch_orders')
-
-    fields_of_interest = [
-        customer,
-        region.r_name.name('region'),
-        orders.o_totalprice.name('amount'),
-        orders.o_orderdate.cast('timestamp').name('odate'),
-    ]
-
-    all_join = (
-        region.join(nation, region.r_regionkey == nation.n_regionkey)
-        .join(customer, customer.c_nationkey == nation.n_nationkey)
-        .join(orders, orders.o_custkey == customer.c_custkey)
-    )
-
-    tpch = all_join[fields_of_interest]
-
-    # Correlated subquery, yikes!
-    t2 = tpch.view()
-    conditional_avg = t2[(t2.region == tpch.region)].amount.mean()
-
-    # `amount` is part of the projection above as an aliased field
-    amount_filter = tpch.amount > conditional_avg
-
-    result = tpch.filter([amount_filter])
-
-    # Now then! Predicate pushdown here is inappropriate, so we check that
-    # it didn't occur.
-    assert isinstance(result.op(), ops.Selection)
-    assert result.op().table == tpch.op()
-
-
-def test_join_predicate_from_derived_raises():
-    # Join predicate references a derived table, but we can salvage and
-    # rewrite it to get the join semantics out
-    # see ibis #74
-    table = ibis.table([('c', 'int32'), ('f', 'double'), ('g', 'string')], 'foo_table')
-
-    table2 = ibis.table([('key', 'string'), ('value', 'double')], 'bar_table')
-
-    filter_pred = table['f'] > 0
-    table3 = table[filter_pred]
-
-    with pytest.raises(com.ExpressionError):
-        table.inner_join(table2, [table3['g'] == table2['key']])
-
-
-def test_bad_join_predicate_raises():
-    table = ibis.table([('c', 'int32'), ('f', 'double'), ('g', 'string')], 'foo_table')
-
-    table2 = ibis.table([('key', 'string'), ('value', 'double')], 'bar_table')
-
-    table3 = ibis.table([('key', 'string'), ('value', 'double')], 'baz_table')
-
-    with pytest.raises(com.ExpressionError):
-        table.inner_join(table2, [table['g'] == table3['key']])
-
-
-def test_filter_self_join():
-    # GH #667
-    purchases = ibis.table(
-        [
-            ('region', 'string'),
-            ('kind', 'string'),
-            ('user', 'int64'),
-            ('amount', 'double'),
-        ],
-        'purchases',
-    )
-
-    metric = purchases.amount.sum().name('total')
-    agged = purchases.group_by(['region', 'kind']).aggregate(metric)
-
-    left = agged[agged.kind == 'foo']
-    right = agged[agged.kind == 'bar']
-
-    cond = left.region == right.region
-    joined = left.join(right, cond)
-
-    metric = (left.total - right.total).name('diff')
-    what = [left.region, metric]
-    projected = joined.select(what)
-
-    proj_exprs = projected.op().selections
-
-    # proj exprs unaffected by analysis
-    assert_equal(proj_exprs[0], left.region.op())
-    assert_equal(proj_exprs[1], metric.op())
-
-
-def test_no_rewrite(con):
-    table = con.table('test1')
-    table4 = table[['c', (table['c'] * 2).name('foo')]]
-    expr = table4['c'] == table4['foo']
-    result = an.substitute_parents(expr.op()).to_expr()
-    expected = expr
-    assert result.equals(expected)
-
-
-def test_join_table_choice():
-    # GH807
-    x = ibis.table(ibis.schema([('n', 'int64')]), 'x')
-    t = x.aggregate(cnt=x.n.count())
-    predicate = t.cnt > 0
-
-    result = an.sub_for(predicate.op(), {t.op(): t.op().table})
-    assert result == predicate.op()
-
-
-def test_is_ancestor_analytic():
-    x = ibis.table(ibis.schema([('col', 'int32')]), 'x')
-    with_filter_col = x[x.columns + [ibis.null().name('filter')]]
-    filtered = with_filter_col[with_filter_col['filter'].isnull()]
-    subquery = filtered[filtered.columns]
-
-    with_analytic = subquery[subquery.columns + [subquery.count().name('analytic')]]
-
-    assert not subquery.op().equals(with_analytic.op())
-
-
-# Pr 2635
-def test_mutation_fusion_no_overwrite():
-    """Test fusion with chained mutation that doesn't overwrite existing
-    columns."""
-    t = ibis.table(ibis.schema([('col', 'int32')]), 't')
-
-    result = t
-    result = result.mutate(col1=t['col'] + 1)
-    result = result.mutate(col2=t['col'] + 2)
-    result = result.mutate(col3=t['col'] + 3)
-    result = result.op()
-
-    first_selection = result
-
-    assert len(result.selections) == 4
-
-    col1 = (t['col'] + 1).name('col1')
-    assert first_selection.selections[1] == col1.op()
-
-    col2 = (t['col'] + 2).name('col2')
-    assert first_selection.selections[2] == col2.op()
-
-    col3 = (t['col'] + 3).name('col3')
-    assert first_selection.selections[3] == col3.op()
-
-
-# Pr 2635
-def test_mutation_fusion_overwrite():
-    """Test fusion with chained mutation that overwrites existing columns."""
-    t = ibis.table(ibis.schema([('col', 'int32')]), 't')
-
-    result = t
-
-    result = result.mutate(col1=t['col'] + 1)
-    result = result.mutate(col2=t['col'] + 2)
-    result = result.mutate(col3=t['col'] + 3)
-    result = result.mutate(col=t['col'] - 1)
-    result = result.mutate(col4=t['col'] + 4)
-
-    second_selection = result.op()
-    first_selection = second_selection.table
-
-    assert len(first_selection.selections) == 4
-    col1 = (t['col'] + 1).name('col1').op()
-    assert first_selection.selections[1] == col1
-
-    col2 = (t['col'] + 2).name('col2').op()
-    assert first_selection.selections[2] == col2
-
-    col3 = (t['col'] + 3).name('col3').op()
-    assert first_selection.selections[3] == col3
-
-    # Since the second selection overwrites existing columns, it will
-    # not have the Table as the first selection
-    assert len(second_selection.selections) == 5
-
-    col = (t['col'] - 1).name('col').op()
-    assert second_selection.selections[0] == col
-
-    col1 = first_selection.to_expr()['col1'].op()
-    assert second_selection.selections[1] == col1
-
-    col2 = first_selection.to_expr()['col2'].op()
-    assert second_selection.selections[2] == col2
-
-    col3 = first_selection.to_expr()['col3'].op()
-    assert second_selection.selections[3] == col3
-
-    col4 = (t['col'] + 4).name('col4').op()
-    assert second_selection.selections[4] == col4
-
-
-# Pr 2635
-def test_select_filter_mutate_fusion():
-    """Test fusion with filter followed by mutation on the same input."""
-
-    t = ibis.table(ibis.schema([('col', 'float32')]), 't')
-
-    result = t[['col']]
-    result = result[result['col'].isnan()]
-    result = result.mutate(col=result['col'].cast('int32'))
-
-    second_selection = result.op()
-    first_selection = second_selection.table
-    assert len(second_selection.selections) == 1
-
-    col = first_selection.to_expr()['col'].cast('int32').name('col').op()
-    assert second_selection.selections[0] == col
-
-    # we don't look past the projection when a filter is encountered, so the
-    # number of selections in the first projection (`first_selection`) is 0
-    #
-    # previously we did, but this was buggy when executing against the pandas
-    # backend
-    #
-    # eventually we will bring this back, but we're trading off the ability
-    # to remove materialize for some performance in the short term
-    assert len(first_selection.selections) == 1
-    assert len(first_selection.predicates) == 1
-
-
-def test_no_filter_means_no_selection():
-    t = ibis.table(dict(a="string"))
-    proj = t.filter([])
-    assert proj.equals(t)
-
-
-def test_mutate_overwrites_existing_column():
-    t = ibis.table(dict(a="string"))
-    mut = t.mutate(a=42).select(["a"])
-    sel = mut.op().selections[0].table.selections[0].arg
-    assert isinstance(sel, ops.Literal)
-    assert sel.value == 42
-
-
-def test_agg_selection_does_not_share_roots():
-    t = ibis.table(dict(a="string"), name="t")
-    s = ibis.table(dict(b="float64"), name="s")
-    gb = t.group_by("a")
-    n = s.count()
+class TestTableExprBasics(BasicTestCase, unittest.TestCase):
 
-    with pytest.raises(com.RelationError, match="Selection expressions"):
-        gb.aggregate(n=n)
+    def test_rewrite_substitute_distinct_tables(self):
+        t = self.con.table('test1')
+        tt = self.con.table('test1')
+
+        expr = t[t.c > 0]
+        expr2 = tt[tt.c > 0]
+
+        metric = t.f.sum().name('metric')
+        expr3 = expr.aggregate(metric)
+
+        result = L.sub_for(expr3, [(expr2, t)])
+        expected = t.aggregate(metric)
+
+        assert_equal(result, expected)
+
+    def test_rewrite_join_projection_without_other_ops(self):
+        # Drop out filters and other commutative table operations. Join
+        # predicates are "lifted" to reference the base, unmodified join roots
+
+        # Star schema with fact table
+        table = self.con.table('star1')
+        table2 = self.con.table('star2')
+        table3 = self.con.table('star3')
+
+        filtered = table[table['f'] > 0]
+
+        pred1 = table['foo_id'] == table2['foo_id']
+        pred2 = filtered['bar_id'] == table3['bar_id']
+
+        j1 = filtered.left_join(table2, [pred1])
+        j2 = j1.inner_join(table3, [pred2])
+
+        # Project out the desired fields
+        view = j2[[filtered, table2['value1'], table3['value2']]]
+
+        # Construct the thing we expect to obtain
+        ex_pred2 = table['bar_id'] == table3['bar_id']
+        ex_expr = (table.left_join(table2, [pred1])
+                   .inner_join(table3, [ex_pred2]))
+
+        rewritten_proj = L.substitute_parents(view)
+        op = rewritten_proj.op()
+        assert_equal(op.table, ex_expr)
+
+        # Ensure that filtered table has been substituted with the base table
+        assert op.selections[0] is table
+
+    def test_rewrite_past_projection(self):
+        table = self.con.table('test1')
+
+        # Rewrite past a projection
+        table3 = table[['c', 'f']]
+        expr = table3['c'] == 2
+
+        result = L.substitute_parents(expr)
+        expected = table['c'] == 2
+        assert_equal(result, expected)
+
+        # Unsafe to rewrite past projection
+        table5 = table[(table.f * 2).name('c'), table.f]
+        expr = table5['c'] == 2
+        result = L.substitute_parents(expr)
+        assert result is expr
+
+    def test_rewrite_expr_with_parent(self):
+        table = self.con.table('test1')
+
+        table2 = table[table['f'] > 0]
+
+        expr = table2['c'] == 2
+
+        result = L.substitute_parents(expr)
+        expected = table['c'] == 2
+        assert_equal(result, expected)
+
+        # Substitution not fully possible if we depend on a new expr in a
+        # projection
+
+        table4 = table[['c', (table['c'] * 2).name('foo')]]
+        expr = table4['c'] == table4['foo']
+        result = L.substitute_parents(expr)
+        expected = table['c'] == table4['foo']
+        assert_equal(result, expected)
+
+    def test_rewrite_distinct_but_equal_objects(self):
+        t = self.con.table('test1')
+        t_copy = self.con.table('test1')
+
+        table2 = t[t_copy['f'] > 0]
+
+        expr = table2['c'] == 2
+
+        result = L.substitute_parents(expr)
+        expected = t['c'] == 2
+        assert_equal(result, expected)
+
+    def test_projection_with_join_pushdown_rewrite_refs(self):
+        # Observed this expression IR issue in a TopK-rewrite context
+        table1 = ibis.table([
+            ('a_key1', 'string'),
+            ('a_key2', 'string'),
+            ('a_value', 'double')
+        ], 'foo')
+
+        table2 = ibis.table([
+            ('b_key1', 'string'),
+            ('b_name', 'string'),
+            ('b_value', 'double')
+        ], 'bar')
+
+        table3 = ibis.table([
+            ('c_key2', 'string'),
+            ('c_name', 'string')
+        ], 'baz')
+
+        proj = (table1.inner_join(table2, [('a_key1', 'b_key1')])
+                .inner_join(table3, [(table1.a_key2, table3.c_key2)])
+                [table1, table2.b_name.name('b'), table3.c_name.name('c'),
+                 table2.b_value])
+
+        cases = [
+            (proj.a_value > 0, table1.a_value > 0),
+            (proj.b_value > 0, table2.b_value > 0)
+        ]
+
+        for higher_pred, lower_pred in cases:
+            result = proj.filter([higher_pred])
+            op = result.op()
+            assert isinstance(op, ops.Projection)
+            filter_op = op.table.op()
+            assert isinstance(filter_op, ops.Filter)
+            new_pred = filter_op.predicates[0]
+            assert_equal(new_pred, lower_pred)
+
+    def test_multiple_join_deeper_reference(self):
+        # Join predicates down the chain might reference one or more root
+        # tables in the hierarchy.
+        table1 = ibis.table({'key1': 'string', 'key2': 'string',
+                            'value1': 'double'})
+        table2 = ibis.table({'key3': 'string', 'value2': 'double'})
+        table3 = ibis.table({'key4': 'string', 'value3': 'double'})
+
+        joined = table1.inner_join(table2, [table1['key1'] == table2['key3']])
+        joined2 = joined.inner_join(table3, [table1['key2'] == table3['key4']])
+
+        # it works, what more should we test here?
+        materialized = joined2.materialize()
+        repr(materialized)
+
+    def test_filter_on_projected_field(self):
+        # See #173. Impala and other SQL engines do not allow filtering on a
+        # just-created alias in a projection
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+        customer = self.con.table('tpch_customer')
+        orders = self.con.table('tpch_orders')
+
+        fields_of_interest = [customer,
+                              region.r_name.name('region'),
+                              orders.o_totalprice.name('amount'),
+                              orders.o_orderdate
+                              .cast('timestamp').name('odate')]
+
+        all_join = (
+            region.join(nation, region.r_regionkey == nation.n_regionkey)
+            .join(customer, customer.c_nationkey == nation.n_nationkey)
+            .join(orders, orders.o_custkey == customer.c_custkey))
+
+        tpch = all_join[fields_of_interest]
+
+        # Correlated subquery, yikes!
+        t2 = tpch.view()
+        conditional_avg = t2[(t2.region == tpch.region)].amount.mean()
+
+        # `amount` is part of the projection above as an aliased field
+        amount_filter = tpch.amount > conditional_avg
+
+        result = tpch.filter([amount_filter])
+
+        # Now then! Predicate pushdown here is inappropriate, so we check that
+        # it didn't occur.
+
+        # If filter were pushed below projection, the top-level operator type
+        # would be Projection instead.
+        assert type(result.op()) == ops.Filter
+
+    def test_bad_join_predicate_raises(self):
+        # Join predicate references a derived table, but we can salvage and
+        # rewrite it to get the join semantics out
+        # see ibis #74
+        table = ibis.table([
+            ('c', 'int32'),
+            ('f', 'double'),
+            ('g', 'string')
+        ], 'foo_table')
+
+        table2 = ibis.table([
+            ('key', 'string'),
+            ('value', 'double')
+        ], 'bar_table')
+
+        filter_pred = table['f'] > 0
+        table3 = table[filter_pred]
+
+        with self.assertRaises(com.ExpressionError):
+            table.inner_join(table2, [table3['g'] == table2['key']])
+
+        # expected = table.inner_join(table2, [table['g'] == table2['key']])
+        # assert_equal(result, expected)
+
+    def test_filter_self_join(self):
+        # GH #667
+        purchases = ibis.table([('region', 'string'),
+                                ('kind', 'string'),
+                                ('user', 'int64'),
+                                ('amount', 'double')], 'purchases')
+
+        metric = purchases.amount.sum().name('total')
+        agged = (purchases.group_by(['region', 'kind'])
+                 .aggregate(metric))
+
+        left = agged[agged.kind == 'foo']
+        right = agged[agged.kind == 'bar']
+
+        cond = left.region == right.region
+        joined = left.join(right, cond)
+
+        # unmodified by analysis
+        assert_equal(joined.op().predicates[0], cond)
+
+        metric = (left.total - right.total).name('diff')
+        what = [left.region, metric]
+        projected = joined.projection(what)
+
+        proj_exprs = projected.op().selections
+
+        # proj exprs unaffected by analysis
+        assert_equal(proj_exprs[0], left.region)
+        assert_equal(proj_exprs[1], metric)
```

### Comparing `ibis_framework-5.1.0/ibis/tests/expr/test_interactive.py` & `ibis-framework-v0.6.0/ibis/expr/tests/test_interactive.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,105 +8,86 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
+from ibis.compat import unittest
+from ibis.expr.tests.mocks import MockConnection
+import ibis.config as config
 
-from ibis import config
-from ibis.tests.expr.mocks import MockBackend
 
+class TestInteractiveUse(unittest.TestCase):
 
-@pytest.fixture
-def con():
-    return MockBackend()
+    def setUp(self):
+        self.con = MockConnection()
 
+    def test_interactive_execute_on_repr(self):
+        table = self.con.table('functional_alltypes')
+        expr = table.bigint_col.sum()
+        with config.option_context('interactive', True):
+            repr(expr)
 
-def test_interactive_execute_on_repr(con):
-    table = con.table('functional_alltypes')
-    expr = table.bigint_col.sum()
-    with config.option_context('interactive', True):
-        repr(expr)
+        assert len(self.con.executed_queries) > 0
 
-    assert len(con.executed_queries) > 0
+    def test_default_limit(self):
+        table = self.con.table('functional_alltypes')
 
-
-def test_repr_png_is_none_in_interactive(con):
-    table = con.table('functional_alltypes')
-
-    with config.option_context('interactive', True):
-        assert table._repr_png_() is None
-
-
-def test_repr_png_is_not_none_in_not_interactive(con):
-    pytest.importorskip('ibis.expr.visualize')
-
-    table = con.table('functional_alltypes')
-
-    with config.option_context('interactive', False), config.option_context(
-        'graphviz_repr', True
-    ):
-        assert table._repr_png_() is not None
-
-
-def test_default_limit(con, snapshot):
-    table = con.table('functional_alltypes').select("id", "bool_col")
-
-    with config.option_context('interactive', True):
-        repr(table)
-
-    snapshot.assert_match(con.executed_queries[0], "out.sql")
-
-
-def test_respect_set_limit(con, snapshot):
-    table = con.table('functional_alltypes').select("id", "bool_col").limit(10)
-
-    with config.option_context('interactive', True):
-        repr(table)
-
-    snapshot.assert_match(con.executed_queries[0], "out.sql")
-
-
-def test_disable_query_limit(con, snapshot):
-    table = con.table('functional_alltypes').select("id", "bool_col")
-
-    with config.option_context('interactive', True):
-        with config.option_context('sql.default_limit', None):
+        with config.option_context('interactive', True):
             repr(table)
 
-    snapshot.assert_match(con.executed_queries[0], "out.sql")
-
+        expected = """\
+SELECT *
+FROM functional_alltypes
+LIMIT {0}""".format(config.options.sql.default_limit)
 
-def test_interactive_non_compilable_repr_not_fail(con):
-    # #170
-    table = con.table('functional_alltypes')
+        assert self.con.executed_queries[0] == expected
 
-    expr = table.string_col.topk(3)
-
-    # it works!
-    with config.option_context('interactive', True):
-        repr(expr)
-
-
-def test_histogram_repr_no_query_execute(con):
-    t = con.table('functional_alltypes')
-    tier = t.double_col.histogram(10).name('bucket')
-    expr = t.group_by(tier).size()
-    with config.option_context('interactive', True):
-        expr._repr()
-    assert con.executed_queries == []
-
-
-def test_compile_no_execute(con):
-    t = con.table('functional_alltypes')
-    t.double_col.sum().compile()
-    assert con.executed_queries == []
+    def test_respect_set_limit(self):
+        table = self.con.table('functional_alltypes').limit(10)
 
+        with config.option_context('interactive', True):
+            repr(table)
 
-def test_isin_rule_supressed_exception_repr_not_fail(con):
-    with config.option_context('interactive', True):
-        t = con.table('functional_alltypes')
-        bool_clause = t['string_col'].notin(['1', '4', '7'])
-        expr = t[bool_clause]['string_col'].value_counts()
-        repr(expr)
+        expected = """\
+SELECT *
+FROM functional_alltypes
+LIMIT 10"""
+
+        assert self.con.executed_queries[0] == expected
+
+    def test_disable_query_limit(self):
+        table = self.con.table('functional_alltypes')
+
+        with config.option_context('interactive', True):
+            with config.option_context('sql.default_limit', None):
+                repr(table)
+
+        expected = """\
+SELECT *
+FROM functional_alltypes"""
+
+        assert self.con.executed_queries[0] == expected
+
+    def test_interactive_non_compilable_repr_not_fail(self):
+        # #170
+        table = self.con.table('functional_alltypes')
+
+        expr = table.string_col.topk(3)
+
+        # it works!
+        with config.option_context('interactive', True):
+            repr(expr)
+
+    def test_histogram_repr_no_query_execute(self):
+        t = self.con.table('functional_alltypes')
+        tier = t.double_col.histogram(10).name('bucket')
+        expr = t.group_by(tier).size()
+        with config.option_context('interactive', True):
+            expr._repr()
+        assert self.con.executed_queries == []
+
+    def test_compile_no_execute(self):
+        t = self.con.table('functional_alltypes')
+        t.double_col.sum().compile()
+        assert self.con.executed_queries == []
```

### Comparing `ibis_framework-5.1.0/ibis/tests/expr/test_pipe.py` & `ibis-framework-v0.6.0/ibis/expr/tests/test_pipe.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,53 +8,52 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-
+from ibis.compat import unittest
 import ibis
 
 
-@pytest.fixture
-def pipe_table():
-    return ibis.table(
-        [
+class TestPipe(unittest.TestCase):
+
+    def setUp(self):
+        self.table = ibis.table([
             ('key1', 'string'),
             ('key2', 'string'),
             ('key3', 'string'),
-            ('value', 'double'),
-        ],
-        'foo_table',
-    )
-
-
-def test_pipe_positional_args(pipe_table):
-    def my_func(data, foo, bar):
-        return data[bar] + foo
+            ('value', 'double')
+        ], 'foo_table')
 
-    result = pipe_table.pipe(my_func, 4, 'value')
-    expected = pipe_table['value'] + 4
+    def test_pipe_positional_args(self):
+        def my_func(data, foo, bar):
+            return data[bar] + foo
 
-    assert result.equals(expected)
+        result = self.table.pipe(my_func, 4, 'value')
+        expected = self.table['value'] + 4
 
+        assert result.equals(expected)
 
-def test_pipe_keyword_args(pipe_table):
-    def my_func(data, foo=None, bar=None):
-        return data[bar] + foo
+    def test_pipe_keyword_args(self):
+        def my_func(data, foo=None, bar=None):
+            return data[bar] + foo
 
-    result = pipe_table.pipe(my_func, foo=4, bar='value')
-    expected = pipe_table['value'] + 4
+        result = self.table.pipe(my_func, foo=4, bar='value')
+        expected = self.table['value'] + 4
 
-    assert result.equals(expected)
+        assert result.equals(expected)
 
+    def test_pipe_pass_to_keyword(self):
+        def my_func(x, y, data=None):
+            return data[x] + y
 
-def test_pipe_pass_to_keyword(pipe_table):
-    def my_func(x, y, data=None):
-        return data[x] + y
+        result = self.table.pipe((my_func, 'data'), 'value', 4)
+        expected = self.table['value'] + 4
 
-    result = pipe_table.pipe((my_func, 'data'), 'value', 4)
-    expected = pipe_table['value'] + 4
+        assert result.equals(expected)
 
-    assert result.equals(expected)
+    def test_call_pipe_equivalence(self):
+        result = self.table(lambda x: x['key1'].cast('double').sum())
+        expected = self.table.key1.cast('double').sum()
+        assert result.equals(expected)
```

### Comparing `ibis_framework-5.1.0/ibis/tests/expr/test_table.py` & `ibis-framework-v0.6.0/ibis/sql/tests/test_compiler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1863 +1,2091 @@
-import datetime
-import pickle
-import re
-from typing import List
-
-import numpy as np
-import pandas as pd
-import pytest
-from pytest import param
+# Copyright 2014 Cloudera Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import ibis
-import ibis.common.exceptions as com
-import ibis.expr.analysis as an
-import ibis.expr.datatypes as dt
-import ibis.expr.operations as ops
-import ibis.expr.schema as sch
-import ibis.expr.types as ir
-import ibis.selectors as s
-from ibis import _
-from ibis import literal as L
-from ibis.common.exceptions import RelationError
-from ibis.expr import api
-from ibis.expr.types import Column, Table
-from ibis.tests.expr.mocks import MockAlchemyBackend, MockBackend
-from ibis.tests.util import assert_equal, assert_pickle_roundtrip
-
-
-@pytest.fixture
-def set_ops_schema_top():
-    return [('key', 'string'), ('value', 'double')]
-
-
-@pytest.fixture
-def set_ops_schema_bottom():
-    return [('key', 'string'), ('key2', 'string'), ('value', 'double')]
-
-
-@pytest.fixture
-def setops_table_foo(set_ops_schema_top):
-    return ibis.table(set_ops_schema_top, 'foo')
-
-
-@pytest.fixture
-def setops_table_bar(set_ops_schema_top):
-    return ibis.table(set_ops_schema_top, 'bar')
-
-
-@pytest.fixture
-def setops_table_baz(set_ops_schema_bottom):
-    return ibis.table(set_ops_schema_bottom, 'baz')
-
-
-@pytest.fixture
-def setops_relation_error_message():
-    return 'Table schemas must be equal for set operations'
-
-
-def test_empty_schema():
-    table = api.table([], 'foo')
-    assert not table.schema()
-
-
-def test_columns(con):
-    t = con.table('alltypes')
-    result = t.columns
-    expected = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k']
-    assert result == expected
 
+from ibis.impala.compiler import build_ast, to_sql
 
-def test_view_new_relation(table):
-    # For assisting with self-joins and other self-referential operations
-    # where we need to be able to treat instances of the same Table as
-    # semantically distinct
-    #
-    # This thing is not exactly a projection, since it has no semantic
-    # meaning when it comes to execution
-    tview = table.view()
+from ibis import impala
 
-    roots = an.find_immediate_parent_tables(tview.op())
-    assert len(roots) == 1
-    assert roots[0] is tview.op()
+from ibis.expr.tests.mocks import MockConnection
+from ibis.compat import unittest
+import ibis.common as com
 
+import ibis.expr.api as api
+import ibis.expr.operations as ops
 
-def test_getitem_column_select(table):
-    for k in table.columns:
-        col = table[k]
-
-        # Make sure it's the right type
-        assert isinstance(col, Column)
-
-
-def test_table_tab_completion():
-    table = ibis.table({"a": "int", "b": "int", "for": "int", "with spaces": "int"})
-    # Only valid python identifiers in getattr tab completion
-    attrs = set(dir(table))
-    assert {"a", "b"}.issubset(attrs)
-    assert {"for", "with spaces"}.isdisjoint(attrs)
-    # All columns in getitem tab completion
-    items = set(table._ipython_key_completions_())
-    assert items.issuperset(table.columns)
-
-
-def test_getitem_attribute(table):
-    result = table.a
-    assert_equal(result, table['a'])
-
-    # Project and add a name that conflicts with a Table built-in
-    # attribute
-    view = table[[table, table['a'].name('schema')]]
-    assert not isinstance(view.schema, Column)
 
+class TestASTBuilder(unittest.TestCase):
 
-def test_getitem_missing_column(table):
-    with pytest.raises(com.IbisTypeError, match="oops"):
-        table["oops"]
+    def setUp(self):
+        self.con = MockConnection()
 
+    def test_ast_with_projection_join_filter(self):
+        table = self.con.table('test1')
+        table2 = self.con.table('test2')
 
-def test_getattr_missing_column(table):
-    with pytest.raises(AttributeError, match="oops"):
-        table.oops  # noqa: B018
+        filter_pred = table['f'] > 0
 
+        table3 = table[filter_pred]
 
-def test_typo_method_name_recommendation(table):
-    with pytest.raises(AttributeError, match="order_by"):
-        table.sort("a")
+        join_pred = table3['g'] == table2['key']
 
-    # Existing columns take precedence over raising an error
-    # for a common method typo
-    table2 = table.relabel({"a": "sort"})
-    assert isinstance(table2.sort, Column)
+        joined = table2.inner_join(table3, [join_pred])
+        result = joined[[table3, table2['value']]]
 
+        ast = build_ast(result)
+        stmt = ast.queries[0]
 
-def test_projection(table):
-    cols = ['f', 'a', 'h']
+        def foo():
+            table3 = table[filter_pred]
+            joined = table2.inner_join(table3, [join_pred])
+            result = joined[[table3, table2['value']]]
+            return result
 
-    proj = table[cols]
-    assert isinstance(proj, Table)
-    assert isinstance(proj.op(), ops.Selection)
+        assert len(stmt.select_set) == 2
+        assert len(stmt.where) == 1
+        assert stmt.where[0] is filter_pred
 
-    assert proj.schema().names == tuple(cols)
-    for c in cols:
-        expr = proj[c]
-        assert isinstance(expr, type(table[c]))
+        # Check that the join has been rebuilt to only include the root tables
+        tbl = stmt.table_set
+        tbl_node = tbl.op()
+        assert isinstance(tbl_node, ops.InnerJoin)
+        assert tbl_node.left is table2
+        assert tbl_node.right is table
 
+        # table expression substitution has been made in the predicate
+        assert tbl_node.predicates[0].equals(table['g'] == table2['key'])
 
-def test_projection_no_list(table):
-    expr = (table.f * 2).name('bar')
-    result = table.select(expr)
-    expected = table.select([expr])
-    assert_equal(result, expected)
+    def test_ast_with_aggregation_join_filter(self):
+        table = self.con.table('test1')
+        table2 = self.con.table('test2')
 
+        filter_pred = table['f'] > 0
+        table3 = table[filter_pred]
+        join_pred = table3['g'] == table2['key']
 
-def test_projection_with_exprs(table):
-    # unnamed expr to test
-    mean_diff = (table['a'] - table['c']).mean()
+        joined = table2.inner_join(table3, [join_pred])
 
-    col_exprs = [table['b'].log().name('log_b'), mean_diff.name('mean_diff')]
+        met1 = (table3['f'] - table2['value']).mean().name('foo')
+        result = joined.aggregate([met1, table3['f'].sum().name('bar')],
+                                  by=[table3['g'], table2['key']])
 
-    proj = table[col_exprs + ['g']]
-    schema = proj.schema()
-    assert schema.names == ('log_b', 'mean_diff', 'g')
-    assert schema.types == (dt.double, dt.double, dt.string)
+        ast = build_ast(result)
+        stmt = ast.queries[0]
 
-    # Test with unnamed expr
-    proj = table.select(['g', table['a'] - table['c']])
-    schema = proj.schema()
-    assert schema.names == ('g', 'Subtract(a, c)')
-    assert schema.types == (dt.string, dt.int64)
+        # hoisted metrics
+        ex_metrics = [(table['f'] - table2['value']).mean().name('foo'),
+                      table['f'].sum().name('bar')]
+        ex_by = [table['g'], table2['key']]
 
+        # hoisted join and aggregate
+        expected_table_set = \
+            table2.inner_join(table, [table['g'] == table2['key']])
+        assert stmt.table_set.equals(expected_table_set)
 
-def test_projection_duplicate_names(table):
-    with pytest.raises(com.IntegrityError):
-        table.select([table.c, table.c])
+        # Check various exprs
+        for res, ex in zip(stmt.select_set, ex_by + ex_metrics):
+            assert res.equals(ex)
 
+        for res, ex in zip(stmt.group_by, ex_by):
+            assert stmt.select_set[res].equals(ex)
 
-def test_projection_invalid_root(table):
-    schema1 = {'foo': 'double', 'bar': 'int32'}
+        # Check we got the filter
+        assert len(stmt.where) == 1
+        assert stmt.where[0].equals(filter_pred)
 
-    left = api.table(schema1, name='foo')
-    right = api.table(schema1, name='bar')
 
-    exprs = [right['foo'], right['bar']]
-    with pytest.raises(RelationError):
-        left.select(exprs)
+class TestNonTabularResults(unittest.TestCase):
 
+    """
 
-def test_projection_with_star_expr(table):
-    new_expr = (table['a'] * 5).name('bigger_a')
+    """
 
-    t = table
+    def setUp(self):
+        self.con = MockConnection()
+        self.table = self.con.table('alltypes')
 
-    # it lives!
-    proj = t[t, new_expr]
-    repr(proj)
+    def test_simple_scalar_aggregates(self):
+        from pandas import DataFrame
 
-    ex_names = table.schema().names + ('bigger_a',)
-    assert proj.schema().names == ex_names
+        # Things like table.column.{sum, mean, ...}()
+        table = self.con.table('alltypes')
 
-    # cannot pass an invalid table expression
-    t2 = t.aggregate([t['a'].sum().name('sum(a)')], by=['g'])
-    with pytest.raises(RelationError):
-        t[[t2]]
-    # TODO: there may be some ways this can be invalid
+        expr = table[table.c > 0].f.sum()
 
+        ast = build_ast(expr)
+        query = ast.queries[0]
 
-def test_projection_convenient_syntax(table):
-    proj = table[table, table['a'].name('foo')]
-    proj2 = table[[table, table['a'].name('foo')]]
-    assert_equal(proj, proj2)
+        sql_query = query.compile()
+        expected = """SELECT sum(`f`) AS `sum`
+FROM alltypes
+WHERE `c` > 0"""
 
+        assert sql_query == expected
 
-def test_projection_mutate_analysis_bug(con):
-    # GH #549
+        # Maybe the result handler should act on the cursor. Not sure.
+        handler = query.result_handler
+        output = DataFrame({'sum': [5]})
+        assert handler(output) == 5
 
-    t = con.table('airlines')
+    def test_table_column_unbox(self):
+        from pandas import DataFrame
 
-    filtered = t[t.depdelay.notnull()]
-    leg = ibis.literal('-').join([t.origin, t.dest])
-    mutated = filtered.mutate(leg=leg)
+        table = self.table
+        m = table.f.sum().name('total')
+        agged = table[table.c > 0].group_by('g').aggregate([m])
+        expr = agged.g
 
-    # it works!
-    mutated['year', 'month', 'day', 'depdelay', 'leg']
+        ast = build_ast(expr)
+        query = ast.queries[0]
 
+        sql_query = query.compile()
+        expected = """\
+SELECT `g`
+FROM (
+  SELECT `g`, sum(`f`) AS `total`
+  FROM alltypes
+  WHERE `c` > 0
+  GROUP BY 1
+) t0"""
 
-def test_projection_self(table):
-    result = table[table]
-    expected = table.select(table)
+        assert sql_query == expected
 
-    assert_equal(result, expected)
+        # Maybe the result handler should act on the cursor. Not sure.
+        handler = query.result_handler
+        output = DataFrame({'g': ['foo', 'bar', 'baz']})
+        assert (handler(output) == output['g']).all()
 
+    def test_complex_array_expr_projection(self):
+        # May require finding the base table and forming a projection.
+        expr = (self.table.group_by('g')
+                .aggregate([self.table.count().name('count')]))
+        expr2 = expr.g.cast('double')
 
-def test_projection_array_expr(table):
-    result = table[table.a]
-    expected = table[[table.a]]
-    assert_equal(result, expected)
+        query = impala.compile(expr2)
+        expected = """SELECT CAST(`g` AS double) AS `tmp`
+FROM (
+  SELECT `g`, count(*) AS `count`
+  FROM alltypes
+  GROUP BY 1
+) t0"""
+        assert query == expected
 
+    def test_scalar_exprs_no_table_refs(self):
+        expr1 = ibis.now()
+        expected1 = """\
+SELECT now() AS `tmp`"""
 
-@pytest.mark.parametrize("empty", [list(), dict()])
-def test_projection_no_expr(table, empty):
-    with pytest.raises(com.IbisTypeError, match="must select at least one"):
-        table.select(empty)
+        expr2 = ibis.literal(1) + ibis.literal(2)
+        expected2 = """\
+SELECT 1 + 2 AS `tmp`"""
 
+        cases = [
+            (expr1, expected1),
+            (expr2, expected2)
+        ]
 
-def test_mutate(table):
-    expr = table.mutate(
-        [
-            (table.a + 1).name("x1"),
-            table.b.sum().name("x2"),
-            (_.a + 2).name("x3"),
-            lambda _: (_.a + 3).name("x4"),
-            4,
-            "five",
+        for expr, expected in cases:
+            result = impala.compile(expr)
+            assert result == expected
+
+    def test_expr_list_no_table_refs(self):
+        exlist = ibis.api.expr_list([ibis.literal(1).name('a'),
+                                     ibis.now().name('b'),
+                                     ibis.literal(2).log().name('c')])
+        result = impala.compile(exlist)
+        expected = """\
+SELECT 1 AS `a`, now() AS `b`, ln(2) AS `c`"""
+        assert result == expected
+
+    def test_isnull_case_expr_rewrite_failure(self):
+        # #172, case expression that was not being properly converted into an
+        # aggregation
+        reduction = self.table.g.isnull().ifelse(1, 0).sum()
+
+        result = impala.compile(reduction)
+        expected = """\
+SELECT sum(CASE WHEN `g` IS NULL THEN 1 ELSE 0 END) AS `sum`
+FROM alltypes"""
+        assert result == expected
+
+
+def _get_query(expr):
+    ast = build_ast(expr)
+    return ast.queries[0]
+
+nation = api.table([
+    ('n_regionkey', 'int32'),
+    ('n_nationkey', 'int32'),
+    ('n_name', 'string')
+], 'nation')
+
+region = api.table([
+    ('r_regionkey', 'int32'),
+    ('r_name', 'string')
+], 'region')
+
+customer = api.table([
+    ('c_nationkey', 'int32'),
+    ('c_name', 'string'),
+    ('c_acctbal', 'double')
+], 'customer')
+
+
+def _table_wrapper(name, tname=None):
+    @property
+    def f(self):
+        return self._table_from_schema(name, tname)
+    return f
+
+
+class ExprTestCases(object):
+
+    _schemas = {
+        'foo': [
+            ('job', 'string'),
+            ('dept_id', 'string'),
+            ('year', 'int32'),
+            ('y', 'double')
         ],
-        kw1=(table.a + 6),
-        kw2=table.b.sum(),
-        kw3=(_.a + 7),
-        kw4=lambda _: (_.a + 8),
-        kw5=9,
-        kw6="ten",
-    )
-    expected = table[
-        table,
-        (table.a + 1).name("x1"),
-        table.b.sum().name("x2"),
-        (table.a + 2).name("x3"),
-        (table.a + 3).name("x4"),
-        ibis.literal(4).name("4"),
-        ibis.literal("five").name("'five'"),
-        (table.a + 6).name("kw1"),
-        table.b.sum().name("kw2"),
-        (table.a + 7).name("kw3"),
-        (table.a + 8).name("kw4"),
-        ibis.literal(9).name("kw5"),
-        ibis.literal("ten").name("kw6"),
-    ]
-    assert_equal(expr, expected)
-
-
-def test_mutate_alter_existing_columns(table):
-    new_f = table.f * 2
-    foo = table.d * 2
-    expr = table.mutate(f=new_f, foo=foo)
-
-    expected = table[
-        'a',
-        'b',
-        'c',
-        'd',
-        'e',
-        new_f.name('f'),
-        'g',
-        'h',
-        'i',
-        'j',
-        'k',
-        foo.name('foo'),
-    ]
-
-    assert_equal(expr, expected)
-
-
-def test_replace_column():
-    tb = api.table([('a', 'int32'), ('b', 'double'), ('c', 'string')])
-
-    expr = tb.b.cast('int32')
-    tb2 = tb.mutate(b=expr)
-    expected = tb[tb.a, expr.name('b'), tb.c]
-
-    assert_equal(tb2, expected)
-
-
-def test_filter_no_list(table):
-    pred = table.a > 5
-
-    result = table.filter(pred)
-    expected = table[pred]
-    assert_equal(result, expected)
-
-
-def test_add_predicate(table):
-    pred = table['a'] > 5
-    result = table[pred]
-    assert isinstance(result.op(), ops.Selection)
-
-
-def test_invalid_predicate(table, schema):
-    # a lookalike
-    table2 = api.table(schema, name='bar')
-    predicate = table2.a > 5
-    with pytest.raises(RelationError):
-        table.filter(predicate)
-
-
-def test_add_predicate_coalesce(table):
-    # Successive predicates get combined into one rather than nesting. This
-    # is mainly to enhance readability since we could handle this during
-    # expression evaluation anyway.
-    pred1 = table['a'] > 5
-    pred2 = table['b'] > 0
-
-    result = table[pred1][pred2]
-    expected = table.filter([pred1, pred2])
-    assert_equal(result, expected)
-
-    # 59, if we are not careful, we can obtain broken refs
-    interm = table[pred1]
-    result = interm.filter([interm['b'] > 0])
-    assert_equal(result, expected)
-
-
-def test_repr_same_but_distinct_objects(con):
-    t = con.table('test1')
-    t_copy = con.table('test1')
-    table2 = t[t_copy['f'] > 0]
-
-    result = repr(table2)
-    assert result.count('DatabaseTable') == 1
-
-
-def test_filter_fusion_distinct_table_objects(con):
-    t = con.table('test1')
-    tt = con.table('test1')
-
-    expr = t[t.f > 0][t.c > 0]
-    expr2 = t[t.f > 0][tt.c > 0]
-    expr3 = t[tt.f > 0][tt.c > 0]
-    expr4 = t[tt.f > 0][t.c > 0]
-
-    assert_equal(expr, expr2)
-    assert repr(expr) == repr(expr2)
-    assert_equal(expr, expr3)
-    assert_equal(expr, expr4)
-
-
-def test_column_relabel():
-    table = api.table({"x": "int32", "y": "string", "z": "double"})
-    sol = sch.schema({"x_1": "int32", "y_1": "string", "z": "double"})
-
-    # Using a mapping
-    res = table.relabel({"x": "x_1", "y": "y_1"}).schema()
-    assert_equal(res, sol)
-
-    # Using a function
-    res = table.relabel(lambda x: None if x == "z" else f"{x}_1").schema()
-    assert_equal(res, sol)
-
-    # Mapping with unknown columns errors
-    with pytest.raises(KeyError, match="is not an existing column"):
-        table.relabel({"missing": "oops"})
-
-
-def test_relabel_format_string():
-    t = ibis.table({"x": "int", "y": "int", "z": "int"})
-
-    res = t.relabel("_{name}_")
-    sol = t.relabel({"x": "_x_", "y": "_y_", "z": "_z_"})
-    assert_equal(res, sol)
-
-    with pytest.raises(ValueError, match="Format strings must"):
-        t.relabel("no format string parameter")
-
-    with pytest.raises(ValueError, match="Format strings must"):
-        t.relabel("{unknown} format string parameter")
+        'bar': [
+            ('x', 'double'),
+            ('job', 'string')
+        ],
+        't1': [
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('value1', 'double')
+        ],
+        't2': [
+            ('key1', 'string'),
+            ('key2', 'string')
+        ]
+    }
 
+    def _table_from_schema(self, name, tname=None):
+        tname = tname or name
+        return api.table(self._schemas[name], tname)
+
+    def _case_multiple_joins(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+        t3 = self.con.table('star3')
+
+        predA = t1['foo_id'] == t2['foo_id']
+        predB = t1['bar_id'] == t3['bar_id']
+
+        what = (t1.left_join(t2, [predA])
+                .inner_join(t3, [predB])
+                .projection([t1, t2['value1'], t3['value2']]))
+        return what
 
-def test_relabel_snake_case():
-    cases = [
-        ("cola", "cola"),
-        ("ColB", "col_b"),
-        ("colC", "col_c"),
-        ("col-d", "col_d"),
-        ("col_e", "col_e"),
-        (" Column F ", "column_f"),
-        ("Column G-with-hyphens", "column_g_with_hyphens"),
-        ("Col H notCamelCase", "col_h_notcamelcase"),
-    ]
-    t = ibis.table({c: "int" for c, _ in cases})
-    res = t.relabel("snake_case")
-    sol = t.relabel(dict(cases))
-    assert_equal(res, sol)
+    def _case_join_between_joins(self):
+        t1 = api.table([
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('value1', 'double'),
+        ], 'first')
 
+        t2 = api.table([
+            ('key1', 'string'),
+            ('value2', 'double'),
+        ], 'second')
 
-def test_limit(table):
-    limited = table.limit(10, offset=5)
-    assert limited.op().n == 10
-    assert limited.op().offset == 5
+        t3 = api.table([
+            ('key2', 'string'),
+            ('key3', 'string'),
+            ('value3', 'double'),
+        ], 'third')
 
+        t4 = api.table([
+            ('key3', 'string'),
+            ('value4', 'double')
+        ], 'fourth')
 
-def test_sort_by_deprecated(table):
-    with pytest.warns(FutureWarning):
-        x = table.sort_by("f")
-    y = table.order_by("f")
-    assert x.equals(y)
+        left = t1.inner_join(t2, [('key1', 'key1')])[t1, t2.value2]
+        right = t3.inner_join(t4, [('key3', 'key3')])[t3, t4.value4]
 
+        joined = left.inner_join(right, [('key2', 'key2')])
 
-def test_order_by(table):
-    result = table.order_by(['f']).op()
+        # At one point, the expression simplification was resulting in bad refs
+        # here (right.value3 referencing the table inside the right join)
+        exprs = [left, right.value3, right.value4]
+        projected = joined.projection(exprs)
 
-    sort_key = result.sort_keys[0]
+        return projected
 
-    assert_equal(sort_key.expr, table.f.op())
-    assert sort_key.ascending
+    def _case_join_just_materialized(self):
+        t1 = self.con.table('tpch_nation')
+        t2 = self.con.table('tpch_region')
+        t3 = self.con.table('tpch_customer')
 
-    # non-list input. per #150
-    result2 = table.order_by('f').op()
-    assert_equal(result, result2)
+        # GH #491
+        return (t1.inner_join(t2, t1.n_regionkey == t2.r_regionkey)
+                .inner_join(t3, t1.n_nationkey == t3.c_nationkey))
 
-    result2 = table.order_by([('f', False)])
-    result3 = table.order_by([('f', 'descending')])
-    result4 = table.order_by([('f', 0)])
+    def _case_semi_anti_joins(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
 
-    key2 = result2.op().sort_keys[0]
-    key3 = result3.op().sort_keys[0]
-    key4 = result4.op().sort_keys[0]
+        sj = t1.semi_join(t2, [t1.foo_id == t2.foo_id])[[t1]]
+        aj = t1.anti_join(t2, [t1.foo_id == t2.foo_id])[[t1]]
 
-    assert key2.descending
-    assert key3.descending
-    assert key4.descending
-    assert_equal(result2, result3)
+        return sj, aj
 
+    def _case_self_reference_simple(self):
+        t1 = self.con.table('star1')
+        return t1.view()
 
-def test_order_by_desc_deferred_sort_key(table):
-    result = table.group_by('g').size().order_by(ibis.desc('count'))
+    def _case_self_reference_join(self):
+        t1 = self.con.table('star1')
+        t2 = t1.view()
+        return t1.inner_join(t2, [t1.foo_id == t2.bar_id])[[t1]]
 
-    tmp = table.group_by('g').size()
-    expected = tmp.order_by((tmp['count'], False))
-    expected2 = tmp.order_by(ibis.desc(tmp['count']))
+    def _case_join_projection_subquery_bug(self):
+        # From an observed bug, derived from tpch tables
+        geo = (nation.inner_join(region, [('n_regionkey', 'r_regionkey')])
+               [nation.n_nationkey,
+                nation.n_name.name('nation'),
+                region.r_name.name('region')])
 
-    assert_equal(result, expected)
-    assert_equal(result, expected2)
+        expr = (geo.inner_join(customer, [('n_nationkey', 'c_nationkey')])
+                [customer, geo])
 
+        return expr
 
-def test_order_by_asc_deferred_sort_key(table):
-    result = table.group_by('g').size().order_by(ibis.asc('count'))
+    def _case_where_simple_comparisons(self):
+        t1 = self.con.table('star1')
 
-    tmp = table.group_by('g').size()
-    expected = tmp.order_by(tmp['count'])
-    expected2 = tmp.order_by(ibis.asc(tmp['count']))
+        what = t1.filter([t1.f > 0, t1.c < t1.f * 2])
 
-    assert_equal(result, expected)
-    assert_equal(result, expected2)
+        return what
 
+    def _case_where_with_join(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
 
-@pytest.mark.parametrize(
-    ("key", "expected"),
-    [
-        param(ibis.NA, ibis.NA.op(), id="na"),
-        param(ibis.random(), ibis.random().op(), id="random"),
-        param(1.0, L(1.0).op(), id="float"),
-        param(L("a"), L("a").op(), id="string"),
-        param(L([1, 2, 3]), L([1, 2, 3]).op(), id="array"),
-    ],
-)
-def test_order_by_scalar(table, key, expected):
-    result = table.order_by(key)
-    assert result.op().sort_keys == (ops.SortKey(expected),)
-
-
-@pytest.mark.parametrize(
-    "key",
-    [
-        "bogus",
-        ("bogus", False),
-        ibis.desc("bogus"),
-        1000,
-        (1000, False),
-        _.bogus,
-        _.bogus.desc(),
-    ],
-)
-@pytest.mark.parametrize(
-    "expr_func",
-    [
-        param(lambda t: t, id="table"),
-        param(lambda t: t.select("a", "b"), id="selection"),
-        param(lambda t: t.group_by("a").agg(new=_.b.sum()), id="aggregation"),
-    ],
-)
-def test_order_by_nonexistent_column_errors(table, expr_func, key):
-    # `order_by` is implemented on a few different operations, we check them
-    # all in turn here.
-    expr = expr_func(table)
-    # Depending on the expression, this can raise a few different errors.
-    # For now just check that an exception is raised.
-    with pytest.raises(Exception):
-        expr.order_by(key)
+        # This also tests some cases of predicate pushdown
+        e1 = (t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+              .projection([t1, t2.value1, t2.value3])
+              .filter([t1.f > 0, t2.value3 < 1000]))
 
+        e2 = (t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+              .filter([t1.f > 0, t2.value3 < 1000])
+              .projection([t1, t2.value1, t2.value3]))
 
-def test_slice(table):
-    expr = table[:5]
-    expr2 = table[:5:1]
-    assert_equal(expr, table.limit(5))
-    assert_equal(expr, expr2)
+        return e1, e2
 
-    expr = table[2:7]
-    expr2 = table[2:7:1]
-    assert_equal(expr, table.limit(5, offset=2))
-    assert_equal(expr, expr2)
+    def _case_subquery_used_for_self_join(self):
+        # There could be cases that should look in SQL like
+        # WITH t0 as (some subquery)
+        # select ...
+        # from t0 t1
+        #   join t0 t2
+        #     on t1.kind = t2.subkind
+        # ...
+        # However, the Ibis code will simply have an expression (projection or
+        # aggregation, say) built on top of the subquery expression, so we need
+        # to extract the subquery unit (we see that it appears multiple times
+        # in the tree).
+        t = self.con.table('alltypes')
 
-    with pytest.raises(ValueError):
-        table[2:15:2]
+        agged = t.aggregate([t.f.sum().name('total')], by=['g', 'a', 'b'])
+        view = agged.view()
+        metrics = [(agged.total - view.total).max().name('metric')]
+        expr = (agged.inner_join(view, [agged.a == view.b])
+                .aggregate(metrics, by=[agged.g]))
 
-    with pytest.raises(ValueError):
-        table[5:]
+        return expr
 
-    with pytest.raises(ValueError):
-        table[:-5]
+    def _case_subquery_factor_correlated_subquery(self):
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+        customer = self.con.table('tpch_customer')
+        orders = self.con.table('tpch_orders')
 
-    with pytest.raises(ValueError):
-        table[-10:-5]
+        fields_of_interest = [customer,
+                              region.r_name.name('region'),
+                              orders.o_totalprice.name('amount'),
+                              orders.o_orderdate
+                              .cast('timestamp').name('odate')]
 
+        tpch = (region.join(nation, region.r_regionkey == nation.n_regionkey)
+                .join(customer, customer.c_nationkey == nation.n_nationkey)
+                .join(orders, orders.o_custkey == customer.c_custkey)
+                [fields_of_interest])
 
-def test_table_count(table):
-    result = table.count()
-    assert isinstance(result, ir.IntegerScalar)
-    assert isinstance(result.op(), ops.Alias)
-    assert isinstance(result.op().arg, ops.CountStar)
-    assert result.get_name() == 'count'
+        # Self-reference + correlated subquery complicates things
+        t2 = tpch.view()
+        conditional_avg = t2[t2.region == tpch.region].amount.mean()
+        amount_filter = tpch.amount > conditional_avg
 
+        return tpch[amount_filter].limit(10)
 
-def test_len_raises_expression_error(table):
-    with pytest.raises(com.ExpressionError):
-        len(table)
+    def _case_self_join_subquery_distinct_equal(self):
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
 
+        j1 = (region.join(nation, region.r_regionkey == nation.n_regionkey)
+              [region, nation])
 
-def test_sum_expr_basics(table, int_col):
-    # Impala gives bigint for all integer types
-    result = table[int_col].sum()
-    assert isinstance(result, ir.IntegerScalar)
-    assert isinstance(result.op(), ops.Sum)
+        j2 = (region.join(nation, region.r_regionkey == nation.n_regionkey)
+              [region, nation].view())
 
+        expr = (j1.join(j2, j1.r_regionkey == j2.r_regionkey)
+                [j1.r_name, j2.n_name])
 
-def test_sum_expr_basics_floats(table, float_col):
-    # Impala gives double for all floating point types
-    result = table[float_col].sum()
-    assert isinstance(result, ir.FloatingScalar)
-    assert isinstance(result.op(), ops.Sum)
+        return expr
 
+    def _case_cte_factor_distinct_but_equal(self):
+        t = self.con.table('alltypes')
+        tt = self.con.table('alltypes')
 
-def test_mean_expr_basics(table, numeric_col):
-    result = table[numeric_col].mean()
-    assert isinstance(result, ir.FloatingScalar)
-    assert isinstance(result.op(), ops.Mean)
+        expr1 = t.group_by('g').aggregate(t.f.sum().name('metric'))
+        expr2 = tt.group_by('g').aggregate(tt.f.sum().name('metric')).view()
 
+        expr = expr1.join(expr2, expr1.g == expr2.g)[[expr1]]
 
-def test_aggregate_no_keys(table):
-    metrics = [
-        table['a'].sum().name('sum(a)'),
-        table['c'].mean().name('mean(c)'),
-    ]
+        return expr
 
-    # A Table, which in SQL at least will yield a table with a single
-    # row
-    result = table.aggregate(metrics)
-    assert isinstance(result, Table)
+    def _case_tpch_self_join_failure(self):
+        # duplicating the integration test here
 
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+        customer = self.con.table('tpch_customer')
+        orders = self.con.table('tpch_orders')
 
-def test_aggregate_keys_basic(table):
-    metrics = [
-        table['a'].sum().name('sum(a)'),
-        table['c'].mean().name('mean(c)'),
-    ]
+        fields_of_interest = [
+            region.r_name.name('region'),
+            nation.n_name.name('nation'),
+            orders.o_totalprice.name('amount'),
+            orders.o_orderdate.cast('timestamp').name('odate')]
 
-    # A Table, which in SQL at least will yield a table with a single
-    # row
-    result = table.aggregate(metrics, by=['g'])
-    assert isinstance(result, Table)
+        joined_all = (
+            region.join(nation, region.r_regionkey == nation.n_regionkey)
+            .join(customer, customer.c_nationkey == nation.n_nationkey)
+            .join(orders, orders.o_custkey == customer.c_custkey)
+            [fields_of_interest])
 
-    # it works!
-    repr(result)
+        year = joined_all.odate.year().name('year')
+        total = joined_all.amount.sum().cast('double').name('total')
+        annual_amounts = (joined_all
+                          .group_by(['region', year])
+                          .aggregate(total))
 
+        current = annual_amounts
+        prior = annual_amounts.view()
 
-def test_aggregate_non_list_inputs(table):
-    # per #150
-    metric = table.f.sum().name('total')
-    by = 'g'
-    having = table.c.sum() > 10
+        yoy_change = (current.total - prior.total).name('yoy_change')
+        yoy = (current.join(prior, current.year == (prior.year - 1))
+               [current.region, current.year, yoy_change])
+        return yoy
 
-    result = table.aggregate(metric, by=by, having=having)
-    expected = table.aggregate([metric], by=[by], having=[having])
-    assert_equal(result, expected)
+    def _case_subquery_in_filter_predicate(self):
+        # E.g. comparing against some scalar aggregate value. See Ibis #43
+        t1 = self.con.table('star1')
 
+        pred = t1.f > t1.f.mean()
+        expr = t1[pred]
 
-def test_aggregate_keywords(table):
-    t = table
+        # This brought out another expression rewriting bug, since the filtered
+        # table isn't found elsewhere in the expression.
+        pred2 = t1.f > t1[t1.foo_id == 'foo'].f.mean()
+        expr2 = t1[pred2]
 
-    expr = t.aggregate(foo=t.f.sum(), bar=lambda x: x.f.mean(), by='g')
-    expr2 = t.group_by('g').aggregate(foo=t.f.sum(), bar=lambda x: x.f.mean())
-    expected = t.aggregate([t.f.sum().name('foo'), t.f.mean().name('bar')], by='g')
+        return expr, expr2
 
-    assert_equal(expr, expected)
-    assert_equal(expr2, expected)
+    def _case_filter_subquery_derived_reduction(self):
+        t1 = self.con.table('star1')
 
+        # Reduction can be nested inside some scalar expression
+        pred3 = t1.f > t1[t1.foo_id == 'foo'].f.mean().log()
+        pred4 = t1.f > (t1[t1.foo_id == 'foo'].f.mean().log() + 1)
 
-def test_groupby_alias(table):
-    expected = table.group_by('g').size()
-    with pytest.warns(FutureWarning, match="deprecated"):
-        result = table.groupby('g').size()
-    assert_equal(result, expected)
+        expr3 = t1[pred3]
+        expr4 = t1[pred4]
 
+        return expr3, expr4
 
-def test_summary_expand_list(table):
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        summ = table.f.summary()
+    def _case_topk_operation(self):
+        # TODO: top K with filter in place
 
-    metric = table.g.group_concat().name('bar')
-    result = table.aggregate([metric, summ])
-    expected = table.aggregate([metric] + summ)
-    assert_equal(result, expected)
+        table = api.table([
+            ('foo', 'string'),
+            ('bar', 'string'),
+            ('city', 'string'),
+            ('v1', 'double'),
+            ('v2', 'double'),
+        ], 'tbl')
 
+        what = table.city.topk(10, by=table.v2.mean())
+        e1 = table[what]
 
-def test_summary_prefix_suffix(table):
-    def get_names(exprs):
-        return [e.get_name() for e in exprs]
+        # Test the default metric (count)
+        what = table.city.topk(10)
+        e2 = table[what]
 
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        assert get_names(table.g.summary(prefix="string_")) == [
-            'string_count',
-            'string_nulls',
-            'string_uniques',
-        ]
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        assert get_names(table.g.summary(suffix="_string")) == [
-            'count_string',
-            'nulls_string',
-            'uniques_string',
-        ]
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        assert get_names(table.g.summary(prefix="pre_", suffix="_post")) == [
-            'pre_count_post',
-            'pre_nulls_post',
-            'pre_uniques_post',
-        ]
+        return e1, e2
 
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        assert get_names(table.f.summary(prefix="float_")) == [
-            "float_count",
-            "float_nulls",
-            "float_min",
-            "float_max",
-            "float_sum",
-            "float_mean",
-            "float_approx_nunique",
+    def _case_simple_aggregate_query(self):
+        t1 = self.con.table('star1')
+        cases = [
+            t1.aggregate([t1['f'].sum().name('total')],
+                         [t1['foo_id']]),
+            t1.aggregate([t1['f'].sum().name('total')],
+                         ['foo_id', 'bar_id'])
         ]
-    with pytest.warns(FutureWarning, match="is deprecated"):
-        assert get_names(table.f.summary(suffix="_numeric")) == [
-            "count_numeric",
-            "nulls_numeric",
-            "min_numeric",
-            "max_numeric",
-            "sum_numeric",
-            "mean_numeric",
-            "approx_nunique_numeric",
-        ]
-
-
-def test_filter_aggregate_pushdown_predicate(table):
-    # In the case where we want to add a predicate to an aggregate
-    # expression after the fact, rather than having to backpedal and add it
-    # before calling aggregate.
-    #
-    # TODO (design decision): This could happen automatically when adding a
-    # predicate originating from the same root table; if an expression is
-    # created from field references from the aggregated table then it
-    # becomes a filter predicate applied on top of a view
-
-    pred = table.f > 0
-    metrics = [table.a.sum().name('total')]
-    agged = table.aggregate(metrics, by=['g'])
-    filtered = agged.filter([pred])
-    expected = table[pred].aggregate(metrics, by=['g'])
-    assert_equal(filtered, expected)
-
-
-def test_filter_on_literal_then_aggregate(table):
-    # Mostly just a smoketest, this used to error on construction
-    expr = table.filter(ibis.literal(True)).agg(lambda t: t.a.sum().name("total"))
-    assert expr.columns == ["total"]
-
-
-@pytest.mark.parametrize(
-    "case_fn",
-    [
-        param(lambda t: t.f.sum(), id="non_boolean"),
-        param(lambda t: t.f > 2, id="non_scalar"),
-    ],
-)
-def test_aggregate_post_predicate(table, case_fn):
-    # Test invalid having clause
-    metrics = [table.f.sum().name('total')]
-    by = ['g']
-    having = [case_fn(table)]
-
-    with pytest.raises(com.IbisTypeError):
-        table.aggregate(metrics, by=by, having=having)
-
-
-def test_group_by_having_api(table):
-    # #154, add a HAVING post-predicate in a composable way
-    metric = table.f.sum().name('foo')
-    postp = table.d.mean() > 1
-
-    expr = table.group_by('g').having(postp).aggregate(metric)
-
-    expected = table.aggregate(metric, by='g', having=postp)
-    assert_equal(expr, expected)
-
-
-def test_group_by_kwargs(table):
-    t = table
-    expr = t.group_by(['f', t.h], z='g', z2=t.d).aggregate(t.d.mean().name('foo'))
-    expected = t.group_by(['f', t.h, t.g.name('z'), t.d.name('z2')]).aggregate(
-        t.d.mean().name('foo')
-    )
-    assert_equal(expr, expected)
-
-
-def test_compound_aggregate_expr(table):
-    # See ibis #24
-    compound_expr = (table['a'].sum() / table['a'].mean()).name('foo')
-    assert an.is_reduction(compound_expr.op())
-
-    # Validates internally
-    table.aggregate([compound_expr])
-
-
-def test_groupby_convenience(table):
-    metrics = [table.f.sum().name('total')]
 
-    expr = table.group_by('g').aggregate(metrics)
-    expected = table.aggregate(metrics, by=['g'])
-    assert_equal(expr, expected)
+        return cases
 
-    group_expr = table.g.cast('double').name('g')
-    expr = table.group_by(group_expr).aggregate(metrics)
-    expected = table.aggregate(metrics, by=[group_expr])
-    assert_equal(expr, expected)
+    def _case_aggregate_having(self):
+        # Filtering post-aggregation predicate
+        t1 = self.con.table('star1')
 
+        total = t1.f.sum().name('total')
+        metrics = [total]
 
-def test_group_by_count_size(table):
-    # #148, convenience for interactive use, and so forth
-    result1 = table.group_by('g').size()
-    result2 = table.group_by('g').count()
+        e1 = t1.aggregate(metrics, by=['foo_id'], having=[total > 10])
+        e2 = t1.aggregate(metrics, by=['foo_id'], having=[t1.count() > 100])
 
-    expected = table.group_by('g').aggregate([table.count().name('count')])
+        return e1, e2
 
-    assert_equal(result1, expected)
-    assert_equal(result2, expected)
+    def _case_aggregate_count_joined(self):
+        # count on more complicated table
+        region = self.con.table('tpch_region')
+        nation = self.con.table('tpch_nation')
+        join_expr = region.r_regionkey == nation.n_regionkey
+        joined = region.inner_join(nation, join_expr)
+        table_ref = joined[nation, region.r_name.name('region')]
 
-    result = table.group_by('g').count('foo')
-    expected = table.group_by('g').aggregate([table.count().name('foo')])
-    assert_equal(result, expected)
+        return table_ref.count()
 
+    def _case_sort_by(self):
+        table = self.con.table('star1')
 
-def test_group_by_column_select_api(table):
-    grouped = table.group_by('g')
-
-    result = grouped.f.sum()
-    expected = grouped.aggregate(table.f.sum().name('sum(f)'))
-    assert_equal(result, expected)
-
-    supported_functions = ['sum', 'mean', 'count', 'size', 'max', 'min']
-
-    # make sure they all work
-    for fn in supported_functions:
-        getattr(grouped.f, fn)()
-
-
-def test_value_counts_convenience(table):
-    # #152
-    result = table.g.value_counts()
-    expected = table.select('g').group_by('g').aggregate(g_count=lambda t: t.count())
-
-    assert_equal(result, expected)
-
-
-def test_isin_value_counts(table):
-    # #157, this code path was untested before
-    bool_clause = table.g.notin(['1', '4', '7'])
-    # it works!
-    bool_clause.name('notin').value_counts()
-
-
-def test_value_counts_unnamed_expr(con):
-    nation = con.table('tpch_nation')
-
-    expr = nation.n_name.lower().value_counts()
-    expected = nation.n_name.lower().name('Lowercase(n_name)').value_counts()
-    assert_equal(expr, expected)
-
-
-def test_aggregate_unnamed_expr(con):
-    nation = con.table('tpch_nation')
-    expr = nation.n_name.lower().left(1)
-
-    agg = nation.group_by(expr).aggregate(nation.count().name('metric'))
-    schema = agg.schema()
-    assert schema.names == ('Substring(Lowercase(n_name), 0, 1)', 'metric')
-    assert schema.types == (dt.string, dt.int64)
-
-
-def test_join_no_predicate_list(con):
-    region = con.table('tpch_region')
-    nation = con.table('tpch_nation')
-
-    pred = region.r_regionkey == nation.n_regionkey
-    joined = region.inner_join(nation, pred)
-    expected = region.inner_join(nation, [pred])
-    assert_equal(joined, expected)
-
-
-def test_join_deferred(con):
-    region = con.table("tpch_region")
-    nation = con.table("tpch_nation")
-    res = region.join(nation, _.r_regionkey == nation.n_regionkey)
-    exp = region.join(nation, region.r_regionkey == nation.n_regionkey)
-    assert_equal(res, exp)
-
+        return [
+            table.sort_by('f'),
+            table.sort_by(('f', 0)),
+            table.sort_by(['c', ('f', 0)])
+        ]
 
-def test_asof_join():
-    left = ibis.table([('time', 'int32'), ('value', 'double')])
-    right = ibis.table([('time', 'int32'), ('value2', 'double')])
-    joined = api.asof_join(left, right, 'time')
+    def _case_limit(self):
+        star1 = self.con.table('star1')
 
-    assert joined.columns == [
-        "time_x",
-        "value",
-        "time_y",
-        "value2",
-    ]
-    pred = joined.op().table.predicates[0]
-    assert pred.left.name == pred.right.name == 'time'
+        cases = [
+            star1.limit(10),
+            star1.limit(10, offset=5),
+            star1[star1.f > 0].limit(10),
 
+            # Semantically, this should produce a subquery
+            star1.limit(10)[lambda x: x.f > 0]
+        ]
 
-def test_asof_join_with_by():
-    left = ibis.table([('time', 'int32'), ('key', 'int32'), ('value', 'double')])
-    right = ibis.table([('time', 'int32'), ('key', 'int32'), ('value2', 'double')])
-    joined = api.asof_join(left, right, 'time', by='key')
-    assert joined.columns == [
-        "time_x",
-        "key_x",
-        "value",
-        "time_y",
-        "key_y",
-        "value2",
-    ]
-    by = joined.op().table.by[0]
-    assert by.left.name == by.right.name == 'key'
+        return cases
 
+    foo = _table_wrapper('foo')
+    bar = _table_wrapper('bar')
+    t1 = _table_wrapper('t1', 'foo')
+    t2 = _table_wrapper('t2', 'bar')
+
+    def _case_where_uncorrelated_subquery(self):
+        return self.foo[self.foo.job.isin(self.bar.job)]
+
+    def _case_where_correlated_subquery(self):
+        t1 = self.foo
+        t2 = t1.view()
+
+        stat = t2[t1.dept_id == t2.dept_id].y.mean()
+        return t1[t1.y > stat]
+
+    def _case_exists(self):
+        t1, t2 = self.t1, self.t2
+
+        cond = (t1.key1 == t2.key1).any()
+        expr = t1[cond]
+
+        cond2 = ((t1.key1 == t2.key1) & (t2.key2 == 'foo')).any()
+        expr2 = t1[cond2]
+
+        return expr, expr2
+
+    def _case_not_exists(self):
+        t1, t2 = self.t1, self.t2
+
+        cond = (t1.key1 == t2.key1).any()
+        return t1[-cond]
+
+    def _case_join_with_limited_table(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        limited = t1.limit(100)
+        joined = (limited.inner_join(t2, [limited.foo_id == t2.foo_id])
+                  [[limited]])
+        return joined
+
+    def _case_union(self, distinct=False):
+        table = self.con.table('functional_alltypes')
+
+        t1 = (table[table.int_col > 0]
+              [table.string_col.name('key'),
+               table.float_col.cast('double').name('value')])
+        t2 = (table[table.int_col <= 0]
+                   [table.string_col.name('key'),
+                    table.double_col.name('value')])
+
+        expr = t1.union(t2, distinct=distinct)
+
+        return expr
+
+    def _case_simple_case(self):
+        t = self.con.table('alltypes')
+        return (t.g.case()
+                .when('foo', 'bar')
+                .when('baz', 'qux')
+                .else_('default')
+                .end())
+
+    def _case_search_case(self):
+        t = self.con.table('alltypes')
+        return (ibis.case()
+                .when(t.f > 0, t.d * 2)
+                .when(t.c < 0, t.a * 2)
+                .end())
+
+    def _case_self_reference_in_exists(self):
+        t = self.con.table('functional_alltypes')
+        t2 = t.view()
+
+        cond = (t.string_col == t2.string_col).any()
+        semi = t[cond]
+        anti = t[-cond]
+
+        return semi, anti
+
+    def _case_self_reference_limit_exists(self):
+        alltypes = self.con.table('functional_alltypes')
+        t = alltypes.limit(100)
+        t2 = t.view()
+        return t[-(t.string_col == t2.string_col).any()]
+
+    def _case_limit_cte_extract(self):
+        alltypes = self.con.table('functional_alltypes')
+        t = alltypes.limit(100)
+        t2 = t.view()
+        return t.join(t2).projection(t)
+
+    def _case_subquery_aliased(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        agged = t1.aggregate([t1.f.sum().name('total')], by=['foo_id'])
+        what = (agged.inner_join(t2, [agged.foo_id == t2.foo_id])
+                [agged, t2.value1])
+
+        return what
+
+    def _case_filter_self_join_analysis_bug(self):
+        purchases = ibis.table([('region', 'string'),
+                                ('kind', 'string'),
+                                ('user', 'int64'),
+                                ('amount', 'double')], 'purchases')
+
+        metric = purchases.amount.sum().name('total')
+        agged = (purchases.group_by(['region', 'kind'])
+                 .aggregate(metric))
+
+        left = agged[agged.kind == 'foo']
+        right = agged[agged.kind == 'bar']
+
+        joined = left.join(right, left.region == right.region)
+        result = joined[left.region,
+                        (left.total - right.total).name('diff')]
+
+        return result, purchases
+
+    def _case_projection_fuse_filter(self):
+        # Probably test this during the evaluation phase. In SQL, "fusable"
+        # table operations will be combined together into a single select
+        # statement
+        #
+        # see ibis #71 for more on this
+
+        t = ibis.table([
+            ('a', 'int8'),
+            ('b', 'int16'),
+            ('c', 'int32'),
+            ('d', 'int64'),
+            ('e', 'float'),
+            ('f', 'double'),
+            ('g', 'string'),
+            ('h', 'boolean')
+        ], 'foo')
+
+        proj = t['a', 'b', 'c']
+
+        # Rewrite a little more aggressively here
+        expr1 = proj[t.a > 0]
+
+        # at one point these yielded different results
+        filtered = t[t.a > 0]
+
+        expr2 = filtered[t.a, t.b, t.c]
+        expr3 = filtered.projection(['a', 'b', 'c'])
+
+        return expr1, expr2, expr3
+
+
+class TestSelectSQL(unittest.TestCase, ExprTestCases):
+
+    @classmethod
+    def setUpClass(cls):
+        cls.con = MockConnection()
+
+    def _compare_sql(self, expr, expected):
+        result = to_sql(expr)
+        assert result == expected
+
+    def test_nameless_table(self):
+        # Ensure that user gets some kind of sensible error
+        nameless = api.table([('key', 'string')])
+        self.assertRaises(com.RelationError, to_sql, nameless)
+
+        with_name = api.table([('key', 'string')], name='baz')
+        result = to_sql(with_name)
+        assert result == 'SELECT *\nFROM baz'
+
+    def test_physical_table_reference_translate(self):
+        # If an expression's table leaves all reference database tables, verify
+        # we translate correctly
+        table = self.con.table('alltypes')
+
+        query = _get_query(table)
+        sql_string = query.compile()
+        expected = "SELECT *\nFROM alltypes"
+        assert sql_string == expected
+
+    def test_simple_joins(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        pred = t1['foo_id'] == t2['foo_id']
+        pred2 = t1['bar_id'] == t2['foo_id']
+        cases = [
+            (t1.inner_join(t2, [pred])[[t1]],
+             """SELECT t0.*
+FROM star1 t0
+  INNER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""),
+            (t1.left_join(t2, [pred])[[t1]],
+             """SELECT t0.*
+FROM star1 t0
+  LEFT OUTER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""),
+            (t1.outer_join(t2, [pred])[[t1]],
+             """SELECT t0.*
+FROM star1 t0
+  FULL OUTER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""),
+            # multiple predicates
+            (t1.inner_join(t2, [pred, pred2])[[t1]],
+             """SELECT t0.*
+FROM star1 t0
+  INNER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id` AND
+       t0.`bar_id` = t1.`foo_id`"""),
+        ]
 
-@pytest.mark.parametrize(
-    ('ibis_interval', 'timedelta_interval'),
-    [
-        [ibis.interval(days=2), pd.Timedelta('2 days')],
-        [ibis.interval(days=2), datetime.timedelta(days=2)],
-        [ibis.interval(hours=5), pd.Timedelta('5 hours')],
-        [ibis.interval(hours=5), datetime.timedelta(hours=5)],
-        [ibis.interval(minutes=7), pd.Timedelta('7 minutes')],
-        [ibis.interval(minutes=7), datetime.timedelta(minutes=7)],
-        [ibis.interval(seconds=9), pd.Timedelta('9 seconds')],
-        [ibis.interval(seconds=9), datetime.timedelta(seconds=9)],
-        [ibis.interval(milliseconds=11), pd.Timedelta('11 milliseconds')],
-        [ibis.interval(milliseconds=11), datetime.timedelta(milliseconds=11)],
-        [ibis.interval(microseconds=15), pd.Timedelta('15 microseconds')],
-        [ibis.interval(microseconds=15), datetime.timedelta(microseconds=15)],
-        [ibis.interval(nanoseconds=17), pd.Timedelta('17 nanoseconds')],
-    ],
+        for expr, expected_sql in cases:
+            result_sql = to_sql(expr)
+            assert result_sql == expected_sql
+
+    def test_multiple_joins(self):
+        what = self._case_multiple_joins()
+
+        result_sql = to_sql(what)
+        expected_sql = """SELECT t0.*, t1.`value1`, t2.`value2`
+FROM star1 t0
+  LEFT OUTER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`
+  INNER JOIN star3 t2
+    ON t0.`bar_id` = t2.`bar_id`"""
+        assert result_sql == expected_sql
+
+    def test_join_between_joins(self):
+        projected = self._case_join_between_joins()
+
+        result = to_sql(projected)
+        expected = """SELECT t0.*, t1.`value3`, t1.`value4`
+FROM (
+  SELECT t2.*, t3.`value2`
+  FROM `first` t2
+    INNER JOIN second t3
+      ON t2.`key1` = t3.`key1`
+) t0
+  INNER JOIN (
+    SELECT t2.*, t3.`value4`
+    FROM third t2
+      INNER JOIN fourth t3
+        ON t2.`key3` = t3.`key3`
+  ) t1
+    ON t0.`key2` = t1.`key2`"""
+        assert result == expected
+
+    def test_join_just_materialized(self):
+        joined = self._case_join_just_materialized()
+        result = to_sql(joined)
+        expected = """SELECT *
+FROM tpch_nation t0
+  INNER JOIN tpch_region t1
+    ON t0.`n_regionkey` = t1.`r_regionkey`
+  INNER JOIN tpch_customer t2
+    ON t0.`n_nationkey` = t2.`c_nationkey`"""
+        assert result == expected
+
+        result = to_sql(joined.materialize())
+        assert result == expected
+
+    def test_join_no_predicates_for_impala(self):
+        # Impala requires that joins without predicates be written explicitly
+        # as CROSS JOIN, since result sets can accidentally get too large if a
+        # query is executed before predicates are written
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        joined2 = t1.cross_join(t2)[[t1]]
+
+        expected = """SELECT t0.*
+FROM star1 t0
+  CROSS JOIN star2 t1"""
+        result2 = to_sql(joined2)
+        assert result2 == expected
+
+        for jtype in ['inner_join', 'left_join', 'outer_join']:
+            joined = getattr(t1, jtype)(t2)[[t1]]
+
+            result = to_sql(joined)
+            assert result == expected
+
+    def test_semi_anti_joins(self):
+        sj, aj = self._case_semi_anti_joins()
+
+        result = to_sql(sj)
+        expected = """SELECT t0.*
+FROM star1 t0
+  LEFT SEMI JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""
+        assert result == expected
+
+        result = to_sql(aj)
+        expected = """SELECT t0.*
+FROM star1 t0
+  LEFT ANTI JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""
+        assert result == expected
+
+    def test_self_reference_simple(self):
+        expr = self._case_self_reference_simple()
+
+        result_sql = to_sql(expr)
+        expected_sql = "SELECT *\nFROM star1"
+        assert result_sql == expected_sql
+
+    def test_join_self_reference(self):
+        result = self._case_self_reference_join()
+
+        result_sql = to_sql(result)
+        expected_sql = """SELECT t0.*
+FROM star1 t0
+  INNER JOIN star1 t1
+    ON t0.`foo_id` = t1.`bar_id`"""
+        assert result_sql == expected_sql
+
+    def test_join_projection_subquery_broken_alias(self):
+        expr = self._case_join_projection_subquery_bug()
+
+        result = to_sql(expr)
+        expected = """SELECT t1.*, t0.*
+FROM (
+  SELECT t2.`n_nationkey`, t2.`n_name` AS `nation`, t3.`r_name` AS `region`
+  FROM nation t2
+    INNER JOIN region t3
+      ON t2.`n_regionkey` = t3.`r_regionkey`
+) t0
+  INNER JOIN customer t1
+    ON t0.`n_nationkey` = t1.`c_nationkey`"""
+        assert result == expected
+
+    def test_where_simple_comparisons(self):
+        what = self._case_where_simple_comparisons()
+        result = to_sql(what)
+        expected = """SELECT *
+FROM star1
+WHERE `f` > 0 AND
+      `c` < (`f` * 2)"""
+        assert result == expected
+
+    def test_where_in_array_literal(self):
+        # e.g.
+        # where string_col in (v1, v2, v3)
+        raise unittest.SkipTest
+
+    def test_where_with_join(self):
+        e1, e2 = self._case_where_with_join()
+
+        expected_sql = """SELECT t0.*, t1.`value1`, t1.`value3`
+FROM star1 t0
+  INNER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`
+WHERE t0.`f` > 0 AND
+      t1.`value3` < 1000"""
+
+        result_sql = to_sql(e1)
+        assert result_sql == expected_sql
+
+        result2_sql = to_sql(e2)
+        assert result2_sql == expected_sql
+
+    def test_where_no_pushdown_possible(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        joined = (t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+                  [t1, (t1.f - t2.value1).name('diff')])
+
+        filtered = joined[joined.diff > 1]
+
+        # TODO: I'm not sure if this is exactly what we want
+        expected_sql = """SELECT *
+FROM (
+  SELECT t0.*, t0.`f` - t1.`value1` AS `diff`
+  FROM star1 t0
+    INNER JOIN star2 t1
+      ON t0.`foo_id` = t1.`foo_id`
+  WHERE t0.`f` > 0 AND
+        t1.`value3` < 1000
 )
-def test_asof_join_with_tolerance(ibis_interval, timedelta_interval):
-    left = ibis.table([('time', 'int32'), ('key', 'int32'), ('value', 'double')])
-    right = ibis.table([('time', 'int32'), ('key', 'int32'), ('value2', 'double')])
-
-    joined = api.asof_join(left, right, 'time', tolerance=ibis_interval).op()
-    tolerance = joined.table.tolerance
-    assert_equal(tolerance, ibis_interval.op())
-
-    joined = api.asof_join(left, right, 'time', tolerance=timedelta_interval).op()
-    tolerance = joined.table.tolerance
-    assert isinstance(tolerance.to_expr(), ir.IntervalScalar)
-    assert isinstance(tolerance, ops.Literal)
-
-
-def test_equijoin_schema_merge():
-    table1 = ibis.table([('key1', 'string'), ('value1', 'double')])
-    table2 = ibis.table([('key2', 'string'), ('stuff', 'int32')])
-
-    pred = table1['key1'] == table2['key2']
-    join_types = ['inner_join', 'left_join', 'outer_join']
-
-    ex_schema = sch.schema(
-        ['key1', 'value1', 'key2', 'stuff'],
-        ['string', 'double', 'string', 'int32'],
-    )
-
-    for fname in join_types:
-        f = getattr(table1, fname)
-        joined = f(table2, [pred])
-        assert_equal(joined.schema(), ex_schema)
-
-
-def test_join_combo_with_projection(table):
-    # Test a case where there is column name overlap, but the projection
-    # passed makes it a non-issue. Highly relevant with self-joins
-    #
-    # For example, where left/right have some field names in common:
-    # SELECT left.*, right.a, right.b
-    # FROM left join right on left.key = right.key
-    t = table
-    t2 = t.mutate(foo=t.f * 2, bar=t.f * 4)
+WHERE `diff` > 1"""
 
-    # this works
-    joined = t.left_join(t2, [t['g'] == t2['g']])
-    proj = joined.select([t, t2['foo'], t2['bar']])
-    repr(proj)
+        raise unittest.SkipTest
 
+        result_sql = to_sql(filtered)
+        assert result_sql == expected_sql
 
-def test_join_getitem_projection(con):
-    region = con.table('tpch_region')
-    nation = con.table('tpch_nation')
-
-    pred = region.r_regionkey == nation.n_regionkey
-    joined = region.inner_join(nation, pred)
-
-    result = joined[nation]
-    expected = joined.select(nation)
-    assert_equal(result, expected)
-
-
-def test_self_join(table):
-    # Self-joins are problematic with this design because column
-    # expressions may reference either the left or right  For example:
-    #
-    # SELECT left.key, sum(left.value - right.value) as total_deltas
-    # FROM table left
-    #  INNER JOIN table right
-    #    ON left.current_period = right.previous_period + 1
-    # GROUP BY 1
-    #
-    # One way around the self-join issue is to force the user to add
-    # prefixes to the joined fields, then project using those. Not that
-    # satisfying, though.
-    left = table
-    right = table.view()
-    metric = (left['a'] - right['b']).mean().name('metric')
-
-    joined = left.inner_join(right, [right['g'] == left['g']])
-
-    # Project out left table schema
-    proj = joined[[left]]
-    assert_equal(proj.schema(), left.schema())
-
-    # Try aggregating on top of joined
-    aggregated = joined.aggregate([metric], by=[left['g']])
-    ex_schema = api.Schema({'g': 'string', 'metric': 'double'})
-    assert_equal(aggregated.schema(), ex_schema)
-
-
-def test_self_join_no_view_convenience(table):
-    # #165, self joins ought to be possible when the user specifies the
-    # column names to join on rather than referentially-valid expressions
-
-    result = table.join(table, [('g', 'g')])
-    expected_cols = [f"{c}_x" if c != 'g' else 'g' for c in table.columns]
-    expected_cols.extend(f"{c}_y" for c in table.columns if c != 'g')
-    assert result.columns == expected_cols
-
-
-def test_join_reference_bug(con):
-    # GH#403
-    orders = con.table('tpch_orders')
-    customer = con.table('tpch_customer')
-    lineitem = con.table('tpch_lineitem')
-
-    items = orders.join(lineitem, orders.o_orderkey == lineitem.l_orderkey)[
-        lineitem, orders.o_custkey, orders.o_orderpriority
-    ].join(customer, [('o_custkey', 'c_custkey')])
-    items['o_orderpriority'].value_counts()
-
-
-def test_join_project_after(table):
-    # e.g.
-    #
-    # SELECT L.foo, L.bar, R.baz, R.qux
-    # FROM table1 L
-    #   INNER JOIN table2 R
-    #     ON L.key = R.key
-    #
-    # or
-    #
-    # SELECT L.*, R.baz
-    # ...
-    #
-    # The default for a join is selecting all fields if possible
-    table1 = ibis.table([('key1', 'string'), ('value1', 'double')])
-    table2 = ibis.table([('key2', 'string'), ('stuff', 'int32')])
-
-    pred = table1['key1'] == table2['key2']
-
-    joined = table1.left_join(table2, [pred])
-    projected = joined.select([table1, table2['stuff']])
-    assert projected.schema().names == ('key1', 'value1', 'stuff')
-
-    projected = joined.select([table2, table1['key1']])
-    assert projected.schema().names == ('key2', 'stuff', 'key1')
-
+    def test_where_with_between(self):
+        t = self.con.table('alltypes')
+
+        what = t.filter([t.a > 0, t.f.between(0, 1)])
+        result = to_sql(what)
+        expected = """SELECT *
+FROM alltypes
+WHERE `a` > 0 AND
+      `f` BETWEEN 0 AND 1"""
+        assert result == expected
+
+    def test_where_analyze_scalar_op(self):
+        # root cause of #310
+
+        table = self.con.table('functional_alltypes')
+
+        expr = (table.filter([table.timestamp_col <
+                             (ibis.timestamp('2010-01-01') + ibis.month(3)),
+                             table.timestamp_col < (ibis.now() +
+                                                    ibis.day(10))])
+                .count())
+
+        result = to_sql(expr)
+        expected = """\
+SELECT count(*) AS `count`
+FROM functional_alltypes
+WHERE `timestamp_col` < months_add('2010-01-01 00:00:00', 3) AND
+      `timestamp_col` < days_add(now(), 10)"""
+        assert result == expected
+
+    def test_bug_duplicated_where(self):
+        # GH #539
+        table = self.con.table('airlines')
+
+        t = table['arrdelay', 'dest']
+        expr = (t.group_by('dest')
+                .mutate(dest_avg=t.arrdelay.mean(),
+                        dev=t.arrdelay - t.arrdelay.mean()))
+
+        worst = expr[expr.dev.notnull()].sort_by(ibis.desc('dev')).limit(10)
+        result = to_sql(worst)
+        expected = """\
+SELECT *
+FROM (
+  SELECT `arrdelay`, `dest`,
+         avg(`arrdelay`) OVER (PARTITION BY `dest`) AS `dest_avg`,
+         `arrdelay` - avg(`arrdelay`) OVER (PARTITION BY `dest`) AS `dev`
+  FROM airlines
+) t0
+WHERE `dev` IS NOT NULL
+ORDER BY `dev` DESC
+LIMIT 10"""
+        assert result == expected
+
+    def test_simple_aggregate_query(self):
+        expected = [
+            """SELECT `foo_id`, sum(`f`) AS `total`
+FROM star1
+GROUP BY 1""",
+            """SELECT `foo_id`, `bar_id`, sum(`f`) AS `total`
+FROM star1
+GROUP BY 1, 2"""
+        ]
 
-def test_semi_join_schema(table):
-    # A left semi join discards the schema of the right table
-    table1 = ibis.table([('key1', 'string'), ('value1', 'double')])
-    table2 = ibis.table([('key2', 'string'), ('stuff', 'double')])
+        cases = self._case_simple_aggregate_query()
+        for expr, expected_sql in zip(cases, expected):
+            result_sql = to_sql(expr)
+            assert result_sql == expected_sql
+
+    def test_aggregate_having(self):
+        e1, e2 = self._case_aggregate_having()
+
+        result = to_sql(e1)
+        expected = """SELECT `foo_id`, sum(`f`) AS `total`
+FROM star1
+GROUP BY 1
+HAVING sum(`f`) > 10"""
+        assert result == expected
+
+        result = to_sql(e2)
+        expected = """SELECT `foo_id`, sum(`f`) AS `total`
+FROM star1
+GROUP BY 1
+HAVING count(*) > 100"""
+        assert result == expected
+
+    def test_aggregate_table_count_metric(self):
+        expr = self.con.table('star1').count()
+
+        result = to_sql(expr)
+        expected = """SELECT count(*) AS `count`
+FROM star1"""
+        assert result == expected
+
+    def test_aggregate_count_joined(self):
+        expr = self._case_aggregate_count_joined()
+
+        result = to_sql(expr)
+        expected = """SELECT count(*) AS `count`
+FROM (
+  SELECT t2.*, t1.`r_name` AS `region`
+  FROM tpch_region t1
+    INNER JOIN tpch_nation t2
+      ON t1.`r_regionkey` = t2.`n_regionkey`
+) t0"""
+        assert result == expected
+
+    def test_expr_template_field_name_binding(self):
+        # Given an expression with no concrete links to actual database tables,
+        # indicate a mapping between the distinct unbound table leaves of the
+        # expression and some database tables with compatible schemas but
+        # potentially different column names
+        pass
 
-    pred = table1['key1'] == table2['key2']
-    semi_joined = table1.semi_join(table2, [pred])
+    def test_no_aliases_needed(self):
+        table = api.table([
+            ('key1', 'string'),
+            ('key2', 'string'),
+            ('value', 'double')
+        ])
 
-    result_schema = semi_joined.schema()
-    assert_equal(result_schema, table1.schema())
+        expr = table.aggregate([table['value'].sum().name('total')],
+                               by=['key1', 'key2'])
 
+        query = _get_query(expr)
+        context = query.context
+        assert not context.need_aliases()
 
-def test_cross_join(table):
-    metrics = [
-        table['a'].sum().name('sum_a'),
-        table['b'].mean().name('mean_b'),
-    ]
-    scalar_aggs = table.aggregate(metrics)
+    def test_table_names_overlap_default_aliases(self):
+        # see discussion in #104; this actually is not needed for query
+        # correctness, and only makes the generated SQL nicer
+        raise unittest.SkipTest
 
-    joined = table.cross_join(scalar_aggs)
-    agg_schema = api.Schema({'sum_a': 'int64', 'mean_b': 'double'})
-    with pytest.warns(FutureWarning):
-        ex_schema = table.schema().merge(agg_schema)
-    assert_equal(joined.schema(), ex_schema)
+        t0 = api.table([
+            ('key', 'string'),
+            ('v1', 'double')
+        ], 't1')
 
+        t1 = api.table([
+            ('key', 'string'),
+            ('v2', 'double')
+        ], 't0')
 
-def test_cross_join_multiple(table):
-    a = table['a', 'b', 'c']
-    b = table['d', 'e']
-    c = table['f', 'h']
+        expr = t0.join(t1, t0.key == t1.key)[t0.key, t0.v1, t1.v2]
 
-    joined = ibis.cross_join(a, b, c)
-    expected = a.cross_join(b.cross_join(c))
-    assert joined.equals(expected)
+        result = to_sql(expr)
+        expected = """\
+SELECT t2.`key`, t2.`v1`, t3.`v2`
+FROM t0 t2
+  INNER JOIN t1 t3
+    ON t2.`key` = t3.`key`"""
 
+        assert result == expected
 
-def test_filter_join():
-    table1 = ibis.table({'key1': 'string', 'key2': 'string', 'value1': 'double'})
-    table2 = ibis.table({'key3': 'string', 'value2': 'double'})
+    def test_context_aliases_multiple_join(self):
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+        t3 = self.con.table('star3')
 
-    # It works!
-    joined = table1.inner_join(table2, [table1['key1'] == table2['key3']])
-    filtered = joined.filter([table1.value1 > 0])
-    repr(filtered)
+        expr = (t1.left_join(t2, [t1['foo_id'] == t2['foo_id']])
+                .inner_join(t3, [t1['bar_id'] == t3['bar_id']])
+                [[t1, t2['value1'], t3['value2']]])
 
+        query = _get_query(expr)
+        context = query.context
 
-def test_inner_join_overlapping_column_names():
-    t1 = ibis.table([('foo', 'string'), ('bar', 'string'), ('value1', 'double')])
-    t2 = ibis.table([('foo', 'string'), ('bar', 'string'), ('value2', 'double')])
+        assert context.get_ref(t1) == 't0'
+        assert context.get_ref(t2) == 't1'
+        assert context.get_ref(t3) == 't2'
 
-    joined = t1.join(t2, 'foo')
-    expected = t1.join(t2, t1.foo == t2.foo)
-    assert_equal(joined, expected)
-    assert joined.columns == ["foo", "bar_x", "value1", "bar_y", "value2"]
+    def test_fuse_projections(self):
+        table = api.table([
+            ('foo', 'int32'),
+            ('bar', 'int64'),
+            ('value', 'double')
+        ], name='tbl')
 
-    joined = t1.join(t2, ['foo', 'bar'])
-    expected = t1.join(t2, [t1.foo == t2.foo, t1.bar == t2.bar])
-    assert_equal(joined, expected)
-    assert joined.columns == ["foo", "bar", "value1", "value2"]
+        # Cases where we project in both cases using the base table reference
+        f1 = (table['foo'] + table['bar']).name('baz')
+        pred = table['value'] > 0
 
-    # Equality predicates don't have same name, need to rename
-    joined = t1.join(t2, t1.foo == t2.bar)
-    assert joined.columns == ["foo_x", "bar_x", "value1", "foo_y", "bar_y", "value2"]
+        table2 = table[table, f1]
+        table2_filtered = table2[pred]
 
-    # Not all predicates are equality, still need to rename
-    joined = t1.join(t2, ["foo", t1.value1 < t2.value2])
-    assert joined.columns == ["foo_x", "bar_x", "value1", "foo_y", "bar_y", "value2"]
+        f2 = (table2['foo'] * 2).name('qux')
+        f3 = (table['foo'] * 2).name('qux')
 
+        table3 = table2.projection([table2, f2])
 
-def test_join_key_alternatives(con):
-    t1 = con.table('star1')
-    t2 = con.table('star2')
+        # fusion works even if there's a filter
+        table3_filtered = table2_filtered.projection([table2, f2])
 
-    # Join with tuples
-    joined = t1.inner_join(t2, [('foo_id', 'foo_id')])
-    joined2 = t1.inner_join(t2, [(t1.foo_id, t2.foo_id)])
+        expected = table[table, f1, f3]
+        expected2 = table[pred][table, f1, f3]
 
-    # Join with single expr
-    joined3 = t1.inner_join(t2, t1.foo_id == t2.foo_id)
+        assert table3.equals(expected)
+        assert table3_filtered.equals(expected2)
 
-    expected = t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+        ex_sql = """SELECT *, `foo` + `bar` AS `baz`, `foo` * 2 AS `qux`
+FROM tbl"""
 
-    assert_equal(joined, expected)
-    assert_equal(joined2, expected)
-    assert_equal(joined3, expected)
+        ex_sql2 = """SELECT *, `foo` + `bar` AS `baz`, `foo` * 2 AS `qux`
+FROM tbl
+WHERE `value` > 0"""
 
-    with pytest.raises(com.ExpressionError):
-        t1.inner_join(t2, [('foo_id', 'foo_id', 'foo_id')])
+        table3_sql = to_sql(table3)
+        table3_filt_sql = to_sql(table3_filtered)
 
+        assert table3_sql == ex_sql
+        assert table3_filt_sql == ex_sql2
 
-def test_join_invalid_refs(con):
-    t1 = con.table('star1')
-    t2 = con.table('star2')
-    t3 = con.table('star3')
+        # Use the intermediate table refs
+        table3 = table2.projection([table2, f2])
 
-    predicate = t1.bar_id == t3.bar_id
-    with pytest.raises(com.RelationError):
-        t1.inner_join(t2, [predicate])
+        # fusion works even if there's a filter
+        table3_filtered = table2_filtered.projection([table2, f2])
 
+        expected = table[table, f1, f3]
+        expected2 = table[pred][table, f1, f3]
 
-def test_join_invalid_expr_type(con):
-    left = con.table('star1')
-    invalid_right = left.foo_id
-    join_key = ['bar_id']
+        assert table3.equals(expected)
+        assert table3_filtered.equals(expected2)
 
-    with pytest.raises(com.IbisTypeError, match="Argument is not a table"):
-        left.inner_join(invalid_right, join_key)
+    def test_projection_filter_fuse(self):
+        expr1, expr2, expr3 = self._case_projection_fuse_filter()
 
+        sql1 = to_sql(expr1)
+        sql2 = to_sql(expr2)
+        sql3 = to_sql(expr3)
 
-def test_join_non_boolean_expr(con):
-    t1 = con.table('star1')
-    t2 = con.table('star2')
+        assert sql1 == sql2
+        assert sql1 == sql3
 
-    # oops
-    predicate = t1.f * t2.value1
-    with pytest.raises(com.ExpressionError):
-        t1.inner_join(t2, [predicate])
+    def test_bug_project_multiple_times(self):
+        # 108
+        customer = self.con.table('tpch_customer')
+        nation = self.con.table('tpch_nation')
+        region = self.con.table('tpch_region')
 
+        joined = (
+            customer.inner_join(nation,
+                                [customer.c_nationkey == nation.n_nationkey])
+            .inner_join(region,
+                        [nation.n_regionkey == region.r_regionkey])
+        )
+        proj1 = [customer, nation.n_name, region.r_name]
+        step1 = joined[proj1]
 
-def test_unravel_compound_equijoin(table):
-    t1 = ibis.table(
-        [
-            ('key1', 'string'),
-            ('key2', 'string'),
-            ('key3', 'string'),
-            ('value1', 'double'),
-        ],
-        'foo_table',
-    )
+        topk_by = step1.c_acctbal.cast('double').sum()
+        pred = step1.n_name.topk(10, by=topk_by)
 
-    t2 = ibis.table(
-        [
+        proj_exprs = [step1.c_name, step1.r_name, step1.n_name]
+        step2 = step1[pred]
+        expr = step2.projection(proj_exprs)
+
+        # it works!
+        result = to_sql(expr)
+        expected = """\
+SELECT `c_name`, `r_name`, `n_name`
+FROM (
+  SELECT t1.*, t2.`n_name`, t3.`r_name`
+  FROM tpch_customer t1
+    INNER JOIN tpch_nation t2
+      ON t1.`c_nationkey` = t2.`n_nationkey`
+    INNER JOIN tpch_region t3
+      ON t2.`n_regionkey` = t3.`r_regionkey`
+    LEFT SEMI JOIN (
+      SELECT t2.`n_name`, sum(CAST(t1.`c_acctbal` AS double)) AS `sum`
+      FROM tpch_customer t1
+        INNER JOIN tpch_nation t2
+          ON t1.`c_nationkey` = t2.`n_nationkey`
+        INNER JOIN tpch_region t3
+          ON t2.`n_regionkey` = t3.`r_regionkey`
+      GROUP BY 1
+      ORDER BY `sum` DESC
+      LIMIT 10
+    ) t4
+      ON t2.`n_name` = t4.`n_name`
+) t0"""
+        assert result == expected
+
+    def test_aggregate_projection_subquery(self):
+        t = self.con.table('alltypes')
+
+        proj = t[t.f > 0][t, (t.a + t.b).name('foo')]
+
+        result = to_sql(proj)
+        expected = """SELECT *, `a` + `b` AS `foo`
+FROM alltypes
+WHERE `f` > 0"""
+        assert result == expected
+
+        def agg(x):
+            return x.aggregate([x.foo.sum().name('foo total')], by=['g'])
+
+        # predicate gets pushed down
+        filtered = proj[proj.g == 'bar']
+
+        result = to_sql(filtered)
+        expected = """SELECT *, `a` + `b` AS `foo`
+FROM alltypes
+WHERE `f` > 0 AND
+      `g` = 'bar'"""
+        assert result == expected
+
+        agged = agg(filtered)
+        result = to_sql(agged)
+        expected = """SELECT `g`, sum(`foo`) AS `foo total`
+FROM (
+  SELECT *, `a` + `b` AS `foo`
+  FROM alltypes
+  WHERE `f` > 0 AND
+        `g` = 'bar'
+) t0
+GROUP BY 1"""
+        assert result == expected
+
+        # Pushdown is not possible (in Impala, Postgres, others)
+        agged2 = agg(proj[proj.foo < 10])
+
+        result = to_sql(agged2)
+        expected = """SELECT t0.`g`, sum(t0.`foo`) AS `foo total`
+FROM (
+  SELECT *, `a` + `b` AS `foo`
+  FROM alltypes
+  WHERE `f` > 0
+) t0
+WHERE t0.`foo` < 10
+GROUP BY 1"""
+        assert result == expected
+
+    def test_subquery_aliased(self):
+        case = self._case_subquery_aliased()
+
+        expected = """SELECT t0.*, t1.`value1`
+FROM (
+  SELECT `foo_id`, sum(`f`) AS `total`
+  FROM star1
+  GROUP BY 1
+) t0
+  INNER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""
+        self._compare_sql(case, expected)
+
+    def test_double_nested_subquery_no_aliases(self):
+        # We don't require any table aliasing anywhere
+        t = api.table([
             ('key1', 'string'),
             ('key2', 'string'),
             ('key3', 'string'),
-            ('value2', 'double'),
-        ],
-        'bar_table',
-    )
+            ('value', 'double')
+        ], 'foo_table')
 
-    p1 = t1.key1 == t2.key1
-    p2 = t1.key2 == t2.key2
-    p3 = t1.key3 == t2.key3
-
-    joined = t1.inner_join(t2, [p1 & p2 & p3])
-    expected = t1.inner_join(t2, [p1, p2, p3])
-    assert_equal(joined, expected)
-
-
-def test_union(
-    setops_table_foo,
-    setops_table_bar,
-    setops_table_baz,
-    setops_relation_error_message,
-):
-    result = setops_table_foo.union(setops_table_bar)
-    assert isinstance(result.op().table, ops.Union)
-    assert not result.op().table.distinct
-
-    result = setops_table_foo.union(setops_table_bar, distinct=True)
-    assert result.op().table.distinct
-
-    with pytest.raises(RelationError, match=setops_relation_error_message):
-        setops_table_foo.union(setops_table_baz)
-
-
-def test_intersection(
-    setops_table_foo,
-    setops_table_bar,
-    setops_table_baz,
-    setops_relation_error_message,
-):
-    result = setops_table_foo.intersect(setops_table_bar)
-    assert isinstance(result.op().table, ops.Intersection)
-
-    with pytest.raises(RelationError, match=setops_relation_error_message):
-        setops_table_foo.intersect(setops_table_baz)
-
-
-def test_difference(
-    setops_table_foo,
-    setops_table_bar,
-    setops_table_baz,
-    setops_relation_error_message,
-):
-    result = setops_table_foo.difference(setops_table_bar)
-    assert isinstance(result.op().table, ops.Difference)
-
-    with pytest.raises(RelationError, match=setops_relation_error_message):
-        setops_table_foo.difference(setops_table_baz)
-
-
-def test_column_ref_on_projection_rename(con):
-    region = con.table('tpch_region')
-    nation = con.table('tpch_nation')
-    customer = con.table('tpch_customer')
-
-    joined = region.inner_join(
-        nation, [region.r_regionkey == nation.n_regionkey]
-    ).inner_join(customer, [customer.c_nationkey == nation.n_nationkey])
-
-    proj_exprs = [
-        customer,
-        nation.n_name.name('nation'),
-        region.r_name.name('region'),
-    ]
-    joined = joined.select(proj_exprs)
-
-    metrics = [joined.c_acctbal.sum().name('metric')]
-
-    # it works!
-    joined.aggregate(metrics, by=['region'])
-
-
-@pytest.fixture
-def t1():
-    return ibis.table(
-        [('key1', 'string'), ('key2', 'string'), ('value1', 'double')], 'foo'
-    )
-
-
-@pytest.fixture
-def t2():
-    return ibis.table([('key1', 'string'), ('key2', 'string')], 'bar')
-
-
-@pytest.mark.parametrize(
-    ("func", "expected_type"),
-    [
-        param(
-            lambda t1, t2: (t1.key1 == t2.key1).any(),
-            ops.UnresolvedExistsSubquery,
-            id="exists",
-        ),
-        param(
-            lambda t1, t2: -(t1.key1 == t2.key1).any(),
-            ops.UnresolvedNotExistsSubquery,
-            id="not_exists",
-        ),
-        param(
-            lambda t1, t2: -(-(t1.key1 == t2.key1).any()),
-            ops.UnresolvedExistsSubquery,
-            id="not_not_exists",
-        ),
-    ],
+        agg1 = t.aggregate([t.value.sum().name('total')],
+                           by=['key1', 'key2', 'key3'])
+        agg2 = agg1.aggregate([agg1.total.sum().name('total')],
+                              by=['key1', 'key2'])
+        agg3 = agg2.aggregate([agg2.total.sum().name('total')],
+                              by=['key1'])
+
+        result = to_sql(agg3)
+        expected = """SELECT `key1`, sum(`total`) AS `total`
+FROM (
+  SELECT `key1`, `key2`, sum(`total`) AS `total`
+  FROM (
+    SELECT `key1`, `key2`, `key3`, sum(`value`) AS `total`
+    FROM foo_table
+    GROUP BY 1, 2, 3
+  ) t1
+  GROUP BY 1, 2
+) t0
+GROUP BY 1"""
+        assert result == expected
+
+    def test_aggregate_projection_alias_bug(self):
+        # Observed in use
+        t1 = self.con.table('star1')
+        t2 = self.con.table('star2')
+
+        what = (t1.inner_join(t2, [t1.foo_id == t2.foo_id])
+                [[t1, t2.value1]])
+
+        what = what.aggregate([what.value1.sum().name('total')],
+                              by=[what.foo_id])
+
+        # TODO: Not fusing the aggregation with the projection yet
+        result = to_sql(what)
+        expected = """SELECT `foo_id`, sum(`value1`) AS `total`
+FROM (
+  SELECT t1.*, t2.`value1`
+  FROM star1 t1
+    INNER JOIN star2 t2
+      ON t1.`foo_id` = t2.`foo_id`
+) t0
+GROUP BY 1"""
+        assert result == expected
+
+    def test_aggregate_fuse_with_projection(self):
+        # see above test case
+        pass
+
+    def test_subquery_used_for_self_join(self):
+        expr = self._case_subquery_used_for_self_join()
+
+        result = to_sql(expr)
+        expected = """WITH t0 AS (
+  SELECT `g`, `a`, `b`, sum(`f`) AS `total`
+  FROM alltypes
+  GROUP BY 1, 2, 3
 )
-def test_unresolved_existence_predicate(t1, t2, func, expected_type):
-    expr = func(t1, t2)
-    assert isinstance(expr, ir.BooleanColumn)
-
-    op = expr.op()
-    assert isinstance(op, expected_type)
-
-
-@pytest.mark.parametrize(
-    ("func", "expected_type", "expected_negated_type"),
-    [
-        param(
-            lambda t1, t2: t1[(t1.key1 == t2.key1).any()],
-            ops.ExistsSubquery,
-            ops.NotExistsSubquery,
-            id="exists",
-        ),
-        param(
-            lambda t1, t2: t1[-(t1.key1 == t2.key1).any()],
-            ops.NotExistsSubquery,
-            ops.ExistsSubquery,
-            id="not_exists",
-        ),
-        param(
-            lambda t1, t2: t1[-(-(t1.key1 == t2.key1).any())],
-            ops.ExistsSubquery,
-            ops.NotExistsSubquery,
-            id="not_not_exists",
-        ),
-    ],
+SELECT t0.`g`, max(t0.`total` - t1.`total`) AS `metric`
+FROM t0
+  INNER JOIN t0 t1
+    ON t0.`a` = t1.`b`
+GROUP BY 1"""
+        assert result == expected
+
+    def test_subquery_factor_correlated_subquery(self):
+        # #173, #183 and other issues
+
+        expr = self._case_subquery_factor_correlated_subquery()
+
+        result = to_sql(expr)
+        expected = """\
+WITH t0 AS (
+  SELECT t6.*, t1.`r_name` AS `region`, t3.`o_totalprice` AS `amount`,
+         CAST(t3.`o_orderdate` AS timestamp) AS `odate`
+  FROM tpch_region t1
+    INNER JOIN tpch_nation t2
+      ON t1.`r_regionkey` = t2.`n_regionkey`
+    INNER JOIN tpch_customer t6
+      ON t6.`c_nationkey` = t2.`n_nationkey`
+    INNER JOIN tpch_orders t3
+      ON t3.`o_custkey` = t6.`c_custkey`
 )
-def test_resolve_existence_predicate(
-    t1,
-    t2,
-    func,
-    expected_type,
-    expected_negated_type,
-):
-    expr = func(t1, t2)
-    op = expr.op()
-    assert isinstance(op, ops.Selection)
-
-    pred = op.predicates[0].to_expr()
-    assert isinstance(pred.op(), expected_type)
-    assert isinstance((-pred).op(), expected_negated_type)
-
-
-def test_aggregate_metrics(table):
-    functions = [
-        lambda x: x.e.sum().name('esum'),
-        lambda x: x.f.sum().name('fsum'),
-    ]
-    exprs = [table.e.sum().name('esum'), table.f.sum().name('fsum')]
-
-    result = table.aggregate(functions[0])
-    expected = table.aggregate(exprs[0])
-    assert_equal(result, expected)
-
-    result = table.aggregate(functions)
-    expected = table.aggregate(exprs)
-    assert_equal(result, expected)
-
-
-def test_group_by_keys(table):
-    m = table.mutate(foo=table.f * 2, bar=table.e / 2)
-
-    expr = m.group_by(lambda x: x.foo).size()
-    expected = m.group_by('foo').size()
-    assert_equal(expr, expected)
-
-    expr = m.group_by([lambda x: x.foo, lambda x: x.bar]).size()
-    expected = m.group_by(['foo', 'bar']).size()
-    assert_equal(expr, expected)
-
-
-def test_having(table):
-    m = table.mutate(foo=table.f * 2, bar=table.e / 2)
-
-    expr = m.group_by('foo').having(lambda x: x.foo.sum() > 10).size()
-    expected = m.group_by('foo').having(m.foo.sum() > 10).size()
-
-    assert_equal(expr, expected)
-
-
-def test_filter(table):
-    m = table.mutate(foo=table.f * 2, bar=table.e / 2)
-
-    result = m.filter(lambda x: x.foo > 10)
-    result2 = m[lambda x: x.foo > 10]
-    expected = m[m.foo > 10]
-
-    assert_equal(result, expected)
-    assert_equal(result2, expected)
-
-    result = m.filter([lambda x: x.foo > 10, lambda x: x.bar < 0])
-    expected = m.filter([m.foo > 10, m.bar < 0])
-    assert_equal(result, expected)
-
-
-def test_order_by2(table):
-    m = table.mutate(foo=table.e + table.f)
-
-    result = m.order_by(lambda x: -x.foo)
-    expected = m.order_by(-m.foo)
-    assert_equal(result, expected)
-
-    result = m.order_by(lambda x: ibis.desc(x.foo))
-    expected = m.order_by(ibis.desc('foo'))
-    assert_equal(result, expected)
-
-    result = m.order_by(ibis.desc(lambda x: x.foo))
-    expected = m.order_by(ibis.desc('foo'))
-    assert_equal(result, expected)
-
-    result = m.order_by(ibis.asc(lambda x: x.foo))
-    expected = m.order_by('foo')
-    assert_equal(result, expected)
-
-
-def test_projection2(table):
-    m = table.mutate(foo=table.f * 2)
-
-    def f(x):
-        return (x.foo * 2).name('bar')
-
-    result = m.select([f, 'f'])
-    result2 = m[f, 'f']
-    expected = m.select([f(m), 'f'])
-    assert_equal(result, expected)
-    assert_equal(result2, expected)
-
-
-def test_mutate2(table):
-    m = table.mutate(foo=table.f * 2)
-
-    def g(x):
-        return x.foo * 2
-
-    def h(x):
-        return x.bar * 2
-
-    result = m.mutate(bar=g).mutate(baz=h)
-
-    m2 = m.mutate(bar=g(m))
-    expected = m2.mutate(baz=h(m2))
-
-    assert_equal(result, expected)
-
-
-def test_groupby_mutate(table):
-    t = table
-
-    g = t.group_by('g').order_by('f')
-    expr = g.mutate(foo=lambda x: x.f.lag(), bar=lambda x: x.f.rank())
-    expected = g.mutate(foo=t.f.lag(), bar=t.f.rank())
-
-    assert_equal(expr, expected)
-
-
-def test_groupby_projection(table):
-    t = table
-
-    g = t.group_by('g').order_by('f')
-    expr = g.select([lambda x: x.f.lag().name('foo'), lambda x: x.f.rank().name('bar')])
-    expected = g.select([t.f.lag().name('foo'), t.f.rank().name('bar')])
-
-    assert_equal(expr, expected)
-
-
-def test_set_column(table):
-    def g(x):
-        return x.f * 2
-
-    with pytest.warns(FutureWarning, match=r"5\.1"):
-        result = table.set_column('f', g)
-    with pytest.warns(FutureWarning, match=r"6\.0"):
-        expected = table.set_column('f', table.f * 2)
-    assert_equal(result, expected)
-
-
-def test_pickle_table_expr():
-    schema = [('time', 'timestamp'), ('key', 'string'), ('value', 'double')]
-    t0 = ibis.table(schema, name='t0')
-    raw = pickle.dumps(t0, protocol=2)
-    t1 = pickle.loads(raw)
-    assert t1.equals(t0)
-
-
-def test_pickle_table_node(table):
-    n0 = table.op()
-    assert_pickle_roundtrip(n0)
-
-
-def test_pickle_projection_node(table):
-    m = table.mutate(foo=table.f * 2)
-
-    def f(x):
-        return (x.foo * 2).name('bar')
-
-    node = m.select([f, 'f']).op()
-
-    assert_pickle_roundtrip(node)
-
-
-def test_pickle_group_by(table):
-    m = table.mutate(foo=table.f * 2, bar=table.e / 2)
-    expr = m.group_by(lambda x: x.foo).size()
-    node = expr.op()
-
-    assert_pickle_roundtrip(node)
-
-
-def test_pickle_asof_join():
-    left = ibis.table([('time', 'int32'), ('value', 'double')])
-    right = ibis.table([('time', 'int32'), ('value2', 'double')])
-    joined = api.asof_join(left, right, 'time')
-    node = joined.op()
-
-    assert_pickle_roundtrip(node)
-
-
-def test_group_by_key_function():
-    t = ibis.table([('a', 'timestamp'), ('b', 'string'), ('c', 'double')])
-    expr = t.group_by(new_key=lambda t: t.b.length()).aggregate(foo=t.c.mean())
-    assert expr.columns == ['new_key', 'foo']
-
-
-def test_unbound_table_name():
-    t = ibis.table([('a', 'timestamp')])
-    name = t.op().name
-    match = re.match(r'^unbound_table_\d+$', name)
-    assert match is not None
-
-
-class MyTable:
-    a: int
-    b: str
-    c: List[float]
-
-
-def test_unbound_table_using_class_definition():
-    expected_schema = ibis.schema({'a': 'int64', 'b': 'string', 'c': 'array<double>'})
-
-    t1 = ibis.table(MyTable)
-    t2 = ibis.table(MyTable, name="MyNamedTable")
-
-    cases = {t1: "MyTable", t2: "MyNamedTable"}
-    for t, name in cases.items():
-        assert isinstance(t, ir.TableExpr)
-        assert isinstance(t.op(), ops.UnboundTable)
-        assert t.schema() == expected_schema
-        assert t.get_name() == name
-
-
-def test_mutate_chain():
-    one = ibis.table([('a', 'string'), ('b', 'string')], name='t')
-    two = one.mutate(b=lambda t: t.b.fillna('Short Term'))
-    three = two.mutate(a=lambda t: t.a.fillna('Short Term'))
-    a, b = three.op().selections
-
-    # we can't fuse these correctly yet
-    assert isinstance(a, ops.Alias)
-    assert isinstance(a.arg, ops.IfNull)
-    assert isinstance(b, ops.TableColumn)
-
-    expr = b.table.selections[1]
-    assert isinstance(expr, ops.Alias)
-    assert isinstance(expr.arg, ops.IfNull)
-
-
-# TODO(kszucs): move this test case to ibis/tests/sql since it requires the
-# sql backend to be executed
-def test_multiple_dbcon():
-    """Expr from multiple connections to same DB should be compatible."""
-    con1 = MockBackend()
-    con2 = MockBackend()
-
-    con1.table('alltypes').union(con2.table('alltypes')).execute()
-
-
-def test_multiple_db_different_backends():
-    con1 = MockBackend()
-    con2 = MockAlchemyBackend()
-
-    backend1_table = con1.table('alltypes')
-    backend2_table = con2.table('alltypes')
-
-    expr = backend1_table.union(backend2_table)
-    with pytest.raises(com.IbisError, match="Multiple backends"):
-        expr.compile()
-
-
-def test_merge_as_of_allows_overlapping_columns():
-    # GH3295
-    table = ibis.table(
-        [
-            ("field", "string"),
-            ("value", "float64"),
-            ("timestamp_received", "timestamp"),
-        ],
-        name="t",
-    )
-
-    signal_one = table[
-        table['field'].contains('signal_one') & table['field'].contains('current')
-    ]
-    signal_one = signal_one[
-        'value', 'timestamp_received', 'field'
-    ]  # select columns we care about
-    signal_one = signal_one.relabel({'value': 'current', 'field': 'signal_one'})
-
-    signal_two = table[
-        table['field'].contains('signal_two') & table['field'].contains('voltage')
-    ]
-    signal_two = signal_two[
-        'value', 'timestamp_received', 'field'
-    ]  # select columns we care about
-    signal_two = signal_two.relabel({'value': 'voltage', 'field': 'signal_two'})
-
-    merged = ibis.api.asof_join(signal_one, signal_two, 'timestamp_received')
-    assert merged.columns == [
-        'current',
-        'timestamp_received_x',
-        'signal_one',
-        'voltage',
-        'timestamp_received_y',
-        'signal_two',
-    ]
-
-
-def test_select_from_unambiguous_join_with_strings():
-    # GH1387
-    t = ibis.table([('a', 'int64'), ('b', 'string')])
-    s = ibis.table([('b', 'int64'), ('c', 'string')])
-    joined = t.left_join(s, [t.b == s.c])
-    expr = joined[t, 'c']
-    assert expr.columns == ["a", "b", "c"]
-
-
-def test_filter_applied_to_join():
-    # GH2437
-    countries = ibis.table([("iso_alpha3", "string")])
-    gdp = ibis.table([("country_code", "string"), ("year", "int64")])
-
-    expr = countries.inner_join(
-        gdp,
-        predicates=[countries["iso_alpha3"] == gdp["country_code"]],
-    ).filter(gdp["year"] == 2017)
-    assert expr.columns == ["iso_alpha3", "country_code", "year"]
-
-
-@pytest.mark.parametrize("how", ["inner", "left", "outer", "right"])
-def test_join_suffixes(how):
-    left = ibis.table([("id", "int64"), ("first_name", "string")])
-    right = ibis.table([("id", "int64"), ("last_name", "string")])
-
-    method = getattr(left, f"{how}_join")
-    expr = method(right, suffixes=("_left", "_right"))
-    assert expr.columns == ["id_left", "first_name", "id_right", "last_name"]
-
-
-def test_drop():
-    t = ibis.table(dict.fromkeys("abcd", "int"))
-
-    assert t.drop() is t
-
-    res = t.drop("a")
-    assert res.equals(t.select("b", "c", "d"))
-
-    res = t.drop("a", "b")
-    assert res.equals(t.select("c", "d"))
-
-    assert res.equals(t.select("c", "d"))
-
-    assert res.equals(t.drop(s.matches("a|b")))
-
-    with pytest.raises(KeyError):
-        t.drop("e")
-
-
-def test_python_table_ambiguous():
-    with pytest.raises(NotImplementedError):
-        ibis.memtable(
-            [(1,)],
-            schema=ibis.schema(dict(a="int8")),
-            columns=["a"],
-        )
-
-
-def test_memtable_filter():
-    # Mostly just a smoketest, this used to error on construction
-    t = ibis.memtable([(1, 2), (3, 4), (5, 6)], columns=["x", "y"])
-    expr = t.filter(t.x > 1)
-    assert expr.columns == ["x", "y"]
-
-
-def test_default_backend_with_unbound_table():
-    t = ibis.table(dict(a="int"), name="t")
-    expr = t.a.sum()
-
-    with pytest.raises(
-        com.IbisError,
-        match="Expression contains unbound tables",
-    ):
-        assert expr.execute()
-
-
-def test_numpy_ufuncs_dont_cast_tables():
-    t = ibis.table(dict.fromkeys("abcd", "int"))
-    for arg in [np.int64(1), np.array([1, 2, 3])]:
-        for left, right in [(t, arg), (arg, t)]:
-            with pytest.raises(TypeError):
-                left + right
-
-
-def test_array_string_compare():
-    t = ibis.table(schema=dict(by="string", words="array<string>"), name="t")
-    expr = t[t.by == "foo"].mutate(words=_.words.unnest()).filter(_.words == "the")
-    assert expr is not None
-
-
-@pytest.mark.parametrize("value", [True, False])
-@pytest.mark.parametrize(
-    "api",
-    [
-        param(lambda t, value: t[value], id="getitem"),
-        param(lambda t, value: t.filter(value), id="filter"),
-    ],
+SELECT t0.*
+FROM t0
+WHERE t0.`amount` > (
+  SELECT avg(t4.`amount`) AS `mean`
+  FROM t0 t4
+  WHERE t4.`region` = t0.`region`
 )
-def test_filter_with_literal(value, api):
-    t = ibis.table(dict(a="string"))
-    filt = api(t, ibis.literal(value))
-    assert filt is not None
-
-    # ints are invalid predicates
-    int_val = ibis.literal(int(value))
-    with pytest.raises((NotImplementedError, com.IbisTypeError)):
-        api(t, int_val)
-
-
-def test_cast():
-    t = ibis.table(dict(a="int", b="string", c="float"), name="t")
-
-    assert t.cast({"a": "string"}).equals(t.mutate(a=t.a.cast("string")))
-
-    with pytest.raises(
-        com.IbisError, match="fields that are not in the table: .+'d'.+"
-    ):
-        t.cast({"d": "array<int>"}).equals(t.select())
-
-    assert t.cast(ibis.schema({"a": "string", "b": "int"})).equals(
-        t.mutate(a=t.a.cast("string"), b=t.b.cast("int"))
-    )
-    assert t.cast([("a", "string"), ("b", "float")]).equals(
-        t.mutate(a=t.a.cast("string"), b=t.b.cast("float"))
-    )
-
-
-def test_pivot_longer():
-    diamonds = ibis.table(
-        {
-            'carat': 'float64',
-            'cut': 'string',
-            'color': 'string',
-            'clarity': 'string',
-            'depth': 'float64',
-            'table': 'float64',
-            'price': 'int64',
-            'x': 'float64',
-            'y': 'float64',
-            'z': 'float64',
-        },
-        name="diamonds",
-    )
-    res = diamonds.pivot_longer(s.c("x", "y", "z"), names_to="pos", values_to="xyz")
-    assert res.schema().names == (
-        "carat",
-        "cut",
-        "color",
-        "clarity",
-        "depth",
-        "table",
-        "price",
-        "pos",
-        "xyz",
-    )
-
-
-def test_pivot_longer_strip_prefix():
-    t = ibis.table(
-        dict(artist="string", track="string", wk1="int", wk2="int", wk3="int")
-    )
-    expr = t.pivot_longer(
-        s.startswith("wk"),
-        names_to="week",
-        names_pattern=r"wk(.+)",
-        names_transform=int,
-        values_to="rank",
-        values_transform=_.cast("int"),
-    )
-    schema = ibis.schema(dict(artist="string", track="string", week="int8", rank="int"))
-    assert expr.schema() == schema
-
-
-def test_pivot_longer_pluck_regex():
-    t = ibis.table(
-        dict(artist="string", track="string", x_wk1="int", x_wk2="int", x_wk3="int")
-    )
-    expr = t.pivot_longer(
-        s.matches("^.+wk.$"),
-        names_to=["other_var", "week"],
-        names_pattern=r"(.)_wk(\d)",
-        names_transform=dict(other_var=str.upper, week=int),
-        values_to="rank",
-        values_transform=_.cast("int"),
-    )
-    schema = ibis.schema(
-        dict(
-            artist="string", track="string", other_var="string", week="int8", rank="int"
-        )
-    )
-    assert expr.schema() == schema
+LIMIT 10"""
+        assert result == expected
 
+    def test_self_join_subquery_distinct_equal(self):
+        expr = self._case_self_join_subquery_distinct_equal()
 
-def test_pivot_longer_no_match():
-    t = ibis.table(
-        dict(artist="string", track="string", x_wk1="int", x_wk2="int", x_wk3="int")
-    )
-    with pytest.raises(
-        com.IbisInputError, match="Selector returned no columns to pivot on"
-    ):
-        t.pivot_longer(
-            s.matches("foo"),
-            names_to=["other_var", "week"],
-            names_pattern=r"(.)_wk(\d)",
-            names_transform=dict(other_var=str.upper, week=int),
-            values_to="rank",
-            values_transform=_.cast("int"),
-        )
+        result = to_sql(expr)
+        expected = """\
+WITH t0 AS (
+  SELECT t2.*, t3.*
+  FROM tpch_region t2
+    INNER JOIN tpch_nation t3
+      ON t2.`r_regionkey` = t3.`n_regionkey`
+)
+SELECT t0.`r_name`, t1.`n_name`
+FROM t0
+  INNER JOIN t0 t1
+    ON t0.`r_regionkey` = t1.`r_regionkey`"""
+
+        assert result == expected
+
+    def test_limit_with_self_join(self):
+        t = self.con.table('functional_alltypes')
+        t2 = t.view()
+
+        expr = t.join(t2, t.tinyint_col < t2.timestamp_col.minute()).count()
+
+        # it works
+        result = to_sql(expr)
+        expected = """\
+SELECT count(*) AS `count`
+FROM functional_alltypes t0
+  INNER JOIN functional_alltypes t1
+    ON t0.`tinyint_col` < extract(t1.`timestamp_col`, 'minute')"""
+        assert result == expected
+
+    def test_cte_factor_distinct_but_equal(self):
+        expr = self._case_cte_factor_distinct_but_equal()
+
+        result = to_sql(expr)
+        expected = """\
+WITH t0 AS (
+  SELECT `g`, sum(`f`) AS `metric`
+  FROM alltypes
+  GROUP BY 1
+)
+SELECT t0.*
+FROM t0
+  INNER JOIN t0 t1
+    ON t0.`g` = t1.`g`"""
+
+        assert result == expected
+
+    def test_tpch_self_join_failure(self):
+        yoy = self._case_tpch_self_join_failure()
+        to_sql(yoy)
+
+    def test_extract_subquery_nested_lower(self):
+        # We may have a join between two tables requiring subqueries, and
+        # buried inside these there may be a common subquery. Let's test that
+        # we find it and pull it out to the top level to avoid repeating
+        # ourselves.
+        pass
+
+    def test_subquery_in_filter_predicate(self):
+        expr, expr2 = self._case_subquery_in_filter_predicate()
+
+        result = to_sql(expr)
+        expected = """SELECT *
+FROM star1
+WHERE `f` > (
+  SELECT avg(`f`) AS `mean`
+  FROM star1
+)"""
+        assert result == expected
+
+        result = to_sql(expr2)
+        expected = """SELECT *
+FROM star1
+WHERE `f` > (
+  SELECT avg(`f`) AS `mean`
+  FROM star1
+  WHERE `foo_id` = 'foo'
+)"""
+        assert result == expected
+
+    def test_filter_subquery_derived_reduction(self):
+        expr3, expr4 = self._case_filter_subquery_derived_reduction()
+
+        result = to_sql(expr3)
+        expected = """SELECT *
+FROM star1
+WHERE `f` > (
+  SELECT ln(avg(`f`)) AS `tmp`
+  FROM star1
+  WHERE `foo_id` = 'foo'
+)"""
+        assert result == expected
+
+        result = to_sql(expr4)
+        expected = """SELECT *
+FROM star1
+WHERE `f` > (
+  SELECT ln(avg(`f`)) + 1 AS `tmp`
+  FROM star1
+  WHERE `foo_id` = 'foo'
+)"""
+        assert result == expected
+
+    def test_topk_operation(self):
+        filtered, filtered2 = self._case_topk_operation()
+
+        query = to_sql(filtered)
+        expected = """SELECT t0.*
+FROM tbl t0
+  LEFT SEMI JOIN (
+    SELECT `city`, avg(`v2`) AS `mean`
+    FROM tbl
+    GROUP BY 1
+    ORDER BY `mean` DESC
+    LIMIT 10
+  ) t1
+    ON t0.`city` = t1.`city`"""
+        assert query == expected
+
+        query = to_sql(filtered2)
+        expected = """SELECT t0.*
+FROM tbl t0
+  LEFT SEMI JOIN (
+    SELECT `city`, count(`city`) AS `count`
+    FROM tbl
+    GROUP BY 1
+    ORDER BY `count` DESC
+    LIMIT 10
+  ) t1
+    ON t0.`city` = t1.`city`"""
+        assert query == expected
+
+    def test_topk_predicate_pushdown_bug(self):
+        # Observed on TPCH data
+        cplusgeo = (
+            customer.inner_join(nation, [customer.c_nationkey ==
+                                         nation.n_nationkey])
+                    .inner_join(region, [nation.n_regionkey ==
+                                         region.r_regionkey])
+            [customer, nation.n_name, region.r_name])
+
+        pred = cplusgeo.n_name.topk(10, by=cplusgeo.c_acctbal.sum())
+        expr = cplusgeo.filter([pred])
+
+        result = to_sql(expr)
+        expected = """\
+SELECT t0.*, t1.`n_name`, t2.`r_name`
+FROM customer t0
+  INNER JOIN nation t1
+    ON t0.`c_nationkey` = t1.`n_nationkey`
+  INNER JOIN region t2
+    ON t1.`n_regionkey` = t2.`r_regionkey`
+  LEFT SEMI JOIN (
+    SELECT t1.`n_name`, sum(t0.`c_acctbal`) AS `sum`
+    FROM customer t0
+      INNER JOIN nation t1
+        ON t0.`c_nationkey` = t1.`n_nationkey`
+      INNER JOIN region t2
+        ON t1.`n_regionkey` = t2.`r_regionkey`
+    GROUP BY 1
+    ORDER BY `sum` DESC
+    LIMIT 10
+  ) t3
+    ON t1.`n_name` = t3.`n_name`"""
+        assert result == expected
+
+    def test_topk_analysis_bug(self):
+        # GH #398
+        airlines = ibis.table([('dest', 'string'),
+                               ('origin', 'string'),
+                               ('arrdelay', 'int32')], 'airlines')
+
+        dests = ['ORD', 'JFK', 'SFO']
+        t = airlines[airlines.dest.isin(dests)]
+        delay_filter = t.dest.topk(10, by=t.arrdelay.mean())
+        expr = t[delay_filter].group_by('origin').size()
+
+        result = to_sql(expr)
+        expected = """\
+SELECT t0.`origin`, count(*) AS `count`
+FROM airlines t0
+  LEFT SEMI JOIN (
+    SELECT `dest`, avg(`arrdelay`) AS `mean`
+    FROM airlines
+    WHERE `dest` IN ('ORD', 'JFK', 'SFO')
+    GROUP BY 1
+    ORDER BY `mean` DESC
+    LIMIT 10
+  ) t1
+    ON t0.`dest` = t1.`dest`
+WHERE t0.`dest` IN ('ORD', 'JFK', 'SFO')
+GROUP BY 1"""
+
+        assert result == expected
+
+    def test_topk_to_aggregate(self):
+        t = ibis.table([('dest', 'string'),
+                        ('origin', 'string'),
+                        ('arrdelay', 'int32')], 'airlines')
+
+        top = t.dest.topk(10, by=t.arrdelay.mean())
+
+        result = to_sql(top)
+        expected = to_sql(top.to_aggregation())
+        assert result == expected
+
+    def test_bottomk(self):
+        pass
+
+    def test_topk_antijoin(self):
+        # Get the "other" category somehow
+        pass
+
+    def test_case_in_projection(self):
+        t = self.con.table('alltypes')
+
+        expr = (t.g.case()
+                .when('foo', 'bar')
+                .when('baz', 'qux')
+                .else_('default').end())
+
+        expr2 = (api.case()
+                 .when(t.g == 'foo', 'bar')
+                 .when(t.g == 'baz', t.g)
+                 .end())
+
+        proj = t[expr.name('col1'), expr2.name('col2'), t]
+
+        result = to_sql(proj)
+        expected = """SELECT
+  CASE `g`
+    WHEN 'foo' THEN 'bar'
+    WHEN 'baz' THEN 'qux'
+    ELSE 'default'
+  END AS `col1`,
+  CASE
+    WHEN `g` = 'foo' THEN 'bar'
+    WHEN `g` = 'baz' THEN `g`
+    ELSE NULL
+  END AS `col2`, *
+FROM alltypes"""
+        assert result == expected
+
+    def test_identifier_quoting(self):
+        data = api.table([
+            ('date', 'int32'),
+            ('explain', 'string')
+        ], 'table')
+
+        expr = data[data.date.name('else'), data.explain.name('join')]
+
+        result = to_sql(expr)
+        expected = """SELECT `date` AS `else`, `explain` AS `join`
+FROM `table`"""
+        assert result == expected
+
+    def test_scalar_subquery_different_table(self):
+        t1, t2 = self.foo, self.bar
+        expr = t1[t1.y > t2.x.max()]
+
+        result = to_sql(expr)
+        expected = """SELECT *
+FROM foo
+WHERE `y` > (
+  SELECT max(`x`) AS `max`
+  FROM bar
+)"""
+        assert result == expected
+
+    def test_where_uncorrelated_subquery(self):
+        expr = self._case_where_uncorrelated_subquery()
+
+        result = to_sql(expr)
+        expected = """SELECT *
+FROM foo
+WHERE `job` IN (
+  SELECT `job`
+  FROM bar
+)"""
+        assert result == expected
+
+    def test_where_correlated_subquery(self):
+        expr = self._case_where_correlated_subquery()
+        result = to_sql(expr)
+        expected = """SELECT t0.*
+FROM foo t0
+WHERE t0.`y` > (
+  SELECT avg(t1.`y`) AS `mean`
+  FROM foo t1
+  WHERE t0.`dept_id` = t1.`dept_id`
+)"""
+        assert result == expected
+
+    def test_where_array_correlated(self):
+        # Test membership in some record-dependent values, if this is supported
+        pass
+
+    def test_exists(self):
+        e1, e2 = self._case_exists()
+
+        result = to_sql(e1)
+        expected = """SELECT t0.*
+FROM foo t0
+WHERE EXISTS (
+  SELECT 1
+  FROM bar t1
+  WHERE t0.`key1` = t1.`key1`
+)"""
+        assert result == expected
+
+        result = to_sql(e2)
+        expected = """SELECT t0.*
+FROM foo t0
+WHERE EXISTS (
+  SELECT 1
+  FROM bar t1
+  WHERE t0.`key1` = t1.`key1` AND
+        t1.`key2` = 'foo'
+)"""
+        assert result == expected
+
+    def test_exists_subquery_repr(self):
+        # GH #660
+        t1, t2 = self.t1, self.t2
+
+        cond = t1.key1 == t2.key1
+        expr = t1[cond.any()]
+        stmt = build_ast(expr).queries[0]
+
+        repr(stmt.where[0])
+
+    def test_not_exists(self):
+        expr = self._case_not_exists()
+        result = to_sql(expr)
+        expected = """SELECT t0.*
+FROM foo t0
+WHERE NOT EXISTS (
+  SELECT 1
+  FROM bar t1
+  WHERE t0.`key1` = t1.`key1`
+)"""
+        assert result == expected
+
+    def test_filter_inside_exists(self):
+        events = ibis.table([('session_id', 'int64'),
+                             ('user_id', 'int64'),
+                             ('event_type', 'int32'),
+                             ('ts', 'timestamp')], 'events')
+
+        purchases = ibis.table([('item_id', 'int64'),
+                                ('user_id', 'int64'),
+                                ('price', 'double'),
+                                ('ts', 'timestamp')], 'purchases')
+        filt = purchases.ts > '2015-08-15'
+        cond = (events.user_id == purchases[filt].user_id).any()
+        expr = events[cond]
+
+        result = to_sql(expr)
+        expected = """\
+SELECT t0.*
+FROM events t0
+WHERE EXISTS (
+  SELECT 1
+  FROM purchases t1
+  WHERE t1.`ts` > '2015-08-15' AND
+        t0.`user_id` = t1.`user_id`
+)"""
+
+        assert result == expected
+
+    def test_self_reference_in_exists(self):
+        semi, anti = self._case_self_reference_in_exists()
+
+        result = to_sql(semi)
+        expected = """\
+SELECT t0.*
+FROM functional_alltypes t0
+WHERE EXISTS (
+  SELECT 1
+  FROM functional_alltypes t1
+  WHERE t0.`string_col` = t1.`string_col`
+)"""
+        assert result == expected
+
+        result = to_sql(anti)
+        expected = """\
+SELECT t0.*
+FROM functional_alltypes t0
+WHERE NOT EXISTS (
+  SELECT 1
+  FROM functional_alltypes t1
+  WHERE t0.`string_col` = t1.`string_col`
+)"""
+        assert result == expected
+
+    def test_self_reference_limit_exists(self):
+        case = self._case_self_reference_limit_exists()
+
+        expected = """\
+WITH t0 AS (
+  SELECT *
+  FROM functional_alltypes
+  LIMIT 100
+)
+SELECT *
+FROM t0
+WHERE NOT EXISTS (
+  SELECT 1
+  FROM t0 t1
+  WHERE t0.`string_col` = t1.`string_col`
+)"""
+        self._compare_sql(case, expected)
+
+    def test_limit_cte_extract(self):
+        case = self._case_limit_cte_extract()
+
+        expected = """\
+WITH t0 AS (
+  SELECT *
+  FROM functional_alltypes
+  LIMIT 100
+)
+SELECT t0.*
+FROM t0
+  CROSS JOIN t0 t1"""
+
+        self._compare_sql(case, expected)
+
+    def test_sort_by(self):
+        cases = self._case_sort_by()
+
+        expected = [
+            """SELECT *
+FROM star1
+ORDER BY `f`""",
+            """SELECT *
+FROM star1
+ORDER BY `f` DESC""",
+            """SELECT *
+FROM star1
+ORDER BY `c`, `f` DESC"""
+        ]
 
+        for case, ex in zip(cases, expected):
+            result = to_sql(case)
+            assert result == ex
+
+    def test_limit(self):
+        cases = self._case_limit()
+
+        expected = [
+            """SELECT *
+FROM star1
+LIMIT 10""",
+            """SELECT *
+FROM star1
+LIMIT 10 OFFSET 5""",
+            """SELECT *
+FROM star1
+WHERE `f` > 0
+LIMIT 10""",
+            """SELECT *
+FROM (
+  SELECT *
+  FROM star1
+  LIMIT 10
+) t0
+WHERE `f` > 0"""
+        ]
 
-def test_pivot_wider():
-    fish = ibis.table({"fish": "int", "station": "string", "seen": "int"}, name="fish")
-    res = fish.pivot_wider(
-        names=["Release", "Lisbon"], names_from="station", values_from="seen"
-    )
-    assert res.schema().names == ("fish", "Release", "Lisbon")
-    with pytest.raises(
-        com.IbisInputError, match="No matching names columns in `names_from`"
-    ):
-        fish.pivot_wider(names=["Release", "Lisbon"], values_from="seen")
-
-
-def test_invalid_deferred():
-    t = ibis.table(dict(value="int", lagged_value="int"), name="t")
-
-    with pytest.raises(com.IbisTypeError, match="Deferred input is not allowed"):
-        ibis.greatest(t.value, ibis._.lagged_value)
-
-
-@pytest.mark.parametrize("keep", ["last", None])
-def test_invalid_distinct(keep):
-    t = ibis.table(dict(a="int"), name="t")
-    with pytest.raises(com.IbisError, match="Only keep='first'"):
-        t.distinct(keep=keep)
-
-
-def test_invalid_keep_distinct():
-    t = ibis.table(dict(a="int", b="string"), name="t")
-    with pytest.raises(com.IbisError, match="Invalid value for `keep`:"):
-        t.distinct(on="a", keep="invalid")
+        for case, ex in zip(cases, expected):
+            result = to_sql(case)
+            assert result == ex
+
+    def test_join_with_limited_table(self):
+        joined = self._case_join_with_limited_table()
+
+        result = to_sql(joined)
+        expected = """SELECT t0.*
+FROM (
+  SELECT *
+  FROM star1
+  LIMIT 100
+) t0
+  INNER JOIN star2 t1
+    ON t0.`foo_id` = t1.`foo_id`"""
+
+        assert result == expected
+
+    def test_sort_by_on_limit_yield_subquery(self):
+        # x.limit(...).sort_by(...)
+        #   is semantically different from
+        # x.sort_by(...).limit(...)
+        #   and will often yield different results
+        t = self.con.table('functional_alltypes')
+        expr = (t.group_by('string_col')
+                .aggregate([t.count().name('nrows')])
+                .limit(5)
+                .sort_by('string_col'))
+
+        result = to_sql(expr)
+        expected = """SELECT *
+FROM (
+  SELECT `string_col`, count(*) AS `nrows`
+  FROM functional_alltypes
+  GROUP BY 1
+  LIMIT 5
+) t0
+ORDER BY `string_col`"""
+        assert result == expected
+
+    def test_multiple_limits(self):
+        t = self.con.table('functional_alltypes')
+
+        expr = t.limit(20).limit(10)
+        stmt = build_ast(expr).queries[0]
+
+        assert stmt.limit['n'] == 10
+
+    def test_top_convenience(self):
+        # x.top(10, by=field)
+        # x.top(10, by=[field1, field2])
+        pass
+
+    def test_self_aggregate_in_predicate(self):
+        # Per ibis #43
+        pass
+
+    def test_self_join_filter_analysis_bug(self):
+        expr, _ = self._case_filter_self_join_analysis_bug()
+
+        expected = """\
+WITH t0 AS (
+  SELECT `region`, `kind`, sum(`amount`) AS `total`
+  FROM purchases
+  GROUP BY 1, 2
+)
+SELECT t1.`region`, t1.`total` - t2.`total` AS `diff`
+FROM (
+  SELECT *
+  FROM t0
+  WHERE `kind` = 'foo'
+) t1
+  INNER JOIN (
+    SELECT *
+    FROM t0
+    WHERE `kind` = 'bar'
+  ) t2
+    ON t1.`region` = t2.`region`"""
+        self._compare_sql(expr, expected)
+
+
+class TestUnions(unittest.TestCase, ExprTestCases):
+
+    def setUp(self):
+        self.con = MockConnection()
+
+    def test_union(self):
+        union1 = self._case_union()
+
+        result = to_sql(union1)
+        expected = """\
+SELECT `string_col` AS `key`, CAST(`float_col` AS double) AS `value`
+FROM functional_alltypes
+WHERE `int_col` > 0
+UNION ALL
+SELECT `string_col` AS `key`, `double_col` AS `value`
+FROM functional_alltypes
+WHERE `int_col` <= 0"""
+        assert result == expected
+
+    def test_union_distinct(self):
+        union = self._case_union(distinct=True)
+        result = to_sql(union)
+        expected = """\
+SELECT `string_col` AS `key`, CAST(`float_col` AS double) AS `value`
+FROM functional_alltypes
+WHERE `int_col` > 0
+UNION
+SELECT `string_col` AS `key`, `double_col` AS `value`
+FROM functional_alltypes
+WHERE `int_col` <= 0"""
+        assert result == expected
+
+    def test_union_project_column(self):
+        # select a column, get a subquery
+        union1 = self._case_union()
+        expr = union1[[union1.key]]
+        result = to_sql(expr)
+        expected = """SELECT `key`
+FROM (
+  SELECT `string_col` AS `key`, CAST(`float_col` AS double) AS `value`
+  FROM functional_alltypes
+  WHERE `int_col` > 0
+  UNION ALL
+  SELECT `string_col` AS `key`, `double_col` AS `value`
+  FROM functional_alltypes
+  WHERE `int_col` <= 0
+) t0"""
+        assert result == expected
+
+
+class TestDistinct(unittest.TestCase):
+
+    def setUp(self):
+        self.con = MockConnection()
+
+    def test_table_distinct(self):
+        t = self.con.table('functional_alltypes')
+
+        expr = t[t.string_col, t.int_col].distinct()
+
+        result = to_sql(expr)
+        expected = """SELECT DISTINCT `string_col`, `int_col`
+FROM functional_alltypes"""
+        assert result == expected
+
+    def test_array_distinct(self):
+        t = self.con.table('functional_alltypes')
+        expr = t.string_col.distinct()
+
+        result = to_sql(expr)
+        expected = """SELECT DISTINCT `string_col`
+FROM functional_alltypes"""
+        assert result == expected
+
+    def test_count_distinct(self):
+        t = self.con.table('functional_alltypes')
+
+        metric = t.int_col.nunique().name('nunique')
+        expr = t[t.bigint_col > 0].group_by('string_col').aggregate([metric])
+
+        result = to_sql(expr)
+        expected = """\
+SELECT `string_col`, COUNT(DISTINCT `int_col`) AS `nunique`
+FROM functional_alltypes
+WHERE `bigint_col` > 0
+GROUP BY 1"""
+        assert result == expected
+
+    def test_multiple_count_distinct(self):
+        # Impala and some other databases will not execute multiple
+        # count-distincts in a single aggregation query. This error reporting
+        # will be left to the database itself, for now.
+        t = self.con.table('functional_alltypes')
+        metrics = [t.int_col.nunique().name('int_card'),
+                   t.smallint_col.nunique().name('smallint_card')]
+
+        expr = t.group_by('string_col').aggregate(metrics)
+
+        result = to_sql(expr)
+        expected = """\
+SELECT `string_col`, COUNT(DISTINCT `int_col`) AS `int_card`,
+       COUNT(DISTINCT `smallint_col`) AS `smallint_card`
+FROM functional_alltypes
+GROUP BY 1"""
+        assert result == expected
```

