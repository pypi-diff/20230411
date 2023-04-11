# Comparing `tmp/polars_lts_cpu-0.17.1.tar.gz` & `tmp/polars_lts_cpu-0.17.2.tar.gz`

## Comparing `polars_lts_cpu-0.17.1.tar` & `polars_lts_cpu-0.17.2.tar`

### file list

```diff
@@ -1,1076 +1,1081 @@
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     4125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    15873 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     5808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9585 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12448 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23538 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    21989 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13483 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     7231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     2779 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123      952 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123     4012 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123     9096 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/SQL.sublime-syntax
--rw-r--r--   0     1001      123    21158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/theme
--rw-r--r--   0     1001      123     1450 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/highlighter.rs
--rw-r--r--   0     1001      123     5052 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/mod.rs
--rw-r--r--   0     1001      123     1043 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/prompt.rs
--rw-r--r--   0     1001      123    13598 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    16415 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123    26866 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123      342 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/main.rs
--rw-r--r--   0     1001      123    13264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     3386 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0     5945 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     4674 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2831 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123      764 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4184 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1211 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    22402 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17171 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    18847 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5804 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     3670 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    20940 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14345 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31804 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2044 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27332 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18867 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9563 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20901 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14987 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47889 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1033 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3604 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28016 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21349 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31233 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25209 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    12866 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7580 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9245 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123     9974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4892 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12177 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7354 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4790 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9629 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      633 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      353 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1114 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0    10379 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10815 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10121 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6441 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123      552 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    19936 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1382 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2263 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    13129 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5150 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7001 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19456 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     3567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    13166 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23438 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2517 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9391 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6295 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    24977 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16465 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22261 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7755 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11559 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     1592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    29283 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2701 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42068 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    11442 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5532 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7644 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    37711 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     7643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    47350 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123      218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    12291 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17027 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16303 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     2953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11583 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124249 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    19811 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8778 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2149 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      453 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2707 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1903 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15766 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123     8247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    17338 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    24117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9318 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10951 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    13039 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5718 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14668 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14348 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6308 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5191 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7851 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11097 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9836 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4062 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    36305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      673 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1355 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18378 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123    32703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1181 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7757 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123     1125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     4292 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/take_agg.rs
--rw-r--r--   0     1001      123     3897 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2716 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6501 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4555 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123    24282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs
--rw-r--r--   0     1001      123     2150 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20859 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23521 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     7893 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      600 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      376 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    19550 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123    17253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     6950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      969 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9323 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13163 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123     1431 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1366 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123      344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123    13120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123     1668 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     1364 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      190 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/is_in.rs
--rw-r--r--   0     1001      123     8119 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123    16613 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123     2051 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      200 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    12568 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    18280 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2627 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123    38368 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    70400 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2094 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    14993 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      156 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11390 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25701 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    25056 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29650 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15193 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    12019 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9746 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8148 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15287 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3260 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3210 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14494 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    27950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27236 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13850 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19767 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11955 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/Makefile
--rw-r--r--   0     1001      123    10846 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/README.md
--rw-r--r--   0     1001      123      651 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/build.rs
--rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7304 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1023 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1072 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1086 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      722 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     5941 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/api.py
--rw-r--r--   0     1001      123    24553 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/config.py
--rw-r--r--   0     1001      123    25409 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   301533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2524 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1356 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    14468 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7049 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dependencies.py
--rw-r--r--   0     1001      123     2954 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/categorical.py
--rw-r--r--   0     1001      123    65759 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/datetime.py
--rw-r--r--   0     1001      123   249864 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/meta.py
--rw-r--r--   0     1001      123    44215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/struct.py
--rw-r--r--   0     1001      123     1941 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29688 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/eager.py
--rw-r--r--   0     1001      123    88870 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     5309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   165937 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24010 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/categorical.py
--rw-r--r--   0     1001      123    43693 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/list.py
--rw-r--r--   0     1001      123   160561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/series.py
--rw-r--r--   0     1001      123    26584 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/__init__.py
--rw-r--r--   0     1001      123    23938 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/_parametric.py
--rw-r--r--   0     1001      123      929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/_private.py
--rw-r--r--   0     1001      123    13264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/asserts.py
--rw-r--r--   0     1001      123      551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/parametric.py
--rw-r--r--   0     1001      123     5681 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/type_aliases.py
--rw-r--r--   0     1001      123     1035 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/__init__.py
--rw-r--r--   0     1001      123    47827 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8948 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2226 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/various.py
--rw-r--r--   0     1001      123     5299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/pyproject.toml
--rw-r--r--   0     1001      123      690 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/requirements-lint.txt
--rw-r--r--   0     1001      123     1610 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/mod.rs
--rw-r--r--   0     1001      123    71436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5214 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/batched_csv.rs
--rw-r--r--   0     1001      123    47903 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/conversion.rs
--rw-r--r--   0     1001      123    45496 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/apply.rs
--rw-r--r--   0     1001      123    32612 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62204 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/utils.rs
--rw-r--r--   0     1001      123    20790 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lib.rs
--rw-r--r--   0     1001      123     4050 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/list_construction.rs
--rw-r--r--   0     1001      123     7902 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/npy.rs
--rw-r--r--   0     1001      123     1022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/py_modules.rs
--rw-r--r--   0     1001      123    54555 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     5018 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     3707 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     5709 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     7584 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3394 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    11514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2552 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123    14169 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27073 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    89703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    38972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     7127 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11067 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3361 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6828 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2851 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11918 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13357 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    13569 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12741 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    15640 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     4637 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     3952 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     7840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3881 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123    16263 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9805 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    32466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   118730 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1009 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    15408 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    10759 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    32596 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    48110 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     3960 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    10976 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2226 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83327 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    63097 2023-04-10 19:13:55.000000 polars_lts_cpu-0.17.1/Cargo.lock
--rw-r--r--   0        0        0    13384 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/PKG-INFO
+-rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123     4012 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123     9096 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/assets/SQL.sublime-syntax
+-rw-r--r--   0     1001      123    21158 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/assets/theme
+-rw-r--r--   0     1001      123     1450 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/highlighter.rs
+-rw-r--r--   0     1001      123     5052 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/mod.rs
+-rw-r--r--   0     1001      123     1043 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/prompt.rs
+-rw-r--r--   0     1001      123    13598 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    16610 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123    26950 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123      342 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/main.rs
+-rw-r--r--   0     1001      123    13264 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     3386 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0        0        0     5945 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     4674 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2831 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9288 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47120 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123      764 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13592 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4184 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1211 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    22402 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17409 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    18847 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5804 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     3670 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    20940 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14345 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31804 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2044 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      419 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27332 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18867 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9563 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20901 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14987 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4293 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14819 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47889 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2953 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1033 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6501 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4555 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123    24282 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs
+-rw-r--r--   0     1001      123     2150 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23521 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     7893 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      567 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      600 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      376 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    19550 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7265 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10476 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7368 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     4125 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    15873 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20048 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     5808 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9585 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31306 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      535 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123      320 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12448 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7059 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2008 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    23538 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20089 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24202 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      353 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1114 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8679 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1179 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20729 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1382 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2263 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    13129 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5150 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7001 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19456 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     3567 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    13166 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23438 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2517 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9391 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6295 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    24977 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15089 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123    22261 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2489 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11559 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     1592 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    29283 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2701 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42068 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    11442 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5532 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7644 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    37711 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6561 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     7643 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    47350 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123      218 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    12291 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14048 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39434 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10535 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    17027 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16303 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     2953 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11583 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124249 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    20041 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5950 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8778 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2149 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      453 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2707 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1903 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15766 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123     8247 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    17338 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    24117 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9318 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10951 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    13039 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18120 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15344 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5718 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14668 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14348 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6308 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5191 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7851 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11097 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9836 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4062 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    36305 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18378 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123    32703 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1181 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0    10379 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3269 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20419 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       32 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30146 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10815 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10121 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6441 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123      552 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13483 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     7231 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3680 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3413 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123      952 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3604 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28016 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21349 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31233 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25209 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    12866 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7580 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9245 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123     9974 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4892 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12177 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7354 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4790 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9629 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      633 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123    17253 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      969 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9323 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13163 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4169 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123      344 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    13120 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      665 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     1364 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    17430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      200 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    12740 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    18280 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2627 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    38368 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    67107 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2094 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    14993 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      156 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6819 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11390 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25701 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    25056 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29650 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15193 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    12019 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9746 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8148 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15287 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3260 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14494 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6715 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28281 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2692 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27332 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13850 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19819 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10197 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15273 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4615 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13048 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11955 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     2986 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     4292 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/take_agg.rs
+-rw-r--r--   0     1001      123     3897 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2716 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5020 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/Makefile
+-rw-r--r--   0     1001      123    10844 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/README.md
+-rw-r--r--   0     1001      123      651 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      450 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1567 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7302 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1339 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      388 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1038 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1072 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123      968 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      339 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      722 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1118 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123      647 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     5941 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/api.py
+-rw-r--r--   0     1001      123    24553 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/config.py
+-rw-r--r--   0     1001      123    25409 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5057 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   301542 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2524 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    11189 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1356 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    14468 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7049 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/dependencies.py
+-rw-r--r--   0     1001      123     2954 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    65759 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   250561 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44215 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1941 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29688 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/functions/eager.py
+-rw-r--r--   0     1001      123    88870 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     5309 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   165937 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24010 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/categorical.py
+-rw-r--r--   0     1001      123    43693 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/list.py
+-rw-r--r--   0     1001      123   160680 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/series.py
+-rw-r--r--   0     1001      123    26584 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/testing/__init__.py
+-rw-r--r--   0     1001      123    25164 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/testing/_parametric.py
+-rw-r--r--   0     1001      123      929 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/testing/_private.py
+-rw-r--r--   0     1001      123    13264 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      551 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/testing/parametric.py
+-rw-r--r--   0     1001      123     5681 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1035 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    47827 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8948 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/polars/utils/various.py
+-rw-r--r--   0     1001      123     5299 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/pyproject.toml
+-rw-r--r--   0     1001      123      690 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/requirements-lint.txt
+-rw-r--r--   0     1001      123     1610 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10959 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71436 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3906 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5214 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/batched_csv.rs
+-rw-r--r--   0     1001      123    48063 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/conversion.rs
+-rw-r--r--   0     1001      123    45496 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    32660 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62357 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20790 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/lib.rs
+-rw-r--r--   0     1001      123     4050 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/list_construction.rs
+-rw-r--r--   0     1001      123     7902 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/npy.rs
+-rw-r--r--   0     1001      123     1022 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/py_modules.rs
+-rw-r--r--   0     1001      123    54555 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     5018 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123     3707 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     5709 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     7584 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3394 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    11514 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2552 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123    14169 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27448 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    89703 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      218 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1907 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    38970 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     7127 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11067 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5916 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3361 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6828 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2851 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11918 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13357 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3229 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    13569 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12741 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    15640 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     4637 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     3952 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     7840 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3881 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123    16263 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19137 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9805 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19916 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    32653 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3497 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   118730 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1009 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    15839 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    10759 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    32596 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    48110 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4008 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    10976 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2226 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83595 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10344 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-11 14:48:58.000000 polars_lts_cpu-0.17.2/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    63097 2023-04-11 14:50:04.000000 polars_lts_cpu-0.17.2/Cargo.lock
+-rw-r--r--   0        0        0    13382 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.2/PKG-INFO
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files 1% similar despite different names*

```diff
@@ -269,17 +269,17 @@
             .map(|opt_s| opt_s.and_then(|s| s.as_ref().arg_max().map(|idx| idx as IdxSize)))
             .collect_trusted();
         out.rename(ca.name());
         out
     }
 
     #[cfg(feature = "diff")]
