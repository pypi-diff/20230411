# Comparing `tmp/google-dataproc-templates-0.1.0b0.tar.gz` & `tmp/google-dataproc-templates-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-dataproc-templates-0.1.0b0.tar", last modified: Fri Mar 17 13:18:44 2023, max compression
+gzip compressed data, was "google-dataproc-templates-0.2.0b0.tar", last modified: Tue Apr 11 11:21:58 2023, max compression
```

## Comparing `google-dataproc-templates-0.1.0b0.tar` & `google-dataproc-templates-0.2.0b0.tar`

### file list

```diff
@@ -1,111 +1,125 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.239920 google-dataproc-templates-0.1.0b0/
--rw-rw-r--   0 root         (0)     1003      677 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     9494 2023-03-17 13:18:44.239920 google-dataproc-templates-0.1.0b0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     9183 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.219927 google-dataproc-templates-0.1.0b0/dataproc_templates/
--rw-rw-r--   0 root         (0)     1003      652 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/__init__.py
--rw-rw-r--   0 root         (0)     1003     2087 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/base_template.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.219927 google-dataproc-templates-0.1.0b0/dataproc_templates/bigquery/
--rw-rw-r--   0 root         (0)     1003      623 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     4081 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.219927 google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/
--rw-rw-r--   0 root         (0)     1003      682 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/__init__.py
--rw-rw-r--   0 root         (0)     1003     6346 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003     6943 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.223926 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/
--rw-rw-r--   0 root         (0)     1003      676 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/__init__.py
--rw-rw-r--   0 root         (0)     1003     5256 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003     3681 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
--rw-rw-r--   0 root         (0)     1003     7568 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_gcs.py
--rw-rw-r--   0 root         (0)     1003     5843 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
--rw-rw-r--   0 root         (0)     1003     5496 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_mongo.py
--rw-rw-r--   0 root         (0)     1003     5160 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/text_to_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.223926 google-dataproc-templates-0.1.0b0/dataproc_templates/hbase/
--rw-rw-r--   0 root         (0)     1003      617 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hbase/__init__.py
--rw-rw-r--   0 root         (0)     1003     4232 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hbase/hbase_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.223926 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/
--rw-rw-r--   0 root         (0)     1003      668 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/__init__.py
--rw-rw-r--   0 root         (0)     1003     5394 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/hive_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003     5769 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/hive_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.223926 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/util/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/util/__init__.py
--rw-rw-r--   0 root         (0)     1003     3240 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.223926 google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/
--rw-rw-r--   0 root         (0)     1003      571 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/__init__.py
--rw-rw-r--   0 root         (0)     1003     8001 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003    10998 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
--rw-rw-r--   0 root         (0)     1003    10387 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/
--rw-rw-r--   0 root         (0)     1003      665 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/__init__.py
--rw-rw-r--   0 root         (0)     1003     4446 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/kafka_to_bq.py
--rw-rw-r--   0 root         (0)     1003     4065 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/kafka_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/mongo/
--rw-rw-r--   0 root         (0)     1003      616 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/mongo/__init__.py
--rw-rw-r--   0 root         (0)     1003     4837 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/mongo/mongo_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/redshift/
--rw-rw-r--   0 root         (0)     1003      571 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/redshift/__init__.py
--rw-rw-r--   0 root         (0)     1003     6883 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/redshift/redshift_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/s3/
--rw-rw-r--   0 root         (0)     1003      620 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/s3/__init__.py
--rw-rw-r--   0 root         (0)     1003     6185 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/s3/s3_to_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/snowflake/
--rw-rw-r--   0 root         (0)     1003      624 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/snowflake/__init__.py
--rw-rw-r--   0 root         (0)     1003    11122 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
--rw-rw-r--   0 root         (0)     1003     2463 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/template_name.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.227924 google-dataproc-templates-0.1.0b0/dataproc_templates/util/
--rw-rw-r--   0 root         (0)     1003      683 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/util/__init__.py
--rw-rw-r--   0 root         (0)     1003     2617 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/util/argument_parsing.py
--rw-rw-r--   0 root         (0)     1003    13171 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/util/template_constants.py
--rw-rw-r--   0 root         (0)     1003     1642 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/dataproc_templates/util/tracking.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.231923 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/
--rw-r--r--   0 root         (0)     1003     9494 2023-03-17 13:18:44.000000 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2896 2023-03-17 13:18:44.000000 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-17 13:18:44.000000 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       44 2023-03-17 13:18:44.000000 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       24 2023-03-17 13:18:44.000000 google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-17 13:18:44.239920 google-dataproc-templates-0.1.0b0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3327 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.215929 google-dataproc-templates-0.1.0b0/test/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.231923 google-dataproc-templates-0.1.0b0/test/bigquery/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     7319 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/bigquery/test_bigquery_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.231923 google-dataproc-templates-0.1.0b0/test/cassandra/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/cassandra/__init__.py
--rw-rw-r--   0 root         (0)     1003     1977 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/cassandra/test_cassandra_to_bq.py
--rw-rw-r--   0 root         (0)     1003     1981 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/cassandra/test_cassandra_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.231923 google-dataproc-templates-0.1.0b0/test/gcs/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/__init__.py
--rw-rw-r--   0 root         (0)     1003     8440 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003     2543 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_bigtable.py
--rw-rw-r--   0 root         (0)     1003     9106 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_gcs.py
--rw-rw-r--   0 root         (0)     1003     7714 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_jdbc.py
--rw-rw-r--   0 root         (0)     1003    10132 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_mongo.py
--rw-rw-r--   0 root         (0)     1003    10712 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/gcs/test_text_to_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/hbase/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hbase/__init__.py
--rw-rw-r--   0 root         (0)     1003     2959 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hbase/test_hbase_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/hive/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hive/__init__.py
--rw-rw-r--   0 root         (0)     1003     5503 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hive/test_hive_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003     6031 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hive/test_hive_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/hive/util/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hive/util/__init__.py
--rw-rw-r--   0 root         (0)     1003     2439 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/hive/util/test_hive_ddl_extractor.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/jdbc/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/jdbc/__init__.py
--rw-rw-r--   0 root         (0)     1003     9315 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_bigquery.py
--rw-rw-r--   0 root         (0)     1003    13319 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_gcs.py
--rw-rw-r--   0 root         (0)     1003    12109 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_jdbc.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/mongo/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/mongo/__init__.py
--rw-rw-r--   0 root         (0)     1003     8870 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/mongo/test_mongo_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/redshift/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/redshift/__init__.py
--rw-rw-r--   0 root         (0)     1003    14423 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/redshift/test_redshift_to_gcs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.235921 google-dataproc-templates-0.1.0b0/test/s3/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/s3/__init__.py
--rw-rw-r--   0 root         (0)     1003    12993 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/s3/test_s3_to_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 13:18:44.239920 google-dataproc-templates-0.1.0b0/test/util/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/util/__init__.py
--rw-rw-r--   0 root         (0)     1003     1944 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/test/util/test_argument_parsing.py
--rw-rw-r--   0 root         (0)     1003       27 2023-03-17 13:14:54.000000 google-dataproc-templates-0.1.0b0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/base_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/template_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/dataproc_templates/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_reader_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_writer_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/template_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/azure/test_azure_blob_storage_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/bigquery/test_bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hbase/test_hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/util/test_hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/mongo/test_mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/pubsublite/test_pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/redshift/test_redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/s3/test_s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/util/test_argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/version.py
```

### Comparing `google-dataproc-templates-0.1.0b0/MANIFEST.in` & `google-dataproc-templates-0.2.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/PKG-INFO` & `google-dataproc-templates-0.2.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: google-dataproc-templates
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: Google Dataproc templates written in Python
 Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
 
 # Dataproc Templates (Python - PySpark)
+* [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
 * [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
@@ -24,14 +25,15 @@
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.1.0b0/README.md` & `google-dataproc-templates-0.2.0b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
 
 # Dataproc Templates (Python - PySpark)
+* [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
 * [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
@@ -14,14 +15,15 @@
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/base_template.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/base_template.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/bigquery/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from logging import Logger
 import argparse
 import pprint
 
 from pyspark.sql import SparkSession, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['BigQueryToGCSTemplate']
 
 
 class BigQueryToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing exports from BigQuery to GCS
+    Dataproc template implementing exports from BigQuery to Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
@@ -52,15 +55,15 @@
                 constants.FORMAT_JSON
             ]
         )
         parser.add_argument(
             f'--{constants.BQ_GCS_OUTPUT_LOCATION}',
             dest=constants.BQ_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.BQ_GCS_OUTPUT_MODE}',
             dest=constants.BQ_GCS_OUTPUT_MODE,
             required=False,
             default=constants.OUTPUT_MODE_APPEND,
             help=(
@@ -71,49 +74,39 @@
             choices=[
                 constants.OUTPUT_MODE_OVERWRITE,
                 constants.OUTPUT_MODE_APPEND,
                 constants.OUTPUT_MODE_IGNORE,
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("bigquery.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
         input_table: str = args[constants.BQ_GCS_INPUT_TABLE]
-        output_format: str = args[constants.BQ_GCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.BQ_GCS_OUTPUT_MODE]
+
         output_location: str = args[constants.BQ_GCS_OUTPUT_LOCATION]
+        output_format: str = args[constants.BQ_GCS_OUTPUT_FORMAT]
 
         logger.info(
-            "Starting Bigquery to GCS spark job with parameters:\n"
+            "Starting Bigquery to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
         input_data = spark.read \
             .format(constants.FORMAT_BIGQUERY) \
             .option(constants.TABLE, input_table) \
             .load()
 
         # Write
         writer: DataFrameWriter = input_data.write.mode(output_mode)
-
-        if output_format == constants.FORMAT_PRQT:
-            writer.parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer.json(output_location)
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "bigquery.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
         parser.add_argument(
             f'--{constants.CASSANDRA_TO_BQ_TEMP_LOCATION}',
             dest=constants.CASSANDRA_TO_BQ_TEMP_LOCATION,
             required=True,
-            help='GCS location for staging, Format: <bucket-name>'
+            help='Cloud Storage location for staging, Format: <bucket-name>'
         )
         parser.add_argument(
             f'--{constants.CASSANDRA_TO_BQ_QUERY}',
             dest=constants.CASSANDRA_TO_BQ_QUERY,
             required=False,
             help='Optional query for selective exports'
         )
@@ -95,25 +95,25 @@
             required=False,
             help='Keyspace Name of Cassandra Table'
         )
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
-        if (not getattr(known_args, constants.CASSANDRA_TO_BQ_QUERY) 
-            and (not getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_KEYSPACE) 
+        if (not getattr(known_args, constants.CASSANDRA_TO_BQ_QUERY)
+            and (not getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_KEYSPACE)
             or not getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_TABLE))):
-            
+
             sys.exit("ArgumentParser Error: Either of cassandratobq.input.keyspace and cassandratobq.input.table "
                         + "OR cassandratobq.input.query needs to be provided as argument to read data from Cassandra")
 
         elif (getattr(known_args, constants.CASSANDRA_TO_BQ_QUERY)
-            and (getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_KEYSPACE) 
+            and (getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_KEYSPACE)
             or getattr(known_args, constants.CASSANDRA_TO_BQ_INPUT_TABLE))):
-            
+
             sys.exit("ArgumentParser Error: Both cassandratobq.input.keyspace and cassandratobq.input.table "
                         + "AND cassandratobq.input.query cannot be provided as arguments at the same time.")
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,47 +7,49 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
- 
+
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 import sys
- 
+
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
- 
+
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
 from pyspark import SparkConf, SparkContext
 from pyspark.sql import SparkSession
 
- 
+
 __all__ = ['CassandraToGCSTemplate']
- 
- 
+
+
 class CassandraToGCSTemplate(BaseTemplate):
    """
    Dataproc template implementing exports from CASSANDRA to GCS
    """
 
    @staticmethod
    def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
        parser: argparse.ArgumentParser = argparse.ArgumentParser()
- 
+
        parser.add_argument(
            f'--{constants.CASSANDRA_TO_GCS_INPUT_HOST}',
            dest=constants.CASSANDRA_TO_GCS_INPUT_HOST,
            required=True,
-           help='CASSANDRA GCS Input Host IP'
+           help='CASSANDRA Cloud Storage Input Host IP'
        )
        parser.add_argument(
            f'--{constants.CASSANDRA_TO_GCS_OUTPUT_FORMAT}',
            dest=constants.CASSANDRA_TO_GCS_OUTPUT_FORMAT,
            required=True,
            help='Output file format (one of: avro,parquet,csv,json)',
            choices=[
@@ -57,15 +59,15 @@
                constants.FORMAT_JSON
            ]
        )
        parser.add_argument(
            f'--{constants.CASSANDRA_TO_GCS_OUTPUT_PATH}',
            dest=constants.CASSANDRA_TO_GCS_OUTPUT_PATH,
            required=True,
-           help='GCS location for output files'
+           help='Cloud Storage location for output files'
        )
        parser.add_argument(
            f'--{constants.CASSANDRA_TO_GCS_OUTPUT_SAVEMODE}',
            dest=constants.CASSANDRA_TO_GCS_OUTPUT_SAVEMODE,
            required=False,
            default=constants.OUTPUT_MODE_APPEND,
            help=(
@@ -82,97 +84,86 @@
        )
        parser.add_argument(
             f'--{constants.CASSANDRA_TO_GCS_CATALOG}',
             dest=constants.CASSANDRA_TO_GCS_CATALOG,
             required=False,
             default="casscon",
             help='To provide a name for connection between Cassandra and GCS'
-        )
+       )
        parser.add_argument(
             f'--{constants.CASSANDRA_TO_GCS_QUERY}',
             dest=constants.CASSANDRA_TO_GCS_QUERY,
             required=False,
             help='Optional query for selective exports'
-        )
+       )
 
        parser.add_argument(
             f'--{constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE}',
             dest=constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE,
             required=(constants.CASSANDRA_TO_GCS_QUERY is None),
-            help='CASSANDRA GCS Input Keyspace'
-        )
+            help='CASSANDRA Cloud Storage Input Keyspace'
+       )
        parser.add_argument(
            f'--{constants.CASSANDRA_TO_GCS_INPUT_TABLE}',
            dest=constants.CASSANDRA_TO_GCS_INPUT_TABLE,
            required=(constants.CASSANDRA_TO_GCS_QUERY is None),
-           help='CASSANDRA GCS Input Table'
-        )
- 
+           help='CASSANDRA Cloud Storage Input Table'
+       )
+       add_spark_options(parser, constants.get_csv_output_spark_options("cassandra.gcs.output."))
+
        known_args: argparse.Namespace
        known_args, _ = parser.parse_known_args(args)
