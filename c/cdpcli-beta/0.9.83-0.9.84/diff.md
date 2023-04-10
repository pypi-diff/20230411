# Comparing `tmp/cdpcli-beta-0.9.83.tar.gz` & `tmp/cdpcli-beta-0.9.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.83.tar", last modified: Fri Mar 24 21:53:13 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.84.tar", last modified: Mon Apr 10 20:24:10 2023, max compression
```

## Comparing `cdpcli-beta-0.9.83.tar` & `cdpcli-beta-0.9.84.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.153981 cdpcli-beta-0.9.83/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-03-24 21:53:13.153981 cdpcli-beta-0.9.83/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15955 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31027 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3777 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-03-24 21:53:09.000000 cdpcli-beta-0.9.83/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    28907 2023-03-24 21:53:09.000000 cdpcli-beta-0.9.83/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   142870 2023-03-24 21:53:11.000000 cdpcli-beta-0.9.83/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   101029 2023-03-24 21:53:10.000000 cdpcli-beta-0.9.83/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.137981 cdpcli-beta-0.9.83/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31579 2023-03-24 21:53:11.000000 cdpcli-beta-0.9.83/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-03-24 21:53:10.000000 cdpcli-beta-0.9.83/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-03-24 21:53:11.000000 cdpcli-beta-0.9.83/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-03-24 21:53:10.000000 cdpcli-beta-0.9.83/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   177884 2023-03-24 21:53:09.000000 cdpcli-beta-0.9.83/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   173157 2023-03-24 21:53:08.000000 cdpcli-beta-0.9.83/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-03-24 21:53:10.000000 cdpcli-beta-0.9.83/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-03-24 21:53:09.000000 cdpcli-beta-0.9.83/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56974 2023-03-24 21:53:11.000000 cdpcli-beta-0.9.83/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    71620 2023-03-24 21:53:11.000000 cdpcli-beta-0.9.83/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30891 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    28629 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.133981 cdpcli-beta-0.9.83/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.141981 cdpcli-beta-0.9.83/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.145981 cdpcli-beta-0.9.83/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3846 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17210 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.145981 cdpcli-beta-0.9.83/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.145981 cdpcli-beta-0.9.83/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25184 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18645 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5031 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.145981 cdpcli-beta-0.9.83/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.145981 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-03-24 21:53:12.000000 cdpcli-beta-0.9.83/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-03-24 21:53:13.153981 cdpcli-beta-0.9.83/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.133981 cdpcli-beta-0.9.83/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:53:13.149981 cdpcli-beta-0.9.83/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32934 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5370 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3411 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4366 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4666 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6971 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-03-24 21:40:46.000000 cdpcli-beta-0.9.83/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-04-10 20:24:06.000000 cdpcli-beta-0.9.84/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29076 2023-04-10 20:24:06.000000 cdpcli-beta-0.9.84/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   142870 2023-04-10 20:24:08.000000 cdpcli-beta-0.9.84/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   102756 2023-04-10 20:24:07.000000 cdpcli-beta-0.9.84/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31579 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.503410 cdpcli-beta-0.9.84/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-04-10 20:24:07.000000 cdpcli-beta-0.9.84/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-04-10 20:24:08.000000 cdpcli-beta-0.9.84/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-04-10 20:24:07.000000 cdpcli-beta-0.9.84/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   177884 2023-04-10 20:24:06.000000 cdpcli-beta-0.9.84/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   173157 2023-04-10 20:24:06.000000 cdpcli-beta-0.9.84/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-04-10 20:24:07.000000 cdpcli-beta-0.9.84/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-04-10 20:24:06.000000 cdpcli-beta-0.9.84/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56974 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    71962 2023-04-10 20:24:08.000000 cdpcli-beta-0.9.84/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30891 2023-04-10 20:24:09.000000 cdpcli-beta-0.9.84/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.499410 cdpcli-beta-0.9.84/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.507410 cdpcli-beta-0.9.84/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.511410 cdpcli-beta-0.9.84/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.511410 cdpcli-beta-0.9.84/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    26147 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.511410 cdpcli-beta-0.9.84/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.511410 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-04-10 20:24:10.000000 cdpcli-beta-0.9.84/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.499410 cdpcli-beta-0.9.84/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:24:10.515410 cdpcli-beta-0.9.84/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32934 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-04-10 20:14:23.000000 cdpcli-beta-0.9.84/versioneer.py
```

### Comparing `cdpcli-beta-0.9.83/LICENSE.txt` & `cdpcli-beta-0.9.84/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.84/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/PKG-INFO` & `cdpcli-beta-0.9.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.83
+Version: 0.9.84
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.83/README.md` & `cdpcli-beta-0.9.84/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/__init__.py` & `cdpcli-beta-0.9.84/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/argparser.py` & `cdpcli-beta-0.9.84/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/argprocess.py` & `cdpcli-beta-0.9.84/cdpcli/argprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,33 +56,35 @@
         super(ParamUnknownKeyError, self).__init__(full_message)
 
 
 class TooComplexError(Exception):
     pass
 
 
-def unpack_argument(cli_argument, value):
-    override = uri_param(cli_argument, value)
+def unpack_argument(cli_argument, value, parsed_globals):
+    override = uri_param(cli_argument, value, parsed_globals)
     if override is not None:
         value = override
     return value
 
 