-    fn lst_diff(&self, n: usize, null_behavior: NullBehavior) -> ListChunked {
+    fn lst_diff(&self, n: i64, null_behavior: NullBehavior) -> PolarsResult<ListChunked> {
         let ca = self.as_list();
-        ca.apply_amortized(|s| s.as_ref().diff(n, null_behavior))
+        ca.try_apply_amortized(|s| s.as_ref().diff(n, null_behavior))
     }
 
     fn lst_shift(&self, periods: i64) -> ListChunked {
         let ca = self.as_list();
         ca.apply_amortized(|s| s.as_ref().shift(periods))
     }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 use crate::series::ops::SeriesSealed;
 
 fn log<T: PolarsNumericType>(ca: &ChunkedArray<T>, base: f64) -> Float64Chunked {
     ca.cast_and_apply_in_place(|v: f64| v.log(base))
 }
 
+fn log1p<T: PolarsNumericType>(ca: &ChunkedArray<T>) -> Float64Chunked {
+    ca.cast_and_apply_in_place(|v: f64| v.ln_1p())
+}
+
 fn exp<T: PolarsNumericType>(ca: &ChunkedArray<T>) -> Float64Chunked {
     ca.cast_and_apply_in_place(|v: f64| v.exp())
 }
 
 pub trait LogSeries: SeriesSealed {
     /// Compute the logarithm to a given base
     fn log(&self, base: f64) -> Series {
@@ -24,14 +28,31 @@
             UInt64 => log(s.u64().unwrap(), base).into_series(),
             Float32 => s.f32().unwrap().apply(|v| v.log(base as f32)).into_series(),
             Float64 => s.f64().unwrap().apply(|v| v.log(base)).into_series(),
             _ => s.cast(&DataType::Float64).unwrap().log(base),
         }
     }
 
+    /// Compute the natural logarithm of all elements plus one in the input array
+    fn log1p(&self) -> Series {
+        let s = self.as_series().to_physical_repr();
+        let s = s.as_ref();
+
+        use DataType::*;
+        match s.dtype() {
+            Int32 => log1p(s.i32().unwrap()).into_series(),
+            Int64 => log1p(s.i64().unwrap()).into_series(),
+            UInt32 => log1p(s.u32().unwrap()).into_series(),
+            UInt64 => log1p(s.u64().unwrap()).into_series(),
+            Float32 => s.f32().unwrap().apply(|v| v.ln_1p()).into_series(),
+            Float64 => s.f64().unwrap().apply(|v| v.ln_1p()).into_series(),
+            _ => s.cast(&DataType::Float64).unwrap().log1p(),
+        }
+    }
+
     /// Calculate the exponential of all elements in the input array.
     fn exp(&self) -> Series {
         let s = self.as_series().to_physical_repr();
         let s = s.as_ref();
 
         use DataType::*;
         match s.dtype() {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/README.md` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/SQL.sublime-syntax` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/assets/SQL.sublime-syntax`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/theme` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/assets/theme`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/highlighter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/highlighter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/prompt.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/cli/prompt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/functions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
     /// ```
     Log10,
     /// SQL 'log' function
     /// ```sql
     /// SELECT LOG(column_1, 10) from df;
     /// ```
     Log,
+    /// SQL 'log1p' function
+    /// ```sql
+    /// SELECT LOG1P(column_1) from df;
+    /// ```
+    Log1p,
     /// SQL 'pow' function
     /// ```sql
     /// SELECT POW(column_1, 2) from df;
     /// ```
     Pow,
     // ----
     // String functions
@@ -243,14 +248,15 @@
             "ceil" | "ceiling" => Self::Ceil,
             "exp" => Self::Exp,
             "floor" => Self::Floor,
             "ln" => Self::Ln,
             "log2" => Self::Log2,
             "log10" => Self::Log10,
             "log" => Self::Log,
+            "log1p" => Self::Log1p,
             "pow" => Self::Pow,
             // ----
             // String functions
             // ----
             "lower" => Self::Lower,
             "upper" => Self::Upper,
             "ltrim" => Self::LTrim,
@@ -304,14 +310,15 @@
             Ceil => self.visit_unary(Expr::ceil),
             Exp => self.visit_unary(Expr::exp),
             Floor => self.visit_unary(Expr::floor),
             Ln => self.visit_unary(|e| e.log(std::f64::consts::E)),
             Log2 => self.visit_unary(|e| e.log(2.0)),
             Log10 => self.visit_unary(|e| e.log(10.0)),
             Log => self.visit_binary(Expr::log),
+            Log1p => self.visit_unary(Expr::log1p),
             Pow => self.visit_binary::<Expr>(Expr::pow),
             // ----
             // String functions
             // ----
             Lower => self.visit_unary(|e| e.str().to_lowercase()),
             Upper => self.visit_unary(|e| e.str().to_uppercase()),
             LTrim => match function.args.len() {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,15 @@
                 CEIL(a) AS ceil,
                 EXP(a) AS exp,
                 FLOOR(a) AS floor,
                 LN(a) AS ln,
                 LOG2(a) AS log2,
                 LOG10(a) AS log10,
                 LOG(a, 5) AS log5,
+                LOG1P(a) AS log1p,
                 POW(a, 2) AS pow
             FROM df"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let df_pl = df
             .lazy()
             .select(&[
                 col("a"),
@@ -335,14 +336,15 @@
                 col("a").ceil().alias("ceil"),
                 col("a").exp().alias("exp"),
                 col("a").floor().alias("floor"),
                 col("a").log(std::f64::consts::E).alias("ln"),
                 col("a").log(2.0).alias("log2"),
                 col("a").log(10.0).alias("log10"),
                 col("a").log(5.0).alias("log5"),
+                col("a").log1p().alias("log1p"),
                 col("a").pow(2.0).alias("pow"),
             ])
             .collect()
             .unwrap();
         assert!(df_sql.frame_equal_missing(&df_pl));
     }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files 6% similar despite different names*

```diff
@@ -151,15 +151,17 @@
             AggState::AggregatedList(s) => {
                 let ca = s.list().unwrap();
                 let out = ca.apply_to_inner(&|s| self.eval_and_flatten(&mut [s]))?;
                 (out.into_series(), true)
             }
             AggState::AggregatedFlat(s) => (self.eval_and_flatten(&mut [s.clone()])?, true),
             AggState::NotAggregated(s) | AggState::Literal(s) => {
-                (self.eval_and_flatten(&mut [s.clone()])?, false)
+                let (out, aggregated) = (self.eval_and_flatten(&mut [s.clone()])?, false);
+                check_map_output_len(s.len(), out.len(), &self.expr)?;
+                (out, aggregated)
             }
         };
 
         ac.with_series(s, aggregated, Some(&self.expr))?;
         Ok(ac)
     }
     fn apply_multiple_group_aware<'a>(
@@ -218,15 +220,15 @@
     let list_arr = ca.downcast_iter().next().unwrap();
     let offset = list_arr.offsets().as_slice();
     (offset[offset.len() - 1] as usize) == list_arr.len()
 }
 
 fn check_map_output_len(input_len: usize, output_len: usize, expr: &Expr) -> PolarsResult<()> {
     polars_ensure!(
-        input_len == output_len, expr = expr, ComputeError:
+        input_len == output_len, expr = expr, InvalidOperation:
         "output length of `map` must be equal to that of the input length; \
         consider using `apply` instead"
     );
     Ok(())
 }
 
 impl PhysicalExpr for ApplyExpr {
@@ -308,17 +310,17 @@
     fn as_stats_evaluator(&self) -> Option<&dyn polars_io::predicates::StatsEvaluator> {
         let function = match &self.expr {
             Expr::Function { function, .. } => function,
             _ => return None,
         };
 
         match function {
-            FunctionExpr::IsNull => Some(self),
+            FunctionExpr::Boolean(BooleanFunction::IsNull) => Some(self),
             #[cfg(feature = "is_in")]
-            FunctionExpr::IsIn => Some(self),
+            FunctionExpr::Boolean(BooleanFunction::IsIn) => Some(self),
             _ => None,
         }
     }
     fn as_partitioned_aggregator(&self) -> Option<&dyn PartitionedAggregation> {
         if self.inputs.len() == 1 && matches!(self.collect_groups, ApplyOptions::ApplyFlat) {
             Some(self)
         } else {
@@ -405,27 +407,27 @@
             Expr::Function {
                 function, input, ..
             } => (function, input),
             _ => return Ok(true),
         };
 
         match function {
-            FunctionExpr::IsNull => {
+            FunctionExpr::Boolean(BooleanFunction::IsNull) => {
                 let root = expr_to_leaf_column_name(&self.expr)?;
 
                 match stats.get_stats(&root).ok() {
                     Some(st) => match st.null_count() {
                         Some(0) => Ok(false),
                         _ => Ok(true),
                     },
                     None => Ok(true),
                 }
             }
             #[cfg(feature = "is_in")]
-            FunctionExpr::IsIn => {
+            FunctionExpr::Boolean(BooleanFunction::IsIn) => {
                 let root = match expr_to_leaf_column_name(&input[0]) {
                     Ok(root) => root,
                     Err(_) => return Ok(true),
                 };
 
                 let input: &Series = match &input[1] {
                     Expr::Literal(LiteralValue::Series(s)) => s,
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/json.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/hash.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.17.2/local_dependencies/polars/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .DEFAULT_GOAL := help
 
-BASE ?= master
+BASE ?= main
 
 .PHONY: fmt check check-features clippy clippy-default test test-doc integration-tests
 
 fmt:
 	cargo fmt --all
 	dprint fmt
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use polars_arrow::array::list::AnonymousBuilder;
+use polars_arrow::array::null::MutableNullArray;
 use polars_arrow::prelude::*;
 
 use super::*;
 
 pub trait ListBuilderTrait {
     fn append_opt_series(&mut self, opt_s: Option<&Series>) {
         match opt_s {
@@ -80,24 +81,26 @@
         Self {
             builder,
             field,
             fast_explode: true,
         }
     }
 
+    #[inline]
     pub fn append_slice(&mut self, items: &[T::Native]) {
         let values = self.builder.mut_values();
         values.extend_from_slice(items);
         self.builder.try_push_valid().unwrap();
 
         if items.is_empty() {
             self.fast_explode = false;
         }
     }
 
+    #[inline]
     pub fn append_opt_slice(&mut self, opt_v: Option<&[T::Native]>) {
         match opt_v {
             Some(items) => self.append_slice(items),
             None => {
                 self.builder.push_null();
             }
         }
@@ -178,14 +181,15 @@
     }
 }
 
 type LargePrimitiveBuilder<T> = MutableListArray<i64, MutablePrimitiveArray<T>>;
 type LargeListUtf8Builder = MutableListArray<i64, MutableUtf8Array<i64>>;
 type LargeListBinaryBuilder = MutableListArray<i64, MutableBinaryArray<i64>>;
 type LargeListBooleanBuilder = MutableListArray<i64, MutableBooleanArray>;
+type LargeListNullBuilder = MutableListArray<i64, MutableNullArray>;
 
 pub struct ListUtf8ChunkedBuilder {
     builder: LargeListUtf8Builder,
     field: Field,
     fast_explode: bool,
 }
 
@@ -198,14 +202,15 @@
         ListUtf8ChunkedBuilder {
             builder,
             field,
             fast_explode: true,
         }
     }
 
+    #[inline]
     pub fn append_trusted_len_iter<'a, I: Iterator<Item = Option<&'a str>> + TrustedLen>(
         &mut self,
         iter: I,
     ) {
         let values = self.builder.mut_values();
 
         if iter.size_hint().0 == 0 {
@@ -213,32 +218,35 @@
         }
         // Safety
         // trusted len, trust the type system
         unsafe { values.extend_trusted_len_unchecked(iter) };
         self.builder.try_push_valid().unwrap();
     }
 
+    #[inline]
     pub fn append_values_iter<'a, I: Iterator<Item = &'a str>>(&mut self, iter: I) {
         let values = self.builder.mut_values();
 
         if iter.size_hint().0 == 0 {
             self.fast_explode = false;
         }
         values.extend_values(iter);
         self.builder.try_push_valid().unwrap();
     }
 
+    #[inline]
     pub(crate) fn append(&mut self, ca: &Utf8Chunked) {
         let value_builder = self.builder.mut_values();
         value_builder.try_extend(ca).unwrap();
         self.builder.try_push_valid().unwrap();
     }
 }
 
 impl ListBuilderTrait for ListUtf8ChunkedBuilder {
+    #[inline]
     fn append_opt_series(&mut self, opt_s: Option<&Series>) {
         match opt_s {
             Some(s) => self.append_series(s),
             None => {
                 self.append_null();
             }
         }
@@ -246,14 +254,15 @@
 
     #[inline]
     fn append_null(&mut self) {
         self.fast_explode = false;
         self.builder.push_null();
     }
 
+    #[inline]
     fn append_series(&mut self, s: &Series) {
         if s.is_empty() {
             self.fast_explode = false;
         }
         let ca = s.utf8().unwrap();
         self.append(ca)
     }
@@ -409,14 +418,36 @@
     }
 
     fn finish(&mut self) -> ListChunked {
         finish_list_builder!(self)
     }
 }
 
+impl ListBuilderTrait for LargeListNullBuilder {
+    #[inline]
+    fn append_series(&mut self, _s: &Series) {
+        self.push_null()
+    }
+
+    #[inline]
+    fn append_null(&mut self) {
+        self.push_null()
+    }
+
+    fn finish(&mut self) -> ListChunked {
+        unsafe {
+            ListChunked::from_chunks_and_dtype_unchecked(
+                "",
+                vec![self.as_box()],
+                DataType::List(Box::new(DataType::Null)),
+            )
+        }
+    }
+}
+
 pub fn get_list_builder(
     dt: &DataType,
     value_capacity: usize,
     list_capacity: usize,
     name: &str,
 ) -> PolarsResult<Box<dyn ListBuilderTrait>> {
     let physical_type = dt.to_physical();
@@ -426,14 +457,15 @@
         DataType::Object(_) => polars_bail!(opq = list_builder, &physical_type),
         #[cfg(feature = "dtype-struct")]
         DataType::Struct(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
             name,
             list_capacity,
             Some(physical_type),
         ))),
+        DataType::Null => Ok(Box::new(LargeListNullBuilder::with_capacity(list_capacity))),
         DataType::List(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
             name,
             list_capacity,
             Some(physical_type),
         ))),
         _ => {
             macro_rules! get_primitive_builder {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 use std::hash::Hash;
 
-use hashbrown::hash_set::HashSet;
-
 use crate::prelude::*;
 use crate::utils::{try_get_supertype, CustomIterTools};
 
 unsafe fn is_in_helper<T, P>(ca: &ChunkedArray<T>, other: &Series) -> PolarsResult<BooleanChunked>
 where
     T: PolarsNumericType,
     P: Eq + Hash + Copy,
 {
-    let mut set = HashSet::with_capacity(other.len());
+    let mut set = PlHashSet::with_capacity(other.len());
 
     let other = ca.unpack_series_matching_type(other)?;
     other.downcast_iter().for_each(|iter| {
         iter.into_iter().for_each(|opt_val| {
             // Safety
             // bit sizes are/ should be equal
             let ptr = &opt_val.copied() as *const Option<T::Native> as *const Option<P>;
@@ -160,64 +158,24 @@
                             }
                         }
                     }
                 } else {
                     unreachable!()
                 }
             }
-            DataType::List(dt) if DataType::Utf8 == **dt => {
-                let mut ca: BooleanChunked = if self.len() == 1 && other.len() != 1 {
-                    let value = self.get(0);
-                    other
-                        .list()?
-                        .amortized_iter()
-                        .map(|opt_s| {
-                            opt_s.map(|s| {
-                                let ca = s.as_ref().unpack::<Utf8Type>().unwrap();
-                                ca.into_iter().any(|a| a == value)
-                            }) == Some(true)
-                        })
-                        .collect_trusted()
-                } else {
-                    self.into_iter()
-                        .zip(other.list()?.amortized_iter())
-                        .map(|(value, series)| match (value, series) {
-                            (val, Some(series)) => {
-                                let ca = series.as_ref().unpack::<Utf8Type>().unwrap();
-                                ca.into_iter().any(|a| a == val)
-                            }
-                            _ => false,
-                        })
-                        .collect_trusted()
-                };
-                ca.rename(self.name());
-                Ok(ca)
-            }
-            DataType::Utf8 => {
-                let mut set = HashSet::with_capacity(other.len());
-
-                let other = other.utf8()?;
-                other.downcast_iter().for_each(|iter| {
-                    iter.into_iter().for_each(|opt_val| {
-                        set.insert(opt_val);
-                    })
-                });
-                let mut ca: BooleanChunked = self
-                    .into_iter()
-                    .map(|opt_val| set.contains(&opt_val))
-                    .collect_trusted();
-                ca.rename(self.name());
-                Ok(ca)
-            }
+            DataType::List(dt) if DataType::Utf8 == **dt => self.as_binary().is_in(
+                &other
+                    .cast(&DataType::List(Box::new(DataType::Binary)))
+                    .unwrap(),
+            ),
+            DataType::Utf8 => self
+                .as_binary()
+                .is_in(&other.cast(&DataType::Binary).unwrap()),
             _ => polars_bail!(opq = is_in, self.dtype(), other.dtype()),
         }
-        .map(|mut ca| {
-            ca.rename(self.name());
-            ca
-        })
     }
 }
 
 impl IsIn for BinaryChunked {
     fn is_in(&self, other: &Series) -> PolarsResult<BooleanChunked> {
         match other.dtype() {
             DataType::List(dt) if DataType::Binary == **dt => {
@@ -245,15 +203,15 @@
                         })
                         .collect_trusted()
                 };
                 ca.rename(self.name());
                 Ok(ca)
             }
             DataType::Binary => {
-                let mut set = HashSet::with_capacity(other.len());
+                let mut set = PlHashSet::with_capacity(other.len());
 
                 let other = other.binary()?;
                 other.downcast_iter().for_each(|iter| {
                     iter.into_iter().for_each(|opt_val| {
                         set.insert(opt_val);
                     })
                 });
@@ -365,30 +323,32 @@
 
                 polars_ensure!(
                     self.fields().len() == other.fields().len(),
                     ComputeError: "`is_in`: mismatch in the number of struct fields: {} and {}",
                     self.fields().len(), other.fields().len()
                 );
 
-                let out = self
-                    .fields()
-                    .iter()
-                    .zip(other.fields())
-                    .map(|(lhs, rhs)| lhs.is_in(rhs))
-                    .collect::<PolarsResult<Vec<_>>>()?;
-
-                let out = out.into_iter().reduce(|acc, val| {
-                    // all false
-                    if !acc.any() {
-                        acc
-                    } else {
-                        acc & val
-                    }
+                let mut anyvalues = Vec::with_capacity(other.len() * other.fields().len());
+                // Safety:
+                // the iterator is unsafe as the lifetime is tied to the iterator
+                // so we copy to an owned buffer first
+                other.into_iter().for_each(|val| {
+                    anyvalues.extend_from_slice(val);
                 });
-                out.ok_or_else(|| polars_err!(ComputeError: "no fields in struct"))
+
+                // then we fill the set
+                let mut set = PlHashSet::with_capacity(other.len());
+                for key in anyvalues.chunks_exact(other.fields().len()) {
+                    set.insert(key);
+                }
+                // and then we check for membership
+                let mut ca: BooleanChunked =
+                    self.into_iter().map(|vals| set.contains(&vals)).collect();
+                ca.rename(self.name());
+                Ok(ca)
             }
         }
     }
 }
 
 #[cfg(test)]
 mod test {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         truthy
     } else {
         falsy
     }
 }
 
 fn prepare_mask(mask: &BooleanArray) -> BooleanArray {
-    // make sure that zip works same as master branch
+    // make sure that zip works same as main branch
     // that is that null are ignored from mask and that we take from the right array
 
     match mask.validity() {
         // nulls are set to true meaning we take from the right in the zip/ if_then_else kernel
         Some(validity) if validity.unset_bits() != 0 => {
             let mask = mask.values() & validity;
             BooleanArray::from_data_default(mask, None)
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,14 @@
                 let v = val.extract::<u8>()?;
                 builder.append_value(v == 1)
             }
             (Int32(builder), AnyValue::Null) => builder.append_null(),
             (Int32(builder), val) => builder.append_value(val.extract()?),
             (Int64(builder), AnyValue::Null) => builder.append_null(),
             (Int64(builder), val) => builder.append_value(val.extract()?),
-            #[cfg(feature = "dtype-u8")]
-            (UInt8(builder), AnyValue::Null) => builder.append_null(),
-            #[cfg(feature = "dtype-u16")]
-            (UInt16(builder), val) => builder.append_value(val.extract()?),
             (UInt32(builder), AnyValue::Null) => builder.append_null(),
             (UInt32(builder), val) => builder.append_value(val.extract()?),
             (UInt64(builder), AnyValue::Null) => builder.append_null(),
             (UInt64(builder), val) => builder.append_value(val.extract()?),
             (Float32(builder), AnyValue::Null) => builder.append_null(),
             (Float64(builder), AnyValue::Null) => builder.append_null(),
             (Float32(builder), val) => builder.append_value(val.extract()?),
@@ -73,14 +69,22 @@
             (Int8(builder), AnyValue::Null) => builder.append_null(),
             #[cfg(feature = "dtype-i8")]
             (Int8(builder), val) => builder.append_value(val.extract()?),
             #[cfg(feature = "dtype-i16")]
             (Int16(builder), AnyValue::Null) => builder.append_null(),
             #[cfg(feature = "dtype-i16")]
             (Int16(builder), val) => builder.append_value(val.extract()?),
+            #[cfg(feature = "dtype-u8")]
+            (UInt8(builder), AnyValue::Null) => builder.append_null(),
+            #[cfg(feature = "dtype-u8")]
+            (UInt8(builder), val) => builder.append_value(val.extract()?),
+            #[cfg(feature = "dtype-u16")]
+            (UInt16(builder), AnyValue::Null) => builder.append_null(),
+            #[cfg(feature = "dtype-u16")]
+            (UInt16(builder), val) => builder.append_value(val.extract()?),
             #[cfg(feature = "dtype-date")]
             (Date(builder), AnyValue::Null) => builder.append_null(),
             #[cfg(feature = "dtype-date")]
             (Date(builder), AnyValue::Date(v)) => builder.append_value(v),
             #[cfg(feature = "dtype-datetime")]
             (Datetime(builder, _, _), AnyValue::Null) => builder.append_null(),
             #[cfg(feature = "dtype-datetime")]
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 use crate::prelude::*;
 use crate::series::ops::NullBehavior;
 
 impl Series {
-    pub fn diff(&self, n: usize, null_behavior: NullBehavior) -> Series {
+    pub fn diff(&self, n: i64, null_behavior: NullBehavior) -> PolarsResult<Series> {
         use DataType::*;
         let s = match self.dtype() {
             UInt8 => self.cast(&Int16).unwrap(),
             UInt16 => self.cast(&Int32).unwrap(),
             UInt32 | UInt64 => self.cast(&Int64).unwrap(),
             _ => self.clone(),
         };
 
         match null_behavior {
-            NullBehavior::Ignore => &s - &s.shift(n as i64),
+            NullBehavior::Ignore => Ok(&s - &s.shift(n)),
             NullBehavior::Drop => {
+                polars_ensure!(n > 0, InvalidOperation: "only positive integer allowed if nulls are dropped in 'diff' operation");
+                let n = n as usize;
                 let len = s.len() - n;
-                &self.slice(n as i64, len) - &s.slice(0, len)
+                Ok(&self.slice(n as i64, len) - &s.slice(0, len))
             }
         }
     }
 }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 use crate::prelude::*;
 use crate::series::ops::NullBehavior;
 
 impl Series {
-    pub fn pct_change(&self, n: usize) -> PolarsResult<Series> {
+    pub fn pct_change(&self, n: i64) -> PolarsResult<Series> {
         match self.dtype() {
             DataType::Float64 | DataType::Float32 => {}
             _ => return self.cast(&DataType::Float64)?.pct_change(n),
         }
         let nn = self.fill_null(FillNullStrategy::Forward(None))?;
-        nn.diff(n, NullBehavior::Ignore).divide(&nn.shift(n as i64))
+        nn.diff(n, NullBehavior::Ignore)?.divide(&nn.shift(n))
     }
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 use crate::prelude::*;
 use crate::utils::CustomIterTools;
 
 pub mod default_arrays;
 mod get;
 pub mod list;
+pub mod null;
 pub mod slice;
 pub mod utf8;
 
 pub use get::ArrowGetItem;
 pub use slice::*;
 
 pub trait ValueSize {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/take_agg.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/take_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.17.2/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files 15% similar despite different names*

```diff
@@ -9,22 +9,21 @@
     Contains { pat: Vec<u8>, literal: bool },
     StartsWith(Vec<u8>),
     EndsWith(Vec<u8>),
 }
 
 impl Display for BinaryFunction {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        use self::*;
+        use BinaryFunction::*;
         let s = match self {
-            BinaryFunction::Contains { .. } => "contains",
-            BinaryFunction::StartsWith(_) => "starts_with",
-            BinaryFunction::EndsWith(_) => "ends_with",
+            Contains { .. } => "contains",
+            StartsWith(_) => "starts_with",
+            EndsWith(_) => "ends_with",
         };
-
-        write!(f, "str.{s}")
+        write!(f, "bin.{s}")
     }
 }
 
 pub(super) fn contains(s: &Series, pat: &[u8], literal: bool) -> PolarsResult<Series> {
     let ca = s.binary()?;
     if literal {
         ca.contains_literal(pat).map(|ca| ca.into_series())
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+#[cfg(feature = "abs")]
+mod abs;
 #[cfg(feature = "arg_where")]
 mod arg_where;
 mod binary;
+mod boolean;
 #[cfg(feature = "round_series")]
 mod clip;
+mod cum;
 #[cfg(feature = "temporal")]
 mod datetime;
 mod dispatch;
 mod fill_null;
-#[cfg(feature = "is_in")]
-mod is_in;
 mod list;
+#[cfg(feature = "log")]
+mod log;
 mod nan;
 mod pow;
 #[cfg(all(feature = "rolling_window", feature = "moment"))]
 mod rolling;
 #[cfg(feature = "row_hash")]
 mod row_hash;
 mod schema;
@@ -27,43 +31,44 @@
 mod strings;
 #[cfg(feature = "dtype-struct")]
 mod struct_;
 #[cfg(any(feature = "temporal", feature = "date_offset"))]
 mod temporal;
 #[cfg(feature = "trigonometry")]
 mod trigonometry;
+mod unique;
 
 use std::fmt::{Display, Formatter};
 
 pub(super) use list::ListFunction;
 use polars_core::prelude::*;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
 pub(crate) use self::binary::BinaryFunction;
+pub use self::boolean::BooleanFunction;
 #[cfg(feature = "temporal")]
 pub(super) use self::datetime::TemporalFunction;
-pub(super) use self::nan::NanFunction;
 #[cfg(feature = "strings")]
 pub(crate) use self::strings::StringFunction;
 #[cfg(feature = "dtype-struct")]
 pub(super) use self::struct_::StructFunction;
 #[cfg(feature = "trigonometry")]
 pub(super) use self::trigonometry::TrigonometricFunction;
 use super::*;
 
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 #[derive(Clone, PartialEq, Debug)]
 pub enum FunctionExpr {
+    #[cfg(feature = "abs")]
+    Abs,
     NullCount,
     Pow,
     #[cfg(feature = "row_hash")]
     Hash(u64, u64, u64, u64),
-    #[cfg(feature = "is_in")]
-    IsIn,
     #[cfg(feature = "arg_where")]
     ArgWhere,
     #[cfg(feature = "search_sorted")]
     SearchSorted(SearchSortedSide),
     #[cfg(feature = "strings")]
     StringExpr(StringFunction),
     BinaryExpr(BinaryFunction),
@@ -83,63 +88,81 @@
     RollingSkew {
         window_size: usize,
         bias: bool,
     },
     ShiftAndFill {
         periods: i64,
     },
-    Nan(NanFunction),
+    DropNans,
     #[cfg(feature = "round_series")]
     Clip {
         min: Option<AnyValue<'static>>,
         max: Option<AnyValue<'static>>,
     },
     ListExpr(ListFunction),
     #[cfg(feature = "dtype-struct")]
     StructExpr(StructFunction),
     #[cfg(feature = "top_k")]
     TopK {
         k: usize,
         descending: bool,
     },
     Shift(i64),
+    Cumcount {
+        reverse: bool,
+    },
+    Cumsum {
+        reverse: bool,
+    },
+    Cumprod {
+        reverse: bool,
+    },
+    Cummin {
+        reverse: bool,
+    },
+    Cummax {
+        reverse: bool,
+    },
     Reverse,
-    IsNull,
-    IsNotNull,
-    Not,
-    #[cfg(feature = "is_unique")]
-    IsUnique,
-    #[cfg(feature = "is_unique")]
-    IsDuplicated,
+    Boolean(BooleanFunction),
     Coalesce,
     ShrinkType,
     #[cfg(feature = "diff")]
-    Diff(usize, NullBehavior),
+    Diff(i64, NullBehavior),
     #[cfg(feature = "interpolate")]
     Interpolate(InterpolationMethod),
     #[cfg(feature = "dot_product")]
     Dot,
     #[cfg(feature = "log")]
     Entropy {
         base: f64,
         normalize: bool,
     },
+    #[cfg(feature = "log")]
+    Log {
+        base: f64,
+    },
+    #[cfg(feature = "log")]
+    Log1p,
+    #[cfg(feature = "log")]
+    Exp,
+    Unique(bool),
 }
 
 impl Display for FunctionExpr {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         use FunctionExpr::*;
 
         let s = match self {
+            #[cfg(feature = "abs")]
+            Abs => "abs",
             NullCount => "null_count",
             Pow => "pow",
             #[cfg(feature = "row_hash")]
             Hash(_, _, _, _) => "hash",
-            #[cfg(feature = "is_in")]
-            IsIn => "is_in",
             #[cfg(feature = "arg_where")]
             ArgWhere => "arg_where",
             #[cfg(feature = "search_sorted")]
             SearchSorted(_) => "search_sorted",
             #[cfg(feature = "strings")]
             StringExpr(s) => return write!(f, "{s}"),
             BinaryExpr(b) => return write!(f, "{b}"),
@@ -151,55 +174,64 @@
             Trigonometry(func) => return write!(f, "{func}"),
             #[cfg(feature = "sign")]
             Sign => "sign",
             FillNull { .. } => "fill_null",
             #[cfg(all(feature = "rolling_window", feature = "moment"))]
             RollingSkew { .. } => "rolling_skew",
             ShiftAndFill { .. } => "shift_and_fill",
-            Nan(func) => match func {
-                NanFunction::IsNan => "is_nan",
-                NanFunction::IsNotNan => "is_not_nan",
-                NanFunction::DropNans => "drop_nans",
-            },
+            DropNans => "drop_nans",
             #[cfg(feature = "round_series")]
             Clip { min, max } => match (min, max) {
                 (Some(_), Some(_)) => "clip",
                 (None, Some(_)) => "clip_max",
                 (Some(_), None) => "clip_min",
                 _ => unreachable!(),
             },
             ListExpr(func) => return write!(f, "{func}"),
             #[cfg(feature = "dtype-struct")]
             StructExpr(func) => return write!(f, "{func}"),
             #[cfg(feature = "top_k")]
             TopK { .. } => "top_k",
             Shift(_) => "shift",
+            Cumcount { .. } => "cumcount",
+            Cumsum { .. } => "cumsum",
+            Cumprod { .. } => "cumprod",
+            Cummin { .. } => "cummin",
+            Cummax { .. } => "cummax",
             Reverse => "reverse",
-            Not => "is_not",
-            IsNull => "is_null",
-            IsNotNull => "is_not_null",
-            #[cfg(feature = "is_unique")]
-            IsUnique => "is_unique",
-            #[cfg(feature = "is_unique")]
-            IsDuplicated => "is_duplicated",
+            Boolean(func) => return write!(f, "{func}"),
             Coalesce => "coalesce",
             ShrinkType => "shrink_dtype",
             #[cfg(feature = "diff")]
             Diff(_, _) => "diff",
             #[cfg(feature = "interpolate")]
             Interpolate(_) => "interpolate",
             #[cfg(feature = "dot_product")]
             Dot => "dot",
             #[cfg(feature = "log")]
             Entropy { .. } => "entropy",
+            #[cfg(feature = "log")]
+            Log { .. } => "log",
+            #[cfg(feature = "log")]
+            Log1p => "log1p",
+            #[cfg(feature = "log")]
+            Exp => "exp",
+            Unique(stable) => {
+                if *stable {
+                    "unique_stable"
+                } else {
+                    "unique"
+                }
+            }
         };
         write!(f, "{s}")
     }
 }
 
+#[macro_export]
 macro_rules! wrap {
     ($e:expr) => {
         SpecialEq::new(Arc::new($e))
     };
 }
 
 // Fn(&[Series], args)
@@ -268,32 +300,30 @@
     }};
 }
 
 impl From<FunctionExpr> for SpecialEq<Arc<dyn SeriesUdf>> {
     fn from(func: FunctionExpr) -> Self {
         use FunctionExpr::*;
         match func {
+            #[cfg(feature = "abs")]
+            Abs => map!(abs::abs),
             NullCount => {
                 let f = |s: &mut [Series]| {
                     let s = &s[0];
                     Ok(Some(Series::new(s.name(), [s.null_count() as IdxSize])))
                 };
                 wrap!(f)
             }
             Pow => {
                 wrap!(pow::pow)
             }
             #[cfg(feature = "row_hash")]
             Hash(k0, k1, k2, k3) => {
                 map!(row_hash::row_hash, k0, k1, k2, k3)
             }
-            #[cfg(feature = "is_in")]
-            IsIn => {
-                wrap!(is_in::is_in)
-            }
             #[cfg(feature = "arg_where")]
             ArgWhere => {
                 wrap!(arg_where::arg_where)
             }
             #[cfg(feature = "search_sorted")]
             SearchSorted(side) => {
                 map_as_slice!(search_sorted::search_sorted_impl, side)
@@ -323,15 +353,15 @@
             #[cfg(all(feature = "rolling_window", feature = "moment"))]
             RollingSkew { window_size, bias } => {
                 map!(rolling::rolling_skew, window_size, bias)
             }
             ShiftAndFill { periods } => {
                 map_as_slice!(shift_and_fill::shift_and_fill, periods)
             }
-            Nan(n) => n.into(),
+            DropNans => map_owned!(nan::drop_nans),
             #[cfg(feature = "round_series")]
             Clip { min, max } => {
                 map_owned!(clip::clip, min.clone(), max.clone())
             }
             ListExpr(lf) => {
                 use ListFunction::*;
                 match lf {
@@ -356,36 +386,42 @@
                 }
             }
             #[cfg(feature = "top_k")]
             TopK { k, descending } => {
                 map!(top_k, k, descending)
             }
             Shift(periods) => map!(dispatch::shift, periods),
+            Cumcount { reverse } => map!(cum::cumcount, reverse),
+            Cumsum { reverse } => map!(cum::cumsum, reverse),
+            Cumprod { reverse } => map!(cum::cumprod, reverse),
+            Cummin { reverse } => map!(cum::cummin, reverse),
+            Cummax { reverse } => map!(cum::cummax, reverse),
             Reverse => map!(dispatch::reverse),
-            IsNull => map!(dispatch::is_null),
-            IsNotNull => map!(dispatch::is_not_null),
-            Not => map!(dispatch::is_not),
-            #[cfg(feature = "is_unique")]
-            IsUnique => map!(dispatch::is_unique),
-            #[cfg(feature = "is_unique")]
-            IsDuplicated => map!(dispatch::is_duplicated),
+            Boolean(func) => func.into(),
             Coalesce => map_as_slice!(fill_null::coalesce),
             ShrinkType => map_owned!(shrink_type::shrink),
             #[cfg(feature = "diff")]
             Diff(n, null_behavior) => map!(dispatch::diff, n, null_behavior),
             #[cfg(feature = "interpolate")]
             Interpolate(method) => {
                 map!(dispatch::interpolate, method)
             }
             #[cfg(feature = "dot_product")]
             Dot => {
                 map_as_slice!(dispatch::dot_impl)
             }
             #[cfg(feature = "log")]
-            Entropy { base, normalize } => map!(dispatch::entropy, base, normalize),
+            Entropy { base, normalize } => map!(log::entropy, base, normalize),
+            #[cfg(feature = "log")]
+            Log { base } => map!(log::log, base),
+            #[cfg(feature = "log")]
+            Log1p => map!(log::log1p),
+            #[cfg(feature = "log")]
+            Exp => map!(log::exp),
+            Unique(stable) => map!(unique::unique, stable),
         }
     }
 }
 
 #[cfg(feature = "strings")]
 impl From<StringFunction> for SpecialEq<Arc<dyn SeriesUdf>> {
     fn from(func: StringFunction) -> Self {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -100,21 +100,21 @@
                     polars_bail!(op = "cast-timezone", got = dt, expected = "Datetime");
                 }
             })
         };
 
         use FunctionExpr::*;
         match self {
+            #[cfg(feature = "abs")]
+            Abs => same_type(),
             NullCount => with_dtype(IDX_DTYPE),
             Pow => float_dtype(),
             Coalesce => super_type(),
             #[cfg(feature = "row_hash")]
             Hash(..) => with_dtype(DataType::UInt64),
-            #[cfg(feature = "is_in")]
-            IsIn => with_dtype(DataType::Boolean),
             #[cfg(feature = "arg_where")]
             ArgWhere => with_dtype(IDX_DTYPE),
             #[cfg(feature = "search_sorted")]
             SearchSorted(_) => with_dtype(IDX_DTYPE),
             #[cfg(feature = "strings")]
             StringExpr(s) => {
                 use StringFunction::*;
@@ -179,15 +179,15 @@
             Trigonometry(_) => float_dtype(),
             #[cfg(feature = "sign")]
             Sign => with_dtype(DataType::Int64),
             FillNull { super_type, .. } => with_dtype(super_type.clone()),
             #[cfg(all(feature = "rolling_window", feature = "moment"))]
             RollingSkew { .. } => float_dtype(),
             ShiftAndFill { .. } => same_type(),
-            Nan(n) => n.get_field(fields),
+            DropNans => same_type(),
             #[cfg(feature = "round_series")]
             Clip { .. } => same_type(),
             ListExpr(l) => {
                 use ListFunction::*;
                 match l {
                     Concat => inner_super_type_list(),
                     #[cfg(feature = "is_in")]
@@ -237,17 +237,20 @@
                         }
                     }
                 }
             }
             #[cfg(feature = "top_k")]
             TopK { .. } => same_type(),
             Shift(..) | Reverse => same_type(),