-       if (not getattr(known_args, constants.CASSANDRA_TO_GCS_QUERY) 
-            and (not getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE) 
+       if (not getattr(known_args, constants.CASSANDRA_TO_GCS_QUERY)
+            and (not getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE)
             or not getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_TABLE))):
 
             sys.exit("ArgumentParser Error: Either of cassandratogcs.input.keyspace and cassandratogcs.input.table "
                         + "OR cassandratogcs.input.query needs to be provided as argument to read data from Cassandra")
 
        elif (getattr(known_args, constants.CASSANDRA_TO_GCS_QUERY)
-            and (getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE) 
+            and (getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE)
             or getattr(known_args, constants.CASSANDRA_TO_GCS_INPUT_TABLE))):
 
             sys.exit("ArgumentParser Error: Both cassandratogcs.input.keyspace and cassandratogcs.input.table "
                         + "AND cassandratogcs.input.query cannot be provided as arguments at the same time.")
- 
- 
+
+
        return vars(known_args)
- 
+
    def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
- 
+
        logger: Logger = self.get_logger(spark=spark)
- 
+
        # Arguments
        input_host: str = args[constants.CASSANDRA_TO_GCS_INPUT_HOST]
        input_keyspace: str = args[constants.CASSANDRA_TO_GCS_INPUT_KEYSPACE]
        input_table: str = args[constants.CASSANDRA_TO_GCS_INPUT_TABLE]
        output_format: str = args[constants.CASSANDRA_TO_GCS_OUTPUT_FORMAT]
-       output_mode: str = args[constants.CASSANDRA_TO_GCS_OUTPUT_SAVEMODE]
        output_location: str = args[constants.CASSANDRA_TO_GCS_OUTPUT_PATH]
+       output_mode: str = args[constants.CASSANDRA_TO_GCS_OUTPUT_SAVEMODE]
        catalog: str = args[constants.CASSANDRA_TO_GCS_CATALOG]
        query: str = args[constants.CASSANDRA_TO_GCS_QUERY]
- 
+
        logger.info(
-           "Starting CASSANDRA to GCS spark job with parameters:\n"
+           "Starting CASSANDRA to Cloud Storage spark job with parameters:\n"
            f"{pprint.pformat(args)}"
        )
-       
+
        # Set configuration to connect to Cassandra by overwriting the spark session
        spark = (
         SparkSession
         .builder
         .appName("CassandraToGCS")
         .config(constants.SQL_EXTENSION, constants.CASSANDRA_EXTENSION)
         .config(f"spark.sql.catalog.{catalog}", constants.CASSANDRA_CATALOG)
         .config(f"spark.sql.catalog.{catalog}.spark.cassandra.connection.host",input_host)
         .getOrCreate())
- 
+
        # Read
        if(not query):
            input_data = spark.read.table(f"{catalog}.{input_keyspace}.{input_table}")
        else:
-           input_data = spark.sql(query)  
- 
+           input_data = spark.sql(query)
+
        # Write
        writer: DataFrameWriter = input_data.write.mode(output_mode)
- 
-       if output_format == constants.FORMAT_PRQT:
-           writer.parquet(output_location)
-       elif output_format == constants.FORMAT_AVRO:
-           writer \
-               .format(constants.FORMAT_AVRO) \
-               .save(output_location)
-       elif output_format == constants.FORMAT_CSV:
-           writer \
-               .option(constants.HEADER, True) \
-               .csv(output_location)
-       elif output_format == constants.FORMAT_JSON:
-           writer.json(output_location)
+       persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "cassandratogcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigquery.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 # limitations under the License.
 
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import SparkSession
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['GCSToBigQueryTemplate']
 
 
 class GCSToBigQueryTemplate(BaseTemplate):
     """
     Dataproc template implementing loads from GCS into BigQuery
     """
@@ -34,15 +37,15 @@
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.GCS_BQ_INPUT_LOCATION}',
             dest=constants.GCS_BQ_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input files'
+            help='Cloud Storage location of the input files'
         )
         parser.add_argument(
             f'--{constants.GCS_BQ_OUTPUT_DATASET}',
             dest=constants.GCS_BQ_OUTPUT_DATASET,
             required=True,
             help='BigQuery dataset for the output table'
         )
@@ -52,23 +55,24 @@
             required=True,
             help='BigQuery output table name'
         )
         parser.add_argument(
             f'--{constants.GCS_BQ_INPUT_FORMAT}',
             dest=constants.GCS_BQ_INPUT_FORMAT,
             required=True,
-            help='Input file format (one of: avro,parquet,csv,json)',
+            help='Input file format (one of: avro,parquet,csv,json,delta)',
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
                 constants.FORMAT_JSON,
                 constants.FORMAT_DELTA
             ]
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("gcs.bigquery.input."))
         parser.add_argument(
             f'--{constants.GCS_BQ_LD_TEMP_BUCKET_NAME}',
             dest=constants.GCS_BQ_LD_TEMP_BUCKET_NAME,
             required=True,
             help='Spark BigQuery connector temporary bucket'
         )
         parser.add_argument(
@@ -95,49 +99,30 @@
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
-        input_file_location: str = args[constants.GCS_BQ_INPUT_LOCATION]
+        input_location: str = args[constants.GCS_BQ_INPUT_LOCATION]
+        input_format: str = args[constants.GCS_BQ_INPUT_FORMAT]
         big_query_dataset: str = args[constants.GCS_BQ_OUTPUT_DATASET]
         big_query_table: str = args[constants.GCS_BQ_OUTPUT_TABLE]
-        input_file_format: str = args[constants.GCS_BQ_INPUT_FORMAT]
         bq_temp_bucket: str = args[constants.GCS_BQ_LD_TEMP_BUCKET_NAME]
         output_mode: str = args[constants.GCS_BQ_OUTPUT_MODE]
 
         logger.info(
-            "Starting GCS to Bigquery spark job with parameters:\n"
+            "Starting Cloud Storage to BigQuery Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
-        input_data: DataFrame
-
-        if input_file_format == constants.FORMAT_PRQT:
-            input_data = spark.read \
-                .parquet(input_file_location)
-        elif input_file_format == constants.FORMAT_AVRO:
-            input_data = spark.read \
-                .format(constants.FORMAT_AVRO_EXTD) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_CSV:
-            input_data = spark.read \
-                .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_JSON:
-            input_data = spark.read \
-                .json(input_file_location)
-        elif input_file_format == constants.FORMAT_DELTA:
-            input_data = spark.read \
-                .format(constants.FORMAT_DELTA) \
-                .load(input_file_location)
+        input_data = ingest_dataframe_from_cloud_storage(
+            spark, args, input_location, input_format, "gcs.bigquery.input."
+        )
 
         # Write
         input_data.write \
             .format(constants.FORMAT_BIGQUERY) \
             .option(constants.TABLE, big_query_dataset + "." + big_query_table) \
             .option(constants.GCS_BQ_TEMP_BUCKET, bq_temp_bucket) \
             .mode(output_mode) \
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_bigtable.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigtable.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 # limitations under the License.
 
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import SparkSession
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['GCSToBigTableTemplate']
 
 
 class GCSToBigTableTemplate(BaseTemplate):
     """
     Dataproc template implementing loads from GCS into BigTable
     """
@@ -34,28 +37,30 @@
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.GCS_BT_INPUT_LOCATION}',
             dest=constants.GCS_BT_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input files'
+            help='Cloud Storage location of the input files'
         )
         parser.add_argument(
             f'--{constants.GCS_BT_INPUT_FORMAT}',
             dest=constants.GCS_BT_INPUT_FORMAT,
             required=True,
-            help='Input file format (one of: avro,parquet,csv,json)',
+            help='Input file format (one of: avro,parquet,csv,json,delta)',
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
-                constants.FORMAT_JSON
+                constants.FORMAT_JSON,
+                constants.FORMAT_DELTA
             ]
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("gcs.bigtable.input."))
         parser.add_argument(
             f'--{constants.GCS_BT_HBASE_CATALOG_JSON}',
             dest=constants.GCS_BT_HBASE_CATALOG_JSON,
             required=True,
             help='HBase catalog inline json'
         )
 
@@ -65,42 +70,27 @@
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
-        input_file_location: str = args[constants.GCS_BT_INPUT_LOCATION]
-        input_file_format: str = args[constants.GCS_BT_INPUT_FORMAT]
+        input_location: str = args[constants.GCS_BT_INPUT_LOCATION]
+        input_format: str = args[constants.GCS_BT_INPUT_FORMAT]
         catalog: str = ''.join(args[constants.GCS_BT_HBASE_CATALOG_JSON].split())
 
         logger.info(
-            "Starting GCS to BigTable spark job with parameters:\n"
+            "Starting Cloud Storage to BigTable Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
-        input_data: DataFrame
-
-        if input_file_format == constants.FORMAT_PRQT:
-            input_data = spark.read \
-                .parquet(input_file_location)
-        elif input_file_format == constants.FORMAT_AVRO:
-            input_data = spark.read \
-                .format(constants.FORMAT_AVRO_EXTD) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_CSV:
-            input_data = spark.read \
-                .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_JSON:
-            input_data = spark.read \
-                .json(input_file_location)
+        input_data = ingest_dataframe_from_cloud_storage(
+            spark, args, input_location, input_format, "gcs.bigtable.input."
+        )
 
         # Write
         input_data.write \
             .format(constants.FORMAT_HBASE) \
             .options(catalog=catalog) \
             .option('hbase.spark.use.hbasecontext', "false") \
             .save()
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,61 +18,68 @@
 import pprint
 import sys
 
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
 import dataproc_templates.util.template_constants as constants
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 
 
 __all__ = ['GCSToGCSTemplate']
 
+
 class GCSToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing loads from GCS into GCS post SQL transformation
+    Dataproc template implementing loads from Cloud Storage into Cloud Storage post SQL transformation
     """
-    
+
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
-        
+
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_INPUT_LOCATION}',
             dest=constants.GCS_TO_GCS_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input files'
+            help='Cloud Storage location of the input files'
         )
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_INPUT_FORMAT}',
             dest=constants.GCS_TO_GCS_INPUT_FORMAT,
             required=True,
-            help='GCS input file format (one of: avro,parquet,csv,json)',
+            help='Cloud Storage input file format (one of: avro,parquet,csv,json,delta)',
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
-                constants.FORMAT_JSON
+                constants.FORMAT_JSON,
+                constants.FORMAT_DELTA
             ]
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("gcs.gcs.input."))
+        add_spark_options(parser, constants.get_csv_output_spark_options("gcs.gcs.output."))
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_TEMP_VIEW_NAME}',
             dest=constants.GCS_TO_GCS_TEMP_VIEW_NAME,
             required=False,
             default="",
             help='Temp view name for creating a spark sql view on source data. This name has to match with the table name that will be used in the SQL query'
         )
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_SQL_QUERY}',
             dest=constants.GCS_TO_GCS_SQL_QUERY,
             required=False,
             default="",
             help='SQL query for data transformation. This must use the temp view name as the table to query from.'
         )
-        
+
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_OUTPUT_PARTITION_COLUMN}',
             dest=constants.GCS_TO_GCS_OUTPUT_PARTITION_COLUMN,
             required=False,
             default="",
             help='Partition column name to partition the final output in destination bucket'
         )
@@ -89,15 +96,15 @@
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
                 constants.FORMAT_JSON
             ]
         )
-        
+
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_OUTPUT_MODE}',
             dest=constants.GCS_TO_GCS_OUTPUT_MODE,
             required=False,
             default=constants.OUTPUT_MODE_APPEND,
             help=(
                 'Output write mode '
@@ -107,91 +114,68 @@
             choices=[
                 constants.OUTPUT_MODE_OVERWRITE,
                 constants.OUTPUT_MODE_APPEND,
                 constants.OUTPUT_MODE_IGNORE,
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
-        
+
         parser.add_argument(
             f'--{constants.GCS_TO_GCS_OUTPUT_LOCATION}',
             dest=constants.GCS_TO_GCS_OUTPUT_LOCATION,
             required=True,
             help=(
-                'destination GCS location'
+                'Destination Cloud Storage location'
             )
         )
-        
+
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
-        
+
         if getattr(known_args, constants.GCS_TO_GCS_SQL_QUERY) and not getattr(known_args, constants.GCS_TO_GCS_TEMP_VIEW_NAME):
             sys.exit('ArgumentParser Error: Temp view name cannot be null if you want to do data transformations with query')
 
         return vars(known_args)
-    
+
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
         # Arguments
-        gcs_input_location: str = args[constants.GCS_TO_GCS_INPUT_LOCATION]
-        gcs_input_format: str = args[constants.GCS_TO_GCS_INPUT_FORMAT]
+        input_location: str = args[constants.GCS_TO_GCS_INPUT_LOCATION]
+        input_format: str = args[constants.GCS_TO_GCS_INPUT_FORMAT]
         gcs_temp_view: str = args[constants.GCS_TO_GCS_TEMP_VIEW_NAME]
         sql_query: str = args[constants.GCS_TO_GCS_SQL_QUERY]
         output_partition_column: str = args[constants.GCS_TO_GCS_OUTPUT_PARTITION_COLUMN]
-        gcs_output_mode: str = args[constants.GCS_TO_GCS_OUTPUT_MODE]
-        gcs_output_format: str = args[constants.GCS_TO_GCS_OUTPUT_FORMAT]
-        gcs_output_location: str = args[constants.GCS_TO_GCS_OUTPUT_LOCATION]
-        
+        output_mode: str = args[constants.GCS_TO_GCS_OUTPUT_MODE]
+        output_format: str = args[constants.GCS_TO_GCS_OUTPUT_FORMAT]
+        output_location: str = args[constants.GCS_TO_GCS_OUTPUT_LOCATION]
+
         logger.info(
-            "Starting GCS to GCS with tranformations spark job with parameters:\n"
+            "Starting Cloud Storage to Cloud Storage with tranformations Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
-        
+
         # Read
-        input_data: DataFrame
-        
-        if gcs_input_format == constants.FORMAT_PRQT:
-            input_data = spark.read \
-                .parquet(gcs_input_location)
-        elif gcs_input_format == constants.FORMAT_AVRO:
-            input_data = spark.read \
-                .format(constants.FORMAT_AVRO) \
-                .load(gcs_input_location)
-        elif gcs_input_format == constants.FORMAT_CSV:
-            input_data = spark.read \
-                .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
-                .load(gcs_input_location)
-        elif gcs_input_format == constants.FORMAT_JSON:
-            input_data = spark.read \
-                .json(gcs_input_location)
-        
+        input_data = ingest_dataframe_from_cloud_storage(
+            spark,
+            args,
+            input_location,
+            input_format,
+            "gcs.gcs.input.",
+            avro_format_override=constants.FORMAT_AVRO
+        )
+
         if sql_query:
             # Create temp view on source data
             input_data.createOrReplaceTempView(gcs_temp_view)
             # Execute SQL
             output_data = spark.sql(sql_query)
         else:
             output_data = input_data
-        
+
         # Write
         if output_partition_column:
-            writer: DataFrameWriter = output_data.write.mode(gcs_output_mode).partitionBy(output_partition_column)
+            writer: DataFrameWriter = output_data.write.mode(output_mode).partitionBy(output_partition_column)
         else:
-            writer: DataFrameWriter = output_data.write.mode(gcs_output_mode)
-            
-        if gcs_output_format == constants.FORMAT_PRQT:
-            writer \
-                .parquet(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_JSON:
-            writer \
-                .json(gcs_output_location)
+            writer: DataFrameWriter = output_data.write.mode(output_mode)
+
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "gcs.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_jdbc.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_jdbc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,49 +13,54 @@
 # limitations under the License.
 
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import SparkSession
 
 from dataproc_templates import BaseTemplate
 import dataproc_templates.util.template_constants as constants
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
+
 
 __all__ = ['GCSToJDBCTemplate']
 
 
 class GCSToJDBCTemplate(BaseTemplate):
     """
-    Dataproc template implementing loads from GCS into JDBC
+    Dataproc template implementing loads from Cloud Storage into JDBC
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.GCS_JDBC_INPUT_LOCATION}',
             dest=constants.GCS_JDBC_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input files'
