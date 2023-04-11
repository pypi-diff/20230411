# Comparing `tmp/cdk-extensions-0.0.50.tar.gz` & `tmp/cdk-extensions-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.50.tar", last modified: Tue Apr 11 13:58:45 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.51.tar", last modified: Tue Apr 11 15:18:13 2023, max compression
```

## Comparing `cdk-extensions-0.0.50.tar` & `cdk-extensions-0.0.51.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.113065 cdk-extensions-0.0.50/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.117065 cdk-extensions-0.0.50/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1483078 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/_jsii/cdk-extensions@0.0.50.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   621775 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   138026 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.125065 cdk-extensions-0.0.50/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.129065 cdk-extensions-0.0.50/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-11 13:58:30.000000 cdk-extensions-0.0.50/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:58:45.121065 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 13:58:45.000000 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 13:58:45.000000 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:58:45.000000 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 13:58:45.000000 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 13:58:45.000000 cdk-extensions-0.0.50/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.298952 cdk-extensions-0.0.51/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.302953 cdk-extensions-0.0.51/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.302953 cdk-extensions-0.0.51/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.302953 cdk-extensions-0.0.51/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1484223 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/_jsii/cdk-extensions@0.0.51.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   621775 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   153560 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.306953 cdk-extensions-0.0.51/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.310953 cdk-extensions-0.0.51/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-11 15:17:59.000000 cdk-extensions-0.0.51/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:13.302953 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 15:18:13.000000 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 15:18:13.000000 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:18:13.000000 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 15:18:13.000000 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 15:18:13.000000 cdk-extensions-0.0.51/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.50/LICENSE` & `cdk-extensions-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/PKG-INFO` & `cdk-extensions-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.50
+Version: 0.0.51
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.50/README.md` & `cdk-extensions-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/setup.py` & `cdk-extensions-0.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.50",
+    "version": "0.0.51",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -43,15 +43,15 @@
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.50.jsii.tgz"
+            "cdk-extensions@0.0.51.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,48 @@
 from ..ram import (
     ISharedPrincipal as _ISharedPrincipal_9cde791b,
     ResourceShare as _ResourceShare_f0180713,
 )
 
 
 @jsii.data_type(
+    jsii_type="cdk-extensions.ec2_patterns.AddNetworkOptions",
+    jsii_struct_bases=[],
+    name_mapping={"netmask": "netmask"},
+)
+class AddNetworkOptions:
+    def __init__(self, *, netmask: typing.Optional[jsii.Number] = None) -> None:
+        '''
+        :param netmask: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__24d3c1346e4e259fee32303499f123223b892ff23852cdfdf5a57bf21cad7680)
+            check_type(argname="argument netmask", value=netmask, expected_type=type_hints["netmask"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if netmask is not None:
+            self._values["netmask"] = netmask
+
+    @builtins.property
+    def netmask(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("netmask")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "AddNetworkOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.AddPoolOptions",
     jsii_struct_bases=[],
     name_mapping={"cidrs": "cidrs", "default_netmask_length": "defaultNetmaskLength"},
 )
 class AddPoolOptions:
     def __init__(
         self,
@@ -2055,14 +2089,252 @@
 
     def __repr__(self) -> str:
         return "IpAddressManagerSharingProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class NetworkController(
+    _aws_cdk_ceddda9d.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="cdk-extensions.ec2_patterns.NetworkController",
+):
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.IConstruct,
+        id: builtins.str,
+        *,
+        default_netmask: typing.Optional[jsii.Number] = None,
+        account: typing.Optional[builtins.str] = None,
+        environment_from_arn: typing.Optional[builtins.str] = None,
+        physical_name: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param default_netmask: 
+        :param account: The AWS account ID this resource belongs to. Default: - the resource is in the same account as the stack it belongs to
+        :param environment_from_arn: ARN to deduce region and account from. The ARN is parsed and the account and region are taken from the ARN. This should be used for imported resources. Cannot be supplied together with either ``account`` or ``region``. Default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        :param physical_name: The value passed in by users to the physical name prop of the resource. - ``undefined`` implies that a physical name will be allocated by CloudFormation during deployment. - a concrete value implies a specific physical name - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation. Default: - The physical name will be allocated by CloudFormation at deployment time
+        :param region: The AWS region this resource belongs to. Default: - the resource is in the same region as the stack it belongs to
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d930e3de8c120c3fc5f5c70030691aa4f52aa6e26d49c32535c5bce5c960935e)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = NetworkControllerProps(
+            default_netmask=default_netmask,
+            account=account,
+            environment_from_arn=environment_from_arn,
+            physical_name=physical_name,
+            region=region,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="addHub")
+    def add_hub(
+        self,
+        scope: _constructs_77d1e7e8.IConstruct,
+        id: builtins.str,
+        *,
+        netmask: typing.Optional[jsii.Number] = None,
+    ) -> FourTierNetworkHub:
+        '''
+        :param scope: -
+        :param id: -
+        :param netmask: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__74ba1ec928c092f33aeb546fda189638c35c356996133e040cb167d089e3f343)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddNetworkOptions(netmask=netmask)
+
+        return typing.cast(FourTierNetworkHub, jsii.invoke(self, "addHub", [scope, id, options]))
+
+    @jsii.member(jsii_name="addSpoke")
+    def add_spoke(
+        self,
+        scope: _constructs_77d1e7e8.IConstruct,
+        id: builtins.str,
+        *,
+        netmask: typing.Optional[jsii.Number] = None,
+    ) -> FourTierNetworkSpoke:
+        '''
+        :param scope: -
+        :param id: -
+        :param netmask: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f39726d5378c607c7d2408b015e8aed7d5f87a4d39b2235dbde97aa46e8daba2)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddNetworkOptions(netmask=netmask)
+
+        return typing.cast(FourTierNetworkSpoke, jsii.invoke(self, "addSpoke", [scope, id, options]))
+
+    @jsii.member(jsii_name="registerAccount")
+    def _register_account(self, account: builtins.str) -> None:
+        '''
+        :param account: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7a94042b91cf18ea51b81a0607a52121519d15828b001d7f2a7c825c4dc5c4f9)
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+        return typing.cast(None, jsii.invoke(self, "registerAccount", [account]))
+
+    @jsii.member(jsii_name="registerRegion")
+    def _register_region(self, region: builtins.str) -> None:
+        '''
+        :param region: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9ea0364f3254929215baedf3bfe5eb8fb59ce1151f770db5cfc4eb7f7dd9754c)
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+        return typing.cast(None, jsii.invoke(self, "registerRegion", [region]))
+
+    @builtins.property
+    @jsii.member(jsii_name="addressManager")
+    def address_manager(self) -> IpAddressManager:
+        return typing.cast(IpAddressManager, jsii.get(self, "addressManager"))
+
+    @builtins.property
+    @jsii.member(jsii_name="defaultNetmask")
+    def default_netmask(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "defaultNetmask"))
+
+    @builtins.property
+    @jsii.member(jsii_name="globalNetwork")
+    def global_network(self) -> _GlobalNetwork_79ec647c:
+        return typing.cast(_GlobalNetwork_79ec647c, jsii.get(self, "globalNetwork"))
+
+    @builtins.property
+    @jsii.member(jsii_name="registeredAccounts")
+    def registered_accounts(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "registeredAccounts"))
+
+    @builtins.property
+    @jsii.member(jsii_name="registeredRegions")
+    def registered_regions(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "registeredRegions"))
+
+
+@jsii.data_type(
+    jsii_type="cdk-extensions.ec2_patterns.NetworkControllerProps",
+    jsii_struct_bases=[_aws_cdk_ceddda9d.ResourceProps],
+    name_mapping={
+        "account": "account",
+        "environment_from_arn": "environmentFromArn",
+        "physical_name": "physicalName",
+        "region": "region",
+        "default_netmask": "defaultNetmask",
+    },
+)
+class NetworkControllerProps(_aws_cdk_ceddda9d.ResourceProps):
+    def __init__(
+        self,
+        *,
+        account: typing.Optional[builtins.str] = None,
+        environment_from_arn: typing.Optional[builtins.str] = None,
+        physical_name: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+        default_netmask: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param account: The AWS account ID this resource belongs to. Default: - the resource is in the same account as the stack it belongs to
+        :param environment_from_arn: ARN to deduce region and account from. The ARN is parsed and the account and region are taken from the ARN. This should be used for imported resources. Cannot be supplied together with either ``account`` or ``region``. Default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        :param physical_name: The value passed in by users to the physical name prop of the resource. - ``undefined`` implies that a physical name will be allocated by CloudFormation during deployment. - a concrete value implies a specific physical name - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation. Default: - The physical name will be allocated by CloudFormation at deployment time
+        :param region: The AWS region this resource belongs to. Default: - the resource is in the same region as the stack it belongs to
+        :param default_netmask: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1eee37f6e80a88db3d1de97179d49c53732c2177cd8790b1b68e521aa37f3e9d)
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+            check_type(argname="argument environment_from_arn", value=environment_from_arn, expected_type=type_hints["environment_from_arn"])
+            check_type(argname="argument physical_name", value=physical_name, expected_type=type_hints["physical_name"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument default_netmask", value=default_netmask, expected_type=type_hints["default_netmask"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if account is not None:
+            self._values["account"] = account
+        if environment_from_arn is not None:
+            self._values["environment_from_arn"] = environment_from_arn
+        if physical_name is not None:
+            self._values["physical_name"] = physical_name
+        if region is not None:
+            self._values["region"] = region
+        if default_netmask is not None:
+            self._values["default_netmask"] = default_netmask
+
+    @builtins.property
+    def account(self) -> typing.Optional[builtins.str]:
+        '''The AWS account ID this resource belongs to.
+
+        :default: - the resource is in the same account as the stack it belongs to
+        '''
+        result = self._values.get("account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def environment_from_arn(self) -> typing.Optional[builtins.str]:
+        '''ARN to deduce region and account from.
+
+        The ARN is parsed and the account and region are taken from the ARN.
+        This should be used for imported resources.
+
+        Cannot be supplied together with either ``account`` or ``region``.
+
+        :default: - take environment from ``account``, ``region`` parameters, or use Stack environment.
+        '''
+        result = self._values.get("environment_from_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def physical_name(self) -> typing.Optional[builtins.str]:
+        '''The value passed in by users to the physical name prop of the resource.
+
+        - ``undefined`` implies that a physical name will be allocated by
+          CloudFormation during deployment.
+        - a concrete value implies a specific physical name
+        - ``PhysicalName.GENERATE_IF_NEEDED`` is a marker that indicates that a physical will only be generated
+          by the CDK if it is needed for cross-environment references. Otherwise, it will be allocated by CloudFormation.
+
+        :default: - The physical name will be allocated by CloudFormation at deployment time
+        '''
+        result = self._values.get("physical_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def region(self) -> typing.Optional[builtins.str]:
+        '''The AWS region this resource belongs to.
+
+        :default: - the resource is in the same region as the stack it belongs to
+        '''
+        result = self._values.get("region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def default_netmask(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("default_netmask")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "NetworkControllerProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.TransitGatewayHubConfiguration",
     jsii_struct_bases=[],
     name_mapping={
         "allow_external": "allowExternal",
         "auto_accept_shared_attachments": "autoAcceptSharedAttachments",
         "auto_discovery": "autoDiscovery",
@@ -2230,34 +2502,44 @@
     def __repr__(self) -> str:
         return "TransitGatewaySpokeConfiguration(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "AddNetworkOptions",
     "AddPoolOptions",
     "AddSpokeNetworkProps",
     "AllocatePrivateNetworkOptions",
     "FlowLogOptions",
     "FourTierNetwork",
     "FourTierNetworkHub",
     "FourTierNetworkHubProps",
     "FourTierNetworkProps",
     "FourTierNetworkShareProperties",
     "FourTierNetworkSpoke",
     "FourTierNetworkSpokeProps",
     "IpAddressManager",
     "IpAddressManagerProps",
     "IpAddressManagerSharingProps",
+    "NetworkController",
+    "NetworkControllerProps",
     "TransitGatewayHubConfiguration",
     "TransitGatewaySpokeConfiguration",
 ]
 
 publication.publish()
 
+def _typecheckingstub__24d3c1346e4e259fee32303499f123223b892ff23852cdfdf5a57bf21cad7680(
+    *,
+    netmask: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__bafe93fe5666e81af7b6555c6e0b02d696c2267310d93ce406cc5b16333a1449(
     *,
     cidrs: typing.Optional[typing.Sequence[builtins.str]] = None,
     default_netmask_length: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -2563,14 +2845,68 @@
     *,
     allow_external_pricipals: typing.Optional[builtins.bool] = None,
     enabled: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__d930e3de8c120c3fc5f5c70030691aa4f52aa6e26d49c32535c5bce5c960935e(
+    scope: _constructs_77d1e7e8.IConstruct,
+    id: builtins.str,
+    *,
+    default_netmask: typing.Optional[jsii.Number] = None,
+    account: typing.Optional[builtins.str] = None,
+    environment_from_arn: typing.Optional[builtins.str] = None,
+    physical_name: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__74ba1ec928c092f33aeb546fda189638c35c356996133e040cb167d089e3f343(
+    scope: _constructs_77d1e7e8.IConstruct,
+    id: builtins.str,
+    *,
+    netmask: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f39726d5378c607c7d2408b015e8aed7d5f87a4d39b2235dbde97aa46e8daba2(
+    scope: _constructs_77d1e7e8.IConstruct,
+    id: builtins.str,
+    *,
+    netmask: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7a94042b91cf18ea51b81a0607a52121519d15828b001d7f2a7c825c4dc5c4f9(
+    account: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9ea0364f3254929215baedf3bfe5eb8fb59ce1151f770db5cfc4eb7f7dd9754c(
+    region: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1eee37f6e80a88db3d1de97179d49c53732c2177cd8790b1b68e521aa37f3e9d(
+    *,
+    account: typing.Optional[builtins.str] = None,
+    environment_from_arn: typing.Optional[builtins.str] = None,
+    physical_name: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+    default_netmask: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__6667797cf749d298a257c6c716db23d22c81c5c28b1dbf19334ef2de80ebcba5(
     *,
     allow_external: typing.Optional[builtins.bool] = None,
     auto_accept_shared_attachments: typing.Optional[builtins.bool] = None,
     auto_discovery: typing.Optional[builtins.bool] = None,
     default_route_table_id: typing.Optional[builtins.str] = None,
     principals: typing.Optional[typing.Sequence[_ISharedPrincipal_9cde791b]] = None,
```

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.51/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.51/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.50
+Version: 0.0.51
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.50/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.51/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.50.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.51.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

