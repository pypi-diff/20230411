# Comparing `tmp/meltanolabs_target_postgres-0.0.4.tar.gz` & `tmp/meltanolabs_target_postgres-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_postgres-0.0.4.tar", max compression
+gzip compressed data, was "meltanolabs_target_postgres-0.0.5.tar", max compression
```

## Comparing `meltanolabs_target_postgres-0.0.4.tar` & `meltanolabs_target_postgres-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0     1068 2023-01-16 21:54:30.531140 meltanolabs_target_postgres-0.0.4/LICENSE
--rw-r--r--   0        0        0     7294 2023-01-16 21:54:30.531140 meltanolabs_target_postgres-0.0.4/README.md
--rw-r--r--   0        0        0     1775 2023-01-16 21:54:53.691242 meltanolabs_target_postgres-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/.gitignore
--rw-r--r--   0        0        0       21 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/__init__.py
--rw-r--r--   0        0        0     6511 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/connector.py
--rw-r--r--   0        0        0     9055 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/sinks.py
--rw-r--r--   0        0        0     5595 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/target.py
--rw-r--r--   0        0        0       38 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/array_data.singer
--rw-r--r--   0        0        0      394 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/camelcase.singer
--rw-r--r--   0        0        0     1862 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/camelcase_complex_schema.singer
--rw-r--r--   0        0        0      722 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/duplicate_records.singer
--rw-r--r--   0        0        0     4275 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/encoded_strings.singer
--rw-r--r--   0        0        0      104 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/invalid_schema.singer
--rw-r--r--   0        0        0      362 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/large_int.singer
--rw-r--r--   0        0        0      607 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/missing_value.singer
--rw-r--r--   0        0        0     2129 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/multiple_state_messages.singer
--rw-r--r--   0        0        0      407 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/new_array_column.singer
--rw-r--r--   0        0        0      450 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/no_primary_keys.singer
--rw-r--r--   0        0        0      611 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/no_primary_keys_append.singer
--rw-r--r--   0        0        0      641 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/optional_attributes.singer
--rw-r--r--   0        0        0      378 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/record_before_schema.singer
--rw-r--r--   0        0        0      288 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/record_missing_key_property.singer
--rw-r--r--   0        0        0      318 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/record_missing_required_property.singer
--rw-r--r--   0        0        0    51890 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/reserved_keywords.singer
--rw-r--r--   0        0        0      892 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/schema_no_properties.singer
--rw-r--r--   0        0        0     2197 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/schema_updates.singer
--rw-r--r--   0        0        0      554 2023-01-16 21:54:30.535140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/special_chars_in_attributes.singer
--rw-r--r--   0        0        0  1859439 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/tap_aapl.singer
--rw-r--r--   0        0        0    97655 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/tap_countries.singer
--rw-r--r--   0        0        0     1992 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/user_location_data.singer
--rw-r--r--   0        0        0     2323 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/user_location_upsert_data.singer
--rw-r--r--   0        0        0       15 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/.gitignore
--rw-r--r--   0        0        0      453 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/README.md
--rw-r--r--   0        0        0       15 2023-01-16 21:54:30.539140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/__init__.py
--rw-r--r--   0        0        0   763998 2023-01-16 21:54:30.543140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/AAPL.json
--rw-r--r--   0        0        0      352 2023-01-16 21:54:30.543140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/README.md
--rw-r--r--   0        0        0      131 2023-01-16 21:54:30.543140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/__main__.py
--rw-r--r--   0        0        0      654 2023-01-16 21:54:30.543140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/aapl.py
--rw-r--r--   0        0        0  1492450 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/fundamentals.json
--rw-r--r--   0        0        0       28 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/__init__.py
--rw-r--r--   0        0        0     2218 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
--rw-r--r--   0        0        0      817 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
--rw-r--r--   0        0        0      146 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
--rw-r--r--   0        0        0     8021 2023-01-16 21:54:30.547140 meltanolabs_target_postgres-0.0.4/target_postgres/tests/test_standard_target.py
--rw-r--r--   0        0        0     8669 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.4/setup.py
--rw-r--r--   0        0        0     8635 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8242 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/README.md
+-rw-r--r--   0        0        0     1750 2023-04-11 21:02:58.785164 meltanolabs_target_postgres-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/.gitignore
+-rw-r--r--   0        0        0       21 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/__init__.py
+-rw-r--r--   0        0        0     6548 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/connector.py
+-rw-r--r--   0        0        0    11690 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/sinks.py
+-rw-r--r--   0        0        0     6460 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/target.py
+-rw-r--r--   0        0        0       38 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_hard.singer
+-rw-r--r--   0        0        0     1681 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_soft.singer
+-rw-r--r--   0        0        0      668 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/array_data.singer
+-rw-r--r--   0        0        0      394 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase.singer
+-rw-r--r--   0        0        0     1862 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase_complex_schema.singer
+-rw-r--r--   0        0        0      722 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/duplicate_records.singer
+-rw-r--r--   0        0        0     4275 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/encoded_strings.singer
+-rw-r--r--   0        0        0      104 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/invalid_schema.singer
+-rw-r--r--   0        0        0      362 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/large_int.singer
+-rw-r--r--   0        0        0      607 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/missing_value.singer
+-rw-r--r--   0        0        0     2129 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/multiple_state_messages.singer
+-rw-r--r--   0        0        0      407 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/new_array_column.singer
+-rw-r--r--   0        0        0      450 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys.singer
+-rw-r--r--   0        0        0      611 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys_append.singer
+-rw-r--r--   0        0        0      641 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/optional_attributes.singer
+-rw-r--r--   0        0        0      378 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_before_schema.singer
+-rw-r--r--   0        0        0      288 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_missing_key_property.singer
+-rw-r--r--   0        0        0      318 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_missing_required_property.singer
+-rw-r--r--   0        0        0    51890 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/reserved_keywords.singer
+-rw-r--r--   0        0        0      892 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_no_properties.singer
+-rw-r--r--   0        0        0     2197 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_updates.singer
+-rw-r--r--   0        0        0      554 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/special_chars_in_attributes.singer
+-rw-r--r--   0        0        0  1859439 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_aapl.singer
+-rw-r--r--   0        0        0    97655 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_countries.singer
+-rw-r--r--   0        0        0     1851 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer
+-rw-r--r--   0        0        0      357 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/test_activate_version_deletes_data_properly_2.singer
+-rw-r--r--   0        0        0     1992 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_data.singer
+-rw-r--r--   0        0        0     2323 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_upsert_data.singer
+-rw-r--r--   0        0        0       15 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/.gitignore
+-rw-r--r--   0        0        0      453 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/README.md
+-rw-r--r--   0        0        0       15 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/__init__.py
+-rw-r--r--   0        0        0   763998 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/AAPL.json
+-rw-r--r--   0        0        0      352 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/README.md
+-rw-r--r--   0        0        0      131 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/__main__.py
+-rw-r--r--   0        0        0      654 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/aapl.py
+-rw-r--r--   0        0        0  1492450 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/fundamentals.json
+-rw-r--r--   0        0        0       28 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
+-rw-r--r--   0        0        0      817 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
+-rw-r--r--   0        0        0      146 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
+-rw-r--r--   0        0        0    14720 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/test_standard_target.py
+-rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.5/PKG-INFO
```

### Comparing `meltanolabs_target_postgres-0.0.4/LICENSE` & `meltanolabs_target_postgres-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/README.md` & `meltanolabs_target_postgres-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 ## Capabilities
 
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
-
-| Setting              | Required |       Default       | Description                                                                                                                                                                                                                                                               |
-| :------------------- | :------: | :-----------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| host                 |  False   |        None         | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                       |
-| port                 |  False   |        5432         | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                    |
-| user                 |  False   |        None         | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                       |
-| password             |  False   |        None         | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                        |
-| database             |  False   |        None         | Database name. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                                        |
-| sqlalchemy_url       |  False   |        None         | SQLAlchemy connection string. This will override using host, user, password, port, dialect. Note that you must esacpe password special characters properly see https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |
-| dialect+driver       |  False   | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored.                                                                                                              |
-| stream_maps          |  False   |        None         | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html).                                                                                                                               |
-| stream_map_config    |  False   |        None         | User-defined config values to be used within map expressions.                                                                                                                                                                                                             |
-| flattening_enabled   |  False   |        None         | 'True' to enable schema flattening and automatically expand nested properties.                                                                                                                                                                                            |
-| flattening_max_depth |  False   |        None         | The max depth to flatten schemas.                                                                                                                                                                                                                                         |
+| Setting               | Required |       Default       | Description                                                                                                                                                                                                                                                            |
+| :-------------------- | :------: | :-----------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| host                  |  False   |        None         | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
+| port                  |  False   |        5432         | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                 |
+| user                  |  False   |        None         | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
+| password              |  False   |        None         | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                     |
+| database              |  False   |        None         | Database name. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                                     |
+| sqlalchemy_url        |  False   |        None         | SQLAlchemy connection string. This will override using host, user, password, port,dialect. Note that you must escape password special characters properly. See https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |
+| dialect+driver        |  False   | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored.                                                                                                           |
+| default_target_schema |  False   |        None         | Postgres schema to send data to, example: tap-clickup                                                                                                                                                                                                                  |
+| hard_delete           |  False   |          0          | When activate version is sent from a tap this specefies if we should delete the records that don't match, or mark them with a date in the `_sdc_deleted_at` column.                                                                                                    |
+| add_record_metadata   |  False   |          1          | Note that this must be enabled for activate_version to work!This adds _sdc_extracted_at, _sdc_batched_at, and more to every table. See https://sdk.meltano.com/en/latest/implementation/record_metadata.html for more information.                                     |
+| stream_maps           |  False   |        None         | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html).                                                                                                                            |
+| stream_map_config     |  False   |        None         | User-defined config values to be used within map expressions.                                                                                                                                                                                                          |
+| flattening_enabled    |  False   |        None         | 'True' to enable schema flattening and automatically expand nested properties.                                                                                                                                                                                         |
+| flattening_max_depth  |  False   |        None         | The max depth to flatten schemas.                                                                                                                                                                                                                                      |
 
 A full list of supported settings and capabilities is available by running: `target-postgres --about`
 
 ## Installation
 
 - [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)