+            help='Cloud Storage location of the input files'
         )
         parser.add_argument(
             f'--{constants.GCS_JDBC_INPUT_FORMAT}',
             dest=constants.GCS_JDBC_INPUT_FORMAT,
             required=True,
-            help='Input file format (one of: avro,parquet,csv,json)',
+            help='Input file format (one of: avro,parquet,csv,json,delta)',
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
-                constants.FORMAT_JSON
+                constants.FORMAT_JSON,
+                constants.FORMAT_DELTA
             ]
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("gcs.jdbc.input."))
         parser.add_argument(
             f'--{constants.GCS_JDBC_OUTPUT_TABLE}',
             dest=constants.GCS_JDBC_OUTPUT_TABLE,
             required=True,
             help='JDBC output table name'
         )
         parser.add_argument(
@@ -103,56 +108,39 @@
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
-
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
-        input_file_location: str = args[constants.GCS_JDBC_INPUT_LOCATION]
-        input_file_format: str = args[constants.GCS_JDBC_INPUT_FORMAT]
+        input_location: str = args[constants.GCS_JDBC_INPUT_LOCATION]
+        input_format: str = args[constants.GCS_JDBC_INPUT_FORMAT]
         jdbc_url: str = args[constants.GCS_JDBC_OUTPUT_URL]
         jdbc_table: str = args[constants.GCS_JDBC_OUTPUT_TABLE]
         output_mode: str = args[constants.GCS_JDBC_OUTPUT_MODE]
         output_driver: str = args[constants.GCS_JDBC_OUTPUT_DRIVER]
         batch_size: int = args[constants.GCS_JDBC_BATCH_SIZE]
         jdbc_numpartitions: int = args[constants.GCS_JDBC_NUMPARTITIONS]
 
         logger.info(
-            "Starting GCS to JDBC spark job with parameters:\n"
+            "Starting Cloud Storage to JDBC Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
-        input_data: DataFrame
-
-        if input_file_format == constants.FORMAT_PRQT:
-            input_data = spark.read \
-                .parquet(input_file_location)
-        elif input_file_format == constants.FORMAT_AVRO:
-            input_data = spark.read \
-                .format(constants.FORMAT_AVRO_EXTD) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_CSV:
-            input_data = spark.read \
-                .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_JSON:
-            input_data = spark.read \
-                .json(input_file_location)
+        input_data = ingest_dataframe_from_cloud_storage(spark, args, input_location, input_format, "gcs.jdbc.input.")
 
         # Write
         if not jdbc_numpartitions:
             jdbc_numpartitions = input_data.rdd.getNumPartitions()
 
+        # TODO Convert this call to a function in dataproc_templates.util.dataframe_writer_wrappers
         input_data.write \
             .format(constants.FORMAT_JDBC) \
             .option(constants.JDBC_URL, jdbc_url) \
             .option(constants.JDBC_TABLE, jdbc_table) \
             .option(constants.JDBC_DRIVER, output_driver) \
             .option(constants.JDBC_BATCH_SIZE, batch_size) \
             .option(constants.JDBC_NUMPARTITIONS, jdbc_numpartitions) \
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/gcs_to_mongo.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_mongo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,19 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
-from pyspark.sql import SparkSession, DataFrame
-from pyspark import SparkContext, SparkConf
+from pyspark.sql import SparkSession
 
 from dataproc_templates import BaseTemplate
 import dataproc_templates.util.template_constants as constants
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
+
 
 __all__ = ['GCSToMONGOTemplate']
 
 
 class GCSToMONGOTemplate(BaseTemplate):
     """
     Dataproc template implementing loads from GCS into MongoDB Database
@@ -34,28 +36,30 @@
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.GCS_MONGO_INPUT_LOCATION}',
             dest=constants.GCS_MONGO_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input files'
+            help='Cloud Storage location of the input files'
         )
         parser.add_argument(
             f'--{constants.GCS_MONGO_INPUT_FORMAT}',
             dest=constants.GCS_MONGO_INPUT_FORMAT,
             required=True,
-            help='Input file format (one of: avro,parquet,csv,json)',
+            help='Input file format (one of: avro,parquet,csv,json,delta)',
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
-                constants.FORMAT_JSON
+                constants.FORMAT_JSON,
+                constants.FORMAT_DELTA
             ]
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("gcs.mongo.input."))
         parser.add_argument(
             f'--{constants.GCS_MONGO_OUTPUT_URI}',
             dest=constants.GCS_MONGO_OUTPUT_URI,
             required=True,
             help='GCS MONGO Output Connection Uri'
         )
         parser.add_argument(
@@ -101,47 +105,31 @@
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
-        input_file_location: str = args[constants.GCS_MONGO_INPUT_LOCATION]
-        input_file_format: str = args[constants.GCS_MONGO_INPUT_FORMAT]
+        input_location: str = args[constants.GCS_MONGO_INPUT_LOCATION]
+        input_format: str = args[constants.GCS_MONGO_INPUT_FORMAT]
         output_uri:str = args[constants.GCS_MONGO_OUTPUT_URI]
         output_database:str = args[constants.GCS_MONGO_OUTPUT_DATABASE]
         output_collection:str = args[constants.GCS_MONGO_OUTPUT_COLLECTION]
         output_mode:str = args[constants.GCS_MONGO_OUTPUT_MODE]
         batch_size:int = args[constants.GCS_MONGO_BATCH_SIZE]
 
         logger.info(
             "Starting GCS to MONGO spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
-        input_data: DataFrame
-
-        if input_file_format == constants.FORMAT_PRQT:
-            input_data = spark.read \
-                .parquet(input_file_location)
-        elif input_file_format == constants.FORMAT_AVRO:
-            input_data = spark.read \
-                .format(constants.FORMAT_AVRO_EXTD) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_CSV:
-            input_data = spark.read \
-                .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
-                .load(input_file_location)
-        elif input_file_format == constants.FORMAT_JSON:
-            input_data = spark.read \
-                .json(input_file_location)
+        input_data = ingest_dataframe_from_cloud_storage(spark, args, input_location, input_format, "gcs.mongo.input.")
 
+        # Write
         input_data.write.format(constants.FORMAT_MONGO)\
             .option(constants.MONGO_URL, output_uri) \
             .option(constants.MONGO_DATABASE, output_database) \
             .option(constants.MONGO_COLLECTION, output_collection) \
             .option(constants.MONGO_BATCH_SIZE, batch_size) \
             .mode(output_mode) \
             .save()
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/gcs/text_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/text_to_bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,19 +13,22 @@
 # limitations under the License.
 
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import SparkSession
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_reader_wrappers import ingest_dataframe_from_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['TextToBigQueryTemplate']
 
 
 class TextToBigQueryTemplate(BaseTemplate):
     """
     Dataproc template implementing Text loads from GCS into BigQuery
     """
@@ -34,16 +37,17 @@
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.TEXT_BQ_INPUT_LOCATION}',
             dest=constants.TEXT_BQ_INPUT_LOCATION,
             required=True,
-            help='GCS location of the input text files'
+            help='Cloud Storage location of the input text files'
         )
+        add_spark_options(parser, constants.get_csv_input_spark_options("text.bigquery.input."))
         parser.add_argument(
             f'--{constants.TEXT_BQ_OUTPUT_DATASET}',
             dest=constants.TEXT_BQ_OUTPUT_DATASET,
             required=True,
             help='BigQuery dataset for the output table'
         )
         parser.add_argument(
@@ -102,40 +106,40 @@
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
-
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
-        input_file_location: str = args[constants.TEXT_BQ_INPUT_LOCATION]
+        input_location: str = args[constants.TEXT_BQ_INPUT_LOCATION]
         big_query_dataset: str = args[constants.TEXT_BQ_OUTPUT_DATASET]
         big_query_table: str = args[constants.TEXT_BQ_OUTPUT_TABLE]
         bq_temp_bucket: str = args[constants.TEXT_BQ_LD_TEMP_BUCKET_NAME]
         output_mode: str = args[constants.TEXT_BQ_OUTPUT_MODE]
-        input_delimiter: str = args[constants.TEXT_INPUT_DELIMITER]
-        input_file_codec_format: str = args[constants.TEXT_INPUT_COMPRESSION]
+        # These options are redundant but left in place until this template is removed
+        # via issue https://github.com/GoogleCloudPlatform/dataproc-templates/issues/721
+        # input_delimiter: str = args[constants.TEXT_INPUT_DELIMITER]
+        # input_file_codec_format: str = args[constants.TEXT_INPUT_COMPRESSION]
 
         logger.info(
-            "Starting GCS to Bigquery spark job with parameters:\n"
+            "Starting GCS to Bigquery Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
-        input_data: DataFrame
-
-        input_data = spark.read\
-            .option(constants.HEADER, True) \
-            .option(constants.INFER_SCHEMA, True) \
-            .option(constants.INPUT_COMPRESSION, input_file_codec_format)\
-            .option(constants.INPUT_DELIMITER, input_delimiter)\
-            .csv(input_file_location)
+        input_data = ingest_dataframe_from_cloud_storage(
+            spark,
+            args,
+            input_location,
+            constants.FORMAT_CSV,
+            "text.bigquery.input.",
+        )
 
         # Write
         input_data.write \
             .format(constants.FORMAT_BIGQUERY) \
             .option(constants.TABLE, big_query_dataset + "." + big_query_table) \
             .option(constants.TEXT_BQ_TEMP_BUCKET, bq_temp_bucket) \
             .mode(output_mode) \
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hbase/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hbase/hbase_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/hbase_to_gcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 from logging import Logger
 import argparse
 import pprint
 
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['HbaseToGCSTemplate']
 
 
 class HbaseToGCSTemplate(BaseTemplate):
     """
     Dataproc template implementing loads from Hbase into GCS
     """
@@ -34,15 +37,15 @@
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.HBASE_GCS_OUTPUT_LOCATION}',
             dest=constants.HBASE_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.HBASE_GCS_OUTPUT_FORMAT}',
             dest=constants.HBASE_GCS_OUTPUT_FORMAT,
             required=True,
             help='Output file format (one of: avro,parquet,csv,json)',
             choices=[
@@ -69,16 +72,17 @@
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
         parser.add_argument(
             f'--{constants.HBASE_GCS_CATALOG_JSON}',
             dest=constants.HBASE_GCS_CATALOG_JSON,
             required=True,
-            help='Hbase catalog json'
+            help='Hbase catalog JSON'
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("hbase.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
@@ -88,33 +92,21 @@
         # Arguments
         output_location: str = args[constants.HBASE_GCS_OUTPUT_LOCATION]
         output_format: str = args[constants.HBASE_GCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.HBASE_GCS_OUTPUT_MODE]
         catalog: str = ''.join(args[constants.HBASE_GCS_CATALOG_JSON].split())
 
         logger.info(
-            "Starting Hbase to GCS spark job with parameters:\n"
+            "Starting Hbase to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
         input_data: DataFrame
         input_data = spark.read.format(constants.FORMAT_HBASE) \
                            .options(catalog=catalog) \
                            .option("hbase.spark.use.hbasecontext", "false") \
                            .load()
 
-        #write
+        # Write
         writer: DataFrameWriter = input_data.write.mode(output_mode)
-
-        if output_format == constants.FORMAT_PRQT:
-            writer.parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer.json(output_location)
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "hbase.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hive/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hive/hive_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hive/hive_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_gcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 from logging import Logger
 import argparse
 import pprint
 import sys
 from pyspark.sql import SparkSession, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['HiveToGCSTemplate']
 
 
 class HiveToGCSTemplate(BaseTemplate):
     """
     Dataproc template implementing exports from Hive to GCS
     """
@@ -47,23 +50,23 @@
             required=True,
             help='Hive table for exporting data to GCS'
         )
         parser.add_argument(
             f'--{constants.HIVE_GCS_OUTPUT_LOCATION}',
             dest=constants.HIVE_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.HIVE_GCS_OUTPUT_FORMAT}',
             dest=constants.HIVE_GCS_OUTPUT_FORMAT,
             required=False,
             default=constants.FORMAT_PRQT,
             help=(
-                'Output file format ' 
+                'Output file format '
                 '(one of: avro,parquet,csv,json) '
                 '(Defaults to parquet)'
             ),
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
@@ -97,14 +100,15 @@
         parser.add_argument(
             f'--{constants.HIVE_GCS_SQL_QUERY}',
             dest=constants.HIVE_GCS_SQL_QUERY,
             required=False,
             default="",
             help='SQL query for data transformation. This must use the temp view name as the table to query from.'
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("hive.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         if getattr(known_args, constants.HIVE_GCS_SQL_QUERY) and not getattr(known_args, constants.HIVE_GCS_TEMP_VIEW_NAME):
             sys.exit('ArgumentParser Error: Temp view name cannot be null if you want to do data transformations with query')
 
@@ -136,22 +140,9 @@
             # Create temp view on source data
             input_data.createGlobalTempView(hive_temp_view)
             # Execute SQL
             output_data = spark.sql(sql_query)
         else:
             output_data = input_data
 
-        # Write
         writer: DataFrameWriter = output_data.write.mode(output_mode)
-
-        if output_format == constants.FORMAT_PRQT:
-            writer.parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer.json(output_location)
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "hive.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-
 import argparse
 import pprint
 from logging import Logger
 from typing import Any, Dict, Optional, Sequence
 import dataproc_templates.util.template_constants as constants
 from dataproc_templates import BaseTemplate
 from pyspark.sql import SparkSession
 from datetime import datetime
 
-
-class HiveDDLExtractorTemplate(BaseTemplate): 
+class HiveDDLExtractorTemplate(BaseTemplate):
     """
     Dataproc template implementing exports from Hive to BigQuery
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
@@ -44,15 +42,31 @@
 
         parser.add_argument(
             f'--{constants.HIVE_DDL_EXTRACTOR_OUTPUT_GCS_PATH}',
             dest=constants.HIVE_DDL_EXTRACTOR_OUTPUT_GCS_PATH,
             required=True,
             help='GCS output path'
         )
-       
+
+        parser.add_argument(
+            f'--{constants.HIVE_DDL_CONSIDER_SPARK_TABLES}',
+            dest=constants.HIVE_DDL_CONSIDER_SPARK_TABLES,
+            required=False,
+            default=False,
+            help='Flag to extract DDL of Spark tables'
+        )
+
+        parser.add_argument(
+            f'--{constants.HIVE_DDL_TRANSLATION_DISPOSITION}',
+            dest=constants.HIVE_DDL_TRANSLATION_DISPOSITION,
+            required=False,
+            default=False,
+            help='Remove location parameter from HIVE DDL if set to TRUE, to be compatible with BigQuery SQL translator'
+        )
+
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
@@ -61,26 +75,30 @@
         Dataproc template allowing the extraction of DDLs from Hive Metastore
 
         """
         logger: Logger = self.get_logger(spark=spark)
 
         hive_database: str = args[constants.HIVE_DDL_EXTRACTOR_INPUT_DATABASE]
         gcs_output_path: str = args[constants.HIVE_DDL_EXTRACTOR_OUTPUT_GCS_PATH]
+        spark_tbls_flag: bool = args[constants.HIVE_DDL_CONSIDER_SPARK_TABLES]
+        remove_location_flag: bool = args[constants.HIVE_DDL_TRANSLATION_DISPOSITION]
 
         logger.info(
-                "Starting Hive DDL Extraction job with parameters:\n"
-                f"{pprint.pformat(args)}"
-            )
-        
-               
+            "Starting Hive DDL Extraction job with parameters:\n"
+            f"{pprint.pformat(args)}"
+        )
+
         def get_ddl(hive_database, table_name):
-            return spark.sql(f"SHOW CREATE TABLE {hive_database}.{table_name} AS SERDE").rdd.map(lambda x: x[0] + ";").collect()[0]
+            spark_tbls_opt = "" if str(spark_tbls_flag).upper() == "TRUE" else "AS SERDE"
+            ddl_str = spark.sql(f"SHOW CREATE TABLE {hive_database}.{table_name} {spark_tbls_opt}").rdd.map(lambda x: x[0]).collect()[0]
+            ddl_str = ddl_str + ";" if str(remove_location_flag).upper() != "TRUE" else ddl_str.split("\nLOCATION '")[0].split("\nUSING ")[0]+";"
+            return ddl_str
 
         ct = datetime.now().strftime("%m-%d-%Y %H.%M.%S")
         output_path = gcs_output_path+"/"+hive_database+"/"+str(ct)
 
         tables_names = spark.sql(f"SHOW TABLES IN {hive_database}").select("tableName")
         tables_name_list = tables_names.rdd.map(lambda x: x[0]).collect()
-        tables_ddls = [ get_ddl(hive_database, table_name) for table_name in tables_name_list ]
+        tables_ddls = [get_ddl(hive_database, table_name) for table_name in tables_name_list]
 
         ddls_rdd = spark.sparkContext.parallelize(tables_ddls)
         ddls_rdd.coalesce(1).saveAsTextFile(output_path)
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from logging import Logger
 import argparse
 import pprint
 import sys
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['JDBCToGCSTemplate']
 
 
 class JDBCToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing loads from JDBC into GCS
+    Dataproc template implementing loads from JDBC into Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
@@ -101,15 +104,15 @@
             default="",
             help='Custom SQL statement to execute in each reader database session'
         )
         parser.add_argument(
             f'--{constants.JDBCTOGCS_OUTPUT_LOCATION}',
             dest=constants.JDBCTOGCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.JDBCTOGCS_OUTPUT_FORMAT}',
             dest=constants.JDBCTOGCS_OUTPUT_FORMAT,
             required=True,
             help='Output file format (one of: avro,parquet,csv,json)',
             choices=[
@@ -137,15 +140,15 @@
             ]
         )
         parser.add_argument(
             f'--{constants.JDBCTOGCS_OUTPUT_PARTITIONCOLUMN}',
             dest=constants.JDBCTOGCS_OUTPUT_PARTITIONCOLUMN,
             required=False,
             default="",
-            help='GCS partition column name'
+            help='Cloud Storage partition column name'
         )
         parser.add_argument(
             f'--{constants.JDBCTOGCS_TEMP_VIEW_NAME}',
             dest=constants.JDBCTOGCS_TEMP_VIEW_NAME,
             required=False,
             default="",
             help='Temp view name for creating a spark sql view on source data. This name has to match with the table name that will be used in the SQL query'
@@ -153,14 +156,15 @@
         parser.add_argument(
             f'--{constants.JDBCTOGCS_TEMP_SQL_QUERY}',
             dest=constants.JDBCTOGCS_TEMP_SQL_QUERY,
             required=False,
             default="",
             help='SQL query for data transformation. This must use the temp view name as the table to query from.'
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("jdbc.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         if getattr(known_args, constants.JDBCTOGCS_INPUT_TABLE) and getattr(known_args, constants.JDBCTOGCS_INPUT_SQL_QUERY):
             sys.exit('ArgumentParser Error: Arguments cannot have both input table and sql query, use either one.')
 
@@ -188,30 +192,30 @@
         output_format: str = args[constants.JDBCTOGCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.JDBCTOGCS_OUTPUT_MODE]
         output_partitioncolumn: str = args[constants.JDBCTOGCS_OUTPUT_PARTITIONCOLUMN]
         temp_view: str = args[constants.JDBCTOGCS_TEMP_VIEW_NAME]
         temp_sql_query:str = args[constants.JDBCTOGCS_TEMP_SQL_QUERY]
 
         logger.info(
-            "Starting JDBC to GCS Spark job with parameters:\n"
+            "Starting JDBC to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
         input_data: DataFrame
 
         read_properties = {constants.JDBC_URL: input_jdbc_url,
                            constants.JDBC_DRIVER: input_jdbc_driver}
 
         if input_jdbc_table:
             read_properties.update({constants.JDBC_TABLE: input_jdbc_table})
         elif input_jdbc_sql_query:
             read_properties.update({constants.JDBC_QUERY: input_jdbc_sql_query})
         else:
-            logger.error("Arguments must have either input table or input sql query")
+            logger.error("Arguments must have either input table or input SQL query")
             exit(1)
 
         read_properties.update({constants.JDBC_NUMPARTITIONS: jdbc_numpartitions,
                                 constants.JDBC_FETCHSIZE: input_jdbc_fetchsize})
 
         if input_jdbc_sessioninitstatement:
             read_properties[constants.JDBC_SESSIONINITSTATEMENT] = input_jdbc_sessioninitstatement
@@ -241,21 +245,8 @@
 
         # Write
         if (output_partitioncolumn != ""):
             writer: DataFrameWriter = output_data.write.mode(output_mode).partitionBy(output_partitioncolumn)
         else:
             writer: DataFrameWriter = output_data.write.mode(output_mode)
 
-        if output_format == constants.FORMAT_PRQT:
-            writer \
-                .parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer \
-                .json(output_location)
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "jdbc.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/kafka_to_bq.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_bq.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/kafka/kafka_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/mongo/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/mongo/mongo_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/mongo_to_gcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,45 +16,48 @@
 from logging import Logger
 import argparse
 import pprint
 
 from pyspark.sql import SparkSession, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['MongoToGCSTemplate']
 
 
 class MongoToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing exports from Mongo to GCS
+    Dataproc template implementing exports from Mongo to Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.MONGO_GCS_INPUT_URI}',
             dest=constants.MONGO_GCS_INPUT_URI,
             required=True,
-            help='MONGO GCS Input Connection Uri'
+            help='MONGO Cloud Storage Input Connection Uri'
         )
         parser.add_argument(
             f'--{constants.MONGO_GCS_INPUT_DATABASE}',
             dest=constants.MONGO_GCS_INPUT_DATABASE,
             required=True,
-            help='MONGO GCS Input Database Name'
+            help='MONGO Cloud Storage Input Database Name'
         )
         parser.add_argument(
             f'--{constants.MONGO_GCS_INPUT_COLLECTION}',
             dest=constants.MONGO_GCS_INPUT_COLLECTION,
             required=True,
-            help='MONGO GCS Input Collection Name'
+            help='MONGO Cloud Storage Input Collection Name'
         )
         parser.add_argument(
             f'--{constants.MONGO_GCS_OUTPUT_FORMAT}',
             dest=constants.MONGO_GCS_OUTPUT_FORMAT,
             required=True,
             help='Output file format (one of: avro,parquet,csv,json)',
             choices=[
@@ -64,15 +67,15 @@
                 constants.FORMAT_JSON
             ]
         )
         parser.add_argument(
             f'--{constants.MONGO_GCS_OUTPUT_LOCATION}',
             dest=constants.MONGO_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.MONGO_GCS_OUTPUT_MODE}',
             dest=constants.MONGO_GCS_OUTPUT_MODE,
             required=False,
             default=constants.OUTPUT_MODE_APPEND,
             help=(
@@ -83,14 +86,15 @@
             choices=[
                 constants.OUTPUT_MODE_OVERWRITE,
                 constants.OUTPUT_MODE_APPEND,
                 constants.OUTPUT_MODE_IGNORE,
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("mongo.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
@@ -102,34 +106,22 @@
         input_database: str = args[constants.MONGO_GCS_INPUT_DATABASE]
         input_collection: str = args[constants.MONGO_GCS_INPUT_COLLECTION]
         output_format: str = args[constants.MONGO_GCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.MONGO_GCS_OUTPUT_MODE]
         output_location: str = args[constants.MONGO_GCS_OUTPUT_LOCATION]
 
         logger.info(
-            "Starting Mongo to GCS spark job with parameters:\n"
+            "Starting Mongo to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
 
         # Read
         input_data = spark.read \
             .format(constants.FORMAT_MONGO) \
             .option(constants.MONGO_INPUT_URI, input_uri) \
             .option(constants.MONGO_DATABASE, input_database) \
             .option(constants.MONGO_COLLECTION, input_collection) \
             .load()
 
         # Write
         writer: DataFrameWriter = input_data.write.mode(output_mode)
-
-        if output_format == constants.FORMAT_PRQT:
-            writer.parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer.json(output_location)
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "mongo.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/redshift/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/redshift/redshift_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/redshift_to_gcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from logging import Logger
 import argparse
 import pprint
 
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['RedshiftToGCSTemplate']
 
 
 class RedshiftToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing loads from REDSHIFT into GCS
+    Dataproc template implementing loads from REDSHIFT into Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
@@ -72,15 +75,15 @@
             default="",
             help='AWS Secret Keys which allow access to S3'
         )
         parser.add_argument(
             f'--{constants.REDSHIFTTOGCS_OUTPUT_LOCATION}',
             dest=constants.REDSHIFTTOGCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS location for output files'
+            help='Cloud Storage location for output files'
         )
         parser.add_argument(
             f'--{constants.REDSHIFTTOGCS_OUTPUT_FORMAT}',
             dest=constants.REDSHIFTTOGCS_OUTPUT_FORMAT,
             required=True,
             help='Output file format (one of: avro,parquet,csv,json)',
             choices=[
@@ -108,16 +111,17 @@
             ]
         )
         parser.add_argument(
             f'--{constants.REDSHIFTTOGCS_OUTPUT_PARTITIONCOLUMN}',
             dest=constants.REDSHIFTTOGCS_OUTPUT_PARTITIONCOLUMN,
             required=False,
             default="",
-            help='GCS partition column name'
+            help='Cloud Storage partition column name'
         )
+        add_spark_options(parser, constants.get_csv_output_spark_options("redshift.gcs.output."))
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
@@ -127,52 +131,39 @@
         # Arguments
         input_redshift_url: str = args[constants.REDSHIFTTOGCS_INPUT_URL]
         input_redshift_tempdir: str = args[constants.REDSHIFTTOGCS_S3_TEMPDIR]
         input_redshift_table: str = args[constants.REDSHIFTTOGCS_INPUT_TABLE]
         input_redshift_iam_role: str = args[constants.REDSHIFTTOGCS_IAM_ROLEARN]
         input_redshift_accesskey: str = args[constants.REDSHIFTTOGCS_S3_ACCESSKEY]
         input_redshift_secretkey: str = args[constants.REDSHIFTTOGCS_S3_SECRETKEY]
-        
+
         output_location: str = args[constants.REDSHIFTTOGCS_OUTPUT_LOCATION]
         output_format: str = args[constants.REDSHIFTTOGCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.REDSHIFTTOGCS_OUTPUT_MODE]
         output_partitioncolumn: str = args[constants.REDSHIFTTOGCS_OUTPUT_PARTITIONCOLUMN]
 
         logger.info(
-            "Starting REDSHIFT to GCS spark job with parameters:\n"
+            "Starting REDSHIFT to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
-        
+
         # Read
         input_data: DataFrame
-        
+
         spark._jsc.hadoopConfiguration().set(constants.AWS_S3ACCESSKEY, input_redshift_accesskey)
         spark._jsc.hadoopConfiguration().set(constants.AWS_S3SECRETKEY, input_redshift_secretkey)
-        
+
         input_data=spark.read \
                 .format(constants.FORMAT_REDSHIFT) \
                 .option(constants.JDBC_URL, input_redshift_url) \
                 .option(constants.JDBC_TABLE, input_redshift_table) \
                 .option(constants.REDSHIFT_TEMPDIR, input_redshift_tempdir) \
                 .option(constants.REDSHIFT_IAMROLE, input_redshift_iam_role) \
                 .load()
 
         # Write
         if (output_partitioncolumn != ""):
             writer: DataFrameWriter = input_data.write.mode(output_mode).partitionBy(output_partitioncolumn)
         else:
             writer: DataFrameWriter = input_data.write.mode(output_mode)
-            
-        if output_format == constants.FORMAT_PRQT:
-            writer \
-                .parquet(output_location)
-        elif output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(output_location)
-        elif output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(output_location)
-        elif output_format == constants.FORMAT_JSON:
-            writer \
-                .json(output_location)
+
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "redshift.gcs.output.")
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/s3/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/s3/s3_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/s3/s3_to_bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,16 +151,16 @@
         elif input_file_format == constants.FORMAT_AVRO:
             input_data = spark.read \
                 .format(constants.FORMAT_AVRO_EXTD) \
                 .load(input_file_location)
         elif input_file_format == constants.FORMAT_CSV:
             input_data = spark.read \
                 .format(constants.FORMAT_CSV) \
-                .option(constants.HEADER, True) \
-                .option(constants.INFER_SCHEMA, True) \
+                .option(constants.CSV_HEADER, True) \
+                .option(constants.CSV_INFER_SCHEMA, True) \
                 .load(input_file_location)
         elif input_file_format == constants.FORMAT_JSON:
             input_data = spark.read \
                 .json(input_file_location)
 
         # Write
         input_data.write \
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/snowflake/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,105 +17,108 @@
 import argparse
 import pprint
 import sys
 
 from pyspark.sql import SparkSession, DataFrame, DataFrameWriter
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
+
 __all__ = ['SnowflakeToGCSTemplate']
 
 
 class SnowflakeToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing loads from Snowflake to GCS
+    Dataproc template implementing loads from Snowflake to Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_URL}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_URL,
             required=True,
             help='Snowflake connection URL'
         )
 
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_USER}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_USER,
             required=True,
             help='Snowflake user name'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_PASSWORD}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_PASSWORD,
             required=True,
             help='Snowflake password'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_DATABASE}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_DATABASE,
             required=False,
             default="",
             help='Snowflake database name'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_WAREHOUSE}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_WAREHOUSE,
             required=False,
             default="",
             help='Snowflake datawarehouse name'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_AUTOPUSHDOWN}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_AUTOPUSHDOWN,
             required=False,
             default="on",
             help='Snowflake Autopushdown (on|off)'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_SCHEMA}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_SCHEMA,
             required=False,
             default="",
             help='Snowflake Schema, the source table belongs to'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_TABLE}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_TABLE,
             required=False,
             default="",
             help='Snowflake table name'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_SF_QUERY}',
             dest=constants.SNOWFLAKE_TO_GCS_SF_QUERY,
             required=False,
             default="",
             help='Query to be executed on Snowflake to fetch \
                 the desired dataset for migration'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_OUTPUT_LOCATION}',
             dest=constants.SNOWFLAKE_TO_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS output location where the migrated data will be placed'
+            help='Cloud Storage output location where the migrated data will be placed'
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_OUTPUT_MODE}',
             dest=constants.SNOWFLAKE_TO_GCS_OUTPUT_MODE,
             required=False,
             default=constants.OUTPUT_MODE_APPEND,
             help=(
                 'Output write mode '
@@ -125,15 +128,15 @@
             choices=[
                 constants.OUTPUT_MODE_OVERWRITE,
                 constants.OUTPUT_MODE_APPEND,
                 constants.OUTPUT_MODE_IGNORE,
                 constants.OUTPUT_MODE_ERRORIFEXISTS
             ]
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_OUTPUT_FORMAT}',
             dest=constants.SNOWFLAKE_TO_GCS_OUTPUT_FORMAT,
             required=False,
             default=constants.FORMAT_CSV,
             help=(
                 'Output write format '
@@ -143,153 +146,139 @@
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_PRQT,
                 constants.FORMAT_CSV,
                 constants.FORMAT_JSON
             ]
         )
-        
+
         parser.add_argument(
             f'--{constants.SNOWFLAKE_TO_GCS_PARTITION_COLUMN}',
             dest=constants.SNOWFLAKE_TO_GCS_PARTITION_COLUMN,
             required=False,
             default="",
-            help='Column name to partition data by, in GCS bucket'
+            help='Column name to partition data by, in Cloud Storage bucket'
         )
-        
+        add_spark_options(parser, constants.get_csv_output_spark_options("snowflake.gcs.output."))
+
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
-        
-        if ((not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_DATABASE) 
-                or not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_SCHEMA) 
+
+        if ((not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_DATABASE)
+                or not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_SCHEMA)
                 or not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_TABLE))
             and not getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_QUERY)):
 
             sys.exit("ArgumentParser Error: Either of snowflake.to.gcs.sf.database, snowflake.to.gcs.sf.schema and snowflake.to.gcs.sf.table "
                         + "OR snowflake.to.gcs.sf.query needs to be provided as argument to read data from Snowflake")
-            
-        elif ((getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_DATABASE) 
-                or getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_SCHEMA) 
+
+        elif ((getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_DATABASE)
+                or getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_SCHEMA)
                 or getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_TABLE))
             and getattr(known_args, constants.SNOWFLAKE_TO_GCS_SF_QUERY)):
-            
+
             sys.exit("ArgumentParser Error: All three snowflake.to.gcs.sf.database, snowflake.to.gcs.sf.schema and snowflake.to.gcs.sf.table "
                         + "AND snowflake.to.gcs.sf.query cannot be provided as arguments at the same time.")
 
         return vars(known_args)
-    
+
     def get_read_options(self, logger: Logger, args: Dict[str, Any]) -> "tuple[DataFrame, DataFrame]":
-        
+
         # Arguments
         sf_url: str = args[constants.SNOWFLAKE_TO_GCS_SF_URL]
         sf_user: str = args[constants.SNOWFLAKE_TO_GCS_SF_USER]
         sf_pwd: str = args[constants.SNOWFLAKE_TO_GCS_SF_PASSWORD]
         sf_database: str = args[constants.SNOWFLAKE_TO_GCS_SF_DATABASE]
         sf_schema: str = args[constants.SNOWFLAKE_TO_GCS_SF_SCHEMA]
         sf_warehouse: str = args[constants.SNOWFLAKE_TO_GCS_SF_WAREHOUSE]
         sf_autopushdown: str = args[constants.SNOWFLAKE_TO_GCS_SF_AUTOPUSHDOWN]
         sf_table: str = args[constants.SNOWFLAKE_TO_GCS_SF_TABLE]
         sf_query: str = args[constants.SNOWFLAKE_TO_GCS_SF_QUERY]
-        
+
         logger.info(
-            "Starting Snowflake to GCS spark job with parameters:\n"
+            "Starting Snowflake to Cloud Storage Spark job with parameters:\n"
             f"{pprint.pformat(args)}"
         )
-        
-        sf_options = { 
+
+        sf_options = {
                      "sfURL" : sf_url,
                      "sfUser" : sf_user,
                      "sfPassword" : sf_pwd,
                      "sfDatabase" : sf_database,
                      "sfSchema" : sf_schema,
                      "sfWarehouse" : sf_warehouse,
                      "autopushdown" : sf_autopushdown
                     }
-        
+
         data_options = {
             "dbtable" : sf_table,
             "query" : sf_query
         }
-        
+
         return sf_options, data_options
-       
+
+
     def read_data(self, logger: Logger, spark: SparkSession, sf_opt: Dict[str,Any], data_opt: Dict[str,Any] ) -> DataFrame:
-        
+
         if not sf_opt or not data_opt:
             sys.exit("There seems to be an issue in fetching read options. Read options cannot be empty \n")
-            
+
         # Read
         logger.info(
             "Starting process of reading data from source \n"
         )
-        
+
         input_data: DataFrame = spark.read.format(constants.FORMAT_SNOWFLAKE) \
             .options(**sf_opt)
-        
+
         if data_opt["dbtable"]:
             input_data = input_data.option("dbtable",data_opt["dbtable"])
         else:
             input_data = input_data.option("query",data_opt["query"])
-            
-        input_data = input_data.load()        
+
+        input_data = input_data.load()
         count = input_data.count()
-        
+
         if not count :
             sys.exit("The input dataframe is empty. The table is either empty or there is no data for the selected filters")
         else:
             logger.info(
             "Data from source has been read successfully \n"
             )
-            
+
         return input_data
-            
-    def write_data(self, logger: Logger, args: Dict[str, Any], input_data: DataFrame) -> None:   
-        
-        gcs_output_format: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_FORMAT]
-        gcs_output_location: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_LOCATION]
-        gcs_output_mode: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_MODE]
-        gcs_partition_col: str = args[constants.SNOWFLAKE_TO_GCS_PARTITION_COLUMN]
-                    
+
+
+    def write_data(self, logger: Logger, args: Dict[str, Any], input_data: DataFrame) -> None:
+
+        output_format: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_FORMAT]
+        output_location: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_LOCATION]
+        output_mode: str = args[constants.SNOWFLAKE_TO_GCS_OUTPUT_MODE]
+        partition_col: str = args[constants.SNOWFLAKE_TO_GCS_PARTITION_COLUMN]
+
         # Write
         logger.info(
-            "Starting process of writing data to GCS \n"
+            "Starting process of writing data to Cloud Storage \n"
         )
-        
-        if gcs_partition_col:
-            writer: DataFrameWriter = input_data.write.mode(gcs_output_mode) \
-                .partitionBy(gcs_partition_col)
+
+        if partition_col:
+            writer: DataFrameWriter = input_data.write.mode(output_mode) \
+                .partitionBy(partition_col)
         else:
-            writer: DataFrameWriter = input_data.write.mode(gcs_output_mode)
+            writer: DataFrameWriter = input_data.write.mode(output_mode)
+
+        persist_dataframe_to_cloud_storage(writer, args, output_location, output_format, "snowflake.gcs.output.")
 
-        if gcs_output_format == constants.FORMAT_PRQT:
-            writer \
-                .parquet(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_AVRO:
-            writer \
-                .format(constants.FORMAT_AVRO) \
-                .save(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_CSV:
-            writer \
-                .option(constants.HEADER, True) \
-                .csv(gcs_output_location)
-        elif gcs_output_format == constants.FORMAT_JSON:
-            writer \
-                .json(gcs_output_location)
-                
         logger.info(
-            "Data from source has been loaded to GCS successfully"
+            "Data from source has been loaded to Cloud Storage successfully"
         )
 
 
-    def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:  
-        
-        logger: Logger = self.get_logger(spark=spark)  
-        
+    def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
+
+        logger: Logger = self.get_logger(spark=spark)
+
         sf_options, data_options = self.get_read_options(logger, args)
-        
+
         input_data = self.read_data(logger, spark, sf_options, data_options)
-        
+
         self.write_data(logger, args, input_data)
-        
-        
-        
-
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/template_name.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/template_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,19 +36,22 @@
     JDBCTOJDBC = "JDBCTOJDBC"
     JDBCTOGCS = "JDBCTOGCS"
     JDBCTOBIGQUERY = "JDBCTOBIGQUERY"
     MONGOTOGCS = "MONGOTOGCS"
     SNOWFLAKETOGCS = "SNOWFLAKETOGCS"
     REDSHIFTTOGCS = "REDSHIFTTOGCS"
     CASSANDRATOBQ= "CASSANDRATOBQ"
+    AZUREBLOBSTORAGETOBQ = "AZUREBLOBSTORAGETOBQ"
     CASSANDRATOGCS = "CASSANDRATOGCS"
     HIVEDDLEXTRACTOR = "HIVEDDLEXTRACTOR"
     KAFKATOGCS="KAFKATOGCS"
     KAFKATOBQ="KAFKATOBQ"
     S3TOBIGQUERY = "S3TOBIGQUERY"
+    PUBSUBLITETOGCS = "PUBSUBLITETOGCS"
+
 
 
     @classmethod
     def from_string(cls, template_name: str) -> TemplateName:
         """
         Get the TemplateName value from a string.
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/util/__init__.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/util/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/util/argument_parsing.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/util/argument_parsing.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Sequence
+from typing import Optional, Sequence, Union
 import argparse
 
+import dataproc_templates.util.template_constants as constants
 from dataproc_templates import TemplateName
 
 
 def get_template_name(args: Optional[Sequence[str]] = None) -> TemplateName:
     """
     Parses the template name option from the program arguments.
 
@@ -88,7 +89,25 @@
 
     known_args: argparse.Namespace
     known_args, _ = parser.parse_known_args(args=args)
 
     return known_args.log_level
 
 
+def add_spark_options(parser: argparse.ArgumentParser, template_to_spark_option_map: dict, read_options: bool = True) -> None:
+    if not template_to_spark_option_map:
+        return
+
+    for option_name, spark_option_name in template_to_spark_option_map.items():
+        if read_options:
+            help_text = (constants.SPARK_OPTIONS[spark_option_name].get(constants.OPTION_READ_HELP, "")
+                         or constants.SPARK_OPTIONS[spark_option_name].get(constants.OPTION_HELP, ""))
+        else:
+            help_text = (constants.SPARK_OPTIONS[spark_option_name].get(constants.OPTION_WRITE_HELP, "")
+                         or constants.SPARK_OPTIONS[spark_option_name].get(constants.OPTION_HELP, ""))
+        parser.add_argument(
+            f'--{option_name}',
+            dest=option_name,
+            required=False,
+            default=constants.SPARK_OPTIONS[spark_option_name].get(constants.OPTION_DEFAULT, ""),
+            help=help_text
+        )
```

### Comparing `google-dataproc-templates-0.1.0b0/dataproc_templates/util/tracking.py` & `google-dataproc-templates-0.2.0b0/dataproc_templates/util/tracking.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/PKG-INFO` & `google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: google-dataproc-templates
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: Google Dataproc templates written in Python
 Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
 
 # Dataproc Templates (Python - PySpark)
+* [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
 * [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
@@ -24,14 +25,15 @@
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.1.0b0/google_dataproc_templates.egg-info/SOURCES.txt` & `google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 README.md
 setup.cfg
 setup.py
 version.py
 dataproc_templates/__init__.py
 dataproc_templates/base_template.py
 dataproc_templates/template_name.py
+dataproc_templates/azure/__init__.py
+dataproc_templates/azure/azure_blob_storage_to_bigquery.py
 dataproc_templates/bigquery/__init__.py
 dataproc_templates/bigquery/bigquery_to_gcs.py
 dataproc_templates/cassandra/__init__.py
 dataproc_templates/cassandra/cassandra_to_bigquery.py
 dataproc_templates/cassandra/cassandra_to_gcs.py
 dataproc_templates/gcs/__init__.py
 dataproc_templates/gcs/gcs_to_bigquery.py
@@ -30,29 +32,35 @@
 dataproc_templates/jdbc/jdbc_to_gcs.py
 dataproc_templates/jdbc/jdbc_to_jdbc.py
 dataproc_templates/kafka/__init__.py
 dataproc_templates/kafka/kafka_to_bq.py
 dataproc_templates/kafka/kafka_to_gcs.py
 dataproc_templates/mongo/__init__.py
 dataproc_templates/mongo/mongo_to_gcs.py
+dataproc_templates/pubsublite/__init__.py
+dataproc_templates/pubsublite/pubsublite_to_gcs.py
 dataproc_templates/redshift/__init__.py
 dataproc_templates/redshift/redshift_to_gcs.py
 dataproc_templates/s3/__init__.py
 dataproc_templates/s3/s3_to_bigquery.py
 dataproc_templates/snowflake/__init__.py
 dataproc_templates/snowflake/snowflake_to_gcs.py
 dataproc_templates/util/__init__.py
 dataproc_templates/util/argument_parsing.py
+dataproc_templates/util/dataframe_reader_wrappers.py
+dataproc_templates/util/dataframe_writer_wrappers.py
 dataproc_templates/util/template_constants.py
 dataproc_templates/util/tracking.py
 google_dataproc_templates.egg-info/PKG-INFO
 google_dataproc_templates.egg-info/SOURCES.txt
 google_dataproc_templates.egg-info/dependency_links.txt
 google_dataproc_templates.egg-info/requires.txt
 google_dataproc_templates.egg-info/top_level.txt
+test/azure/__init__.py
+test/azure/test_azure_blob_storage_to_bigquery.py
 test/bigquery/__init__.py
 test/bigquery/test_bigquery_to_gcs.py
 test/cassandra/__init__.py
 test/cassandra/test_cassandra_to_bq.py
 test/cassandra/test_cassandra_to_gcs.py
 test/gcs/__init__.py
 test/gcs/test_gcs_to_bigquery.py
@@ -70,13 +78,15 @@
 test/hive/util/test_hive_ddl_extractor.py
 test/jdbc/__init__.py
 test/jdbc/test_jdbc_to_bigquery.py
 test/jdbc/test_jdbc_to_gcs.py
 test/jdbc/test_jdbc_to_jdbc.py
 test/mongo/__init__.py
 test/mongo/test_mongo_to_gcs.py
+test/pubsublite/__init__.py
+test/pubsublite/test_pubsublite_to_gcs.py
 test/redshift/__init__.py
 test/redshift/test_redshift_to_gcs.py
 test/s3/__init__.py
 test/s3/test_s3_to_bigquery.py
 test/util/__init__.py
 test/util/test_argument_parsing.py
```

### Comparing `google-dataproc-templates-0.1.0b0/setup.py` & `google-dataproc-templates-0.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/bigquery/test_bigquery_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/bigquery/test_bigquery_to_gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,18 @@
             .format() \
             .option() \
             .load.assert_called_once()
         mock_spark_session.dataframe.DataFrame.write \
             .mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option.assert_called_once_with(constants.HEADER, True)
+            .options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option() \
+            .options() \
             .csv.assert_called_once_with("gs://test")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_json(self, mock_spark_session):
         """Tests BigQueryToGCSTemplate runs with json format output"""
 
         bigquery_to_gcs_template = BigQueryToGCSTemplate()
```

### Comparing `google-dataproc-templates-0.1.0b0/test/cassandra/test_cassandra_to_bq.py` & `google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_bq.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/cassandra/test_cassandra_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigquery.py`

 * *Files 17% similar despite different names*

```diff
@@ -68,17 +68,45 @@
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode().save.assert_called_once()
 
+
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_json(self, mock_spark_session):
+        """Tests GCSToBigqueryTemplate runs with json format"""
+
+        gcs_to_bigquery_template = GCSToBigQueryTemplate()
+        mock_parsed_args = gcs_to_bigquery_template.parse_args(
+            ["--gcs.bigquery.input.format=json",
+             "--gcs.bigquery.output.mode=errorifexists",
+             "--gcs.bigquery.input.location=gs://test",
+             "--gcs.bigquery.output.dataset=dataset",
+             "--gcs.bigquery.output.table=table",
+             "--gcs.bigquery.temp.bucket.name=bucket"])
+        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
+            constants.FORMAT_BIGQUERY)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option.assert_called_once_with(constants.TABLE, "dataset.table")
+        mock_spark_session.dataframe.DataFrame.write.format().option(
+        ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_ERRORIFEXISTS)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().mode().save.assert_called_once()
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_avro(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with parquet avro"""
+        """Tests GCSToBigqueryTemplate runs with avro"""
 
         gcs_to_bigquery_template = GCSToBigQueryTemplate()
         mock_parsed_args = gcs_to_bigquery_template.parse_args(
             ["--gcs.bigquery.input.format=avro",
              "--gcs.bigquery.output.mode=overwrite",
              "--gcs.bigquery.input.location=gs://test",
              "--gcs.bigquery.output.dataset=dataset",
@@ -98,68 +126,112 @@
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode().save.assert_called_once()
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_csv(self, mock_spark_session):
+    def test_run_delta(self, mock_spark_session):
+        """Tests GCSToBigqueryTemplate runs with delta format"""
+
+        gcs_to_bigquery_template = GCSToBigQueryTemplate()
+        mock_parsed_args = gcs_to_bigquery_template.parse_args(
+            ["--gcs.bigquery.input.format=delta",
+             "--gcs.bigquery.output.mode=overwrite",
+             "--gcs.bigquery.input.location=gs://test",
+             "--gcs.bigquery.output.dataset=dataset",
+             "--gcs.bigquery.output.table=table",
+             "--gcs.bigquery.temp.bucket.name=bucket"])
+        mock_spark_session.read.format().load.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_DELTA)
+        mock_spark_session.read.format().load.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
+            constants.FORMAT_BIGQUERY)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option.assert_called_once_with(constants.TABLE, "dataset.table")
+        mock_spark_session.dataframe.DataFrame.write.format().option(
+        ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().mode().save.assert_called_once()
+
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_csv1(self, mock_spark_session):
         """Tests GCSToBigqueryTemplate runs with csv format"""
 
         gcs_to_bigquery_template = GCSToBigQueryTemplate()
         mock_parsed_args = gcs_to_bigquery_template.parse_args(
             ["--gcs.bigquery.input.format=csv",
              "--gcs.bigquery.output.mode=ignore",
              "--gcs.bigquery.input.location=gs://test",
              "--gcs.bigquery.output.dataset=dataset",
              "--gcs.bigquery.output.table=table",
              "--gcs.bigquery.temp.bucket.name=bucket"])
-        mock_spark_session.read.format().option().option(
-        ).load.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_with(
             constants.FORMAT_CSV)
-        mock_spark_session.read.format().option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.format().option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.format().option().option(
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'true',
+            constants.CSV_INFER_SCHEMA: 'true',
+        })
+        mock_spark_session.read.format().options(
         ).load.assert_called_once_with("gs://test")
+
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode().save.assert_called_once()
 
-
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_json(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with json format"""
+    def test_run_csv2(self, mock_spark_session):
+        """Tests GCSToBigqueryTemplate runs with csv format and some optional csv options"""
 
         gcs_to_bigquery_template = GCSToBigQueryTemplate()
         mock_parsed_args = gcs_to_bigquery_template.parse_args(
-            ["--gcs.bigquery.input.format=json",
-             "--gcs.bigquery.output.mode=errorifexists",
+            ["--gcs.bigquery.input.format=csv",
+             "--gcs.bigquery.output.mode=ignore",
              "--gcs.bigquery.input.location=gs://test",
+             "--gcs.bigquery.input.inferschema=false",
+             "--gcs.bigquery.input.sep=|",
+             "--gcs.bigquery.input.comment=#",
+             "--gcs.bigquery.input.timestampntzformat=yyyy-MM-dd'T'HH:mm:ss",
              "--gcs.bigquery.output.dataset=dataset",
              "--gcs.bigquery.output.table=table",
              "--gcs.bigquery.temp.bucket.name=bucket"])
-        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options(
+        ).load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'true',
+            constants.CSV_INFER_SCHEMA: 'false',
+            constants.CSV_SEP: "|",
+            constants.CSV_COMMENT: "#",
+            constants.CSV_TIMESTAMPNTZFORMAT: "yyyy-MM-dd'T'HH:mm:ss",
+        })
+        mock_spark_session.read.format().options(
+        ).load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
-        ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_ERRORIFEXISTS)
+        ).option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().mode().save.assert_called_once()
+
```

### Comparing `google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_gcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from dataproc_templates.gcs.gcs_to_gcs import GCSToGCSTemplate
 import dataproc_templates.util.template_constants as constants
 
 
 class TestGCSToGCSTemplate:
     """
-    Test suite for GCSToBigQueryTemplate
+    Test suite for GCSToGCSTemplate
     """
 
     def test_parse_args(self):
         gcs_to_gcs_template = GCSToGCSTemplate()
         parsed_args = gcs_to_gcs_template.parse_args(
             ["--gcs.to.gcs.input.location=gs://input",
              "--gcs.to.gcs.input.format=csv",
@@ -42,30 +42,30 @@
         assert parsed_args["gcs.to.gcs.input.format"] == "csv"
         assert parsed_args["gcs.to.gcs.temp.view.name"] == "temp"
         assert parsed_args["gcs.to.gcs.sql.query"] == "select * from temp"
         assert parsed_args["gcs.to.gcs.output.format"] == "csv"
         assert parsed_args["gcs.to.gcs.output.mode"] == "overwrite"
         assert parsed_args["gcs.to.gcs.output.partition.column"] == "column"
         assert parsed_args["gcs.to.gcs.output.location"] == "gs://output"
-    
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_parquet(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with parquet format"""
+        """Tests GCSToGCSTemplate runs with parquet format"""
 
         gcs_to_gcs_template = GCSToGCSTemplate()
         mock_parsed_args = gcs_to_gcs_template.parse_args(
             ["--gcs.to.gcs.input.location=gs://input",
              "--gcs.to.gcs.input.format=parquet",
              "--gcs.to.gcs.temp.view.name=temp",
              "--gcs.to.gcs.sql.query=select * from temp",
              "--gcs.to.gcs.output.format=parquet",
              "--gcs.to.gcs.output.mode=overwrite",
              "--gcs.to.gcs.output.partition.column=column",
              "--gcs.to.gcs.output.location=gs://output"])
-        
+
         mock_spark_session.read.parquet.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_gcs_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.parquet.assert_called_once_with("gs://input")
         mock_spark_session.read.parquet().createOrReplaceTempView.assert_called_once_with("temp")
         mock_spark_session.sql.assert_called_once_with("select * from temp")
         mock_spark_session.sql().write \
@@ -73,124 +73,120 @@
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy.assert_called_once_with("column")
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
             .parquet.assert_called_once_with("gs://output")
-            
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_csv(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with parquet format"""
+        """Tests GCSToGCSTemplate runs with parquet format"""
 
         gcs_to_gcs_template = GCSToGCSTemplate()
         mock_parsed_args = gcs_to_gcs_template.parse_args(
             ["--gcs.to.gcs.input.location=gs://input",
              "--gcs.to.gcs.input.format=csv",
              "--gcs.to.gcs.temp.view.name=temp",
              "--gcs.to.gcs.sql.query=select * from temp",
              "--gcs.to.gcs.output.format=csv",
              "--gcs.to.gcs.output.mode=overwrite",
              "--gcs.to.gcs.output.partition.column=column",
              "--gcs.to.gcs.output.location=gs://output"])
-        
+
         mock_spark_session.read.csv.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_gcs_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_once_with(constants.FORMAT_CSV)
         mock_spark_session.read.format() \
-            .option.assert_called_once_with(constants.HEADER, True)
+            .options.assert_called_once_with(**{constants.CSV_HEADER: 'true',
+                                                constants.CSV_INFER_SCHEMA: 'true'})
         mock_spark_session.read.format() \
-            .option() \
-            .option.assert_called_once_with(constants.INFER_SCHEMA, True)
-        mock_spark_session.read.format() \
-            .option() \
-            .option() \
+            .options() \
             .load.assert_called_once_with("gs://input")
         mock_spark_session.read.format() \
-            .option() \
-            .option() \
+            .options() \
             .load() \
             .createOrReplaceTempView.assert_called_once_with("temp")
-            
+
         mock_spark_session.sql.assert_called_once_with("select * from temp")
         mock_spark_session.sql().write \
             .mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy.assert_called_once_with("column")
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
-            .option.assert_called_once_with(constants.HEADER, True)
-            
+            .options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
-            .option() \
+            .options() \
             .csv.assert_called_once_with("gs://output")
-            
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_avro(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with parquet format"""
+        """Tests GCSToGCSTemplate runs with avro format"""
 
         gcs_to_gcs_template = GCSToGCSTemplate()
         mock_parsed_args = gcs_to_gcs_template.parse_args(
             ["--gcs.to.gcs.input.location=gs://input",
              "--gcs.to.gcs.input.format=avro",
              "--gcs.to.gcs.temp.view.name=temp",
              "--gcs.to.gcs.sql.query=select * from temp",
              "--gcs.to.gcs.output.format=avro",
              "--gcs.to.gcs.output.mode=overwrite",
              "--gcs.to.gcs.output.partition.column=column",
              "--gcs.to.gcs.output.location=gs://output"])
-        
+
         mock_spark_session.read.csv.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_gcs_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_once_with(constants.FORMAT_AVRO)
 
         mock_spark_session.read.format() \
             .load.assert_called_once_with("gs://input")
         mock_spark_session.read.format() \
             .load() \
             .createOrReplaceTempView.assert_called_once_with("temp")
-            
+
         mock_spark_session.sql.assert_called_once_with("select * from temp")
         mock_spark_session.sql().write \
             .mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy.assert_called_once_with("column")
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
             .format.assert_called_once_with(constants.FORMAT_AVRO)
-            
+
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
             .format() \
             .save.assert_called_once_with("gs://output")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_json(self, mock_spark_session):
-        """Tests GCSToBigqueryTemplate runs with parquet format"""
+        """Tests GCSToGCSTemplate runs with json format"""
 
         gcs_to_gcs_template = GCSToGCSTemplate()
         mock_parsed_args = gcs_to_gcs_template.parse_args(
             ["--gcs.to.gcs.input.location=gs://input",
              "--gcs.to.gcs.input.format=json",
              "--gcs.to.gcs.temp.view.name=temp",
              "--gcs.to.gcs.sql.query=select * from temp",
              "--gcs.to.gcs.output.format=json",
              "--gcs.to.gcs.output.mode=overwrite",
              "--gcs.to.gcs.output.partition.column=column",
              "--gcs.to.gcs.output.location=gs://output"])
-        
+
         mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_gcs_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.json.assert_called_once_with("gs://input")
         mock_spark_session.read.json().createOrReplaceTempView.assert_called_once_with("temp")
         mock_spark_session.sql.assert_called_once_with("select * from temp")
         mock_spark_session.sql().write \
@@ -198,8 +194,50 @@
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy.assert_called_once_with("column")
         mock_spark_session.sql().write \
             .mode() \
             .partitionBy() \
             .json.assert_called_once_with("gs://output")
-        
+
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_delta(self, mock_spark_session):
+        """Tests GCSToGCSTemplate runs with delta format"""
+
+        gcs_to_gcs_template = GCSToGCSTemplate()
+        mock_parsed_args = gcs_to_gcs_template.parse_args(
+            ["--gcs.to.gcs.input.location=gs://input",
+             "--gcs.to.gcs.input.format=delta",
+             "--gcs.to.gcs.temp.view.name=temp",
+             "--gcs.to.gcs.sql.query=select * from temp",
+             "--gcs.to.gcs.output.format=avro",
+             "--gcs.to.gcs.output.mode=overwrite",
+             "--gcs.to.gcs.output.partition.column=column",
+             "--gcs.to.gcs.output.location=gs://output"])
+
+        mock_spark_session.read.csv.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_gcs_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.format.assert_called_once_with(constants.FORMAT_DELTA)
+
+        mock_spark_session.read.format() \
+            .load.assert_called_once_with("gs://input")
+        mock_spark_session.read.format() \
+            .load() \
+            .createOrReplaceTempView.assert_called_once_with("temp")
+
+        mock_spark_session.sql.assert_called_once_with("select * from temp")
+        mock_spark_session.sql().write \
+            .mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
+        mock_spark_session.sql().write \
+            .mode() \
+            .partitionBy.assert_called_once_with("column")
+        mock_spark_session.sql().write \
+            .mode() \
+            .partitionBy() \
+            .format.assert_called_once_with(constants.FORMAT_AVRO)
+
+        mock_spark_session.sql().write \
+            .mode() \
+            .partitionBy() \
+            .format() \
+            .save.assert_called_once_with("gs://output")
```

### Comparing `google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_jdbc.py` & `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_jdbc.py`

 * *Files 21% similar despite different names*

```diff
@@ -94,64 +94,128 @@
         ).option().option.assert_called_once_with(constants.JDBC_TABLE, "table")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode().save.assert_called_once()
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_csv(self, mock_spark_session):
+    def test_run_json(self, mock_spark_session):
+        """Tests GCSToJDBCTemplate runs with json format"""
+
+        gcs_to_jdbc_template = GCSToJDBCTemplate()
+        mock_parsed_args = gcs_to_jdbc_template.parse_args(
+            ["--gcs.jdbc.input.format=json",
+             "--gcs.jdbc.input.location=gs://test",
+             "--gcs.jdbc.output.url=url",
+             "--gcs.jdbc.output.table=table",
+             "--gcs.jdbc.output.driver=driver",
+             "--gcs.jdbc.output.mode=append"])
+        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_jdbc_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
+            constants.FORMAT_JDBC)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option.assert_called_once_with(constants.JDBC_TABLE, "table")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().option().mode().save.assert_called_once()
+
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_delta(self, mock_spark_session):
+        """Tests GCSToJDBCTemplate runs with delta"""
+
+        gcs_to_jdbc_template = GCSToJDBCTemplate()
+        mock_parsed_args = gcs_to_jdbc_template.parse_args(
+            ["--gcs.jdbc.input.format=delta",
+             "--gcs.jdbc.input.location=gs://test",
+             "--gcs.jdbc.output.url=url",
+             "--gcs.jdbc.output.table=table",
+             "--gcs.jdbc.output.driver=driver",
+             "--gcs.jdbc.output.mode=append"])
+        mock_spark_session.read.format().load.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_jdbc_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_DELTA)
+        mock_spark_session.read.format().load.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
+            constants.FORMAT_JDBC)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option.assert_called_once_with(constants.JDBC_TABLE, "table")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().option().mode().save.assert_called_once()
+
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_csv1(self, mock_spark_session):
         """Tests GCSToJDBCTemplate runs with csv format"""
 
         gcs_to_jdbc_template = GCSToJDBCTemplate()
         mock_parsed_args = gcs_to_jdbc_template.parse_args(
             ["--gcs.jdbc.input.format=csv",
              "--gcs.jdbc.input.location=gs://test",
+             "--gcs.jdbc.input.header=false",
              "--gcs.jdbc.output.url=url",
              "--gcs.jdbc.output.table=table",
              "--gcs.jdbc.output.driver=driver",
              "--gcs.jdbc.output.mode=append"])
