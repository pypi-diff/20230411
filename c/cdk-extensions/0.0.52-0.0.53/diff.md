# Comparing `tmp/cdk-extensions-0.0.52.tar.gz` & `tmp/cdk-extensions-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.52.tar", last modified: Tue Apr 11 17:17:20 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.53.tar", last modified: Tue Apr 11 18:57:54 2023, max compression
```

## Comparing `cdk-extensions-0.0.52.tar` & `cdk-extensions-0.0.53.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.476669 cdk-extensions-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 17:17:20.476669 cdk-extensions-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:17:20.476669 cdk-extensions-0.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.460667 cdk-extensions-0.0.52/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.464668 cdk-extensions-0.0.52/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.464668 cdk-extensions-0.0.52/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.464668 cdk-extensions-0.0.52/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1484192 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/_jsii/cdk-extensions@0.0.52.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.464668 cdk-extensions-0.0.52/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   621775 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   153560 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.468668 cdk-extensions-0.0.52/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.472668 cdk-extensions-0.0.52/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-11 17:17:06.000000 cdk-extensions-0.0.52/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:17:20.464668 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 17:17:20.000000 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 17:17:20.000000 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:17:20.000000 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 17:17:20.000000 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 17:17:20.000000 cdk-extensions-0.0.52/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.581429 cdk-extensions-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 18:57:54.581429 cdk-extensions-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:57:54.581429 cdk-extensions-0.0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.569429 cdk-extensions-0.0.53/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1485237 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/_jsii/cdk-extensions@0.0.53.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   621775 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   153560 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.577429 cdk-extensions-0.0.53/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.581429 cdk-extensions-0.0.53/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.581429 cdk-extensions-0.0.53/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-11 18:57:41.000000 cdk-extensions-0.0.53/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:57:54.573429 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-11 18:57:54.000000 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 18:57:54.000000 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:57:54.000000 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 18:57:54.000000 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 18:57:54.000000 cdk-extensions-0.0.53/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.52/LICENSE` & `cdk-extensions-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/PKG-INFO` & `cdk-extensions-0.0.53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.52
+Version: 0.0.53
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.52/README.md` & `cdk-extensions-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/setup.py` & `cdk-extensions-0.0.53/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.52",
+    "version": "0.0.53",
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
-            "cdk-extensions@0.0.52.jsii.tgz"
+            "cdk-extensions@0.0.53.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.53/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.53/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.52
+Version: 0.0.53
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.52/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.53/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.52.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.53.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