```

### Comparing `meltanolabs_target_postgres-0.0.4/pyproject.toml` & `meltanolabs_target_postgres-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-postgres"
-version = "0.0.4"
+version = "0.0.5"
 description = "`target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets."
 authors = ["Meltano Team and Contributors"]
 maintainers = ["Meltano Team and Contributors"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://meltano.com"
 repository = "https://github.com/meltanolabs/target-postgres"
@@ -29,26 +29,25 @@
 packages = [
     { include = "target_postgres" }
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = "^0.17.0"
+singer-sdk = ">=0.17,<0.20"
 psycopg2-binary = "2.9.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 tox = "^3.24.4"
 flake8 = "^5.0.4"
-flake8-docstrings = "^1.6.0"
-black = "22.12.0"
-mypy = "^0.991"
-types-requests = "^2.26.1"
-isort = "^5.10.1"
+flake8-docstrings = "^1.7.0"
+black = "23.1.0"
+mypy = "^1.0"
+isort = "^5.11.5"
 remote-pdb="2.1.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "target_postgres"
```

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/.gitignore` & `meltanolabs_target_postgres-0.0.5/target_postgres/.gitignore`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/connector.py` & `meltanolabs_target_postgres-0.0.5/target_postgres/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
         else:
             sqlalchemy_url = URL.create(
                 drivername=config["dialect+driver"],
                 username=config["user"],
                 password=config["password"],
                 host=config["host"],
+                port=config["port"],
                 database=config["database"],
             )
             return cast(str, sqlalchemy_url)
 
     def truncate_table(self, name):
         """Clear table data."""
         self.connection.execute(f"TRUNCATE TABLE {name}")
```

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/target.py` & `meltanolabs_target_postgres-0.0.5/target_postgres/target.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             ),
         ),
         th.Property(
             "user",
             th.StringType,
             description=(
                 "User name used to authenticate. "
-                + "Note if sqlalchemy_url is set this will be ignored.",
+                + "Note if sqlalchemy_url is set this will be ignored."
             ),
         ),
         th.Property(
             "password",
             th.StringType,
             description=(
                 "Password used to authenticate. "
@@ -91,17 +91,17 @@
             ),
         ),
         th.Property(
             "sqlalchemy_url",
             th.StringType,
             description=(
                 "SQLAlchemy connection string. "
-                + "This will override using host, user, password, port,"
-                + "dialect. Note that you must esacpe password special"
-                + "characters properly see"
+                + "This will override using host, user, password, port, "
+                + "dialect. Note that you must esacpe password special "
+                + "characters properly see "
                 + "https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords"  # noqa: E501
             ),
         ),
         th.Property(
             "dialect+driver",
             th.StringType,
             default="postgresql+psycopg2",
@@ -113,14 +113,35 @@
             ),
         ),
         th.Property(
             "default_target_schema",
             th.StringType,
             description="Postgres schema to send data to, example: tap-clickup",
         ),
+        th.Property(
+            "hard_delete",
+            th.BooleanType,
+            default=False,
+            description=(
+                "When activate version is sent from a tap this specefies "
+                + "if we should delete the records that don't match, or mark "
+                + "them with a date in the `_sdc_deleted_at` column."
+            ),
+        ),
+        th.Property(
+            "add_record_metadata",
+            th.BooleanType,
+            default=True,
+            description=(
+                "Note that this must be enabled for activate_version to work!"
+                + "This adds _sdc_extracted_at, _sdc_batched_at, and more to every "
+                + "table. See https://sdk.meltano.com/en/latest/implementation/record_metadata.html "  # noqa: E501
+                + "for more information."
+            ),
+        ),
     ).to_dict()
     default_sink_class = PostgresSink
 
     @property
     def max_parallelism(self) -> int:
         """Get max parallel sinks.
```

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/array_data.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/array_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/camelcase_complex_schema.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase_complex_schema.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/duplicate_records.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/duplicate_records.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/encoded_strings.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/encoded_strings.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/missing_value.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/missing_value.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/multiple_state_messages.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/multiple_state_messages.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/no_primary_keys_append.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys_append.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/optional_attributes.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/optional_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/reserved_keywords.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/reserved_keywords.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/schema_no_properties.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_no_properties.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/schema_updates.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_updates.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/special_chars_in_attributes.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/special_chars_in_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/tap_aapl.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_aapl.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/tap_countries.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_countries.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/user_location_data.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/data_files/user_location_upsert_data.singer` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_upsert_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/AAPL.json` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/AAPL.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/aapl.py` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/aapl.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/aapl/fundamentals.json` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/fundamentals.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/countries_streams.py` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_streams.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/target_postgres/tests/samples/sample_tap_countries/countries_tap.py` & `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_tap.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.4/setup.py` & `meltanolabs_target_postgres-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,156 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: meltanolabs-target-postgres
+Version: 0.0.5
+Summary: `target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets.
+Home-page: https://meltano.com
+License: MIT
+Keywords: Postgres,Singer,ELT,Meltano,Meltano SDK
+Author: Meltano Team and Contributors
+Maintainer: Meltano Team and Contributors
+Requires-Python: >=3.7.1,<3.12
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: psycopg2-binary (==2.9.5)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: singer-sdk (>=0.17,<0.20)
+Project-URL: Repository, https://github.com/meltanolabs/target-postgres
+Description-Content-Type: text/markdown
+
+# `target-postgres`
+
+Target for Postgres.
+
+Built with the [Meltano SDK](https://sdk.meltano.com) for Singer Taps and Targets. This target is in **development**, it probably doesn't work yet, stick with https://hub.meltano.com/loaders/target-postgres . Generally the goal here is to create a generalized target enough so that the SDK can automate >80% of testing for new targets, and potentially so taps can test very easily with a real local target.
+
+# Limitations
+1. Target is not working with Empty key properties. See https://github.com/MeltanoLabs/target-postgres/issues/54
+
+## Capabilities
+
+* `about`
+* `stream-maps`
+* `schema-flattening`
+
+## Settings
+| Setting               | Required |       Default       | Description                                                                                                                                                                                                                                                            |
+| :-------------------- | :------: | :-----------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| host                  |  False   |        None         | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
+| port                  |  False   |        5432         | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                 |
+| user                  |  False   |        None         | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
+| password              |  False   |        None         | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                     |
+| database              |  False   |        None         | Database name. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                                     |
+| sqlalchemy_url        |  False   |        None         | SQLAlchemy connection string. This will override using host, user, password, port,dialect. Note that you must escape password special characters properly. See https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |
+| dialect+driver        |  False   | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored.                                                                                                           |
+| default_target_schema |  False   |        None         | Postgres schema to send data to, example: tap-clickup                                                                                                                                                                                                                  |
+| hard_delete           |  False   |          0          | When activate version is sent from a tap this specefies if we should delete the records that don't match, or mark them with a date in the `_sdc_deleted_at` column.                                                                                                    |
+| add_record_metadata   |  False   |          1          | Note that this must be enabled for activate_version to work!This adds _sdc_extracted_at, _sdc_batched_at, and more to every table. See https://sdk.meltano.com/en/latest/implementation/record_metadata.html for more information.                                     |
+| stream_maps           |  False   |        None         | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html).                                                                                                                            |
+| stream_map_config     |  False   |        None         | User-defined config values to be used within map expressions.                                                                                                                                                                                                          |
+| flattening_enabled    |  False   |        None         | 'True' to enable schema flattening and automatically expand nested properties.                                                                                                                                                                                         |
+| flattening_max_depth  |  False   |        None         | The max depth to flatten schemas.                                                                                                                                                                                                                                      |
+
+A full list of supported settings and capabilities is available by running: `target-postgres --about`
+
+## Installation
+
+- [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)
+
+```bash
+pipx install -e .
+```
+
+## Configuration
+
+### Configure using environment variables
+
+This Singer target will automatically import any environment variables within the working directory's
+`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
+environment variable is set either in the terminal context or in the `.env` file.
+
+### Source Authentication and Authorization
+
+The database account provided must have access to:
+1. Create schemas
+1. Create tables (DDL)
+1. Push Data to tables (DML)
+
+## Usage
+
+You can easily run `target-postgres` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Target Directly
+
+```bash
+target-postgres --version
+target-postgres --help
+# Test using the "Carbon Intensity" sample:
+pipx install git+https://gitlab.com/meltano/tap-carbon-intensity
+tap-carbon-intensity | target-postgres --config /path/to/target-postgres-config.json
+```
+
+## Developer Resources
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+pipx install pre-commit
+pre-commit install
+```
+
+### Create and Run Tests
+
+Create tests within the `target_postgres/tests` subfolder and
+  then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `target-postgres` CLI interface directly using `poetry run`:
+
+```bash
+poetry run target-postgres --help
+```
+
+### Testing with [Meltano](https://meltano.com/)
+
+_**Note:** This target will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Your project comes with a custom `meltano.yml` project file already created.
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke target-postgres --version
+```
 
-packages = \
-['target_postgres',
- 'target_postgres.tests',
- 'target_postgres.tests.samples',
- 'target_postgres.tests.samples.aapl',
- 'target_postgres.tests.samples.sample_tap_countries']
-
-package_data = \
-{'': ['*'],
- 'target_postgres.tests': ['data_files/*'],
- 'target_postgres.tests.samples.sample_tap_countries': ['schemas/*']}
-
-install_requires = \
-['psycopg2-binary==2.9.5',
- 'requests>=2.25.1,<3.0.0',
- 'singer-sdk>=0.17.0,<0.18.0']
-
-entry_points = \
-{'console_scripts': ['target-postgres = '
-                     'target_postgres.target:TargetPostgres.cli']}
-
-setup_kwargs = {
-    'name': 'meltanolabs-target-postgres',
-    'version': '0.0.4',
-    'description': '`target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets.',
-    'long_description': '# `target-postgres`\n\nTarget for Postgres.\n\nBuilt with the [Meltano SDK](https://sdk.meltano.com) for Singer Taps and Targets. This target is in **development**, it probably doesn\'t work yet, stick with https://hub.meltano.com/loaders/target-postgres . Generally the goal here is to create a generalized target enough so that the SDK can automate >80% of testing for new targets, and potentially so taps can test very easily with a real local target.\n\n# Limitations\n1. Target is not working with Empty key properties. See https://github.com/MeltanoLabs/target-postgres/issues/54\n\n## Capabilities\n\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting              | Required |       Default       | Description                                                                                                                                                                                                                                                               |\n| :------------------- | :------: | :-----------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |\n| host                 |  False   |        None         | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                       |\n| port                 |  False   |        5432         | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                    |\n| user                 |  False   |        None         | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                       |\n| password             |  False   |        None         | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                        |\n| database             |  False   |        None         | Database name. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                                        |\n| sqlalchemy_url       |  False   |        None         | SQLAlchemy connection string. This will override using host, user, password, port, dialect. Note that you must esacpe password special characters properly see https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |\n| dialect+driver       |  False   | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored.                                                                                                              |\n| stream_maps          |  False   |        None         | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html).                                                                                                                               |\n| stream_map_config    |  False   |        None         | User-defined config values to be used within map expressions.                                                                                                                                                                                                             |\n| flattening_enabled   |  False   |        None         | \'True\' to enable schema flattening and automatically expand nested properties.                                                                                                                                                                                            |\n| flattening_max_depth |  False   |        None         | The max depth to flatten schemas.                                                                                                                                                                                                                                         |\n\nA full list of supported settings and capabilities is available by running: `target-postgres --about`\n\n## Installation\n\n- [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)\n\n```bash\npipx install -e .\n```\n\n## Configuration\n\n### Configure using environment variables\n\nThis Singer target will automatically import any environment variables within the working directory\'s\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### Source Authentication and Authorization\n\nThe database account provided must have access to:\n1. Create schemas\n1. Create tables (DDL)\n1. Push Data to tables (DML)\n\n## Usage\n\nYou can easily run `target-postgres` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Target Directly\n\n```bash\ntarget-postgres --version\ntarget-postgres --help\n# Test using the "Carbon Intensity" sample:\npipx install git+https://gitlab.com/meltano/tap-carbon-intensity\ntap-carbon-intensity | target-postgres --config /path/to/target-postgres-config.json\n```\n\n## Developer Resources\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\npipx install pre-commit\npre-commit install\n```\n\n### Create and Run Tests\n\nCreate tests within the `target_postgres/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `target-postgres` CLI interface directly using `poetry run`:\n\n```bash\npoetry run target-postgres --help\n```\n\n### Testing with [Meltano](https://meltano.com/)\n\n_**Note:** This target will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nYour project comes with a custom `meltano.yml` project file already created.\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke target-postgres --version\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to\ndevelop your own Singer taps and targets.\n',
-    'author': 'Meltano Team and Contributors',
-    'author_email': 'None',
-    'maintainer': 'Meltano Team and Contributors',
-    'maintainer_email': 'None',
-    'url': 'https://meltano.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.12',
-}
+### SDK Dev Guide
 
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to
+develop your own Singer taps and targets.
 
-setup(**setup_kwargs)
```