-        mock_spark_session.read.format().option().option(
-        ).load.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_jdbc_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_with(
             constants.FORMAT_CSV)
-        mock_spark_session.read.format().option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.format().option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.format().option().option(
-        ).load.assert_called_once_with("gs://test")
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'false',
+            constants.CSV_INFER_SCHEMA: 'true',
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_JDBC)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option.assert_called_once_with(constants.JDBC_TABLE, "table")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode().save.assert_called_once()
 
-
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_json(self, mock_spark_session):
-        """Tests GCSToJDBCTemplate runs with json format"""
+    def test_run_csv2(self, mock_spark_session):
+        """Tests GCSToJDBCTemplate runs with csv format and some optional csv options"""
 
         gcs_to_jdbc_template = GCSToJDBCTemplate()
         mock_parsed_args = gcs_to_jdbc_template.parse_args(
-            ["--gcs.jdbc.input.format=json",
+            ["--gcs.jdbc.input.format=csv",
              "--gcs.jdbc.input.location=gs://test",
+             "--gcs.jdbc.input.inferschema=false",
+             "--gcs.jdbc.input.sep=|",
+             "--gcs.jdbc.input.comment=#",
+             "--gcs.jdbc.input.timestampntzformat=yyyy-MM-dd'T'HH:mm:ss",
              "--gcs.jdbc.output.url=url",
              "--gcs.jdbc.output.table=table",
              "--gcs.jdbc.output.driver=driver",
              "--gcs.jdbc.output.mode=append"])
-        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_jdbc_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'true',
+            constants.CSV_INFER_SCHEMA: 'false',
+            constants.CSV_SEP: "|",
+            constants.CSV_COMMENT: "#",
+            constants.CSV_TIMESTAMPNTZFORMAT: "yyyy-MM-dd'T'HH:mm:ss",
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_JDBC)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option.assert_called_once_with(constants.JDBC_TABLE, "table")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().option().mode().save.assert_called_once()
+
```

### Comparing `google-dataproc-templates-0.1.0b0/test/gcs/test_gcs_to_mongo.py` & `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,98 +100,139 @@
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode().save.assert_called_once()
 
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_avro(self, mock_spark_session):
-        """Tests GCSToMONGOTemplate runs with avro"""
+    def test_run_delta(self, mock_spark_session):
+        """Tests GCSToMONGOTemplate runs with delta"""
 
         gcs_to_mongo_template = GCSToMONGOTemplate()
         mock_parsed_args = gcs_to_mongo_template.parse_args(
-            ["--gcs.mongo.input.format=avro",
+            ["--gcs.mongo.input.format=delta",
              "--gcs.mongo.input.location=gs://test",
              "--gcs.mongo.output.uri=uri",
              "--gcs.mongo.output.database=database",
              "--gcs.mongo.output.collection=collection",
              "--gcs.mongo.output.mode=append"])
         mock_spark_session.read.format().load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_mongo_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_with(
-            constants.FORMAT_AVRO_EXTD)
+            constants.FORMAT_DELTA)
         mock_spark_session.read.format().load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_MONGO)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option.assert_called_once_with(constants.MONGO_DATABASE, "database")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option.assert_called_once_with(constants.MONGO_COLLECTION, "collection")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode().save.assert_called_once()
 