-            IsNotNull | IsNull | Not => with_dtype(DataType::Boolean),
-            #[cfg(feature = "is_unique")]
-            IsUnique | IsDuplicated => with_dtype(DataType::Boolean),
+            Boolean(f) => with_dtype(f.dtype_out()),
+            Cumcount { .. } => with_dtype(IDX_DTYPE),
+            Cumsum { .. } => map_dtype(&cum::dtypes::cumsum),
+            Cumprod { .. } => map_dtype(&cum::dtypes::cumprod),
+            Cummin { .. } => same_type(),
+            Cummax { .. } => same_type(),
             #[cfg(feature = "diff")]
             Diff(_, _) => map_dtype(&|dt| match dt {
                 #[cfg(feature = "dtype-datetime")]
                 DataType::Datetime(tu, _) => DataType::Duration(*tu),
                 #[cfg(feature = "dtype-date")]
                 DataType::Date => DataType::Duration(TimeUnit::Milliseconds),
                 #[cfg(feature = "dtype-time")]
@@ -287,11 +290,12 @@
                 use DataType::*;
                 match dt {
                     Int8 | Int16 | UInt16 | UInt8 => Int64,
                     _ => dt.clone(),
                 }
             }),
             #[cfg(feature = "log")]
-            Entropy { .. } => float_dtype(),
+            Entropy { .. } | Log { .. } | Log1p | Exp => float_dtype(),
+            Unique(_) => same_type(),
         }
     }
 }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files 0% similar despite different names*