-def uri_param(cli_argument, value):
-    if getattr(cli_argument, 'no_paramfile', None):
+def uri_param(cli_argument, value, parsed_globals):
+    if not getattr(parsed_globals, 'expand_param', True):
+        return
+    elif getattr(cli_argument, 'no_paramfile', None):
         return
     else:
-        return _check_for_uri_param(cli_argument, value)
+        return _check_for_uri_param(cli_argument, value, parsed_globals)
 
 
-def _check_for_uri_param(param, value):
+def _check_for_uri_param(param, value, parsed_globals):
     if isinstance(value, list) and len(value) == 1:
         value = value[0]
     try:
-        return get_paramfile(value)
+        return get_paramfile(value, parsed_globals)
     except ResourceLoadingError as e:
         raise ParamError(param.cli_name, six.text_type(e))
 
 
 def unpack_cli_arg(cli_argument, value):
     """
     Parses and unpacks the encoded string command line parameter
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/arguments.py` & `cdpcli-beta-0.9.84/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/auth.py` & `cdpcli-beta-0.9.84/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.84/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/clicommand.py` & `cdpcli-beta-0.9.84/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/clidriver.py` & `cdpcli-beta-0.9.84/cdpcli/clidriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,15 +553,16 @@
                 "Unknown options: %s" % ', '.join(remaining))
         check_should_enable_pagination(self._arg_table,
                                        self._operation_model,
                                        parsed_args,
                                        parsed_globals)
         call_parameters = self._build_call_parameters(parsed_args,
                                                       self.arg_table,
-                                                      self._clidriver.get_form_factor())
+                                                      self._clidriver.get_form_factor(),
+                                                      parsed_globals)
         return self._invoke_operation_callers(client_creator,
                                               call_parameters,
                                               parsed_args,
                                               parsed_globals)
 
     def create_help_command(self):
         return OperationHelpCommand(
@@ -572,34 +573,34 @@
 
     def _add_help(self, parser):
         # The 'help' output is processed a little differently from
         # the operation help because the arg_table has
         # CLIArguments for values.
         parser.add_argument('help', nargs='?')
 
-    def _build_call_parameters(self, args, arg_table, form_factor):
+    def _build_call_parameters(self, args, arg_table, form_factor, parsed_globals):
         # We need to convert the args specified on the command
         # line as valid **kwargs we can hand to botocore.
         service_params = {}
         # args is an argparse.Namespace object so we're using vars()
         # so we can iterate over the parsed key/values.
         parsed_args = vars(args)
         for arg_object in arg_table.values():
             py_name = arg_object.py_name
             if py_name in parsed_args:
                 value = parsed_args[py_name]
-                value = unpack_argument(arg_object, value)
+                value = unpack_argument(arg_object, value, parsed_globals)
                 arg_object.add_to_params(service_params, value)
         # We run the ParamFormFactorVisitor over the input data to check
         # the form factor for arguments.
         ParamFormFactorVisitor(form_factor).visit(
             service_params, self._operation_model.input_shape)
         # We run the ParamFileVisitor over the input data to resolve any
         # paramfile references in it.
-        service_params = ParamFileVisitor().visit(
+        service_params = ParamFileVisitor(parsed_globals).visit(
             service_params, self._operation_model.input_shape)
         return service_params
 
     def _create_argument_table(self):
         argument_table = OrderedDict()
         input_shape = self._operation_model.input_shape
         required_arguments = []
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/client.py` & `cdpcli-beta-0.9.84/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/compat.py` & `cdpcli-beta-0.9.84/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/completer.py` & `cdpcli-beta-0.9.84/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/config.py` & `cdpcli-beta-0.9.84/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/configloader.py` & `cdpcli-beta-0.9.84/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/credentials.py` & `cdpcli-beta-0.9.84/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.84/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/cli.json` & `cdpcli-beta-0.9.84/cdpcli/data/cli.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'options'": "{'no-parameter-expansion': OrderedDict([('action', 'store_false'), ('help', "*

 * *              "'<p>Disable expanding parameters by referring to files or URIs.</p>'), ('dest', "*

 * *              "'expand_param')])}"}*

```diff
@@ -72,14 +72,19 @@
             "help": "<p>Explicitly specify the form factor of the control plane being called. When not given, the form factor is guessed based on the command's endpoint URL.</p>"
         },
         "no-paginate": {
             "action": "store_false",
             "dest": "paginate",
             "help": "<p>Disable automatic pagination.</p>"
         },
+        "no-parameter-expansion": {
+            "action": "store_false",
+            "dest": "expand_param",
+            "help": "<p>Disable expanding parameters by referring to files or URIs.</p>"
+        },
         "no-verify-tls": {
             "action": "store_false",
             "dest": "verify_tls",
             "help": "<p>By default, the CDP CLI uses TLS when communicating with CDP services. For each TLS connection, the CDP CLI will verify TLS certificates. This option overrides the default behavior of verifying TLS certificates.</p>"
         },
         "output": {
             "choices": [
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/compute/compute.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -706,15 +706,15 @@
         type: boolean
         description: True if Liftie is managing this deployment.
       chart:
         description: Chart that the deployment was created from.
         $ref: '#/definitions/Chart'
       status:
         type: string
-        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, and FAILED. New values may be added in the future.
+        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, FAILED, PENDING-INSTALL, PENDING-UPGRADE and PENDING-ROLLBACK. New values may be added in the future.
       upgrades:
         type: array
         items:
           $ref: '#/definitions/AvailableDeploymentUpgrade'
         description: Any upgrades available for this deployment.
   History:
     type: object
@@ -722,15 +722,15 @@
     properties:
       revision:
         type: integer
         format: int32
         description: Helm revision.
       status:
         type: string
-        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, and FAILED. New values may be added in the future.
+        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, FAILED, PENDING-INSTALL, PENDING-UPGRADE and PENDING-ROLLBACK. New values may be added in the future.
       chart:
         description: Chart that the deployment was created from.
         $ref: '#/definitions/Chart'
   DescribeDeploymentResponse:
     type: object
     description: Response structure for describing a deployment.
     properties:
@@ -740,15 +740,15 @@
       history:
         type: array
         items:
           $ref: '#/definitions/History'
         description: History of the deployment.
       overrides:
         type: string
-        description: JSON overrides for the deployment's properties. Deprecated.
+        description: Escaped JSON overrides for the deployment's properties. Deprecated.
         x-deprecated: true
   UpgradeDeploymentRequest:
     type: object
     description: Request structure for upgrading a deployment.
     required:
       - clusterCrn
       - namespace
@@ -764,15 +764,15 @@
         type: string
         description: The name of the deployment.
       chartVersion:
         type: string
         description: The version of the deployment to upgrade to. Defaults to latest version.
       overrides:
         type: string
-        description: JSON overrides for the deployment's properties.
+        description: Escaped JSON overrides for the deployment's properties.
   UpgradeDeploymentResponse:
     type: object
     description: Response structure for upgrading a deployment.
     properties:
       name:
         type: string
         description: The name of the deployment.
@@ -784,15 +784,15 @@
         format: int32
         description: Helm revision.
       message:
         type: string
         description: A message returned about the status of the upgrade operation.
       status:
         type: string
-        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, and FAILED. New values may be added in the future.
+        description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, FAILED, PENDING-INSTALL, PENDING-UPGRADE and PENDING-ROLLBACK. New values may be added in the future.
       chart:
         description: Chart that the deployment was created from.
         $ref: '#/definitions/Chart'
   RollbackDeploymentRequest:
     type: object
     description: Request structure to rollback a deployment.
     required:
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/datalake/datalake.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -522,14 +522,35 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/ListDatalakeBackupsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/datalake/cancelBackup:
+    post:
+      summary: Cancels the specified ongoing backup operation.
+      description: Cancels a currently running backup operation. The operation must be in a STARTED or IN_PROGRESS state. Pending sub-operations will be ignored and marked as cancelled. The operation does not wait for the currently running sub-operation(s) to complete.
+      operationId: cancelBackup
+      x-mutating: true
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CancelBackupRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CancelBackupResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/datalake/replaceRecipes:
     post:
       summary: Replaces recipes for the given instance groups.
       description: Replaces recipes for the given instance groups.
       operationId: replaceRecipes
       x-mutating: true
       parameters:
@@ -1968,14 +1989,36 @@
     description: Response object with the list of backup operations performed on a datalake.
     properties:
       backups:
         type: array
         description: Backup object with details of backup performed.
         items:
           $ref: '#/definitions/DatalakeBackup'
+  CancelBackupRequest:
+    type: object
+    description: The request to cancel a backup operation.
+    required:
+      - backupId
+    properties:
+      backupId:
+        type: string
+        description: Backup-id that identifies the backup to be cancelled.
+      force:
+        type: boolean
+        default: false
+        description: Will mark all unfinished operations as cancelled without waiting for their result and mark backup operation as finished (cancelled, successful or failed) immediately.
+  CancelBackupResponse:
+    type: object
+    description: Response to the cancel backup request.
+    required:
+      - result
+    properties:
+      result:
+        type: string
+        description: Result of the cancel backup request. It can contain a description of the current process state or guidelines to a customer on the next steps.
   DatalakeBackup:
     type: object
     description: Backup object with details of backup performed.
     required:
       - backupName
       - accountId
       - userCrn
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/dw/dw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -829,14 +829,17 @@
         description: The desired number of strong meta servers for this database. A positive, non-zero number is required. Use removeStrongMetaServers to remove strong meta servers entirely. Requires the COD_STRONG_META_SERVERS entitlement.
       removeStrongMetaServers:
         type: boolean
         description: Removes any strong meta servers provisioned for this database. Requires the COD_STRONG_META_SERVERS entitlement.
       catalog:
         type: string
         description: Catalog name for the image.
+      verticalScale:
+        description: Vertical Scale request for database.
+        $ref: '#/definitions/GroupType'
   AutoScalingParameters:
     type: object
     description: A Parameters to configure AutoScaling
     properties:
       targetedValueForMetric:
         type: integer
         format: int64
@@ -2187,8 +2190,14 @@
         type: string
         description: The name or CRN of the database.
       edgeNodes:
         type: array
         items:
           $ref: '#/definitions/EdgeNode'
         description: The list of edge nodes for a database.
+  GroupType:
+    type: string
+    description: "Group type for the database nodes.\n `GATEWAY` - GATEWAY value of the Group variable. `MASTER` - MASTER value of the Group variable."
+    enum:
+      - GATEWAY
+      - MASTER
 x-audit: true
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.84/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.83
+  version: 0.9.84
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.84/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.84/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/doc/style.py` & `cdpcli-beta-0.9.84/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/docs.py` & `cdpcli-beta-0.9.84/cdpcli/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,18 @@
 
     def _json_example_value_name(self, argument_model, include_enum_values=True):
         # If include_enum_values is True, then the valid enum values
         # are included as the sample JSON value.
         if isinstance(argument_model, StringShape):
             if argument_model.enum and include_enum_values:
                 choices = argument_model.enum
+                if not self.show_hidden and argument_model.deprecated_enum_values:
+                    choices = [item
+                               for item in choices
+                               if item not in argument_model.deprecated_enum_values]
                 return '|'.join(['"%s"' % c for c in choices])
             elif argument_model.supported_options and include_enum_values:
                 choices = argument_model.supported_options
                 return '|'.join(['"%s"' % c for c in choices])
             else:
                 return '"string"'
         elif argument_model.type_name == 'boolean':
@@ -579,15 +583,19 @@
             doc.write('Syntax')
             doc.style.start_codeblock()
             example_type = self._json_example_value_name(
                 member, include_enum_values=False)
             doc.write('%s %s ...' % (example_type, example_type))
             if isinstance(member, StringShape):
                 if member.enum:
-                    self._write_possible_values(doc, member.enum)
+                    enum_values = member.enum
+                    if not self.show_hidden and member.deprecated_enum_values:
+                        enum_values = [v for v in enum_values
+                                       if v not in member.deprecated_enum_values]
+                    self._write_possible_values(doc, enum_values)
                 if member.supported_options:
                     self._write_possible_values(doc, member.supported_options)
             doc.style.end_codeblock()
             doc.style.new_paragraph()
         elif cli_argument.cli_type_name not in SCALAR_TYPES:
             doc.style.new_paragraph()
             doc.write('JSON Syntax')
@@ -701,15 +709,19 @@
         doc.style.new_paragraph()
 
     def _document_enums(self, argument, doc):
         if hasattr(argument, 'argument_model'):
             model = argument.argument_model
             if isinstance(model, StringShape):
                 if model.enum:
-                    self._write_possible_values(doc, model.enum)
+                    enum_values = model.enum
+                    if not self.show_hidden and model.deprecated_enum_values:
+                        enum_values = [v for v in enum_values
+                                       if v not in model.deprecated_enum_values]
+                    self._write_possible_values(doc, enum_values)
                 if model.supported_options:
                     self._write_possible_values(doc, model.supported_options)
 
     def _write_possible_values(self, doc, possible_values):
         doc.style.new_paragraph()
         doc.write('Possible values:')
         doc.style.start_ul()
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/endpoint.py` & `cdpcli-beta-0.9.84/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.84/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.84/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.84/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.84/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.84/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/exceptions.py` & `cdpcli-beta-0.9.84/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/cliinputjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,37 +48,37 @@
 
     def invoke(self,
                client_creator,
                operation_model,
                parameters,
                parsed_args,
                parsed_globals):
-        return self.add_to_call_parameters(parameters, parsed_args)
+        return self.add_to_call_parameters(parameters, parsed_args, parsed_globals)
 
-    def add_to_call_parameters(self, call_parameters, parsed_args):
+    def add_to_call_parameters(self, call_parameters, parsed_args, parsed_globals):
 
         # Check if ``--cli-input-json`` was specified in the command line.
         input_json = getattr(parsed_args, 'cli_input_json', None)
         if input_json is not None:
             # Retrieve the JSON from the file if needed.
-            retrieved_json = get_paramfile(input_json)
+            retrieved_json = get_paramfile(input_json, parsed_globals)
             # Nothing was retrieved from the file. So assume the argument
             # is already a JSON string.
             if retrieved_json is None:
                 retrieved_json = input_json
             try:
                 # Try to load the JSON string into a python dictionary
                 input_data = json.loads(retrieved_json)
             except ValueError as e:
                 raise ParamError(
                     self.name, "Invalid JSON: %s\nJSON received: %s"
                                % (e, retrieved_json))
             # We run the ParamFileVisitor over the input data to resolve any
             # paramfile references in it.
-            input_data = ParamFileVisitor().visit(
+            input_data = ParamFileVisitor(parsed_globals).visit(
                 input_data, self._operation_model.input_shape)
             # Add the members from the input JSON to the call parameters.
             self._update_call_parameters(call_parameters, input_data)
         return True
 
     def _update_call_parameters(self, call_parameters, input_data):
         for input_key in input_data.keys():
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             # Convert the name to use dashes instead of underscore
             # as these are how the parameters are stored in the
             # `arg_table`.
             xformed = key.replace('_', '-')
             if xformed in self.arg_table:
                 cli_argument = self.arg_table[xformed]
 
-            value = unpack_argument(cli_argument, value)
+            value = unpack_argument(cli_argument, value, parsed_globals)
 
             # If this parameter has a schema defined, then allow plugins
             # a chance to process and override its value.
             if self._should_allow_override(cli_argument, value):
                 # Unpack the argument, which is a string, into the
                 # correct Python type (dict, list, etc)
                 value = unpack_cli_arg(cli_argument, value)
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/df/createdeployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from cdpcli.exceptions import ClientError, DfExtensionError
 from cdpcli.extensions.df import get_expanded_file_path, upload_workload_asset
 from cdpcli.extensions.workload import set_workload_access_token
 from cdpcli.model import ObjectShape, OperationModel, ShapeResolver
 from cdpcli.utils import CachedProperty
 
 LOG = logging.getLogger('cdpcli.extensions.df.createdeployment')
+MAX_ASSET_SIZE = 150 * 1024 * 1024
 INITIAL_CONFIGURATION_VERSION = 0
 INITIAL_ASSET_VERSION = '0'
 
 SERVICE_NAME = 'df'
 OPERATION_NAME = 'createDeployment'
 OPERATION_CLI_NAME = 'create-deployment'
 OPERATION_SUMMARY = 'Initiate and create deployment on workload'
@@ -557,14 +558,31 @@
                        parameters):
         """
         Upload Assets associated with Deployment when Asset References found
         """
         parameter_groups = parameters.get('parameterGroups', None)
         if parameter_groups:
             deployment_name = parameters.get('deploymentName', None)
+
+            for parameter_group in parameter_groups:
+                parameters = parameter_group['parameters']
+                for parameter in parameters:
+                    asset_references = parameter.get('assetReferences', None)
+                    if asset_references:
+                        for asset_path in asset_references:
+                            file_stats = os.stat(asset_path)
+                            if file_stats.st_size > MAX_ASSET_SIZE:
+                                raise DfExtensionError(
+                                    err_msg='The file size exceeds '
+                                            'the 150 MB limit, file: [{}]'
+                                    .format(asset_path),
+                                    service_name=df_workload_client.meta.service_model
+                                    .service_name,
+                                    operation_name='uploadAsset')
+
             for parameter_group in parameter_groups:
                 parameter_group_name = parameter_group['name']
                 parameters = parameter_group['parameters']
                 for parameter in parameters:
                     asset_references = parameter.get('assetReferences', None)
                     if asset_references:
                         updated_asset_references = []
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.84/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/formatter.py` & `cdpcli-beta-0.9.84/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/help.py` & `cdpcli-beta-0.9.84/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/loader.py` & `cdpcli-beta-0.9.84/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/main.py` & `cdpcli-beta-0.9.84/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/model.py` & `cdpcli-beta-0.9.84/cdpcli/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,18 @@
 
 class StringShape(Shape):
     @CachedProperty
     def enum(self):
         return self._shape_data.get('enum', [])
 
     @CachedProperty
+    def deprecated_enum_values(self):
+        return self._shape_data.get('x-deprecated-enum-values', [])
+
+    @CachedProperty
     def supported_options(self):
         return self._shape_data.get('x-supported-options', [])
 
 
 class ShapeResolver(object):
 
     def __init__(self, definitions):
@@ -498,14 +502,16 @@
         shape = {
             'type': model['type'],
         }
         if 'documentation' in model:
             shape['documentation'] = model['documentation']
         if 'enum' in model:
             shape['enum'] = model['enum']
+        if 'x-deprecated-enum-values' in model:
+            shape['x-deprecated-enum-values'] = model['x-deprecated-enum-values']
         if 'x-supported-options' in model:
             shape['x-supported-options'] = model['x-supported-options']
         if 'x-no-paramfile' in model:
             shape['x-no-paramfile'] = model['x-no-paramfile']
         return shape
 
     def _build_scalar(self, model):
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/paginate.py` & `cdpcli-beta-0.9.84/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/paramfile.py` & `cdpcli-beta-0.9.84/cdpcli/paramfile.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import requests
 
 
 class ResourceLoadingError(Exception):
     pass
 
 
-def get_paramfile(path):
+def get_paramfile(path, parsed_globals):
     """Load parameter based on a resource URI.
 
     It is possible to pass parameters to operations by referring
     to files or URI's.  If such a reference is detected, this
     function attempts to retrieve the data from the file or URI
     and returns it.  If there are any errors or if the ``path``
     does not appear to refer to a file or URI, a ``None`` is