+    @mock.patch.object(pyspark.sql, 'SparkSession')
+    def test_run_json(self, mock_spark_session):
+        """Tests GCSToMONGOTemplate runs with json format"""
+
+        gcs_to_mongo_template = GCSToMONGOTemplate()
+        mock_parsed_args = gcs_to_mongo_template.parse_args(
+            ["--gcs.mongo.input.format=json",
+             "--gcs.mongo.input.location=gs://test",
+             "--gcs.mongo.output.uri=uri",
+             "--gcs.mongo.output.database=database",
+             "--gcs.mongo.output.collection=collection",
+             "--gcs.mongo.output.mode=append"])
+        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        gcs_to_mongo_template.run(mock_spark_session, mock_parsed_args)
+
+        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
+            constants.FORMAT_MONGO)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option.assert_called_once_with(constants.MONGO_DATABASE, "database")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option.assert_called_once_with(constants.MONGO_COLLECTION, "collection")
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
+        mock_spark_session.dataframe.DataFrame.write.format(
+        ).option().option().option().option().mode().save.assert_called_once()
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_csv(self, mock_spark_session):
+    def test_run_csv1(self, mock_spark_session):
         """Tests GCSToMONGOTemplate runs with csv format"""
 
         gcs_to_mongo_template = GCSToMONGOTemplate()
         mock_parsed_args = gcs_to_mongo_template.parse_args(
             ["--gcs.mongo.input.format=csv",
              "--gcs.mongo.input.location=gs://test",
+             "--gcs.mongo.input.header=false",
              "--gcs.mongo.output.uri=uri",
              "--gcs.mongo.output.database=database",
              "--gcs.mongo.output.collection=collection",
              "--gcs.mongo.output.mode=append"])