```diff
@@ -180,18 +180,18 @@
                 GetOutput::from_type(IDX_DTYPE),
             )
             .with_fmt("arr.arg_max")
     }
 
     /// Diff every sublist.
     #[cfg(feature = "diff")]
-    pub fn diff(self, n: usize, null_behavior: NullBehavior) -> Expr {
+    pub fn diff(self, n: i64, null_behavior: NullBehavior) -> Expr {
         self.0
             .map(
-                move |s| Ok(Some(s.list()?.lst_diff(n, null_behavior).into_series())),
+                move |s| Ok(Some(s.list()?.lst_diff(n, null_behavior)?.into_series())),
                 GetOutput::same_type(),
             )
             .with_fmt("arr.diff")
     }
 
     /// Shift every sublist.
     pub fn shift(self, periods: i64) -> Expr {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -264,42 +264,42 @@
     pub fn lt_eq<E: Into<Expr>>(self, other: E) -> Expr {
         binary_expr(self, Operator::LtEq, other.into())
     }
 
     /// Negate `Expr`
     #[allow(clippy::should_implement_trait)]
     pub fn not(self) -> Expr {
-        self.map_private(FunctionExpr::Not)
+        self.map_private(BooleanFunction::IsNot.into())
     }
 
     /// Rename Column.
     pub fn alias(self, name: &str) -> Expr {
         Expr::Alias(Box::new(self), Arc::from(name))
     }
 
     /// Run is_null operation on `Expr`.
     #[allow(clippy::wrong_self_convention)]
     pub fn is_null(self) -> Self {
-        self.map_private(FunctionExpr::IsNull)
+        self.map_private(BooleanFunction::IsNull.into())
     }
 
     /// Run is_not_null operation on `Expr`.
     #[allow(clippy::wrong_self_convention)]
     pub fn is_not_null(self) -> Self {
-        self.map_private(FunctionExpr::IsNotNull)
+        self.map_private(BooleanFunction::IsNotNull.into())
     }
 
     /// Drop null values
     pub fn drop_nulls(self) -> Self {
         self.apply(|s| Ok(Some(s.drop_nulls())), GetOutput::same_type())
     }
 
     /// Drop NaN values
     pub fn drop_nans(self) -> Self {
-        self.apply_private(NanFunction::DropNans.into())
+        self.apply_private(FunctionExpr::DropNans)
     }
 
     /// Reduce groups to minimal value.
     pub fn min(self) -> Self {
         AggExpr::Min {
             input: Box::new(self),
             propagate_nans: false,
@@ -464,26 +464,21 @@
     pub fn tail(self, length: Option<usize>) -> Self {
         let len = length.unwrap_or(10);
         self.slice(lit(-(len as i64)), lit(len as u64))
     }
 
     /// Get unique values of this expression.
     pub fn unique(self) -> Self {
-        self.apply(|s: Series| s.unique().map(Some), GetOutput::same_type())
-            .with_fmt("unique")
+        self.apply_private(FunctionExpr::Unique(false))
     }
 
     /// Get unique values of this expression, while maintaining order.
     /// This requires more work than [`Expr::unique`].
     pub fn unique_stable(self) -> Self {
-        self.apply(
-            |s: Series| s.unique_stable().map(Some),
-            GetOutput::same_type(),
-        )
-        .with_fmt("unique_stable")
+        self.apply_private(FunctionExpr::Unique(true))
     }
 
     /// Get the first index of unique values of this expression.
     pub fn arg_unique(self) -> Self {
         self.apply(
             |s: Series| s.arg_unique().map(|ca| Some(ca.into_series())),
             GetOutput::from_type(IDX_DTYPE),
@@ -856,39 +851,31 @@
             },
         }
     }
 
     /// Get mask of finite values if dtype is Float
     #[allow(clippy::wrong_self_convention)]
     pub fn is_finite(self) -> Self {
-        self.map(
-            |s: Series| s.is_finite().map(|ca| Some(ca.into_series())),
-            GetOutput::from_type(DataType::Boolean),
-        )
-        .with_fmt("is_finite")
+        self.map_private(BooleanFunction::IsFinite.into())
     }
 
     /// Get mask of infinite values if dtype is Float
     #[allow(clippy::wrong_self_convention)]
     pub fn is_infinite(self) -> Self {
-        self.map(
-            |s: Series| s.is_infinite().map(|ca| Some(ca.into_series())),
-            GetOutput::from_type(DataType::Boolean),
-        )
-        .with_fmt("is_infinite")
+        self.map_private(BooleanFunction::IsInfinite.into())
     }
 
     /// Get mask of NaN values if dtype is Float
     pub fn is_nan(self) -> Self {
-        self.map_private(NanFunction::IsNan.into())
+        self.map_private(BooleanFunction::IsNan.into())
     }
 
     /// Get inverse mask of NaN values if dtype is Float
     pub fn is_not_nan(self) -> Self {
-        self.map_private(NanFunction::IsNotNan.into())
+        self.map_private(BooleanFunction::IsNotNan.into())
     }
 
     /// Shift the values in the array by some period. See [the eager implementation](polars_core::series::SeriesTrait::shift).
     pub fn shift(self, periods: i64) -> Self {
         self.apply_private(FunctionExpr::Shift(periods))
     }
 
@@ -898,72 +885,37 @@
             FunctionExpr::ShiftAndFill { periods },
             &[fill_value.into()],
             false,
             true,
         )
     }
 
+    /// Cumulatively count values from 0 to len.
+    pub fn cumcount(self, reverse: bool) -> Self {
+        self.apply_private(FunctionExpr::Cumcount { reverse })
+    }
+
     /// Get an array with the cumulative sum computed at every element
     pub fn cumsum(self, reverse: bool) -> Self {
-        self.apply(
-            move |s: Series| Ok(Some(s.cumsum(reverse))),
-            GetOutput::map_dtype(|dt| {
-                use DataType::*;
-                if dt.is_logical() {
-                    dt.clone()
-                } else {
-                    match dt {
-                        Boolean => UInt32,
-                        Int32 => Int32,
-                        UInt32 => UInt32,
-                        UInt64 => UInt64,
-                        Float32 => Float32,
-                        Float64 => Float64,
-                        _ => Int64,
-                    }
-                }
-            }),
-        )
-        .with_fmt("cumsum")
+        self.apply_private(FunctionExpr::Cumsum { reverse })
     }
 
     /// Get an array with the cumulative product computed at every element
     pub fn cumprod(self, reverse: bool) -> Self {
-        self.apply(
-            move |s: Series| Ok(Some(s.cumprod(reverse))),
-            GetOutput::map_dtype(|dt| {
-                use DataType::*;
-                match dt {
-                    Boolean => Int64,
-                    UInt64 => UInt64,
-                    Float32 => Float32,
-                    Float64 => Float64,
-                    _ => Int64,
-                }
-            }),
-        )
-        .with_fmt("cumprod")
+        self.apply_private(FunctionExpr::Cumprod { reverse })
     }
 
     /// Get an array with the cumulative min computed at every element
     pub fn cummin(self, reverse: bool) -> Self {
-        self.apply(
-            move |s: Series| Ok(Some(s.cummin(reverse))),
-            GetOutput::same_type(),
-        )
-        .with_fmt("cummin")
+        self.apply_private(FunctionExpr::Cummin { reverse })
     }
 
     /// Get an array with the cumulative max computed at every element
     pub fn cummax(self, reverse: bool) -> Self {
-        self.apply(
-            move |s: Series| Ok(Some(s.cummax(reverse))),
-            GetOutput::same_type(),
-        )
-        .with_fmt("cummax")
+        self.apply_private(FunctionExpr::Cummax { reverse })
     }
 
     /// Get the product aggregation of an expression
     pub fn product(self) -> Self {
         let options = FunctionOptions {
             collect_groups: ApplyOptions::ApplyGroups,
             auto_explode: true,
@@ -1054,16 +1006,15 @@
             max: None,
         })
     }
 
     /// Convert all values to their absolute/positive value.
     #[cfg(feature = "abs")]
     pub fn abs(self) -> Self {
-        self.map(move |s: Series| s.abs().map(Some), GetOutput::same_type())
-            .with_fmt("abs")
+        self.map_private(FunctionExpr::Abs)
     }
 
     /// Apply window function over a subgroup.
     /// This is similar to a groupby + aggregation + self join.
     /// Or similar to [window functions in Postgres](https://www.postgresql.org/docs/9.1/tutorial-window.html).
     ///
     /// # Example
@@ -1175,22 +1126,22 @@
         AggExpr::Var(Box::new(self), ddof).into()
     }
 
     /// Get a mask of duplicated values
     #[allow(clippy::wrong_self_convention)]
     #[cfg(feature = "is_unique")]
     pub fn is_duplicated(self) -> Self {
-        self.apply_private(FunctionExpr::IsDuplicated)
+        self.apply_private(BooleanFunction::IsDuplicated.into())
     }
 
     /// Get a mask of unique values
     #[allow(clippy::wrong_self_convention)]
     #[cfg(feature = "is_unique")]
     pub fn is_unique(self) -> Self {
-        self.apply_private(FunctionExpr::IsUnique)
+        self.apply_private(BooleanFunction::IsUnique.into())
     }
 
     /// and operation
     pub fn and<E: Into<Expr>>(self, expr: E) -> Self {
         binary_expr(self, Operator::And, expr.into())
     }
 
@@ -1232,17 +1183,17 @@
         {
             return Expr::Literal(LiteralValue::Boolean(false));
         }
 
         let arguments = &[other];
         // we don't have to apply on groups, so this is faster
         if has_literal {
-            self.map_many_private(FunctionExpr::IsIn, arguments, true)
+            self.map_many_private(BooleanFunction::IsIn.into(), arguments, true)
         } else {
-            self.apply_many_private(FunctionExpr::IsIn, arguments, true, true)
+            self.apply_many_private(BooleanFunction::IsIn.into(), arguments, true, true)
         }
     }
 
     /// Sort this column by the ordering of another column.
     /// Can also be used in a groupby context to sort the groups.
     pub fn sort_by<E: AsRef<[IE]>, IE: Into<Expr> + Clone, R: AsRef<[bool]>>(
         self,
@@ -1282,19 +1233,15 @@
         self.repeat_by_impl(by.into())
     }
 
     #[cfg(feature = "is_first")]
     #[allow(clippy::wrong_self_convention)]
     /// Get a mask of the first unique value.
     pub fn is_first(self) -> Expr {
-        self.apply(
-            |s| polars_ops::prelude::is_first(&s).map(|s| Some(s.into_series())),
-            GetOutput::from_type(DataType::Boolean),
-        )
-        .with_fmt("is_first")
+        self.apply_private(BooleanFunction::IsFirst.into())
     }
 
     #[cfg(feature = "dot_product")]
     fn dot_impl(self, other: Expr) -> Expr {
         self.apply_many_private(FunctionExpr::Dot, &[other], true, true)
     }
 
@@ -1643,20 +1590,20 @@
                 _ => Field::new(fld.name(), IDX_DTYPE),
             }),
         )
         .with_fmt("rank")
     }
 
     #[cfg(feature = "diff")]
-    pub fn diff(self, n: usize, null_behavior: NullBehavior) -> Expr {
+    pub fn diff(self, n: i64, null_behavior: NullBehavior) -> Expr {
         self.apply_private(FunctionExpr::Diff(n, null_behavior))
     }
 
     #[cfg(feature = "pct_change")]
-    pub fn pct_change(self, n: usize) -> Expr {
+    pub fn pct_change(self, n: i64) -> Expr {
         use DataType::*;
         self.apply(
             move |s| s.pct_change(n).map(Some),
             GetOutput::map_dtype(|dt| match dt {
                 Float64 | Float32 => dt.clone(),
                 _ => Float64,
             }),
@@ -1793,35 +1740,14 @@
                 Field::new(fld.name(), DataType::List(Box::new(dtype)))
             })
         };
         self.apply(move |s| s.reshape(&dims).map(Some), output_type)
             .with_fmt("reshape")
     }
 
-    /// Cumulatively count values from 0 to len.
-    pub fn cumcount(self, reverse: bool) -> Self {
-        self.apply(
-            move |s| {
-                if reverse {
-                    let ca: NoNull<UInt32Chunked> = (0u32..s.len() as u32).rev().collect();
-                    let mut ca = ca.into_inner();
-                    ca.rename(s.name());
-                    Ok(Some(ca.into_series()))
-                } else {
-                    let ca: NoNull<UInt32Chunked> = (0u32..s.len() as u32).collect();
-                    let mut ca = ca.into_inner();
-                    ca.rename(s.name());
-                    Ok(Some(ca.into_series()))
-                }
-            },
-            GetOutput::from_type(IDX_DTYPE),
-        )
-        .with_fmt("cumcount")
-    }
-
     #[cfg(feature = "random")]
     pub fn shuffle(self, seed: Option<u64>) -> Self {
         self.apply(move |s| Ok(Some(s.shuffle(seed))), GetOutput::same_type())
             .with_fmt("shuffle")
     }
 
     #[cfg(feature = "random")]
@@ -1894,57 +1820,35 @@
             }),
         )
         .with_fmt("ewm_var")
     }
 
     /// Check if any boolean value is `true`
     pub fn any(self) -> Self {
-        self.apply(
-            move |s| {
-                let boolean = s.bool()?;
-                if boolean.any() {
-                    Ok(Some(Series::new(s.name(), [true])))
-                } else {
-                    Ok(Some(Series::new(s.name(), [false])))
-                }
-            },
-            GetOutput::from_type(DataType::Boolean),
-        )
-        .with_function_options(|mut opt| {
-            opt.fmt_str = "any";
-            opt.auto_explode = true;
-            opt
-        })
+        self.apply_private(BooleanFunction::Any.into())
+            .with_function_options(|mut opt| {
+                opt.auto_explode = true;
+                opt
+            })
     }
 
     /// Shrink numeric columns to the minimal required datatype
     /// needed to fit the extrema of this [`Series`].
     /// This can be used to reduce memory pressure.
     pub fn shrink_dtype(self) -> Self {
         self.map_private(FunctionExpr::ShrinkType)
     }
 
     /// Check if all boolean values are `true`
     pub fn all(self) -> Self {
-        self.apply(
-            move |s| {
-                let boolean = s.bool()?;
-                if boolean.all() {
-                    Ok(Some(Series::new(s.name(), [true])))
-                } else {
-                    Ok(Some(Series::new(s.name(), [false])))
-                }
-            },
-            GetOutput::from_type(DataType::Boolean),
-        )
-        .with_function_options(|mut opt| {
-            opt.fmt_str = "all";
-            opt.auto_explode = true;
-            opt
-        })
+        self.apply_private(BooleanFunction::All.into())
+            .with_function_options(|mut opt| {
+                opt.auto_explode = true;
+                opt
+            })
     }
 
     #[cfg(feature = "dtype-struct")]
     /// Count all unique values and create a struct mapping value to count
     /// Note that it is better to turn multithreaded off in the aggregation context
     pub fn value_counts(self, multithreaded: bool, sorted: bool) -> Self {
         self.apply(
@@ -1977,41 +1881,27 @@
         )
         .with_fmt("unique_counts")
     }
 
     #[cfg(feature = "log")]
     /// Compute the logarithm to a given base
     pub fn log(self, base: f64) -> Self {
-        self.map(
-            move |s| Ok(Some(s.log(base))),
-            GetOutput::map_dtype(|dt| {
-                if matches!(dt, DataType::Float32) {
-                    DataType::Float32
-                } else {
-                    DataType::Float64
-                }
-            }),
-        )
-        .with_fmt("log")
+        self.map_private(FunctionExpr::Log { base })
+    }
+
+    #[cfg(feature = "log")]
+    /// Compute the natural logarithm of all elements plus one in the input array
+    pub fn log1p(self) -> Self {
+        self.map_private(FunctionExpr::Log1p)
     }
 
     #[cfg(feature = "log")]
     /// Calculate the exponential of all elements in the input array
     pub fn exp(self) -> Self {
-        self.map(
-            move |s| Ok(Some(s.exp())),
-            GetOutput::map_dtype(|dt| {
-                if matches!(dt, DataType::Float32) {
-                    DataType::Float32
-                } else {
-                    DataType::Float64
-                }
-            }),
-        )
-        .with_fmt("exp")
+        self.map_private(FunctionExpr::Exp)
     }
 
     #[cfg(feature = "log")]
     /// Compute the entropy as `-sum(pk * log(pk)`.
     /// where `pk` are discrete probabilities.
     pub fn entropy(self, base: f64, normalize: bool) -> Self {
         self.apply_private(FunctionExpr::Entropy { base, normalize })
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                         }
                     )
                 };
                 let is_not_null = |e: &AExpr| {
                     matches!(
                         e,
                         &AExpr::Function {
-                            function: FunctionExpr::IsNotNull,
+                            function: FunctionExpr::Boolean(BooleanFunction::IsNotNull),
                             ..
                         }
                     )
                 };
                 let is_column = |e: &AExpr| matches!(e, &AExpr::Column(_));
                 let is_lit_true =
                     |e: &AExpr| matches!(e, &AExpr::Literal(LiteralValue::Boolean(true)));
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -404,24 +404,32 @@
                 let mut pushdown_right = optimizer::init_hashmap(Some(acc_predicates.len()));
                 let mut local_predicates = Vec::with_capacity(acc_predicates.len());
 
                 for (_, predicate) in acc_predicates {
                     // unique and duplicated can be caused by joins
                     #[cfg(feature = "is_unique")]
                     let matches = {
-                        |e: &AExpr| matches!(e, AExpr::Function{function: FunctionExpr::IsDuplicated | FunctionExpr::IsUnique, ..})
+                        |e: &AExpr| matches!(e, AExpr::Function{
+                            function: FunctionExpr::Boolean(BooleanFunction::IsDuplicated)
+                                | FunctionExpr::Boolean(BooleanFunction::IsUnique),
+                            ..
+                        })
                     };
                     #[cfg(not(feature = "is_unique"))]
                         let matches = {
                         |_e: &AExpr| false
                     };
 
 
                     let checks_nulls =
-                        |e: &AExpr| matches!(e, AExpr::Function{function: FunctionExpr::IsNotNull | FunctionExpr::IsNull, ..} ) ||
+                        |e: &AExpr| matches!(e, AExpr::Function{
+                            function: FunctionExpr::Boolean(BooleanFunction::IsNotNull)
+                                | FunctionExpr::Boolean(BooleanFunction::IsNull),
+                            ..
+                        }) ||
                             // any operation that checks for equality or ordering can be wrong because
                             // the join can produce null values
                             matches!(e, AExpr::BinaryExpr {op, ..} if !matches!(op, Operator::NotEq));
                     if has_aexpr(predicate, expr_arena, matches)
                         // join might create null values.
                         || has_aexpr(predicate, expr_arena, checks_nulls)
                         // only these join types produce null values
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -250,24 +250,24 @@
                     None
                 } else {
                     Some(AExpr::Alias(*falsy, names[0].clone()))
                 }
             }
             AExpr::Function {
                 input,
-                function: FunctionExpr::Not,
+                function: FunctionExpr::Boolean(BooleanFunction::IsNot),
                 ..
             } => {
                 let y = expr_arena.get(input[0]);
 
                 match y {
                     // not(not x) => x
                     AExpr::Function {
                         input,
-                        function: FunctionExpr::Not,
+                        function: FunctionExpr::Boolean(BooleanFunction::IsNot),
                         ..
                     } => Some(expr_arena.get(input[0]).clone()),
                     // not(lit x) => !x
                     AExpr::Literal(LiteralValue::Boolean(b)) => {
                         Some(AExpr::Literal(LiteralValue::Boolean(!b)))
                     }
                     _ => None,
@@ -552,42 +552,42 @@
                 use Operator::*;
                 match (left_is_null, op, right_is_null) {
                     // all null operation null -> null
                     (true, _, true) => Some(AExpr::Literal(LiteralValue::Null)),
                     // null == column -> column.is_null()
                     (true, Eq, false) => Some(AExpr::Function {
                         input: vec![*right],
-                        function: FunctionExpr::IsNull,
+                        function: BooleanFunction::IsNull.into(),
                         options: FunctionOptions {
                             collect_groups: ApplyOptions::ApplyGroups,
                             ..Default::default()
                         },
                     }),
                     // column == null -> column.is_null()
                     (false, Eq, true) => Some(AExpr::Function {
                         input: vec![*left],
-                        function: FunctionExpr::IsNull,
+                        function: BooleanFunction::IsNull.into(),
                         options: FunctionOptions {
                             collect_groups: ApplyOptions::ApplyGroups,
                             ..Default::default()
                         },
                     }),
                     // null != column -> column.is_not_null()
                     (true, NotEq, false) => Some(AExpr::Function {
                         input: vec![*right],
-                        function: FunctionExpr::IsNotNull,
+                        function: BooleanFunction::IsNotNull.into(),
                         options: FunctionOptions {
                             collect_groups: ApplyOptions::ApplyGroups,
                             ..Default::default()
                         },
                     }),
                     // column != null -> column.is_not_null()
                     (false, NotEq, true) => Some(AExpr::Function {
                         input: vec![*left],
-                        function: FunctionExpr::IsNotNull,
+                        function: BooleanFunction::IsNotNull.into(),
                         options: FunctionOptions {
                             collect_groups: ApplyOptions::ApplyGroups,
                             ..Default::default()
                         },
                     }),
                     _ => None,
                 }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             AExpr::BinaryExpr {
                 left: node_left,
                 op,
                 right: node_right,
             } => return process_binary(expr_arena, lp_arena, lp_node, node_left, op, node_right),
             #[cfg(feature = "is_in")]
             AExpr::Function {
-                function: FunctionExpr::IsIn,
+                function: FunctionExpr::Boolean(BooleanFunction::IsIn),
                 ref input,
                 options,
             } => {
                 let input_schema = get_schema(lp_arena, lp_node);
                 let other_node = input[1];
                 let (_, type_left) =
                     unpack!(get_aexpr_and_type(expr_arena, input[0], &input_schema));
@@ -382,15 +382,15 @@
                 };
 
                 let mut input = input.clone();
                 let other_input = expr_arena.add(casted_expr);
                 input[1] = other_input;
 
                 Some(AExpr::Function {
-                    function: FunctionExpr::IsIn,
+                    function: FunctionExpr::Boolean(BooleanFunction::IsIn),
                     input,
                     options,
                 })
             }
             // fill null has a supertype set during projection
             // to make the schema known before the optimization phase
             AExpr::Function {
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files 6% similar despite different names*

```diff
@@ -80,33 +80,33 @@
                     } else {
                         None
                     }
                 }
             }
         }
         AExpr::Function {
-            function: FunctionExpr::Not,
+            function: FunctionExpr::Boolean(BooleanFunction::IsNot),
             input,
             ..
         } => {
             let input = input.first().unwrap();
             let input = predicate_to_pa(*input, expr_arena)?;
             Some(format!("~({input})"))
         }
         AExpr::Function {
-            function: FunctionExpr::IsNull,
+            function: FunctionExpr::Boolean(BooleanFunction::IsNull),
             input,
             ..
         } => {
             let input = input.first().unwrap();
             let input = predicate_to_pa(*input, expr_arena)?;
             Some(format!("({input}).is_null()"))
         }
         AExpr::Function {
-            function: FunctionExpr::IsNotNull,
+            function: FunctionExpr::Boolean(BooleanFunction::IsNotNull),
             input,
             ..
         } => {
             let input = input.first().unwrap();
             let input = predicate_to_pa(*input, expr_arena)?;
             Some(format!("~({input}).is_null()"))
         }