@@ -37,36 +37,44 @@
 
     """
     data = None
     if isinstance(path, six.string_types):
         for prefix, function_spec in PREFIX_MAP.items():
             if path.startswith(prefix):
                 function, kwargs = function_spec
+                kwargs['parsed_globals'] = parsed_globals
                 data = function(prefix, path, **kwargs)
     return data
 
 
-def get_file(prefix, path, mode):
+def get_file(prefix, path, mode, parsed_globals):
     file_path = os.path.expandvars(os.path.expanduser(path[len(prefix):]))
     try:
         with compat_open(file_path, mode) as f:
             return f.read()
     except UnicodeDecodeError:
         raise ResourceLoadingError(
             'Unable to load paramfile (%s), text contents could '
             'not be decoded.  If this is a binary file, please use the '
             'fileb:// prefix instead of the file:// prefix.' % file_path)
     except (OSError, IOError) as e:
         raise ResourceLoadingError('Unable to load paramfile %s: %s' % (
             path, e))
 
 
-def get_uri(prefix, uri):
+def get_uri(prefix, uri, parsed_globals):
     try:
-        r = requests.get(uri)
+        # The TLS verification value can be a boolean or a CA_BUNDLE path. This
+        # is a little odd, but ultimately comes from the python HTTP requests
+        # library we're using.
+        tls_verification = getattr(parsed_globals, 'verify_tls', True)
+        ca_bundle = getattr(parsed_globals, 'ca_bundle', None)
+        if tls_verification and ca_bundle is not None:
+            tls_verification = ca_bundle
+        r = requests.get(uri, verify=tls_verification)
         if r.status_code == 200:
             return r.text
         else:
             raise ResourceLoadingError(
                 "received non 200 status code of %s" % (
                     r.status_code))
     except Exception as e:
@@ -78,14 +86,17 @@
     'fileb://': (get_file, {'mode': 'rb'}),
     'http://': (get_uri, {}),
     'https://': (get_uri, {}),
 }
 
 
 class ParamFileVisitor(object):
+    def __init__(self, parsed_globals):
+        self._parsed_globals = parsed_globals
+
     """
     This visitor's visit method will walk the input params object of the input
     shape, visiting all fields and recursing through complex fields. Any string
     field encountered will get paramfile resolution unless it is marked in the
     model as being x-no-paramfile.
     """
 
@@ -124,30 +135,34 @@
     def _visit_float(self, param, shape, name):
         return param
 
     def _visit_double(self, param, shape, name):
         return param
 
     def _visit_string(self, param, shape, name):
+        if not getattr(self._parsed_globals, 'expand_param', True):
+            return param
         if shape.is_no_paramfile:
             return param
-        override = get_paramfile(param)
+        override = get_paramfile(param, self._parsed_globals)
         if override is not None:
             return override
         return param
 
     def _visit_array(self, param, shape, name):
         visited = []
         for i, item in enumerate(param):
             visited.append(self._visit(item, shape.member, '%s[%s]' % (name, i)))
         return visited
 
     def _visit_datetime(self, param, shape, name):
         return param
 
     def _visit_blob(self, param, shape, name):
+        if not getattr(self._parsed_globals, 'expand_param', True):
+            return param
         if shape.is_no_paramfile:
             return param
-        override = get_paramfile(param)
+        override = get_paramfile(param, self._parsed_globals)
         if override is not None:
             return override
         return param
```

### Comparing `cdpcli-beta-0.9.83/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.84/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/parser.py` & `cdpcli-beta-0.9.84/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.84/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/schema.py` & `cdpcli-beta-0.9.84/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/serialize.py` & `cdpcli-beta-0.9.84/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/shorthand.py` & `cdpcli-beta-0.9.84/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/signers.py` & `cdpcli-beta-0.9.84/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/table.py` & `cdpcli-beta-0.9.84/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/text.py` & `cdpcli-beta-0.9.84/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/textwriter.py` & `cdpcli-beta-0.9.84/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.84/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/translate.py` & `cdpcli-beta-0.9.84/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/utils.py` & `cdpcli-beta-0.9.84/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli/validate.py` & `cdpcli-beta-0.9.84/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.84/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.83
+Version: 0.9.84
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.83/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.84/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/setup.py` & `cdpcli-beta-0.9.84/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/setup_common.py` & `cdpcli-beta-0.9.84/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/__init__.py` & `cdpcli-beta-0.9.84/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.84/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_cliinputjson.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,78 +62,90 @@
         add_cli_input_json(self.operation_model, argument_table)
         arg_handler = argument_table['cli-input-json']
         self.assertIsNotNone(arg_handler)
         self.assertTrue(isinstance(arg_handler, CliInputJSONArgument))
 
     def test_add_to_call_parameters_no_file(self):
         parsed_args = mock.Mock()
+        parsed_globals = mock.Mock()
         # Make the value a JSON string
         parsed_args.cli_input_json = self.input_json
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file(self):
         parsed_args = mock.Mock()
+        parsed_globals = mock.Mock()
         # Make the value a file with JSON located inside.
         parsed_args.cli_input_json = 'file://' + self.temp_file
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file_from_visitor(self):
         temp_file1 = os.path.join(self.temp_dir, 'foo.json')
         with open(temp_file1, 'w') as f:
             f.write("baz")
         temp_file1 = _make_file_uri(temp_file1)
         temp_file2 = os.path.join(self.temp_dir, 'bar.json')
         with open(temp_file2, 'w') as f:
             f.write('{"A": "foo", "B": "file://%s"}' % temp_file1)
         temp_file2 = _make_file_uri(temp_file2)
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = 'file://' + temp_file2
+        parsed_globals = mock.Mock()
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'baz'})
 
     def test_add_to_call_parameters_bad_json(self):
         parsed_args = mock.Mock()
         # Create a bad JSON input
         parsed_args.cli_input_json = self.input_json + ','
+        parsed_globals = mock.Mock()
         call_parameters = {}
         with self.assertRaises(ParamError):
             self.argument.add_to_call_parameters(
                 call_parameters=call_parameters,
-                parsed_args=parsed_args
+                parsed_args=parsed_args,
+                parsed_globals=parsed_globals
             )
 
     def test_add_to_call_parameters_no_clobber(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = self.input_json
+        parsed_globals = mock.Mock()
         # The value for ``A`` should not be clobbered by the input JSON
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'baz', 'B': 'bar'})
 
     def test_no_add_to_call_parameters(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = None
+        parsed_globals = mock.Mock()
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         # Nothing should have been added to the call parameters because
         # ``cli_input_json`` is not in the ``parsed_args``
         self.assertEqual(call_parameters, {'A': 'baz'})
```

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.84/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.84/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_auth.py` & `cdpcli-beta-0.9.84/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.84/tests/unit/test_cli_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
                              'cli-read-timeout',
                              'cli-connect-timeout',
                              'no-paginate',
                              'auth-config',
                              'profile',
                              'cdp-region',
                              'ensure-ascii',
-                             'deprecated']
+                             'deprecated',
+                             'no-parameter-expansion']
     assert_equal(sorted(cli_data['options'].keys()), sorted(validated_cli_options))
 
 
 def test_cdp_region():
     # We skip this test if we're in a container since the CLI data is not simple
     # to find. This is fine, since no additional coverage is offered by running
     # this on different OSes with different versions of python.
```

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_client.py` & `cdpcli-beta-0.9.84/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_completer.py` & `cdpcli-beta-0.9.84/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.84/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.84/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_help.py` & `cdpcli-beta-0.9.84/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.84/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_model.py` & `cdpcli-beta-0.9.84/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.84/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.84/tests/unit/test_paramfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,90 +28,108 @@
 import yaml
 
 MODEL_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'paramfile')
 
 
 class TestParamFile(unittest.TestCase):
     def setUp(self):
+        self.parsed_globals = mock.Mock()
         self.files = FileCreator()
 
     def tearDown(self):
         self.files.remove_all()
 
     def test_text_file(self):
         contents = 'This is a test'
         filename = self.files.create_file('foo', contents)
         prefixed_filename = 'file://' + filename
-        data = get_paramfile(prefixed_filename)
+        data = get_paramfile(prefixed_filename, self.parsed_globals)
         self.assertEqual(data, contents)
         self.assertIsInstance(data, six.string_types)
 
     def test_binary_file(self):
         contents = 'This is a test'
         filename = self.files.create_file('foo', contents)
         prefixed_filename = 'fileb://' + filename
-        data = get_paramfile(prefixed_filename)
+        data = get_paramfile(prefixed_filename, self.parsed_globals)
         self.assertEqual(data, b'This is a test')
         self.assertIsInstance(data, six.binary_type)
 
     @skip_if_windows('Binary content error only occurs '
                      'on non-Windows platforms.')
     def test_cannot_load_text_file(self):
         contents = b'\xbfX\xac\xbe'
         filename = self.files.create_file('foo', contents, mode='wb')
         prefixed_filename = 'file://' + filename
         with self.assertRaises(ResourceLoadingError):
-            get_paramfile(prefixed_filename)
+            get_paramfile(prefixed_filename, self.parsed_globals)
 
     def test_file_does_not_exist_raises_error(self):
         with self.assertRaises(ResourceLoadingError):
-            get_paramfile('file://file/does/not/existsasdf.txt')
+            get_paramfile('file://file/does/not/existsasdf.txt', self.parsed_globals)
 
     def test_no_match_uris_returns_none(self):
-        self.assertIsNone(get_paramfile('foobar://somewhere.bar'))
+        self.assertIsNone(get_paramfile('foobar://somewhere.bar', self.parsed_globals))
 
     def test_non_string_type_returns_none(self):
-        self.assertIsNone(get_paramfile(100))
+        self.assertIsNone(get_paramfile(100, self.parsed_globals))
 
 
 class TestHTTPBasedResourceLoading(unittest.TestCase):
     def setUp(self):
+        self.parsed_globals = mock.Mock(verify_tls=True, ca_bundle=None)
         self.requests_patch = mock.patch('cdpcli.paramfile.requests')
         self.requests_mock = self.requests_patch.start()
         self.response = mock.Mock(status_code=200)
         self.requests_mock.get.return_value = self.response
 
     def tearDown(self):
         self.requests_patch.stop()
 
     def test_resource_from_http(self):
         self.response.text = 'http contents'
-        loaded = get_paramfile('http://foo.bar.baz')
+        loaded = get_paramfile('http://foo.bar.baz', self.parsed_globals)
         self.assertEqual(loaded, 'http contents')
-        self.requests_mock.get.assert_called_with('http://foo.bar.baz')
+        self.requests_mock.get.assert_called_with('http://foo.bar.baz', verify=True)
 
     def test_resource_from_https(self):
         self.response.text = 'http contents'
-        loaded = get_paramfile('https://foo.bar.baz')
+        loaded = get_paramfile('https://foo.bar.baz', self.parsed_globals)
         self.assertEqual(loaded, 'http contents')
-        self.requests_mock.get.assert_called_with('https://foo.bar.baz')
+        self.requests_mock.get.assert_called_with('https://foo.bar.baz', verify=True)
 
     def test_non_200_raises_error(self):
         self.response.status_code = 500
         with self.assertRaisesRegexp(ResourceLoadingError, 'foo\\.bar\\.baz'):
-            get_paramfile('https://foo.bar.baz')
+            get_paramfile('https://foo.bar.baz', self.parsed_globals)
 
     def test_connection_error_raises_error(self):
         self.requests_mock.get.side_effect = Exception("Connection error.")
         with self.assertRaisesRegexp(ResourceLoadingError, 'foo\\.bar\\.baz'):
-            get_paramfile('https://foo.bar.baz')
+            get_paramfile('https://foo.bar.baz', self.parsed_globals)
+
+    def test_resource_from_https_verify_tls_with_ca(self):
+        parsed_globals = mock.Mock(verify_tls=True, ca_bundle='test.cer')
+        self.response.text = 'http contents'
+        loaded = get_paramfile('https://foo.bar.baz', parsed_globals)
+        self.assertEqual(loaded, 'http contents')
+        self.requests_mock.get.assert_called_with('https://foo.bar.baz',
+                                                  verify='test.cer')
+
+    def test_resource_from_https_skip_verify_tls(self):
+        parsed_globals = mock.Mock(verify_tls=False)
+        self.response.text = 'http contents'
+        loaded = get_paramfile('https://foo.bar.baz', parsed_globals)
+        self.assertEqual(loaded, 'http contents')
+        self.requests_mock.get.assert_called_with('https://foo.bar.baz', verify=False)
 
 
 class TestParamFileVisitor(unittest.TestCase):
     def setUp(self):
+        self.parsed_globals = mock.Mock()
         self.model = yaml.safe_load(open(os.path.join(MODEL_DIR, 'service.yaml')))
         self.service_model = ServiceModel(self.model, 'servicename')
         self.resolver = ShapeResolver(self.model['definitions'])
         self.files = FileCreator()
 
     def tearDown(self):
         self.files.remove_all()
@@ -121,46 +139,46 @@
         filename = self.files.create_file('jobOne.hql', contents)
         # We have modified our test model to mark jobXml with x-no-paramfile.
         params = {'clusterName': u'foo',
                   'jobs': [{'hiveJob': {'script': 'file://' + filename,
                                         'jobXml': 'file://' + filename}}]}
         shape = self.resolver.get_shape_by_name(
             'submit-jobs-request', 'SubmitJobsRequest')
-        visited = ParamFileVisitor().visit(params, shape)
+        visited = ParamFileVisitor(self.parsed_globals).visit(params, shape)
         params['jobs'][0]['hiveJob']['script'] = contents
         self.assertEqual(params, visited)
 
     def test_ref_map_visitor(self):
         contents = 'This is a test'
         filename = self.files.create_file('jobOne.hql', contents)
         # We have modified our test model to mark jobXml with x-no-paramfile.
         params = {'jobs': {'job1': {'hiveJob': {'script': 'file://' + filename,
                                     'jobXml': 'file://' + filename}}}}
         shape = self.resolver.get_shape_by_name(
             'map-paramfile-test', 'RefMapParamFileTest')
-        visited = ParamFileVisitor().visit(params, shape)
+        visited = ParamFileVisitor(self.parsed_globals).visit(params, shape)
         params['jobs']['job1']['hiveJob']['script'] = contents
         self.assertEqual(params, visited)
 
     def test_explicit_map_visitor(self):
         contents = 'This is a test'
         filename = self.files.create_file('jobOne.hql', contents)
         # We have modified our test model to mark jobXml with x-no-paramfile.
         params = {'jobs': {'job1': {'script': 'file://' + filename,
                                     'jobXml': 'file://' + filename}}}
         shape = self.resolver.get_shape_by_name(
             'map-paramfile-test', 'ExplicitMapParamFileTest')
-        visited = ParamFileVisitor().visit(params, shape)
+        visited = ParamFileVisitor(self.parsed_globals).visit(params, shape)
         params['jobs']['job1']['script'] = contents
         self.assertEqual(params, visited)
 
     def test_blob_visitor(self):
         contents = b'This is a test'
         filename = self.files.create_file('jobOne.hql', contents, mode='wb')
         # We have modified our test model to mark jobXml with x-no-paramfile.
         params = {'jobs': {'job1': {'script': 'fileb://' + filename,
                                     'jobXml': 'fileb://' + filename}}}
         shape = self.resolver.get_shape_by_name(
             'blob-test', 'BlobParamFileTest')
-        visited = ParamFileVisitor().visit(params, shape)
+        visited = ParamFileVisitor(self.parsed_globals).visit(params, shape)
         params['jobs']['job1']['script'] = contents
         self.assertEqual(params, visited)
```

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.84/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.84/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.84/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_signers.py` & `cdpcli-beta-0.9.84/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.84/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_utils.py` & `cdpcli-beta-0.9.84/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/tests/unit/test_validate.py` & `cdpcli-beta-0.9.84/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.83/versioneer.py` & `cdpcli-beta-0.9.84/versioneer.py`

 * *Files identical despite different names*