-        mock_spark_session.read.format().option().option(
+        mock_spark_session.read.format().options(
         ).load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_mongo_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.read.format.assert_called_with(
             constants.FORMAT_CSV)
-        mock_spark_session.read.format().option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.format().option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.format().option().option(
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'false',
+            constants.CSV_INFER_SCHEMA: 'true',
+        })
+        mock_spark_session.read.format().options(
         ).load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_MONGO)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option.assert_called_once_with(constants.MONGO_DATABASE, "database")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option.assert_called_once_with(constants.MONGO_COLLECTION, "collection")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode().save.assert_called_once()
 
-
     @mock.patch.object(pyspark.sql, 'SparkSession')
-    def test_run_json(self, mock_spark_session):
-        """Tests GCSToMONGOTemplate runs with json format"""
+    def test_run_csv2(self, mock_spark_session):
+        """Tests GCSToMONGOTemplate runs with csv format and some optional csv options"""
 
         gcs_to_mongo_template = GCSToMONGOTemplate()
         mock_parsed_args = gcs_to_mongo_template.parse_args(
-            ["--gcs.mongo.input.format=json",
+            ["--gcs.mongo.input.format=csv",
              "--gcs.mongo.input.location=gs://test",
+             "--gcs.mongo.input.inferschema=false",
+             "--gcs.mongo.input.sep=|",
+             "--gcs.mongo.input.comment=#",
+             "--gcs.mongo.input.timestampntzformat=yyyy-MM-dd'T'HH:mm:ss",
              "--gcs.mongo.output.uri=uri",
              "--gcs.mongo.output.database=database",
              "--gcs.mongo.output.collection=collection",
              "--gcs.mongo.output.mode=append"])
-        mock_spark_session.read.json.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options(
+        ).load.return_value = mock_spark_session.dataframe.DataFrame
         gcs_to_mongo_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.json.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'true',
+            constants.CSV_INFER_SCHEMA: 'false',
+            constants.CSV_SEP: "|",
+            constants.CSV_COMMENT: "#",
+            constants.CSV_TIMESTAMPNTZFORMAT: "yyyy-MM-dd'T'HH:mm:ss",
+        })
+        mock_spark_session.read.format().options(
+        ).load.assert_called_once_with("gs://test")
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_MONGO)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option.assert_called_once_with(constants.MONGO_DATABASE, "database")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option.assert_called_once_with(constants.MONGO_COLLECTION, "collection")
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option().option().option().option().mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.format(
-        ).option().option().option().option().mode().save.assert_called_once()
+        ).option().option().option().option().mode().save.assert_called_once()
```

### Comparing `google-dataproc-templates-0.1.0b0/test/gcs/test_text_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/test/gcs/test_text_to_bigquery.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,52 +33,51 @@
         parsed_args = text_to_bigquery_template.parse_args(
             ["--text.bigquery.input.compression=bzip2",
              "--text.bigquery.output.mode=append",
              "--text.bigquery.input.location=gs://test",
              "--text.bigquery.output.dataset=dataset",
              "--text.bigquery.output.table=table",
              "--text.bigquery.temp.bucket.name=bucket",
-             "--text.bigquery.input.delimiter=|"])
+             "--text.bigquery.input.sep=|"])
 
         assert parsed_args["text.bigquery.input.compression"] == "bzip2"
         assert parsed_args["text.bigquery.output.mode"] == "append"
         assert parsed_args["text.bigquery.input.location"] == "gs://test"
         assert parsed_args["text.bigquery.output.dataset"] == "dataset"
         assert parsed_args["text.bigquery.output.table"] == "table"
         assert parsed_args["text.bigquery.temp.bucket.name"] == "bucket"