```

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.17.2/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/Cargo.toml` & `polars_lts_cpu-0.17.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.1"
+version = "0.17.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.17.1/LICENSE` & `polars_lts_cpu-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/Makefile` & `polars_lts_cpu-0.17.2/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/README.md` & `polars_lts_cpu-0.17.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 | timezone   | Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are on Windows, otherwise no dependencies will be installed |
 
 Releases happen quite often (weekly / every few days) at the moment, so updating polars regularly to get the latest bugfixes / features might not be a bad idea.
 
 ### Rust
 
 You can take latest release from `crates.io`, or if you want to use the latest features / performance improvements
-point to the `master` branch of this repo.
+point to the `main` branch of this repo.
 
 ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "<optional git tag>" }
 ```
 
 Required Rust version `>=1.62`
```

#### html2text {}

```diff
@@ -64,15 +64,15 @@
 for reading from SQL databases | | xlsx2csv | Support for reading from Excel
 files | | deltalake | Support for reading from Delta Lake Tables | | timezone |
 Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are
 on Windows, otherwise no dependencies will be installed | Releases happen quite
 often (weekly / every few days) at the moment, so updating polars regularly to
 get the latest bugfixes / features might not be a bad idea. ### Rust You can
 take latest release from `crates.io`, or if you want to use the latest features