-        assert parsed_args["text.bigquery.input.delimiter"] == "|"
+        assert parsed_args["text.bigquery.input.sep"] == "|"
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_bzip2(self, mock_spark_session):
         """Tests TextToBigqueryTemplate runs with | delimiter and bzip2 compression format"""
 
         text_to_bigquery_template = TextToBigQueryTemplate()
         mock_parsed_args = text_to_bigquery_template.parse_args(
             ["--text.bigquery.input.location=gs://test",
+             "--text.bigquery.input.header=false",
              "--text.bigquery.output.dataset=dataset",
              "--text.bigquery.output.table=table",
              "--text.bigquery.input.compression=bzip2",
              "--text.bigquery.temp.bucket.name=bucket",
              "--text.bigquery.output.mode=ignore",
-             "--text.bigquery.input.delimiter=|"])
+             "--text.bigquery.input.sep=|"])
 
-        mock_spark_session.read.option().option().option(
-        ).option().csv.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         text_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.option().option().option.assert_called_with(
-            constants.INPUT_COMPRESSION, constants.COMPRESSION_BZIP2)
-        mock_spark_session.read.option().option().option().option.assert_called_with(
-            constants.INPUT_DELIMITER, "|")
-        mock_spark_session.read.option().option().option(
-        ).option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'false',
+            constants.CSV_INFER_SCHEMA: 'true',
+            constants.CSV_SEP: "|",
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
+
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
@@ -89,35 +88,38 @@
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_lz4(self, mock_spark_session):
         """Tests TextToBigqueryTemplate runs with | delimiter and lz4 compression format"""
 
         text_to_bigquery_template = TextToBigQueryTemplate()
         mock_parsed_args = text_to_bigquery_template.parse_args(
             ["--text.bigquery.input.location=gs://test",
+             "--text.bigquery.input.header=false",
+             "--text.bigquery.input.compression=lz4",
+             "--text.bigquery.input.comment=#",
+             "--text.bigquery.input.timestampntzformat=yyyy-MM-dd'T'HH:mm:ss",
              "--text.bigquery.output.dataset=dataset",
              "--text.bigquery.output.table=table",
-             "--text.bigquery.input.compression=lz4",
              "--text.bigquery.temp.bucket.name=bucket",
              "--text.bigquery.output.mode=ignore",
-             "--text.bigquery.input.delimiter=|"])
+             "--text.bigquery.input.sep=|"])
 
-        mock_spark_session.read.option().option().option(
-        ).option().csv.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         text_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.option().option().option.assert_called_with(
-            constants.INPUT_COMPRESSION, constants.COMPRESSION_LZ4)
-        mock_spark_session.read.option().option().option().option.assert_called_with(
-            constants.INPUT_DELIMITER, "|")
-        mock_spark_session.read.option().option().option(
-        ).option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'false',
+            constants.CSV_INFER_SCHEMA: 'true',
+            constants.CSV_SEP: "|",
+            constants.CSV_COMMENT: "#",
+            constants.CSV_TIMESTAMPNTZFORMAT: "yyyy-MM-dd'T'HH:mm:ss",
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
+
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
@@ -128,35 +130,36 @@
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_deflate(self, mock_spark_session):
         """Tests TextToBigqueryTemplate runs with | delimiter and deflate compression format"""
 
         text_to_bigquery_template = TextToBigQueryTemplate()
         mock_parsed_args = text_to_bigquery_template.parse_args(
             ["--text.bigquery.input.location=gs://test",
+             "--text.bigquery.input.header=false",
+             "--text.bigquery.input.compression=deflate",
+             "--text.bigquery.input.mode=FAILFAST",
              "--text.bigquery.output.dataset=dataset",
              "--text.bigquery.output.table=table",
-             "--text.bigquery.input.compression=deflate",
              "--text.bigquery.temp.bucket.name=bucket",
              "--text.bigquery.output.mode=ignore",
-             "--text.bigquery.input.delimiter=|"])
+             "--text.bigquery.input.sep=|"])
 
-        mock_spark_session.read.option().option().option(
-        ).option().csv.return_value = mock_spark_session.dataframe.DataFrame
+        mock_spark_session.read.format().options().load.return_value = mock_spark_session.dataframe.DataFrame
         text_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.option().option().option.assert_called_with(
-            constants.INPUT_COMPRESSION, constants.COMPRESSION_DEFLATE)
-        mock_spark_session.read.option().option().option().option.assert_called_with(
-            constants.INPUT_DELIMITER, "|")
-        mock_spark_session.read.option().option().option(
-        ).option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'false',
+            constants.CSV_INFER_SCHEMA: 'true',
+            constants.CSV_MODE: 'FAILFAST',
+            constants.CSV_SEP: "|",
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
+
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
@@ -167,35 +170,37 @@
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_gzip(self, mock_spark_session):
         """Tests TextToBigqueryTemplate runs with | delimiter and gzip compression format"""
 
         text_to_bigquery_template = TextToBigQueryTemplate()
         mock_parsed_args = text_to_bigquery_template.parse_args(
             ["--text.bigquery.input.location=gs://test",
+             "--text.bigquery.input.maxcolumns=100",
+             "--text.bigquery.input.maxcharspercolumn=64",
+             "--text.bigquery.input.compression=gzip",
              "--text.bigquery.output.dataset=dataset",
              "--text.bigquery.output.table=table",
-             "--text.bigquery.input.compression=gzip",
              "--text.bigquery.temp.bucket.name=bucket",
              "--text.bigquery.output.mode=ignore",
-             "--text.bigquery.input.delimiter=|"])
-
-        mock_spark_session.read.option().option().option(
-        ).option().csv.return_value = mock_spark_session.dataframe.DataFrame
+             "--text.bigquery.input.sep=|"])
+        mock_spark_session.read.format().options(
+        ).load.return_value = mock_spark_session.dataframe.DataFrame
         text_to_bigquery_template.run(mock_spark_session, mock_parsed_args)
 
-        mock_spark_session.read.option.assert_called_with(
-            constants.HEADER, True)
-        mock_spark_session.read.option().option.assert_called_with(
-            constants.INFER_SCHEMA, True)
-        mock_spark_session.read.option().option().option.assert_called_with(
-            constants.INPUT_COMPRESSION, constants.COMPRESSION_GZIP)
-        mock_spark_session.read.option().option().option().option.assert_called_with(
-            constants.INPUT_DELIMITER, "|")
-        mock_spark_session.read.option().option().option(
-        ).option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.read.format.assert_called_with(
+            constants.FORMAT_CSV)
+        mock_spark_session.read.format().options.assert_called_with(**{
+            constants.CSV_HEADER: 'true',
+            constants.CSV_INFER_SCHEMA: 'true',
+            constants.CSV_MAXCOLUMNS: '100',
+            constants.CSV_MAXCHARSPERCOLUMN: '64',
+            constants.CSV_SEP: "|",
+        })
+        mock_spark_session.read.format().options().load.assert_called_once_with("gs://test")
+
         mock_spark_session.dataframe.DataFrame.write.format.assert_called_once_with(
             constants.FORMAT_BIGQUERY)
         mock_spark_session.dataframe.DataFrame.write.format(
         ).option.assert_called_once_with(constants.TABLE, "dataset.table")
         mock_spark_session.dataframe.DataFrame.write.format().option(
         ).option.assert_called_once_with(constants.GCS_BQ_TEMP_BUCKET, "bucket")
         mock_spark_session.dataframe.DataFrame.write.format(
```

### Comparing `google-dataproc-templates-0.1.0b0/test/hbase/test_hbase_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/hbase/test_hbase_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/hive/test_hive_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/hive/test_hive_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,18 @@
         hive_to_gcs_template.run(mock_spark_session, mock_parsed_args)
 
         mock_spark_session.table.assert_called_once_with("database.table")
         mock_spark_session.dataframe.DataFrame.write \
             .mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option.assert_called_once_with(constants.HEADER, True)
+            .options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option() \
+            .options() \
             .csv.assert_called_once_with("gs://test")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_json(self, mock_spark_session):
         """Tests HiveToGCSTemplate runs with json format output"""
 
         hive_to_gcs_template = HiveToGCSTemplate()
```

### Comparing `google-dataproc-templates-0.1.0b0/test/hive/util/test_hive_ddl_extractor.py` & `google-dataproc-templates-0.2.0b0/test/hive/util/test_hive_ddl_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
 """
 
-import dataproc_templates.util.template_constants as constants
+
 import mock
 import pyspark
 from dataproc_templates.hive.util.hive_ddl_extractor import \
     HiveDDLExtractorTemplate
 from datetime import datetime
 
 class TestHiveDDLExtractorTemplate:
```

### Comparing `google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,16 +166,16 @@
             constants.JDBC_LOWERBOUND: "1",
             constants.JDBC_UPPERBOUND: "2",
             constants.JDBC_NUMPARTITIONS: "5",
             constants.JDBC_FETCHSIZE: 0
         })
         mock_spark_session.read.format().options().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
-        mock_spark_session.dataframe.DataFrame.write.mode().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.mode().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().options().csv.assert_called_once_with("gs://test")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args5(self, mock_spark_session):
         """Tests JDBCToGCSTemplate write json"""
 
         jdbc_to_gcs_template = JDBCToGCSTemplate()
 
@@ -230,16 +230,16 @@
             constants.JDBC_DRIVER: "driver",
             constants.JDBC_TABLE: "table1",
             constants.JDBC_NUMPARTITIONS: "10",
             constants.JDBC_FETCHSIZE: 0
         })
         mock_spark_session.read.format().options().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
-        mock_spark_session.dataframe.DataFrame.write.mode().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.mode().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().options().csv.assert_called_once_with("gs://test")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args7(self, mock_spark_session):
         """Tests JDBCToGCSTemplate pass args"""
 
         jdbc_to_gcs_template = JDBCToGCSTemplate()
 
@@ -262,9 +262,9 @@
             constants.JDBC_TABLE: "table1",
             constants.JDBC_NUMPARTITIONS: "10",
             constants.JDBC_FETCHSIZE: 0
         })
         mock_spark_session.read.format().options().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.mode().partitionBy.assert_called_once_with("column")
-        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().options().csv.assert_called_once_with("gs://test")
```

### Comparing `google-dataproc-templates-0.1.0b0/test/jdbc/test_jdbc_to_jdbc.py` & `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.1.0b0/test/mongo/test_mongo_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/mongo/test_mongo_to_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,18 +160,18 @@
             .option() \
             .option() \
             .load.assert_called_with()
         mock_spark_session.dataframe.DataFrame.write \
             .mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option.assert_called_once_with(constants.HEADER, True)
+            .options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
         mock_spark_session.dataframe.DataFrame.write \
             .mode() \
-            .option() \
+            .options() \
             .csv.assert_called_once_with("gs://test")
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_json(self, mock_spark_session):
         """Tests MongoToGCSTemplate runs for json format output"""
 
         mongo_to_gcs_template = MongoToGCSTemplate()
```

### Comparing `google-dataproc-templates-0.1.0b0/test/redshift/test_redshift_to_gcs.py` & `google-dataproc-templates-0.2.0b0/test/redshift/test_redshift_to_gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,26 @@
              "--redshifttogcs.iam.rolearn=arn:aws:iam::xxxx:role/role",
              "--redshifttogcs.s3.accesskey=xyz",
              "--redshifttogcs.s3.secretkey=lmn",
              "--redshifttogcs.output.location=gs://test",
              "--redshifttogcs.output.format=csv",
              "--redshifttogcs.output.mode=append",
              "--redshifttogcs.output.partitioncolumn=column"
-             ])       
-        
+             ])
+
         assert parsed_args["redshifttogcs.input.url"] == "url"
         assert parsed_args["redshifttogcs.s3.tempdir"] == "s3a://temp"
         assert parsed_args["redshifttogcs.input.table"] == "table1"
         assert parsed_args["redshifttogcs.iam.rolearn"] == "arn:aws:iam::xxxx:role/role"
         assert parsed_args["redshifttogcs.s3.accesskey"] == "xyz"
         assert parsed_args["redshifttogcs.s3.secretkey"] == "lmn"
         assert parsed_args["redshifttogcs.output.location"] == "gs://test"
         assert parsed_args["redshifttogcs.output.format"] == "csv"
-        assert parsed_args["redshifttogcs.output.mode"] == "append"  
-        assert parsed_args["redshifttogcs.output.partitioncolumn"] == "column"      
+        assert parsed_args["redshifttogcs.output.mode"] == "append"
+        assert parsed_args["redshifttogcs.output.partitioncolumn"] == "column"
 
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args2(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate write parquet"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
@@ -79,15 +79,15 @@
         mock_spark_session.read.format().option.assert_called_with(constants.JDBC_URL, "url")
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_OVERWRITE)
         mock_spark_session.dataframe.DataFrame.write.mode().parquet.assert_called_once_with("gs://test")
-        
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args3(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate write avro"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
         mock_parsed_args = redshift_to_gcs_template.parse_args(
@@ -108,15 +108,15 @@
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.mode().format.assert_called_once_with(constants.FORMAT_AVRO)
         mock_spark_session.dataframe.DataFrame.write.mode().format().save.assert_called_once_with("gs://test")
-        
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args4(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate write csv"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
         mock_parsed_args = redshift_to_gcs_template.parse_args(
@@ -135,17 +135,17 @@
         mock_spark_session.read.format.assert_called_with(constants.FORMAT_REDSHIFT)
         mock_spark_session.read.format().option.assert_called_with(constants.JDBC_URL, "url")
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
-        mock_spark_session.dataframe.DataFrame.write.mode().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().option().csv.assert_called_once_with("gs://test")
-        
+        mock_spark_session.dataframe.DataFrame.write.mode().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().options().csv.assert_called_once_with("gs://test")
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args5(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate write json"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
         mock_parsed_args = redshift_to_gcs_template.parse_args(
@@ -165,15 +165,15 @@
         mock_spark_session.read.format().option.assert_called_with(constants.JDBC_URL, "url")
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_IGNORE)
         mock_spark_session.dataframe.DataFrame.write.mode().json.assert_called_once_with("gs://test")
-        
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args6(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate pass args"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
         mock_parsed_args = redshift_to_gcs_template.parse_args(
@@ -192,17 +192,17 @@
         mock_spark_session.read.format.assert_called_with(constants.FORMAT_REDSHIFT)
         mock_spark_session.read.format().option.assert_called_with(constants.JDBC_URL, "url")
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
-        mock_spark_session.dataframe.DataFrame.write.mode().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().option().csv.assert_called_once_with("gs://test")
-        
+        mock_spark_session.dataframe.DataFrame.write.mode().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().options().csv.assert_called_once_with("gs://test")
+
     @mock.patch.object(pyspark.sql, 'SparkSession')
     def test_run_pass_args7(self, mock_spark_session):
         """Tests RedshiftToGCSTemplate pass args"""
 
         redshift_to_gcs_template = RedshiftToGCSTemplate()
 
         mock_parsed_args = redshift_to_gcs_template.parse_args(
@@ -223,9 +223,9 @@
         mock_spark_session.read.format().option.assert_called_with(constants.JDBC_URL, "url")
         mock_spark_session.read.format().option().option.assert_called_with(constants.JDBC_TABLE, "table1")
         mock_spark_session.read.format().option().option().option.assert_called_with(constants.REDSHIFT_TEMPDIR, "s3a://temp")
         mock_spark_session.read.format().option().option().option().option.assert_called_with(constants.REDSHIFT_IAMROLE, "arn:aws:iam::xxxx:role/role")
         mock_spark_session.read.format().option().option().option().option().load()
         mock_spark_session.dataframe.DataFrame.write.mode.assert_called_once_with(constants.OUTPUT_MODE_APPEND)
         mock_spark_session.dataframe.DataFrame.write.mode().partitionBy.assert_called_once_with("column")
-        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().option.assert_called_once_with(constants.HEADER, True)
-        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().option().csv.assert_called_once_with("gs://test")
+        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().options.assert_called_once_with(**{constants.CSV_HEADER: 'true'})
+        mock_spark_session.dataframe.DataFrame.write.mode().partitionBy().options().csv.assert_called_once_with("gs://test")
```

### Comparing `google-dataproc-templates-0.1.0b0/test/s3/test_s3_to_bigquery.py` & `google-dataproc-templates-0.2.0b0/test/s3/test_s3_to_bigquery.py`

 * *Files identical despite different names*