-/ performance improvements point to the `master` branch of this repo. ```toml
+/ performance improvements point to the `main` branch of this repo. ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "" } ``` Required
 Rust version `>=1.62` ## Contributing Want to contribute? Read our
 [contribution guideline](./CONTRIBUTING.md). ## Python: compile polars from
 source If you want a bleeding edge release or maximal performance you should
 compile **polars** from source. This can be done by going through the following
 steps in sequence: 1. Install the latest [Rust compiler](https://www.rust-
 lang.org/tools/install) 2. Install [maturin](https://maturin.rs/): `pip install
```

### Comparing `polars_lts_cpu-0.17.1/build.rs` & `polars_lts_cpu-0.17.2/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/Makefile` & `polars_lts_cpu-0.17.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.17.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.17.2/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/conf.py` & `polars_lts_cpu-0.17.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     conf_dir_path = os.path.dirname(os.path.realpath(__file__))
     polars_root = os.path.abspath(f"{conf_dir_path}/../../polars")
 
     fn = os.path.relpath(fn, start=polars_root)
 
     return (
-        f"https://github.com/pola-rs/polars/blob/master/py-polars/polars/{fn}{linespec}"
+        f"https://github.com/pola-rs/polars/blob/main/py-polars/polars/{fn}{linespec}"
     )
 
 
 def _minify_classpaths(s: str) -> str:
     # strip private polars classpaths, leaving the classname:
     # * "pli.Expr" -> "Expr"
     # * "polars.expr.expr.Expr" -> "Expr"
```

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/api.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/config.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/computation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Expr.ewm_std
     Expr.ewm_var
     Expr.exp
     Expr.hash
     Expr.kurtosis
     Expr.log
     Expr.log10
+    Expr.log1p
     Expr.mode
     Expr.n_unique
     Expr.null_count
     Expr.pct_change
     Expr.rank
     Expr.rolling_apply
     Expr.rolling_max
```

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/functions.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/io.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/computation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Series.ewm_var
     Series.exp
     Series.hash
     Series.is_between
     Series.kurtosis
     Series.log
     Series.log10
+    Series.log1p
     Series.map_dict
     Series.pct_change
     Series.peak_max
     Series.peak_min
     Series.rank
     Series.rolling_apply
     Series.rolling_max
```

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/docs/source/reference/testing.rst` & `polars_lts_cpu-0.17.2/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/__init__.py` & `polars_lts_cpu-0.17.2/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/api.py` & `polars_lts_cpu-0.17.2/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/config.py` & `polars_lts_cpu-0.17.2/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/convert.py` & `polars_lts_cpu-0.17.2/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/dataframe/_html.py` & `polars_lts_cpu-0.17.2/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/dataframe/frame.py` & `polars_lts_cpu-0.17.2/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module containing logic related to eager DataFrames."""
 from __future__ import annotations
 
 import contextlib
-import math
 import os
 import random
 import typing
 import warnings
 from collections.abc import Sized
 from io import BytesIO, StringIO
 from pathlib import Path
@@ -6277,14 +6276,16 @@
         ╞════════╪════════╪════════╪════════╪════════╪════════╡
         │ A      ┆ B      ┆ C      ┆ 0      ┆ 1      ┆ 2      │
         │ D      ┆ E      ┆ F      ┆ 3      ┆ 4      ┆ 5      │
         │ G      ┆ H      ┆ I      ┆ 6      ┆ 7      ┆ 8      │
         └────────┴────────┴────────┴────────┴────────┴────────┘
 
         """
+        import math
+
         df = self.select(columns) if columns is not None else self
 
         height = df.height
         if how == "vertical":
             n_rows = step
             n_cols = math.ceil(height / n_rows)
         else:
```

### Comparing `polars_lts_cpu-0.17.1/polars/dataframe/groupby.py` & `polars_lts_cpu-0.17.2/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/datatypes/__init__.py` & `polars_lts_cpu-0.17.2/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/datatypes/classes.py` & `polars_lts_cpu-0.17.2/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/datatypes/constants.py` & `polars_lts_cpu-0.17.2/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/datatypes/constructor.py` & `polars_lts_cpu-0.17.2/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/datatypes/convert.py` & `polars_lts_cpu-0.17.2/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/dependencies.py` & `polars_lts_cpu-0.17.2/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/exceptions.py` & `polars_lts_cpu-0.17.2/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/binary.py` & `polars_lts_cpu-0.17.2/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/categorical.py` & `polars_lts_cpu-0.17.2/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/datetime.py` & `polars_lts_cpu-0.17.2/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/expr.py` & `polars_lts_cpu-0.17.2/polars/expr/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -6653,14 +6653,38 @@
         │ 1.0      │
         │ 1.584963 │
         └──────────┘
 
         """
         return self._from_pyexpr(self._pyexpr.log(base))
 
+    def log1p(self) -> Self:
+        """
+        Compute the natural logarithm of each element plus one.
+
+        This computes `log(1 + x)` but is more numerically stable for `x` close to zero.
+
+        Examples
+        --------
+        >>> df = pl.DataFrame({"a": [1, 2, 3]})
+        >>> df.select(pl.col("a").log1p())
+        shape: (3, 1)
+        ┌──────────┐
+        │ a        │
+        │ ---      │
+        │ f64      │
+        ╞══════════╡
+        │ 0.693147 │
+        │ 1.098612 │
+        │ 1.386294 │
+        └──────────┘
+
+        """
+        return self._from_pyexpr(self._pyexpr.log1p())
+
     def entropy(self, base: float = math.e, *, normalize: bool = True) -> Self:
         """
         Computes the entropy.
 
         Uses the formula ``-sum(pk * log(pk)`` where ``pk`` are discrete probabilities.
 
         Parameters
```

### Comparing `polars_lts_cpu-0.17.1/polars/expr/list.py` & `polars_lts_cpu-0.17.2/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/meta.py` & `polars_lts_cpu-0.17.2/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/string.py` & `polars_lts_cpu-0.17.2/polars/expr/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/expr/struct.py` & `polars_lts_cpu-0.17.2/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/functions/__init__.py` & `polars_lts_cpu-0.17.2/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/functions/eager.py` & `polars_lts_cpu-0.17.2/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/functions/lazy.py` & `polars_lts_cpu-0.17.2/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/functions/whenthen.py` & `polars_lts_cpu-0.17.2/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/__init__.py` & `polars_lts_cpu-0.17.2/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/_utils.py` & `polars_lts_cpu-0.17.2/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/avro.py` & `polars_lts_cpu-0.17.2/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/csv/_utils.py` & `polars_lts_cpu-0.17.2/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.17.2/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/csv/functions.py` & `polars_lts_cpu-0.17.2/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/database.py` & `polars_lts_cpu-0.17.2/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/delta.py` & `polars_lts_cpu-0.17.2/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.17.2/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/excel/functions.py` & `polars_lts_cpu-0.17.2/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.17.2/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/ipc/functions.py` & `polars_lts_cpu-0.17.2/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/json.py` & `polars_lts_cpu-0.17.2/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/ndjson.py` & `polars_lts_cpu-0.17.2/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.17.2/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/parquet/functions.py` & `polars_lts_cpu-0.17.2/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.17.2/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.17.2/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/lazyframe/frame.py` & `polars_lts_cpu-0.17.2/polars/lazyframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.17.2/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/_numpy.py` & `polars_lts_cpu-0.17.2/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/binary.py` & `polars_lts_cpu-0.17.2/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/categorical.py` & `polars_lts_cpu-0.17.2/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/datetime.py` & `polars_lts_cpu-0.17.2/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/list.py` & `polars_lts_cpu-0.17.2/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/series.py` & `polars_lts_cpu-0.17.2/polars/series/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1081,14 +1081,17 @@
 
         """
         return self.to_frame().select(F.col(self.name).all()).to_series()[0]
 
     def log(self, base: float = math.e) -> Series:
         """Compute the logarithm to a given base."""
 
+    def log1p(self) -> Series:
+        """Compute the natural logarithm of the input array plus one, element-wise."""
+
     def log10(self) -> Series:
         """Compute the base 10 logarithm of the input array, element-wise."""
 
     def exp(self) -> Series:
         """Compute the exponential, element-wise."""
 
     def drop_nulls(self) -> Series:
```

### Comparing `polars_lts_cpu-0.17.1/polars/series/string.py` & `polars_lts_cpu-0.17.2/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/struct.py` & `polars_lts_cpu-0.17.2/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/series/utils.py` & `polars_lts_cpu-0.17.2/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/slice.py` & `polars_lts_cpu-0.17.2/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/sql/context.py` & `polars_lts_cpu-0.17.2/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/string_cache.py` & `polars_lts_cpu-0.17.2/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/testing/_parametric.py` & `polars_lts_cpu-0.17.2/polars/testing/_parametric.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import os
 import random
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from math import isfinite
-from typing import TYPE_CHECKING, Any, Sequence
+from textwrap import dedent
+from typing import TYPE_CHECKING, Any, Sequence, cast
 
 from hypothesis import settings
 from hypothesis.errors import InvalidArgument, NonInteractiveExampleWarning
 from hypothesis.strategies import (
     booleans,
     composite,
     dates,
@@ -47,14 +48,15 @@
     Utf8,
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.series import Series
 from polars.string_cache import StringCache
 from polars.testing.asserts import is_categorical_dtype
+from polars.type_aliases import Orientation
 
 if TYPE_CHECKING:
     from hypothesis.strategies import DrawFn, SearchStrategy
 
     from polars.lazyframe import LazyFrame
     from polars.type_aliases import OneOrMoreDataTypes, PolarsDataType
 
@@ -449,14 +451,17 @@
                 split_at = series_size // 2
                 s = s[:split_at].append(s[split_at:], append_chunks=True)
             return s
 
     return draw_series()
 
 
+_failed_frame_init_msgs_: set[str] = set()
+
+
 @defines_strategy()
 def dataframes(
     cols: int | column | Sequence[column] | None = None,
     lazy: bool = False,
     *,
     min_cols: int | None = 0,
     max_cols: int | None = MAX_COLS,
@@ -559,25 +564,28 @@
     │ ---       ┆ ---        │
     │ i32       ┆ f64        │
     ╞═══════════╪════════════╡
     │ -15836    ┆ 1.1755e-38 │
     │ 575050513 ┆ NaN        │
     └───────────┴────────────┘
     """  # noqa: 501
+    _failed_frame_init_msgs_.clear()
+
     if isinstance(min_size, int) and min_cols in (0, None):
         min_cols = 1
 
     selectable_dtypes = [
         dtype
         for dtype in (allowed_dtypes or strategy_dtypes)
         if dtype not in (excluded_dtypes or ())
     ]
 
     @composite
     def draw_frames(draw: DrawFn) -> DataFrame | LazyFrame:
+        """Reproducibly generate random DataFrames according to the given spec."""
         with StringCache():
             # if not given, create 'n' cols with random dtypes
             if cols is None or isinstance(cols, int):
                 n = cols or between(
                     draw, int, min_=(min_cols or 0), max_=(max_cols or MAX_COLS)
                 )
                 dtypes_ = [draw(sampled_from(selectable_dtypes)) for _ in range(n)]
@@ -594,48 +602,72 @@
             series_size = (
                 between(
                     draw, int, min_=(min_size or 0), max_=(max_size or MAX_DATA_SIZE)
                 )
                 if size is None
                 else size
             )
-            # init dataframe from generated series data; series data is
-            # given as a python-native sequence (TODO: or as an arrow array).
+
+            # assign names, null probability
             for idx, c in enumerate(coldefs):
                 if c.name is None:
                     c.name = f"col{idx}"
                 if c.null_probability is None:
                     if isinstance(null_probability, dict):
                         c.null_probability = null_probability.get(c.name, 0.0)
                     else:
                         c.null_probability = null_probability
 
-            frame_columns = [
-                c.name if (c.dtype is None) else (c.name, c.dtype) for c in coldefs
-            ]
-            df = DataFrame(
-                data={
-                    c.name: draw(
-                        series(
-                            name=c.name,
-                            dtype=c.dtype,
-                            size=series_size,
-                            null_probability=(c.null_probability or 0.0),
-                            allow_infinities=allow_infinities,
-                            strategy=c.strategy,
-                            unique=c.unique,
-                            chunked=(chunked is None and draw(booleans())),
-                        )
+            # init dataframe from generated series data; series data is
+            # given as a python-native sequence.
+            data = {
+                c.name: draw(
+                    series(
+                        name=c.name,
+                        dtype=c.dtype,
+                        size=series_size,
+                        null_probability=(c.null_probability or 0.0),
+                        allow_infinities=allow_infinities,
+                        strategy=c.strategy,
+                        unique=c.unique,
+                        chunked=(chunked is None and draw(booleans())),
                     )
-                    for c in coldefs
-                },
-                schema=frame_columns,  # type: ignore[arg-type]
-            )
-            # optionally generate frames with n_chunks > 1
-            if series_size > 1 and chunked is True:
-                split_at = series_size // 2
-                df = df[:split_at].vstack(df[split_at:])
+                )
+                for c in coldefs
+            }
 
-            # optionally make lazy
-            return df.lazy() if lazy else df
+            # note: randomly change between row-wise and column-wise frame init
+            orient = cast(Orientation, "row" if draw(booleans()) else "col")
+            data = list(zip(*data.values())) if orient == "row" else data  # type: ignore[assignment]
+            schema = [(c.name, c.dtype) for c in coldefs]
+            try:
+                df = DataFrame(data=data, schema=schema, orient=orient)
+
+                # optionally generate chunked frames
+                if series_size > 1 and chunked is True:
+                    split_at = series_size // 2
+                    df = df[:split_at].vstack(df[split_at:])
+
+                _failed_frame_init_msgs_.clear()
+                return df.lazy() if lazy else df
+
+            except Exception:
+                # print code that will allow any init failure to be reproduced
+                failed_frame_init = dedent(
+                    f"""
+                    # failed frame init: reproduce with...
+                    pl.DataFrame(
+                        data={data!r},
+                        schema={repr(schema).replace("', ","', pl.")},
+                        orient={orient!r},
+                    )
+                    """.replace(
+                        "datetime.", ""
+                    )
+                )
+                # note: this avoids printing the repro twice
+                if failed_frame_init not in _failed_frame_init_msgs_:
+                    _failed_frame_init_msgs_.add(failed_frame_init)
+                    print(failed_frame_init)
+                raise
 
     return draw_frames()
```

### Comparing `polars_lts_cpu-0.17.1/polars/testing/_private.py` & `polars_lts_cpu-0.17.2/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/testing/asserts.py` & `polars_lts_cpu-0.17.2/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/testing/parametric.py` & `polars_lts_cpu-0.17.2/polars/testing/parametric.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/type_aliases.py` & `polars_lts_cpu-0.17.2/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/__init__.py` & `polars_lts_cpu-0.17.2/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/_construction.py` & `polars_lts_cpu-0.17.2/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.17.2/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/_scan.py` & `polars_lts_cpu-0.17.2/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/_wrap.py` & `polars_lts_cpu-0.17.2/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/build_info.py` & `polars_lts_cpu-0.17.2/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/convert.py` & `polars_lts_cpu-0.17.2/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/decorators.py` & `polars_lts_cpu-0.17.2/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/meta.py` & `polars_lts_cpu-0.17.2/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/polars_version.py` & `polars_lts_cpu-0.17.2/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/polars/utils/show_versions.py` & `polars_lts_cpu-0.17.2/polars/utils/show_versions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from __future__ import annotations
 
-import importlib
 import sys
 
 from polars.utils.meta import get_index_type
 from polars.utils.polars_version import get_polars_version
 
-# metadata module must be imported explicitly
-if sys.version_info >= (3, 8):
-    import importlib.metadata
-
 
 def show_versions() -> None:
     """
     Print out version of Polars and dependencies to stdout.
 
     Examples
     --------
@@ -63,21 +58,27 @@
         "xlsx2csv",
         "xlsxwriter",
     ]
     return {name: _get_dependency_version(name) for name in opt_deps}
 
 
 def _get_dependency_version(dep_name: str) -> str:
+    # note: we import 'importlib' here as a significiant optimisation for initial import
+    import importlib
+
+    if sys.version_info >= (3, 8):
+        # importlib.metadata was introduced in Python 3.8;
+        # metadata submodule must be imported explicitly
+        import importlib.metadata
     try:
         module = importlib.import_module(dep_name)
     except ImportError:
         return "<not installed>"
 
     if hasattr(module, "__version__"):
         module_version = module.__version__
     elif sys.version_info >= (3, 8):
-        # importlib.metadata was introduced in Python 3.8
         module_version = importlib.metadata.version(dep_name)
     else:
         module_version = "<version not detected>"
 
     return module_version
```

### Comparing `polars_lts_cpu-0.17.1/polars/utils/various.py` & `polars_lts_cpu-0.17.2/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/pyproject.toml` & `polars_lts_cpu-0.17.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/requirements-dev.txt` & `polars_lts_cpu-0.17.2/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 tzdata; platform_system == 'Windows'
 xlsx2csv
 XlsxWriter
 adbc_driver_sqlite; python_version >= '3.9' and platform_system != 'Windows'
 connectorx==0.3.2a2; python_version >= '3.8'  # Latest full release is broken - unpin when 0.3.2 released
 
 # Tooling
-hypothesis==6.70.1
+hypothesis==6.71.0
 maturin==0.14.10
-pytest==7.2.0
+pytest==7.3.0
 pytest-cov==4.0.0
 pytest-xdist==3.2.0
 
 # Stub files
 pandas-stubs==1.2.0.62
```

### Comparing `polars_lts_cpu-0.17.1/scripts/check_stacklevels.py` & `polars_lts_cpu-0.17.2/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/apply/dataframe.rs` & `polars_lts_cpu-0.17.2/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/apply/mod.rs` & `polars_lts_cpu-0.17.2/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/apply/series.rs` & `polars_lts_cpu-0.17.2/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.17.2/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.17.2/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/batched_csv.rs` & `polars_lts_cpu-0.17.2/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/conversion.rs` & `polars_lts_cpu-0.17.2/src/conversion.rs`

 * *Files 2% similar despite different names*

```diff
@@ -711,14 +711,16 @@
                 let dtype = DataType::from(&val);
                 keys.push(Field::new(key, dtype));
                 vals.push(val)
             }
             Ok(Wrap(AnyValue::StructOwned(Box::new((vals, keys)))))
         } else if ob.is_instance_of::<PyList>()? {
             materialize_list(ob)
+        } else if let Ok(value) = ob.extract::<u64>() {
+            Ok(AnyValue::UInt64(value).into())
         } else if ob.hasattr("_s")? {
             let py_pyseries = ob.getattr("_s").unwrap();
             let series = py_pyseries.extract::<PySeries>().unwrap().series;
             Ok(Wrap(AnyValue::List(series)))
         } else if let Ok(v) = ob.extract::<&'s [u8]>() {
             Ok(AnyValue::Binary(v).into())
         } else {
@@ -775,17 +777,18 @@
                             }
                             "<class 'datetime.date'>" => {
                                 return convert_date(ob);
                             }
                             _ => (),
                         }
                     }
-                    Err(PyErr::from(PyPolarsErr::Other(format!(
-                        "object type not supported {ob:?}",
-                    ))))
+
+                    // this is slow, but hey don't use objects
+                    let v = &ObjectValue { inner: ob.into() };
+                    Ok(Wrap(AnyValue::ObjectOwned(OwnedObject(v.to_boxed()))))
                 }
             }
         }
     }
 }
 
 impl<'s> FromPyObject<'s> for Wrap<Row<'s>> {
```

### Comparing `polars_lts_cpu-0.17.1/src/dataframe.rs` & `polars_lts_cpu-0.17.2/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/datatypes.rs` & `polars_lts_cpu-0.17.2/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/error.rs` & `polars_lts_cpu-0.17.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/file.rs` & `polars_lts_cpu-0.17.2/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/lazy/apply.rs` & `polars_lts_cpu-0.17.2/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/lazy/dataframe.rs` & `polars_lts_cpu-0.17.2/src/lazy/dataframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
             let ldf = self.ldf.clone();
             ldf.collect().map_err(PyPolarsErr::from)
         })?;
         Ok(df.into())
     }
 
     #[allow(clippy::too_many_arguments)]
-    #[cfg(feature = "streaming")]
+    #[cfg(all(feature = "streaming", feature = "parquet"))]
     #[pyo3(signature = (path, compression, compression_level, statistics, row_group_size, data_pagesize_limit, maintain_order))]
     pub fn sink_parquet(
         &self,
         py: Python,
         path: PathBuf,
         compression: &str,
         compression_level: Option<i32>,
@@ -507,15 +507,15 @@
             let ldf = self.ldf.clone();
             ldf.sink_parquet(path, options).map_err(PyPolarsErr::from)
         })?;
         Ok(())
     }
 
     #[allow(clippy::too_many_arguments)]
-    #[cfg(feature = "streaming")]
+    #[cfg(all(feature = "streaming", feature = "ipc"))]
     #[pyo3(signature = (path, compression, maintain_order))]
     pub fn sink_ipc(
         &self,
         py: Python,
         path: PathBuf,
         compression: Option<Wrap<IpcCompression>>,
         maintain_order: bool,
```

### Comparing `polars_lts_cpu-0.17.1/src/lazy/dsl.rs` & `polars_lts_cpu-0.17.2/src/lazy/dsl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -720,14 +720,15 @@
     }
 
     pub fn str_rjust(&self, width: usize, fillchar: char) -> PyExpr {
         self.clone().inner.str().rjust(width, fillchar).into()
     }
 
     #[pyo3(signature = (pat, literal, strict))]
+    #[cfg(feature = "lazy_regex")]
     pub fn str_contains(&self, pat: PyExpr, literal: Option<bool>, strict: bool) -> PyExpr {
         match literal {
             Some(true) => self.inner.clone().str().contains_literal(pat.inner).into(),
             _ => self.inner.clone().str().contains(pat.inner, strict).into(),
         }
     }
 
@@ -859,14 +860,15 @@
                 },
                 GetOutput::same_type(),
             )
             .with_fmt("binary.base64_decode")
             .into()
     }
 
+    #[cfg(feature = "extract_jsonpath")]
     pub fn str_json_extract(&self, dtype: Option<Wrap<DataType>>) -> PyExpr {
         let dtype = dtype.map(|wrap| wrap.0);
 
         let output_type = match dtype.clone() {
             Some(dtype) => GetOutput::from_type(dtype),
             None => GetOutput::from_type(DataType::Unknown),
         };
@@ -1576,15 +1578,15 @@
         self.inner.clone().arr().arg_min().into()
     }
 
     fn lst_arg_max(&self) -> Self {
         self.inner.clone().arr().arg_max().into()
     }
 
-    fn lst_diff(&self, n: usize, null_behavior: Wrap<NullBehavior>) -> PyResult<Self> {
+    fn lst_diff(&self, n: i64, null_behavior: Wrap<NullBehavior>) -> PyResult<Self> {
         Ok(self.inner.clone().arr().diff(n, null_behavior.0).into())
     }
 
     fn lst_shift(&self, periods: i64) -> Self {
         self.inner.clone().arr().shift(periods).into()
     }
 
@@ -1641,20 +1643,20 @@
         let options = RankOptions {
             method: method.0,
             descending,
         };
         self.inner.clone().rank(options, seed).into()
     }
 
-    fn diff(&self, n: usize, null_behavior: Wrap<NullBehavior>) -> Self {
+    fn diff(&self, n: i64, null_behavior: Wrap<NullBehavior>) -> Self {
         self.inner.clone().diff(n, null_behavior.0).into()
     }
 
     #[cfg(feature = "pct_change")]
-    fn pct_change(&self, n: usize) -> Self {
+    fn pct_change(&self, n: i64) -> Self {
         self.inner.clone().pct_change(n).into()
     }
 
     fn skew(&self, bias: bool) -> Self {
         self.inner.clone().skew(bias).into()
     }
     fn kurtosis(&self, fisher: bool, bias: bool) -> Self {
@@ -1803,14 +1805,18 @@
         self.inner.clone().struct_().rename_fields(names).into()
     }
 
     pub fn log(&self, base: f64) -> Self {
         self.inner.clone().log(base).into()
     }
 
+    pub fn log1p(&self) -> Self {
+        self.inner.clone().log1p().into()
+    }
+
     pub fn exp(&self) -> Self {
         self.inner.clone().exp().into()
     }
 
     pub fn entropy(&self, base: f64, normalize: bool) -> Self {
         self.inner.clone().entropy(base, normalize).into()
     }
```

### Comparing `polars_lts_cpu-0.17.1/src/lazy/meta.rs` & `polars_lts_cpu-0.17.2/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/lazy/mod.rs` & `polars_lts_cpu-0.17.2/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/lib.rs` & `polars_lts_cpu-0.17.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/list_construction.rs` & `polars_lts_cpu-0.17.2/src/list_construction.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/npy.rs` & `polars_lts_cpu-0.17.2/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/object.rs` & `polars_lts_cpu-0.17.2/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/series.rs` & `polars_lts_cpu-0.17.2/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/set.rs` & `polars_lts_cpu-0.17.2/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/sql.rs` & `polars_lts_cpu-0.17.2/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/src/utils.rs` & `polars_lts_cpu-0.17.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/README.md` & `polars_lts_cpu-0.17.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.17.2/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.17.2/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/benchmark/test_release.py` & `polars_lts_cpu-0.17.2/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/docs/run_doctest.py` & `polars_lts_cpu-0.17.2/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.17.2/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.17.2/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/parametric/test_series.py` & `polars_lts_cpu-0.17.2/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/parametric/test_testing.py` & `polars_lts_cpu-0.17.2/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/conftest.py` & `polars_lts_cpu-0.17.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from uuid import uuid4
+
 import numpy as np
 
 import polars as pl
 
 
 def test_object_when_then_4702() -> None:
     # please don't ever do this
@@ -88,7 +90,21 @@
         schema={"a": pl.Object},
     )
 
     catted = pl.concat([df1, df2])
     assert catted.shape == (6, 1)
     assert catted.dtypes == [pl.Object]
     assert catted.to_dict(False) == {"a": [1, 2, 3, 1, 4, 3]}
+
+
+def test_object_row_construction() -> None:
+    data = [
+        [uuid4()],
+        [uuid4()],
+        [uuid4()],
+    ]
+    df = pl.DataFrame(
+        data,
+        orient="row",
+    )
+    assert df.dtypes == [pl.Object]
+    assert df["column_0"].to_list() == [value[0] for value in data]
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,7 +884,21 @@
         {
             "numerical": [1, 2, 1],
             "struct": [{"x": 1, "y": 2}, {"x": 3, "y": 4}, {"x": 1, "y": 2}],
         }
     )
 
     df.select("numerical", "struct").unique().sort("numerical")
+
+
+def test_struct_is_in() -> None:
+    s1 = (
+        pl.DataFrame({"x": [4, 3, 4, 9], "y": [0, 4, 6, 2]})
+        .select(pl.struct(["x", "y"]))
+        .to_series()
+    )
+    s2 = (
+        pl.DataFrame({"x": [4, 3, 5, 9], "y": [0, 7, 6, 2]})
+        .select(pl.struct(["x", "y"]))
+        .to_series()
+    )
+    assert s1.is_in(s2).to_list() == [True, False, False, True]
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.17.2/tests/unit/datatypes/test_temporal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.17.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.17.2/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.17.2/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.17.2/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1242,15 +1242,15 @@
 
     # The next value should always be higher if monotonically increasing.
     assert df.filter(pl.col("count") < pl.col("count").shift(1)).is_empty()
 
 
 @pytest.mark.slow()
 def test_read_web_file() -> None:
-    url = "https://raw.githubusercontent.com/pola-rs/polars/master/examples/datasets/foods1.csv"
+    url = "https://raw.githubusercontent.com/pola-rs/polars/main/examples/datasets/foods1.csv"
     df = pl.read_csv(url)
     assert df.shape == (27, 4)
 
 
 @pytest.mark.slow()
 def test_csv_multiline_splits() -> None:
     # create a very unlikely csv file with many multilines in a
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_database.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_json.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_other.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.17.2/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.17.2/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.17.2/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_api.py` & `polars_lts_cpu-0.17.2/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_arity.py` & `polars_lts_cpu-0.17.2/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_cfg.py` & `polars_lts_cpu-0.17.2/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_constructors.py` & `polars_lts_cpu-0.17.2/tests/unit/test_constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -976,7 +976,13 @@
 
     result = pl.Series([FakeDatetime(2020, 1, 1, 3)])
     expected = pl.Series([datetime(2020, 1, 1, 3)])
     assert_series_equal(result, expected)
     result = pl.Series([FakeDate(2020, 1, 1)])
     expected = pl.Series([date(2020, 1, 1)])
     assert_series_equal(result, expected)
+
+
+def test_list_null_constructor() -> None:
+    s = pl.Series("a", [[None], [None]], dtype=pl.List(pl.Null))
+    assert s.dtype == pl.List(pl.Null)
+    assert s.to_list() == [None, None]
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_cse.py` & `polars_lts_cpu-0.17.2/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.17.2/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_df.py` & `polars_lts_cpu-0.17.2/tests/unit/test_df.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_empty.py` & `polars_lts_cpu-0.17.2/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_errors.py` & `polars_lts_cpu-0.17.2/tests/unit/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,35 @@
 
 def test_error_on_reducing_map() -> None:
     df = pl.DataFrame(
         {"id": [0, 0, 0, 1, 1, 1], "t": [2, 4, 5, 10, 11, 14], "y": [0, 1, 1, 2, 3, 4]}
     )
 
     with pytest.raises(
-        pl.ComputeError,
+        pl.InvalidOperationError,
         match=(
             "output length of `map` must be equal to that of the input length; consider using `apply` instead"
         ),
     ):
         df.groupby("id").agg(pl.map(["t", "y"], np.trapz))
 
+    df = pl.DataFrame({"x": [1, 2, 3, 4], "group": [1, 2, 1, 2]})
+
+    with pytest.raises(
+        pl.InvalidOperationError,
+        match=(
+            "output length of `map` must be equal to that of the input length; consider using `apply` instead"
+        ),
+    ):
+        df.select(
+            pl.col("x")
+            .map(lambda x: x.cut(bins=[1, 2, 3], maintain_order=True))
+            .over("group")
+        )
+
 
 def test_error_on_invalid_by_in_asof_join() -> None:
     df1 = pl.DataFrame(
         {
             "a": ["a", "b", "a"],
             "b": [1, 2, 3],
             "c": ["a", "b", "a"],
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.17.2/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_exprs.py` & `polars_lts_cpu-0.17.2/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_fmt.py` & `polars_lts_cpu-0.17.2/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_functions.py` & `polars_lts_cpu-0.17.2/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_interchange.py` & `polars_lts_cpu-0.17.2/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_interop.py` & `polars_lts_cpu-0.17.2/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_lazy.py` & `polars_lts_cpu-0.17.2/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.17.2/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_predicates.py` & `polars_lts_cpu-0.17.2/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_projections.py` & `polars_lts_cpu-0.17.2/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_queries.py` & `polars_lts_cpu-0.17.2/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_schema.py` & `polars_lts_cpu-0.17.2/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_serde.py` & `polars_lts_cpu-0.17.2/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_series.py` & `polars_lts_cpu-0.17.2/tests/unit/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1315,14 +1315,22 @@
     )
 
 
 def test_pct_change() -> None:
     s = pl.Series("a", [1, 2, 4, 8, 16, 32, 64])
     expected = pl.Series("a", [None, None, float("inf"), 3.0, 3.0, 3.0, 3.0])
     assert_series_equal(s.pct_change(2), expected)
+    # negative
+    assert pl.Series(range(5)).pct_change(-1).to_list() == [
+        -1.0,
+        -0.5,
+        -0.3333333333333333,
+        -0.25,
+        None,
+    ]
 
 
 def test_skew() -> None:
     s = pl.Series("a", [1, 2, 3, 2, 2, 3, 0])
 
     assert s.skew(bias=True) == pytest.approx(-0.5953924651018018)
     assert s.skew(bias=False) == pytest.approx(-0.7717168360221258)
@@ -1940,14 +1948,17 @@
 
     expected = pl.Series("a", np.log(a.to_numpy()))
     assert_series_equal(a.log(), expected)
 
     expected = pl.Series("a", np.exp(b.to_numpy()))
     assert_series_equal(b.exp(), expected)
 
+    expected = pl.Series("a", np.log1p(a.to_numpy()))
+    assert_series_equal(a.log1p(), expected)
+
 
 def test_shuffle() -> None:
     a = pl.Series("a", [1, 2, 3])
     out = a.shuffle(2)
     expected = pl.Series("a", [2, 1, 3])
     assert_series_equal(out, expected)
```

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_sql.py` & `polars_lts_cpu-0.17.2/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_streaming.py` & `polars_lts_cpu-0.17.2/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/test_testing.py` & `polars_lts_cpu-0.17.2/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.17.2/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.1/Cargo.lock` & `polars_lts_cpu-0.17.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1708,15 +1708,15 @@
 checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.1"
+version = "0.17.2"
 dependencies = [
  "ahash",
  "bincode",
  "built",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.17.1/PKG-INFO` & `polars_lts_cpu-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.17.1
+Version: 0.17.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,50 +13,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: fsspec; extra == 'fsspec'
-Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Requires-Dist: connectorx; extra == 'connectorx'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
 Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
 Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
-Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
 Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
+Requires-Dist: fsspec; extra == 'fsspec'
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
 Requires-Dist: pandas; extra == 'pandas'
-Provides-Extra: matplotlib
-Provides-Extra: fsspec
-Provides-Extra: deltalake
-Provides-Extra: connectorx
-Provides-Extra: xlsx2csv
+Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: matplotlib; extra == 'matplotlib'
 Provides-Extra: sqlalchemy
 Provides-Extra: timezone
-Provides-Extra: numpy
 Provides-Extra: xlsxwriter
-Provides-Extra: all
+Provides-Extra: deltalake
 Provides-Extra: pyarrow
+Provides-Extra: fsspec
+Provides-Extra: xlsx2csv
 Provides-Extra: pandas
+Provides-Extra: connectorx
+Provides-Extra: all
+Provides-Extra: numpy
+Provides-Extra: matplotlib
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/pola-rs/polars
-Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 Project-URL: Homepage, https://www.pola.rs/
+Project-URL: Changelog, https://github.com/pola-rs/polars/releases
+Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
@@ -212,15 +212,15 @@
 | timezone   | Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are on Windows, otherwise no dependencies will be installed |
 
 Releases happen quite often (weekly / every few days) at the moment, so updating polars regularly to get the latest bugfixes / features might not be a bad idea.
 
 ### Rust
 
 You can take latest release from `crates.io`, or if you want to use the latest features / performance improvements
-point to the `master` branch of this repo.
+point to the `main` branch of this repo.
 
 ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "<optional git tag>" }
 ```
 
 Required Rust version `>=1.62`
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.1 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.2 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: fsspec; extra == 'fsspec' Requires-Dist: deltalake >= 0.8.0;
-extra == 'deltalake' Requires-Dist: connectorx; extra == 'connectorx' Requires-
-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-Dist: sqlalchemy; extra
-== 'sqlalchemy' Requires-Dist: pandas; extra == 'sqlalchemy' Requires-Dist:
-backports.zoneinfo; (python_version < '3.9') and extra == 'timezone' Requires-
-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone' Requires-
-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist: xlsxwriter; extra ==
-'xlsxwriter' Requires-Dist: polars
+python_version < '3.11' Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
+Requires-Dist: pandas; extra == 'sqlalchemy' Requires-Dist: backports.zoneinfo;
+(python_version < '3.9') and extra == 'timezone' Requires-Dist: tzdata;
+(platform_system == 'Windows') and extra == 'timezone' Requires-Dist:
+xlsxwriter; extra == 'xlsxwriter' Requires-Dist: deltalake >= 0.8.0; extra ==
+'deltalake' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
+fsspec; extra == 'fsspec' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra
+== 'pandas' Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist:
+polars
 [pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
-pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra == 'pandas'
-Provides-Extra: matplotlib Provides-Extra: fsspec Provides-Extra: deltalake
-Provides-Extra: connectorx Provides-Extra: xlsx2csv Provides-Extra: sqlalchemy
-Provides-Extra: timezone Provides-Extra: numpy Provides-Extra: xlsxwriter
-Provides-Extra: all Provides-Extra: pyarrow Provides-Extra: pandas License-
-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
-dataframe,arrow,out-of-core Author-email: Ritchie Vink
+extra == 'all' Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist:
+matplotlib; extra == 'matplotlib' Provides-Extra: sqlalchemy Provides-Extra:
+timezone Provides-Extra: xlsxwriter Provides-Extra: deltalake Provides-Extra:
+pyarrow Provides-Extra: fsspec Provides-Extra: xlsx2csv Provides-Extra: pandas
+Provides-Extra: connectorx Provides-Extra: all Provides-Extra: numpy Provides-
+Extra: matplotlib License-File: LICENSE Summary: Blazingly fast DataFrame
+library Keywords: dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/pola-rs/
-polars Project-URL: Changelog, https://github.com/pola-rs/polars/releases
-Project-URL: Homepage, https://www.pola.rs/ Project-URL: Documentation, https:/
-/pola-rs.github.io/polars/py-polars/html/reference/index.html
+charset=UTF-8; variant=GFM Project-URL: Homepage, https://www.pola.rs/ Project-
+URL: Changelog, https://github.com/pola-rs/polars/releases Project-URL:
+Repository, https://github.com/pola-rs/polars Project-URL: Documentation,
+https://pola-rs.github.io/polars/py-polars/html/reference/index.html
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
            Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
 Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
                             | User_Guide | Discord
@@ -98,15 +98,15 @@
 for reading from SQL databases | | xlsx2csv | Support for reading from Excel
 files | | deltalake | Support for reading from Delta Lake Tables | | timezone |
 Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are
 on Windows, otherwise no dependencies will be installed | Releases happen quite
 often (weekly / every few days) at the moment, so updating polars regularly to
 get the latest bugfixes / features might not be a bad idea. ### Rust You can
 take latest release from `crates.io`, or if you want to use the latest features
-/ performance improvements point to the `master` branch of this repo. ```toml
+/ performance improvements point to the `main` branch of this repo. ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "" } ``` Required
 Rust version `>=1.62` ## Contributing Want to contribute? Read our
 [contribution guideline](./CONTRIBUTING.md). ## Python: compile polars from
 source If you want a bleeding edge release or maximal performance you should
 compile **polars** from source. This can be done by going through the following
 steps in sequence: 1. Install the latest [Rust compiler](https://www.rust-
 lang.org/tools/install) 2. Install [maturin](https://maturin.rs/): `pip install
```

