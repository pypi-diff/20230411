# Comparing `tmp/cg-27.2.1.tar.gz` & `tmp/cg-27.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-27.2.1.tar", last modified: Tue Apr 11 10:59:43 2023, max compression
+gzip compressed data, was "dist/cg-27.2.2.tar", last modified: Tue Apr 11 11:20:05 2023, max compression
```

## Comparing `cg-27.2.1.tar` & `cg-27.2.2.tar`

### file list

```diff
@@ -1,1236 +1,1236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-11 10:59:32.000000 cg-27.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-11 10:59:43.000000 cg-27.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 10:59:32.000000 cg-27.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 10:59:32.000000 cg-27.2.1/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/backup_tape.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/db/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/dragen_demux_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-11 10:59:32.000000 cg-27.2.1/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/import_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/set/families.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/set/family.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 10:59:32.000000 cg-27.2.1/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 10:59:32.000000 cg-27.2.1/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-11 10:59:32.000000 cg-27.2.1/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-11 10:59:32.000000 cg-27.2.1/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-11 10:59:32.000000 cg-27.2.1/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 10:59:32.000000 cg-27.2.1/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 10:59:32.000000 cg-27.2.1/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28514 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-11 10:59:32.000000 cg-27.2.1/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 10:59:32.000000 cg-27.2.1/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-11 10:59:32.000000 cg-27.2.1/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 10:59:32.000000 cg-27.2.1/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 10:59:32.000000 cg-27.2.1/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-11 10:59:32.000000 cg-27.2.1/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29722 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/import_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40457 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27621 2023-04-11 10:59:32.000000 cg-27.2.1/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 10:59:32.000000 cg-27.2.1/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39302 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-11 10:59:43.000000 cg-27.2.1/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 10:59:32.000000 cg-27.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-11 10:59:32.000000 cg-27.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:59:43.000000 cg-27.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-11 10:59:32.000000 cg-27.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/test_parse_run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/demultiplex/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/gens/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-11 10:59:32.000000 cg-27.2.1/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/delete/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/delete/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_families.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/set/test_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/test_cli_status_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-11 10:59:32.000000 cg-27.2.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    60792 2023-04-11 10:59:32.000000 cg-27.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/hiseq_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/store/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/fixtures/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/store/api/application_versions.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-11 10:59:32.000000 cg-27.2.1/tests/fixtures/store/api/applications.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-11 10:59:32.000000 cg-27.2.1/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-11 10:59:32.000000 cg-27.2.1/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 10:59:32.000000 cg-27.2.1/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-11 10:59:32.000000 cg-27.2.1/tests/io/test_io_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24823 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-11 10:59:32.000000 cg-27.2.1/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 10:59:32.000000 cg-27.2.1/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/demultiplexing/test_flowcell_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 10:59:32.000000 cg-27.2.1/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 10:59:32.000000 cg-27.2.1/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-11 10:59:32.000000 cg-27.2.1/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 10:59:32.000000 cg-27.2.1/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 10:59:32.000000 cg-27.2.1/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54207 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/api/test_store_import_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27931 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-04-11 10:59:32.000000 cg-27.2.1/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-11 10:59:32.000000 cg-27.2.1/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:43.000000 cg-27.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-11 10:59:32.000000 cg-27.2.1/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-11 11:19:56.000000 cg-27.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-11 11:20:05.000000 cg-27.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 11:19:56.000000 cg-27.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 11:19:56.000000 cg-27.2.2/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/backup_tape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/db/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/dragen_demux_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-11 11:19:56.000000 cg-27.2.2/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/import_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/set/families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/set/family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 11:19:56.000000 cg-27.2.2/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 11:19:56.000000 cg-27.2.2/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-11 11:19:56.000000 cg-27.2.2/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-11 11:19:56.000000 cg-27.2.2/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-11 11:19:56.000000 cg-27.2.2/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 11:19:56.000000 cg-27.2.2/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 11:19:56.000000 cg-27.2.2/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28514 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-11 11:19:56.000000 cg-27.2.2/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 11:19:56.000000 cg-27.2.2/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-11 11:19:56.000000 cg-27.2.2/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 11:19:56.000000 cg-27.2.2/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 11:19:56.000000 cg-27.2.2/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-11 11:19:56.000000 cg-27.2.2/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/import_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40668 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27621 2023-04-11 11:19:56.000000 cg-27.2.2/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 11:19:56.000000 cg-27.2.2/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39302 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-11 11:20:05.000000 cg-27.2.2/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 11:19:56.000000 cg-27.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-11 11:19:56.000000 cg-27.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:20:05.000000 cg-27.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-11 11:19:56.000000 cg-27.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/test_parse_run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/demultiplex/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/gens/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-11 11:19:56.000000 cg-27.2.2/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/delete/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/delete/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/set/test_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/test_cli_status_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-11 11:19:56.000000 cg-27.2.2/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60792 2023-04-11 11:19:56.000000 cg-27.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/hiseq_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/store/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/fixtures/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/store/api/application_versions.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-11 11:19:56.000000 cg-27.2.2/tests/fixtures/store/api/applications.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-11 11:19:56.000000 cg-27.2.2/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-11 11:19:56.000000 cg-27.2.2/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 11:19:56.000000 cg-27.2.2/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-11 11:19:56.000000 cg-27.2.2/tests/io/test_io_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24823 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-11 11:19:56.000000 cg-27.2.2/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 11:19:56.000000 cg-27.2.2/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/demultiplexing/test_flowcell_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 11:19:56.000000 cg-27.2.2/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 11:19:56.000000 cg-27.2.2/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-11 11:19:56.000000 cg-27.2.2/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 11:19:56.000000 cg-27.2.2/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 11:19:56.000000 cg-27.2.2/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54207 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/api/test_store_import_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27931 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-04-11 11:19:56.000000 cg-27.2.2/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-11 11:19:56.000000 cg-27.2.2/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:05.000000 cg-27.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-11 11:19:56.000000 cg-27.2.2/tests/utils/test_utils.py
```

### Comparing `cg-27.2.1/PKG-INFO` & `cg-27.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 27.2.1
+Version: 27.2.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-27.2.1/README.md` & `cg-27.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/crud/create.py` & `cg-27.2.2/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/crud/delete.py` & `cg-27.2.2/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/crud/find.py` & `cg-27.2.2/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/backup.py` & `cg-27.2.2/cg/apps/cgstats/db/models/backup.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/backup_tape.py` & `cg-27.2.2/cg/apps/cgstats/db/models/backup_tape.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/base.py` & `cg-27.2.2/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/datasource.py` & `cg-27.2.2/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/demux.py` & `cg-27.2.2/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/flowcell.py` & `cg-27.2.2/cg/apps/cgstats/db/models/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/project.py` & `cg-27.2.2/cg/apps/cgstats/db/models/project.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/sample.py` & `cg-27.2.2/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/support_params.py` & `cg-27.2.2/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/unaligned.py` & `cg-27.2.2/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/db/models/version.py` & `cg-27.2.2/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/demux_sample.py` & `cg-27.2.2/cg/apps/cgstats/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/dragen_demux_sample.py` & `cg-27.2.2/cg/apps/cgstats/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-27.2.2/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-27.2.2/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/demux_stats.py` & `cg-27.2.2/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-27.2.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-27.2.2/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/parsers/run_info.py` & `cg-27.2.2/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/cgstats/stats.py` & `cg-27.2.2/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/coverage/api.py` & `cg-27.2.2/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/crunchy/crunchy.py` & `cg-27.2.2/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/crunchy/files.py` & `cg-27.2.2/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/crunchy/sbatch.py` & `cg-27.2.2/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-27.2.2/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/demux_report.py` & `cg-27.2.2/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/sample_sheet/create.py` & `cg-27.2.2/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-27.2.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-27.2.2/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-27.2.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/demultiplex/sbatch.py` & `cg-27.2.2/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/gens.py` & `cg-27.2.2/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/gt.py` & `cg-27.2.2/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/hermes/hermes_api.py` & `cg-27.2.2/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/hermes/models.py` & `cg-27.2.2/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/housekeeper/hk.py` & `cg-27.2.2/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/invoice/render.py` & `cg-27.2.2/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-27.2.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-27.2.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-27.2.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-27.2.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/lims/api.py` & `cg-27.2.2/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/lims/batch.py` & `cg-27.2.2/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/lims/order.py` & `cg-27.2.2/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/lims/samplesheet.py` & `cg-27.2.2/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/loqus.py` & `cg-27.2.2/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/madeline/api.py` & `cg-27.2.2/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/mip/confighandler.py` & `cg-27.2.2/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/mutacc_auto.py` & `cg-27.2.2/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-27.2.2/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/orderform/json_orderform_parser.py` & `cg-27.2.2/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/orderform/orderform_parser.py` & `cg-27.2.2/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/osticket.py` & `cg-27.2.2/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/scout/scout_export.py` & `cg-27.2.2/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/scout/scoutapi.py` & `cg-27.2.2/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/slurm/sbatch.py` & `cg-27.2.2/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/slurm/slurm_api.py` & `cg-27.2.2/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/tb/api.py` & `cg-27.2.2/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/tb/models.py` & `cg-27.2.2/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/apps/vogue.py` & `cg-27.2.2/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/add.py` & `cg-27.2.2/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/backup.py` & `cg-27.2.2/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/base.py` & `cg-27.2.2/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/clean.py` & `cg-27.2.2/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/compress/base.py` & `cg-27.2.2/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/compress/fastq.py` & `cg-27.2.2/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/compress/helpers.py` & `cg-27.2.2/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/delete/case.py` & `cg-27.2.2/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/delete/cases.py` & `cg-27.2.2/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/delete/observations.py` & `cg-27.2.2/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/deliver/base.py` & `cg-27.2.2/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/add.py` & `cg-27.2.2/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/base.py` & `cg-27.2.2/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/demux.py` & `cg-27.2.2/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/finish.py` & `cg-27.2.2/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/report.py` & `cg-27.2.2/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/demultiplex/sample_sheet.py` & `cg-27.2.2/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/export.py` & `cg-27.2.2/cg/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/generate/report/base.py` & `cg-27.2.2/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/generate/report/options.py` & `cg-27.2.2/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/generate/report/utils.py` & `cg-27.2.2/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/get.py` & `cg-27.2.2/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/import_cmd.py` & `cg-27.2.2/cg/cli/import_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/set/base.py` & `cg-27.2.2/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/set/families.py` & `cg-27.2.2/cg/cli/set/families.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/set/family.py` & `cg-27.2.2/cg/cli/set/family.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/status.py` & `cg-27.2.2/cg/cli/status.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/store/fastq.py` & `cg-27.2.2/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/store/store.py` & `cg-27.2.2/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/transfer.py` & `cg-27.2.2/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/base.py` & `cg-27.2.2/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/clinical_delivery.py` & `cg-27.2.2/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/coverage.py` & `cg-27.2.2/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/delivery_report.py` & `cg-27.2.2/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/fohm.py` & `cg-27.2.2/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/genotype.py` & `cg-27.2.2/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/gens.py` & `cg-27.2.2/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/gisaid.py` & `cg-27.2.2/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/mutacc.py` & `cg-27.2.2/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/nipt/base.py` & `cg-27.2.2/cg/cli/upload/nipt/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Upload NIPT results via the CLI"""
 
 import logging
 import traceback
-from typing import Optional
+from typing import Optional, List
+from cg.store.models import Analysis
 
 import click
 
 from cg.constants.nipt import Q30_THRESHOLD
 from cg.exc import AnalysisUploadError
 from cg.meta.upload.nipt import NiptUploadAPI
 
@@ -63,16 +64,21 @@
 
     LOG.info("*** NIPT UPLOAD ALL START ***")
 
     nipt_upload_api: NiptUploadAPI = NiptUploadAPI(context.obj)
     nipt_upload_api.set_dry_run(dry_run=dry_run)
 
     all_good = True
-    for analysis_obj in nipt_upload_api.get_all_upload_analyses():
-        internal_id = analysis_obj.family.internal_id
+    analyses: List[Analysis] = nipt_upload_api.get_all_upload_analyses()
+    if not analyses:
+        LOG.info("No analyses found to upload")
+        return
+
+    for analysis in analyses:
+        internal_id = analysis.family.internal_id
 
         if nipt_upload_api.flowcell_passed_qc_value(
             case_id=internal_id, q30_threshold=Q30_THRESHOLD
         ):
             LOG.info("Uploading case: %s", internal_id)
             try:
                 context.invoke(nipt_upload_case, case_id=internal_id, dry_run=dry_run)
```

### Comparing `cg-27.2.1/cg/cli/upload/nipt/ftp.py` & `cg-27.2.2/cg/cli/upload/nipt/ftp.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,12 +55,15 @@
 @click.pass_context
 def nipt_upload_all(context: click.Context, dry_run: bool):
     """Upload all available NIPT results files"""
 
     LOG.info("*** UPLOAD ALL AVAILABLE NIPT RESULTS ***")
 
     nipt_upload_api = NiptUploadAPI(context.obj)
-    upload_nipt_analyses = nipt_upload_api.get_all_upload_analyses()
+    analyses = nipt_upload_api.get_all_upload_analyses()
+    if not analyses:
+        LOG.info("No analyses found for upload")
+        return
 
-    for analysis in upload_nipt_analyses:
+    for analysis in analyses:
         case_id = analysis.family.internal_id
         context.invoke(nipt_upload_case, case_id=case_id, dry_run=dry_run)
```

### Comparing `cg-27.2.1/cg/cli/upload/nipt/statina.py` & `cg-27.2.2/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/observations/observations.py` & `cg-27.2.2/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/observations/utils.py` & `cg-27.2.2/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/scout.py` & `cg-27.2.2/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/utils.py` & `cg-27.2.2/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/validate.py` & `cg-27.2.2/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/upload/vogue.py` & `cg-27.2.2/cg/cli/upload/vogue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Base command for trending"""
 
 import datetime as dt
 import logging
 from pathlib import Path
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple, Dict
 
 import click
 from sqlalchemy.orm import Query
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import Pipeline
 from cg.exc import AnalysisUploadError
 from cg.meta.upload.vogue import UploadVogueAPI
 from cg.meta.workflow.mip_dna import MipDNAAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.store import Store
-from cg.store.models import FamilySample
+from cg.store.models import FamilySample, Analysis
 from housekeeper.store.models import File, Version
+from cg.utils.dispatcher import Dispatcher
 
 LOG = logging.getLogger(__name__)
 
 VOGUE_VALID_BIOINFO = [str(Pipeline.BALSAMIC)]
 
 
 def validate_date(context, param, date_: str) -> Optional[dt.date]:
@@ -220,16 +221,31 @@
     completed_before: Optional[str],
     dry: bool,
 ):
     """Load all cases with recent analysis and a multiqc-json to the trending database."""
 
     status_db: Store = context.obj.status_db
     housekeeper_api: HousekeeperAPI = context.obj.housekeeper_api
+    input_dict: Dict[str, Any] = {
+        "completed_at_after": completed_after,
+        "completed_at_before": completed_before,
+    }
+    function_dispatcher: Dispatcher = Dispatcher(
+        functions=[
+            status_db.get_analysis_for_vogue_upload_completed_after,
+            status_db.get_analysis_for_vogue_upload_completed_before,
+            status_db.get_analyses_for_vogue_upload,
+        ],
+        input_dict=input_dict,
+    )
+    analyses: List[Analysis] = function_dispatcher(input_dict=input_dict)
+    if not analyses:
+        LOG.info("No analyses found for upload to trending.")
+        return
 
-    analyses: Query = status_db.analyses_ready_for_vogue_upload(completed_after, completed_before)
     for analysis in analyses:
         case_name: str = analysis.family.internal_id
         version_obj: Version = housekeeper_api.last_version(case_name)
         if not version_obj:
             continue
 
         # confirm multiqc.json exists
```

### Comparing `cg-27.2.1/cg/cli/workflow/balsamic/base.py` & `cg-27.2.2/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/balsamic/options.py` & `cg-27.2.2/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/balsamic/pon.py` & `cg-27.2.2/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/balsamic/qc.py` & `cg-27.2.2/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/balsamic/umi.py` & `cg-27.2.2/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/base.py` & `cg-27.2.2/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/commands.py` & `cg-27.2.2/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/fastq/base.py` & `cg-27.2.2/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/fluffy/base.py` & `cg-27.2.2/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/microsalt/base.py` & `cg-27.2.2/cg/cli/workflow/microsalt/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,23 +272,31 @@
 @OPTION_DRY_RUN
 @click.pass_context
 def upload_vogue_latest(context: click.Context, dry_run: bool) -> None:
     """Upload the trending reports for all un-uploaded latest analyses to Vogue"""
 
     EXIT_CODE: int = EXIT_SUCCESS
     analysis_api: MicrosaltAnalysisAPI = context.obj.meta_apis["analysis_api"]
-    latest_analyses = list(analysis_api.status_db.get_latest_microsalt_analysis_to_upload())
+    latest_analyses: List[
+        Analysis
+    ] = analysis_api.status_db.get_latest_analysis_to_upload_for_pipeline(
+        pipeline=Pipeline.MICROSALT
+    )
+    if not latest_analyses:
+        LOG.info("No new analyses to upload to Vogue!")
+        return
+
     for analysis in latest_analyses:
-        unique_id: str = analysis.family.internal_id
+        case_internal_id: str = analysis.family.internal_id if analysis.family else None
         try:
-            context.invoke(upload_analysis_vogue, unique_id=unique_id, dry_run=dry_run)
+            context.invoke(upload_analysis_vogue, unique_id=case_internal_id, dry_run=dry_run)
         except Exception as error:
             LOG.error(
                 "Could not upload data for %s to vogue, exception %s",
-                unique_id,
+                case_internal_id,
                 error.__class__.__name__,
             )
             EXIT_CODE: int = EXIT_FAIL
 
     if EXIT_CODE:
         raise click.Abort
```

### Comparing `cg-27.2.1/cg/cli/workflow/mip/base.py` & `cg-27.2.2/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/mip/options.py` & `cg-27.2.2/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/mip_dna/base.py` & `cg-27.2.2/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/mip_rna/base.py` & `cg-27.2.2/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/mutant/base.py` & `cg-27.2.2/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/nextflow/options.py` & `cg-27.2.2/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/rnafusion/base.py` & `cg-27.2.2/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/cli/workflow/rnafusion/options.py` & `cg-27.2.2/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/__init__.py` & `cg-27.2.2/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/compression.py` & `cg-27.2.2/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/constants.py` & `cg-27.2.2/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/delivery.py` & `cg-27.2.2/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/demultiplexing.py` & `cg-27.2.2/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/encryption.py` & `cg-27.2.2/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/gene_panel.py` & `cg-27.2.2/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/housekeeper_tags.py` & `cg-27.2.2/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/lims.py` & `cg-27.2.2/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/nextflow.py` & `cg-27.2.2/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/observations.py` & `cg-27.2.2/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/orderforms.py` & `cg-27.2.2/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/priority.py` & `cg-27.2.2/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/report.py` & `cg-27.2.2/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/rnafusion.py` & `cg-27.2.2/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/scout_upload.py` & `cg-27.2.2/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/sequencing.py` & `cg-27.2.2/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/constants/subject.py` & `cg-27.2.2/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/exc.py` & `cg-27.2.2/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/io/api.py` & `cg-27.2.2/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/io/controller.py` & `cg-27.2.2/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/io/json.py` & `cg-27.2.2/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/io/yaml.py` & `cg-27.2.2/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/archive/ddn_dataflow.py` & `cg-27.2.2/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/backup/backup.py` & `cg-27.2.2/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/backup/pdc.py` & `cg-27.2.2/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/clean/api.py` & `cg-27.2.2/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-27.2.2/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/clean/flow_cell_run_directories.py` & `cg-27.2.2/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/compress/compress.py` & `cg-27.2.2/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/compress/files.py` & `cg-27.2.2/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/deliver.py` & `cg-27.2.2/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/deliver_ticket.py` & `cg-27.2.2/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-27.2.2/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-27.2.2/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/demultiplex/files.py` & `cg-27.2.2/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/encryption/encryption.py` & `cg-27.2.2/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/invoice.py` & `cg-27.2.2/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/meta.py` & `cg-27.2.2/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/observations/balsamic_observations_api.py` & `cg-27.2.2/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-27.2.2/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/observations/observations_api.py` & `cg-27.2.2/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/api.py` & `cg-27.2.2/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/case_submitter.py` & `cg-27.2.2/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/fastq_submitter.py` & `cg-27.2.2/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/lims.py` & `cg-27.2.2/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/metagenome_submitter.py` & `cg-27.2.2/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/microbial_submitter.py` & `cg-27.2.2/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/pool_submitter.py` & `cg-27.2.2/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-27.2.2/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/submitter.py` & `cg-27.2.2/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/orders/ticket_handler.py` & `cg-27.2.2/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/balsamic.py` & `cg-27.2.2/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/balsamic_umi.py` & `cg-27.2.2/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/field_validators.py` & `cg-27.2.2/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/mip_dna.py` & `cg-27.2.2/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/report_api.py` & `cg-27.2.2/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/templates/balsamic_report.html` & `cg-27.2.2/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/templates/bootstrap.html` & `cg-27.2.2/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/report/templates/mip-dna_report.html` & `cg-27.2.2/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/rsync/rsync_api.py` & `cg-27.2.2/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/tar/tar.py` & `cg-27.2.2/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/transfer/external_data.py` & `cg-27.2.2/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/transfer/flowcell.py` & `cg-27.2.2/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/transfer/lims.py` & `cg-27.2.2/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/balsamic/balsamic.py` & `cg-27.2.2/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/coverage.py` & `cg-27.2.2/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/fohm/fohm.py` & `cg-27.2.2/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/gisaid/constants.py` & `cg-27.2.2/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/gisaid/gisaid.py` & `cg-27.2.2/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/gisaid/models.py` & `cg-27.2.2/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/gt.py` & `cg-27.2.2/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/mip/mip_dna.py` & `cg-27.2.2/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/mip/mip_rna.py` & `cg-27.2.2/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/mutacc.py` & `cg-27.2.2/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/nipt/nipt.py` & `cg-27.2.2/cg/meta/upload/nipt/nipt.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,17 @@
         results_file: Path = self.root_dir / hk_results_file
 
         if not results_file.exists():
             raise FileNotFoundError(f"Results file {results_file} not found on hasta!")
 
         return results_file
 
-    def get_all_upload_analyses(self) -> Iterable[Analysis]:
+    def get_all_upload_analyses(self) -> List[Analysis]:
         """Gets all nipt analyses that are ready to be uploaded"""
-        return self.status_db.get_latest_nipt_analysis_to_upload()
+        return self.status_db.get_latest_analysis_to_upload_for_pipeline(pipeline=Pipeline.FLUFFY)
 
     def upload_to_ftp_server(self, results_file: Path) -> None:
         """Upload the result file to the ftp server"""
         if self.dry_run:
             LOG.info(f"Would upload results file to ftp server: {results_file}")
             return
         transport: paramiko.Transport = paramiko.Transport((self.sftp_host, self.sftp_port))
```

### Comparing `cg-27.2.1/cg/meta/upload/rnafusion/rnafusion.py` & `cg-27.2.2/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-27.2.2/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-27.2.2/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/hk_tags.py` & `cg-27.2.2/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-27.2.2/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-27.2.2/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-27.2.2/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-27.2.2/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/upload_api.py` & `cg-27.2.2/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/upload/vogue.py` & `cg-27.2.2/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/analysis.py` & `cg-27.2.2/cg/meta/workflow/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,16 +247,18 @@
             LOG.info("Action %s set for case %s", action, case_id)
             return
         LOG.warning(
             f"Action '{action}' not permitted by StatusDB and will not be set for case {case_id}"
         )
 
     def get_analyses_to_clean(self, before: dt.datetime) -> List[Analysis]:
-        analyses_to_clean = self.status_db.analyses_to_clean(pipeline=self.pipeline, before=before)
-        return analyses_to_clean.all()
+        analyses_to_clean = self.status_db.get_analyses_to_clean(
+            pipeline=self.pipeline, before=before
+        )
+        return analyses_to_clean
 
     def get_cases_to_analyze(self) -> List[Family]:
         return self.status_db.cases_to_analyze(
             pipeline=self.pipeline, threshold=self.threshold_reads
         )
 
     def get_running_cases(self) -> List[Family]:
```

### Comparing `cg-27.2.1/cg/meta/workflow/balsamic.py` & `cg-27.2.2/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/balsamic_pon.py` & `cg-27.2.2/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/balsamic_qc.py` & `cg-27.2.2/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/balsamic_umi.py` & `cg-27.2.2/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/fastq.py` & `cg-27.2.2/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/fluffy.py` & `cg-27.2.2/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/microsalt.py` & `cg-27.2.2/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/mip.py` & `cg-27.2.2/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/mip_dna.py` & `cg-27.2.2/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/mip_rna.py` & `cg-27.2.2/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/mutant.py` & `cg-27.2.2/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/nextflow_common.py` & `cg-27.2.2/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/prepare_fastq.py` & `cg-27.2.2/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/rnafusion.py` & `cg-27.2.2/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/meta/workflow/tower_common.py` & `cg-27.2.2/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/balsamic/config.py` & `cg-27.2.2/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/balsamic/metrics.py` & `cg-27.2.2/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/cg_config.py` & `cg-27.2.2/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/cgstats/stats_sample.py` & `cg-27.2.2/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/compression_data.py` & `cg-27.2.2/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/deliverables/metric_deliverables.py` & `cg-27.2.2/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/demultiplex/demux_results.py` & `cg-27.2.2/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/demultiplex/flow_cell.py` & `cg-27.2.2/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/demultiplex/run_parameters.py` & `cg-27.2.2/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/demultiplex/sbatch.py` & `cg-27.2.2/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/file_data.py` & `cg-27.2.2/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/invoice/invoice.py` & `cg-27.2.2/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/lims/sample.py` & `cg-27.2.2/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/mip/mip_config.py` & `cg-27.2.2/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-27.2.2/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/mip/mip_sample_info.py` & `cg-27.2.2/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/nextflow/deliverables.py` & `cg-27.2.2/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/nextflow/sample.py` & `cg-27.2.2/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/observations/input_files.py` & `cg-27.2.2/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/constants.py` & `cg-27.2.2/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/excel_sample.py` & `cg-27.2.2/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/json_sample.py` & `cg-27.2.2/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/order.py` & `cg-27.2.2/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/orderform_schema.py` & `cg-27.2.2/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/sample_base.py` & `cg-27.2.2/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/orders/samples.py` & `cg-27.2.2/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/report/metadata.py` & `cg-27.2.2/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/report/report.py` & `cg-27.2.2/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/report/sample.py` & `cg-27.2.2/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/report/validators.py` & `cg-27.2.2/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/rnafusion/rnafusion_sample.py` & `cg-27.2.2/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/scout/scout_load_config.py` & `cg-27.2.2/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/slurm/sbatch.py` & `cg-27.2.2/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/models/workflow/mutant.py` & `cg-27.2.2/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/resources/20181012_Indices.csv` & `cg-27.2.2/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/resources/rnafusion_bundle_filenames.csv` & `cg-27.2.2/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/admin.py` & `cg-27.2.2/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/api.py` & `cg-27.2.2/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/app.py` & `cg-27.2.2/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/config.py` & `cg-27.2.2/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/ext.py` & `cg-27.2.2/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/invoices/templates/invoices/index.html` & `cg-27.2.2/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-27.2.2/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/invoices/templates/invoices/layout.html` & `cg-27.2.2/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/invoices/templates/invoices/new.html` & `cg-27.2.2/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/server/invoices/views.py` & `cg-27.2.2/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/add.py` & `cg-27.2.2/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/core.py` & `cg-27.2.2/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/delete.py` & `cg-27.2.2/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/find_basic_data.py` & `cg-27.2.2/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/find_business_data.py` & `cg-27.2.2/cg/store/api/find_business_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,67 +74,69 @@
 
         return (
             self.get_case_by_internal_id(internal_id=case_id)
             .links[ListIndexes.FIRST.value]
             .sample.application_version.application
         )
 
-    def analyses_ready_for_vogue_upload(
-        self,
-        completed_after: Optional[dt.date],
-        completed_before: Optional[dt.date],
-    ) -> Query:
-        """Fetch all cases with a finished analysis that has not been uploaded to Vogue.
-        Optionally fetch those cases finished before and/or after a specified date"""
-        records = self.latest_analyses().filter(Analysis.uploaded_to_vogue_at.is_(None))
-
-        if completed_after:
-            records = records.filter(Analysis.completed_at > completed_after)
-        if completed_before:
-            records = records.filter(Analysis.completed_at < completed_before)
-
-        return records
-
-    def get_latest_nipt_analysis_to_upload(self):
-        """Return latest nipt analysis."""
-        latest_nipt_analyses = self.latest_analyses().filter(Analysis.pipeline == Pipeline.FLUFFY)
-        return latest_nipt_analyses.filter(Analysis.uploaded_at.is_(None))
+    def get_analysis_for_vogue_upload_completed_after(self, completed_at_after: dt.datetime):
+        """Return all cases completed after a given date that have not been uploaded to Vogue."""
+        filter_functions = [
+            AnalysisFilter.FILTER_NOT_UPLOADED_TO_VOGUE,
+            AnalysisFilter.FILTER_COMPLETED_AT_AFTER,
+        ]
+        return apply_analysis_filter(
+            analyses=self._get_latest_analyses_for_cases_query(),
+            filter_functions=filter_functions,
+            completed_at_date=completed_at_after,
+        ).all()
 
-    def get_latest_microsalt_analysis_to_upload(self):
-        """Return latest mircosalt analysis."""
-        return (
-            self.latest_analyses()
-            .filter(Analysis.pipeline == Pipeline.MICROSALT)
-            .filter(Analysis.uploaded_at.is_(None))
-        )
+    def get_analysis_for_vogue_upload_completed_before(self, completed_at_before: dt.datetime):
+        """Return all cases completed before a given date that have not been uploaded to Vogue."""
+        filter_functions = [
+            AnalysisFilter.FILTER_NOT_UPLOADED_TO_VOGUE,
+            AnalysisFilter.FILTER_COMPLETED_AT_BEFORE,
+        ]
+        return apply_analysis_filter(
+            analyses=self._get_latest_analyses_for_cases_query(),
+            filter_functions=filter_functions,
+            completed_at_date=completed_at_before,
+        ).all()
 
-    def latest_analyses(self) -> Query:
-        """Fetch latest analysis for all cases."""
+    def get_analyses_for_vogue_upload(
+        self,
+    ) -> List[Analysis]:
+        """Return the latest analysis not uploaded to Vogue for each case."""
 
-        records = self.Analysis.query
-        sub_query = (
-            self.Analysis.query.join(Analysis.family)
-            .group_by(Family.id)
-            .with_entities(Analysis.family_id, func.max(Analysis.started_at).label("started_at"))
-            .subquery()
-        )
-        records = records.join(
-            sub_query,
-            and_(
-                self.Analysis.family_id == sub_query.c.family_id,
-                self.Analysis.started_at == sub_query.c.started_at,
-            ),
-        )
-        return records
+        return apply_analysis_filter(
+            analyses=self._get_latest_analyses_for_cases_query(),
+            filter_functions=[AnalysisFilter.FILTER_NOT_UPLOADED_TO_VOGUE],
+        ).all()
+
+    def get_analyses_for_each_case_with_latest_started_at_date(self) -> List[Analysis]:
+        """Return analysis for all cases and latest started at date."""
+        return self._get_latest_analyses_for_cases_query().all()
+
+    def get_latest_analysis_to_upload_for_pipeline(self, pipeline: str = None) -> List[Analysis]:
+        """Return latest not uploaded analysis for each case given a pipeline."""
+        filter_functions: List[AnalysisFilter] = [
+            AnalysisFilter.FILTER_WITH_PIPELINE,
+            AnalysisFilter.FILTER_IS_NOT_UPLOADED,
+        ]
+        return apply_analysis_filter(
+            analyses=self._get_latest_analyses_for_cases_query(),
+            filter_functions=filter_functions,
+            pipeline=pipeline,
+        ).all()
 
     def get_analysis_by_case_entry_id_and_started_at(
         self, case_entry_id: int, started_at_date: dt.datetime
     ) -> Analysis:
         """Fetch an analysis."""
-        filter_functions = [
+        filter_functions: List[AnalysisFilter] = [
             AnalysisFilter.FILTER_BY_CASE_ENTRY_ID,
             AnalysisFilter.FILTER_BY_STARTED_AT,
         ]
 
         return apply_analysis_filter(
             analyses=self._get_query(Analysis),
             case_entry_id=case_entry_id,
```

### Comparing `cg-27.2.1/cg/store/api/import_func.py` & `cg-27.2.2/cg/store/api/import_func.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/models.py` & `cg-27.2.2/cg/store/api/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/api/status.py` & `cg-27.2.2/cg/store/api/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,41 +587,42 @@
         )
 
     def analyses_to_upload(self, pipeline: Pipeline = None) -> List[Analysis]:
         """Return analyses that have not been uploaded."""
         analysis_filter_functions: List[AnalysisFilter] = [
             AnalysisFilter.FILTER_WITH_PIPELINE,
             AnalysisFilter.FILTER_COMPLETED,
-            AnalysisFilter.FILTER_NOT_UPLOADED,
+            AnalysisFilter.FILTER_IS_NOT_UPLOADED,
             AnalysisFilter.FILTER_VALID_IN_PRODUCTION,
             AnalysisFilter.ORDER_BY_COMPLETED_AT,
         ]
         return apply_analysis_filter(
             filter_functions=analysis_filter_functions,
             analyses=self._get_join_analysis_case_query(),
             pipeline=pipeline,
         ).all()
 
-    def analyses_to_clean(
+    def get_analyses_to_clean(
         self, before: datetime = datetime.now(), pipeline: Pipeline = None
-    ) -> Query:
-        """Fetch analyses that haven't been cleaned."""
-        records = self.latest_analyses()
-        records = records.filter(
-            Analysis.uploaded_at.isnot(None),
-            Analysis.cleaned_at.is_(None),
-            Analysis.started_at <= before,
-            Family.action.is_(None),
-        )
+    ) -> List[Analysis]:
+        """Return analyses that haven't been cleaned."""
+        filter_functions: List[AnalysisFilter] = [
+            AnalysisFilter.FILTER_IS_UPLOADED,
+            AnalysisFilter.FILTER_IS_NOT_CLEANED,
+            AnalysisFilter.FILTER_STARTED_AT_BEFORE,
+            AnalysisFilter.FILTER_CASE_ACTION_IS_NONE,
+        ]
         if pipeline:
-            records = records.filter(
-                Analysis.pipeline == str(pipeline),
-            )
-
-        return records
+            filter_functions.append(AnalysisFilter.FILTER_WITH_PIPELINE)
+        return apply_analysis_filter(
+            filter_functions=filter_functions,
+            analyses=self._get_latest_analyses_for_cases_query(),
+            pipeline=pipeline,
+            started_at_date=before,
+        ).all()
 
     def get_analyses_for_case_and_pipeline_started_at_before(
         self,
         pipeline: Pipeline,
         started_at_before: datetime,
         case_internal_id: str,
     ) -> List[Analysis]:
@@ -745,15 +746,15 @@
             filter_functions=[CaseFilter.GET_WITH_SCOUT_DELIVERY],
             cases=self._get_join_analysis_case_query(),
             pipeline=pipeline,
         )
         analysis_filter_functions: List[AnalysisFilter] = [
             AnalysisFilter.FILTER_REPORT_BY_PIPELINE,
             AnalysisFilter.FILTER_WITH_DELIVERY_REPORT,
-            AnalysisFilter.FILTER_NOT_UPLOADED,
+            AnalysisFilter.FILTER_IS_NOT_UPLOADED,
             AnalysisFilter.FILTER_VALID_IN_PRODUCTION,
             AnalysisFilter.ORDER_BY_COMPLETED_AT,
         ]
         return apply_analysis_filter(
             filter_functions=analysis_filter_functions, analyses=records, pipeline=pipeline
         )
```

### Comparing `cg-27.2.1/cg/store/filters/status_analysis_filters.py` & `cg-27.2.2/cg/store/filters/status_analysis_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Callable
 from enum import Enum
-from sqlalchemy.orm import Query
+from sqlalchemy.orm import Query, join
 
 
 from cg.constants import REPORT_SUPPORTED_PIPELINES
 from cg.constants.constants import VALID_DATA_IN_PRODUCTION
 from cg.store.models import Analysis, Family
 from cgmodels.cg.constants import Pipeline
 from datetime import datetime
@@ -111,14 +111,19 @@
 
 
 def filter_analyses_not_cleaned(analyses: Query, **kwargs) -> Query:
     """Return a query of analyses that have not been cleaned."""
     return analyses.filter(Analysis.cleaned_at.is_(None))
 
 
+def filter_analysis_case_action_is_none(analyses: Query, **kwargs) -> Query:
+    """Return a query of analyses that do not have active cases."""
+    return analyses.join(Family).filter(Family.action.is_(None))
+
+
 def apply_analysis_filter(
     filter_functions: List[Callable],
     analyses: Query,
     pipeline: Pipeline = None,
     case_entry_id: int = None,
     completed_at_date: datetime = None,
     started_at_date: datetime = None,
@@ -139,22 +144,23 @@
 class AnalysisFilter(Enum):
     """Define Analysis filter functions."""
 
     FILTER_VALID_IN_PRODUCTION: Callable = filter_valid_analyses_in_production
     FILTER_WITH_PIPELINE: Callable = filter_analyses_with_pipeline
     FILTER_COMPLETED: Callable = filter_completed_analyses
     FILTER_NOT_COMPLETED: Callable = filter_not_completed_analyses
-    FILTER_UPLOADED: Callable = filter_uploaded_analyses
-    FILTER_NOT_UPLOADED: Callable = filter_not_uploaded_analyses
+    FILTER_IS_UPLOADED: Callable = filter_uploaded_analyses
+    FILTER_IS_NOT_UPLOADED: Callable = filter_not_uploaded_analyses
     FILTER_WITH_DELIVERY_REPORT: Callable = filter_analyses_with_delivery_report
     FILTER_WITHOUT_DELIVERY_REPORT: Callable = filter_analyses_without_delivery_report
     FILTER_REPORT_BY_PIPELINE: Callable = filter_report_analyses_by_pipeline
     FILTER_BY_CASE_ENTRY_ID: Callable = filter_analyses_by_case_entry_id
     FILTER_COMPLETED_AT_AFTER: Callable = filter_analyses_completed_after
     FILTER_COMPLETED_AT_BEFORE: Callable = filter_analyses_completed_before
     FILTER_NOT_UPLOADED_TO_VOGUE: Callable = filter_analyses_not_uploaded_to_vogue
-    FILTER_NOT_CLEANED: Callable = filter_analyses_not_cleaned
+    FILTER_IS_NOT_CLEANED: Callable = filter_analyses_not_cleaned
     FILTER_STARTED_AT_BEFORE: Callable = filter_analyses_started_before
     FILTER_BY_STARTED_AT: Callable = filter_analyses_by_started_at
+    FILTER_CASE_ACTION_IS_NONE: Callable = filter_analysis_case_action_is_none
     ORDER_BY_UPLOADED_AT: Callable = order_analyses_by_uploaded_at_asc
     ORDER_BY_COMPLETED_AT: Callable = order_analyses_by_completed_at_asc
     ORDER_BY_STARTED_AT_DESC: Callable = order_analyses_by_started_at_desc
```

### Comparing `cg-27.2.1/cg/store/filters/status_application_filters.py` & `cg-27.2.2/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_application_version_filters.py` & `cg-27.2.2/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_bed_filters.py` & `cg-27.2.2/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_bed_version_filters.py` & `cg-27.2.2/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_case_filters.py` & `cg-27.2.2/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_case_sample_filters.py` & `cg-27.2.2/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_collaboration_filters.py` & `cg-27.2.2/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_customer_filters.py` & `cg-27.2.2/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_flow_cell_filters.py` & `cg-27.2.2/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_invoice_filters.py` & `cg-27.2.2/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_organism_filters.py` & `cg-27.2.2/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_panel_filters.py` & `cg-27.2.2/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_pool_filters.py` & `cg-27.2.2/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_sample_filters.py` & `cg-27.2.2/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/filters/status_user_filters.py` & `cg-27.2.2/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/store/models.py` & `cg-27.2.2/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/checksum/checksum.py` & `cg-27.2.2/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/click/EnumChoice.py` & `cg-27.2.2/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/commands.py` & `cg-27.2.2/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/date.py` & `cg-27.2.2/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/dict.py` & `cg-27.2.2/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/dispatcher.py` & `cg-27.2.2/cg/utils/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self.input_dict: Dict[str, any] = input_dict
         self.dispatch_table: Dict[Tuple[str], Callable] = self._generate_dispatch_table()
 
     def __call__(self, input_dict: Dict[str, Any]):
         """Call the dispatcher with the input dict"""
         parameters_not_none, parameter_values_not_none = self._parse_input_dict(input_dict)
         if parameters_not_none not in self.dispatch_table:
-            raise ValueError(f"No matching function found for arguments: {input_dict.keys()}")
+            raise ValueError(f"No matching function found for arguments: {parameters_not_none}")
         return self.dispatch_table[parameters_not_none](
             **dict(zip(parameters_not_none, parameter_values_not_none))
         )
 
     def _parse_input_dict(self, input_dict: Dict[str, Any]) -> [Tuple[str], Tuple[Any]]:
         """Parse the input dict and return a tuple of parameters and values that are not None"""
         parameters_not_none: List[str] = []
```

### Comparing `cg-27.2.1/cg/utils/email.py` & `cg-27.2.2/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/flask/enum.py` & `cg-27.2.2/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg/utils/utils.py` & `cg-27.2.2/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/cg.egg-info/PKG-INFO` & `cg-27.2.2/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 27.2.1
+Version: 27.2.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-27.2.1/cg.egg-info/SOURCES.txt` & `cg-27.2.2/cg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/requirements.txt` & `cg-27.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/setup.py` & `cg-27.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="27.2.1",
+    version="27.2.2",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-27.2.1/tests/apps/cgstats/conftest.py` & `cg-27.2.2/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-27.2.2/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/crud/test_delete.py` & `cg-27.2.2/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-27.2.2/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-27.2.2/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/parsers/test_run_info.py` & `cg-27.2.2/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/test_cgstats_create.py` & `cg-27.2.2/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/cgstats/test_stats.py` & `cg-27.2.2/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/conftest.py` & `cg-27.2.2/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/coverage/test_coverage.py` & `cg-27.2.2/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/crunchy/conftest.py` & `cg-27.2.2/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-27.2.2/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/crunchy/test_config.py` & `cg-27.2.2/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/crunchy/test_crunchy.py` & `cg-27.2.2/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-27.2.2/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/demultiplex/conftest.py` & `cg-27.2.2/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-27.2.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-27.2.2/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/demultiplex/test_parse_run_parameters.py` & `cg-27.2.2/tests/apps/demultiplex/test_parse_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/demultiplex/test_sample_sheet.py` & `cg-27.2.2/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/gens/test_gens_api.py` & `cg-27.2.2/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/gt/conftest.py` & `cg-27.2.2/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/gt/test_gt_api.py` & `cg-27.2.2/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/conftest.py` & `cg-27.2.2/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test__getattr__.py` & `cg-27.2.2/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test_add_file.py` & `cg-27.2.2/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test_bundles.py` & `cg-27.2.2/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test_core.py` & `cg-27.2.2/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test_file.py` & `cg-27.2.2/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/hk/test_version.py` & `cg-27.2.2/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/lims/conftest.py` & `cg-27.2.2/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/lims/test_api.py` & `cg-27.2.2/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/loqus/conftest.py` & `cg-27.2.2/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-27.2.2/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/madeline/conftest.py` & `cg-27.2.2/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/madeline/test_madeline.py` & `cg-27.2.2/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/mip/conftest.py` & `cg-27.2.2/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/mip/test_config_mip.py` & `cg-27.2.2/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/mutacc_auto/conftest.py` & `cg-27.2.2/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-27.2.2/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/orderform/conftest.py` & `cg-27.2.2/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-27.2.2/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-27.2.2/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-27.2.2/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/orderform/test_orderform_parser.py` & `cg-27.2.2/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/scout/conftest.py` & `cg-27.2.2/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/scout/test_get_causative_variants.py` & `cg-27.2.2/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/scout/test_get_scout_cases.py` & `cg-27.2.2/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/scout/test_scout_load_config.py` & `cg-27.2.2/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/scout/test_scout_models.py` & `cg-27.2.2/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/slurm/conftest.py` & `cg-27.2.2/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/slurm/test_slurm_api.py` & `cg-27.2.2/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/test_apps_environ.py` & `cg-27.2.2/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/test_osticket.py` & `cg-27.2.2/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/vogue/conftest.py` & `cg-27.2.2/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/apps/vogue/test_vogue_api.py` & `cg-27.2.2/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/add/test_cli_add.py` & `cg-27.2.2/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/add/test_cli_add_customer.py` & `cg-27.2.2/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/add/test_cli_add_family.py` & `cg-27.2.2/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/add/test_cli_add_relationship.py` & `cg-27.2.2/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/add/test_cli_add_sample.py` & `cg-27.2.2/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/backup/conftest.py` & `cg-27.2.2/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/backup/test_backup_command.py` & `cg-27.2.2/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/clean/conftest.py` & `cg-27.2.2/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/clean/test_balsamic_clean.py` & `cg-27.2.2/tests/cli/clean/test_balsamic_clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     # WHEN dry running with dry run specified
     result = cli_runner.invoke(clean_run_dir, [balsamic_case_clean, "-d", "-y"], obj=clean_context)
     # THEN command should say it would have deleted
     assert result.exit_code == EXIT_SUCCESS
     assert "Would have deleted" in caplog.text
     assert balsamic_case_clean in caplog.text
-    assert analysis_to_clean in base_store.analyses_to_clean(pipeline=Pipeline.BALSAMIC)
+    assert analysis_to_clean in base_store.get_analyses_to_clean(pipeline=Pipeline.BALSAMIC)
 
 
 def test_cleaned_at_valid(
     balsamic_case_clean: str, cli_runner: CliRunner, clean_context: CGConfig, caplog, mocker
 ):
     """Test command with dry run options"""
     # GIVEN a case on disk that could be deleted
```

### Comparing `cg-27.2.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-27.2.2/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-27.2.2/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-27.2.2/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/clean/test_microbial_clean.py` & `cg-27.2.2/tests/cli/clean/test_microbial_clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     # THEN command should say it would have deleted
     assert result.exit_code == EXIT_SUCCESS
     assert "Would have deleted" in caplog.text
     assert microsalt_case_clean_dry in caplog.text
 
     # THEN the analysis should still be in the analyses_to_clean query since this is a dry-ryn
     assert analysis_to_clean.cleaned_at == None
-    assert analysis_to_clean in base_store.analyses_to_clean(pipeline=Pipeline.MICROSALT)
+    assert analysis_to_clean in base_store.get_analyses_to_clean(pipeline=Pipeline.MICROSALT)
 
 
 def test_clean_run(
     microsalt_case_clean: str,
     cli_runner: CliRunner,
     clean_context_microsalt: CGConfig,
     timestamp_yesterday: dt.datetime,
@@ -103,8 +103,8 @@
     # THEN command should say it would have deleted
     assert result.exit_code == EXIT_SUCCESS
     assert microsalt_case_clean in caplog.text
     assert "Cleaned" in caplog.text
 
     # THEN the analysis should no longer be in the analyses_to_clean query
     assert isinstance(analysis_to_clean.cleaned_at, dt.datetime)
-    assert analysis_to_clean not in base_store.analyses_to_clean(pipeline=Pipeline.MICROSALT)
+    assert analysis_to_clean not in base_store.get_analyses_to_clean(pipeline=Pipeline.MICROSALT)
```

### Comparing `cg-27.2.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-27.2.2/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/compress/conftest.py` & `cg-27.2.2/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-27.2.2/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-27.2.2/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/compress/test_compress_helpers.py` & `cg-27.2.2/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/compress/test_store_fastq.py` & `cg-27.2.2/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/conftest.py` & `cg-27.2.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/delete/test_case.py` & `cg-27.2.2/tests/cli/delete/test_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/delete/test_cases.py` & `cg-27.2.2/tests/cli/delete/test_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/deliver/conftest.py` & `cg-27.2.2/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/deliver/test_deliver_base.py` & `cg-27.2.2/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/deliver/test_rsync_base.py` & `cg-27.2.2/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-27.2.2/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/conftest.py` & `cg-27.2.2/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_add_flowcell.py` & `cg-27.2.2/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-27.2.2/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-27.2.2/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-27.2.2/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_stats_command.py` & `cg-27.2.2/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-27.2.2/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/generate/report/conftest.py` & `cg-27.2.2/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-27.2.2/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/generate/report/test_utils.py` & `cg-27.2.2/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/generate/test_cli_base.py` & `cg-27.2.2/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/get/test_cli_get.py` & `cg-27.2.2/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/get/test_cli_get_analysis.py` & `cg-27.2.2/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/get/test_cli_get_case.py` & `cg-27.2.2/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-27.2.2/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/get/test_cli_get_sample.py` & `cg-27.2.2/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/conftest.py` & `cg-27.2.2/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_families.py` & `cg-27.2.2/tests/cli/set/test_families.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_family.py` & `cg-27.2.2/tests/cli/set/test_family.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_flowcell.py` & `cg-27.2.2/tests/cli/set/test_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_list_keys.py` & `cg-27.2.2/tests/cli/set/test_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_sample.py` & `cg-27.2.2/tests/cli/set/test_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/set/test_samples.py` & `cg-27.2.2/tests/cli/set/test_samples.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/store/test_fastq.py` & `cg-27.2.2/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/test_base.py` & `cg-27.2.2/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/test_clean.py` & `cg-27.2.2/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/test_cli_status_cases.py` & `cg-27.2.2/tests/cli/test_cli_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/conftest.py` & `cg-27.2.2/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_scout.py` & `cg-27.2.2/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/upload/test_cli_upload_vogue.py` & `cg-27.2.2/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,100 @@
 """ Test cg.cli.upload.vogue module """
 
 import logging
 
-from cg.cli.upload.vogue import flowcells, reagent_labels, samples
+from cg.cli.upload.vogue import flowcells, reagent_labels, samples, bioinfo_all
 from cg.models.cg_config import CGConfig
 from click.testing import CliRunner
 
 
 def test_cli_upload_vogue_reagent_labes(upload_context: CGConfig, cli_runner: CliRunner, caplog):
     """Testing cli for upload vogue reagent_labels with correct argument"""
 
     # GIVEN a vogue api
     caplog.set_level(logging.DEBUG)
 
     # WHEN running vogue load reagent_labels with the days argument
-    result = cli_runner.invoke(reagent_labels, ["-d", 1], obj=upload_context)
+    result = cli_runner.invoke(cli=reagent_labels, args=["-d", 1], obj=upload_context)
 
     # THEN assert that the correct information was communicated
     assert "REAGENT LABELS" in caplog.text
     # THEN assert that the program exits without errors
     assert result.exit_code == 0
 
 
 def test_cli_upload_vogue_reagent_labes_no_days(upload_context: CGConfig, cli_runner: CliRunner):
     """ """
 
     # GIVEN a vogue api
 
     # WHEN running vogue load reagent_labels without the days argument
-    result = cli_runner.invoke(reagent_labels, [], obj=upload_context)
+    result = cli_runner.invoke(cli=reagent_labels, args=[], obj=upload_context)
 
     # THEN assert that the program exits with a non zero exit code
     assert result.exit_code != 0
 
 
 def test_cli_upload_vogue_samples(upload_context: CGConfig, cli_runner: CliRunner, caplog):
     """Testing cli for upload vogue samples with correct argument"""
 
     # GIVEN a vogue api
     caplog.set_level(logging.DEBUG)
 
     # WHEN running vogue load samples with the days argument
-    result = cli_runner.invoke(samples, ["-d", 1], obj=upload_context)
+    result = cli_runner.invoke(cli=samples, args=["-d", 1], obj=upload_context)
 
     # THEN assert that the correct information was communicated
     assert "SAMPLES" in caplog.text
     # THEN assert that the program exits without errors
     assert result.exit_code == 0
 
 
 def test_cli_upload_vogue_samples_no_days(upload_context: CGConfig, cli_runner: CliRunner):
     """Testing cli for upload vogue samples with wrong argument"""
 
     # GIVEN a vogue api
 
     # WHEN running vogue load samples without the days argument
-    result = cli_runner.invoke(samples, [], obj=upload_context)
+    result = cli_runner.invoke(cli=samples, args=[], obj=upload_context)
 
     # THEN assert that the program exits with a non zero exit code
     assert result.exit_code != 0
 
 
 def test_cli_upload_vogue_flowcells(upload_context: CGConfig, cli_runner: CliRunner, caplog):
     """Testing cli for upload vogue flowcells with correct argument"""
 
     # GIVEN a vogue api
     caplog.set_level(logging.DEBUG)
 
     # WHEN running vogue load flowcells with the days argument
-    result = cli_runner.invoke(flowcells, ["-d", 1], obj=upload_context)
+    result = cli_runner.invoke(cli=flowcells, args=["-d", 1], obj=upload_context)
 
     # THEN assert that the correct information was communicated
     assert "FLOWCELLS" in caplog.text
     # THEN assert that the program exits without errors
     assert result.exit_code == 0
 
 
 def test_cli_upload_vogue_flowcells_no_days(upload_context: CGConfig, cli_runner: CliRunner):
     """Testing cli for upload vogue flowcells with wrong argument"""
 
     # GIVEN a vogue api
 
     # WHEN running vogue load flowcells without the days argument
-    result = cli_runner.invoke(flowcells, [], obj=upload_context)
+    result = cli_runner.invoke(cli=flowcells, args=[], obj=upload_context)
 
     # THEN assert that the program exits with a non zero exit code
     assert result.exit_code != 0
+
+
+def test_cli_upload_vogue_bioinfo_all(upload_context: CGConfig, cli_runner: CliRunner):
+    """Testing cli for upload vogue bioinfo_all with correct argument"""
+
+    # GIVEN a vogue api
+
+    # WHEN running vogue upload bioinfo_all the days argument
+    result = cli_runner.invoke(cli=bioinfo_all, args=["-a", "2020-01-01"], obj=upload_context)
+
+    # THEN assert that the program exits with a  zero exit code
+    assert result.exit_code == 0
```

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/conftest.py` & `cg-27.2.2/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_link.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_run.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-27.2.2/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/conftest.py` & `cg-27.2.2/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-27.2.2/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/conftest.py` & `cg-27.2.2/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-27.2.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-27.2.2/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-27.2.2/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-27.2.2/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-27.2.2/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/microsalt/conftest.py` & `cg-27.2.2/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-27.2.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-27.2.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-27.2.2/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/conftest.py` & `cg-27.2.2/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-27.2.2/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/conftest.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-27.2.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/test_cli_workflow.py` & `cg-27.2.2/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-27.2.2/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/conftest.py` & `cg-27.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-27.2.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-27.2.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-27.2.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-27.2.2/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-27.2.2/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-27.2.2/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-27.2.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-27.2.2/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-27.2.2/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-27.2.2/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-27.2.2/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-27.2.2/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-27.2.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-27.2.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-27.2.2/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/case_export.json` & `cg-27.2.2/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-27.2.2/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-27.2.2/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-27.2.2/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-27.2.2/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-27.2.2/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/mip.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/rml.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-27.2.2/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/data/SampleSheet.csv` & `cg-27.2.2/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/data/cgfixture.db` & `cg-27.2.2/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/data/hkstore.db` & `cg-27.2.2/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/io/example_json.json` & `cg-27.2.2/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-27.2.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-27.2.2/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-27.2.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-27.2.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/report/case_data.json` & `cg-27.2.2/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/report/lims_exported_samples.json` & `cg-27.2.2/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/report/lims_family.json` & `cg-27.2.2/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/store/api/application_versions.xlsx` & `cg-27.2.2/tests/fixtures/store/api/application_versions.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/fixtures/store/api/applications.xlsx` & `cg-27.2.2/tests/fixtures/store/api/applications.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/io/conftest.py` & `cg-27.2.2/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/io/test_io_controller.py` & `cg-27.2.2/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/io/test_io_json.py` & `cg-27.2.2/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/io/test_io_yaml.py` & `cg-27.2.2/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/archive/conftest.py` & `cg-27.2.2/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/archive/test_archiving.py` & `cg-27.2.2/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/backup/conftest.py` & `cg-27.2.2/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/backup/test_meta_backup.py` & `cg-27.2.2/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/backup/test_meta_pdc.py` & `cg-27.2.2/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/clean/conftest.py` & `cg-27.2.2/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-27.2.2/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-27.2.2/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/conftest.py` & `cg-27.2.2/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/test_clean_fastq.py` & `cg-27.2.2/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/test_compress_files.py` & `cg-27.2.2/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-27.2.2/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-27.2.2/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-27.2.2/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/conftest.py` & `cg-27.2.2/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/deliver/conftest.py` & `cg-27.2.2/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-27.2.2/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/deliver/test_delivery_api.py` & `cg-27.2.2/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/demultiplex/conftest.py` & `cg-27.2.2/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-27.2.2/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-27.2.2/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/demultiplex/test_rename_files.py` & `cg-27.2.2/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/encryption/conftest.py` & `cg-27.2.2/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/encryption/test_encryption.py` & `cg-27.2.2/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/observations/conftest.py` & `cg-27.2.2/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-27.2.2/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/conftest.py` & `cg-27.2.2/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-27.2.2/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-27.2.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_meta_orders_api.py` & `cg-27.2.2/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-27.2.2/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_meta_orders_status.py` & `cg-27.2.2/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/orders/test_ticket_handler.py` & `cg-27.2.2/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/report/conftest.py` & `cg-27.2.2/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/report/test_balsamic_api.py` & `cg-27.2.2/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/report/test_field_validators.py` & `cg-27.2.2/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/report/test_mip_dna_api.py` & `cg-27.2.2/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/report/test_report_api.py` & `cg-27.2.2/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/rsync/conftest.py` & `cg-27.2.2/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/rsync/test_rsync.py` & `cg-27.2.2/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/test_invoice.py` & `cg-27.2.2/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/transfer/conftest.py` & `cg-27.2.2/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/transfer/test_external_data.py` & `cg-27.2.2/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-27.2.2/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-27.2.2/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-27.2.2/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/conftest.py` & `cg-27.2.2/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/gisaid/conftest.py` & `cg-27.2.2/tests/meta/upload/gisaid/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-27.2.2/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/mutacc/conftest.py` & `cg-27.2.2/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-27.2.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/nipt/conftest.py` & `cg-27.2.2/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-27.2.2/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/scout/conftest.py` & `cg-27.2.2/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-27.2.2/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-27.2.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-27.2.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-27.2.2/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-27.2.2/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/test_upload_api.py` & `cg-27.2.2/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-27.2.2/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/vogue/conftest.py` & `cg-27.2.2/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-27.2.2/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/workflow/conftest.py` & `cg-27.2.2/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/workflow/test_analysis.py` & `cg-27.2.2/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/workflow/test_balsamic.py` & `cg-27.2.2/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/workflow/test_microsalt.py` & `cg-27.2.2/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-27.2.2/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/balsamic_analysis_mock.py` & `cg-27.2.2/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/crunchy.py` & `cg-27.2.2/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/hk_mock.py` & `cg-27.2.2/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/limsmock.py` & `cg-27.2.2/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/madeline.py` & `cg-27.2.2/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/mip_analysis_mock.py` & `cg-27.2.2/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/osticket.py` & `cg-27.2.2/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/process_mock.py` & `cg-27.2.2/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/report.py` & `cg-27.2.2/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/scout.py` & `cg-27.2.2/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/store_model.py` & `cg-27.2.2/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/mocks/tb_mock.py` & `cg-27.2.2/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/balsamic/conftest.py` & `cg-27.2.2/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-27.2.2/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/conftest.py` & `cg-27.2.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/demultiplexing/conftest.py` & `cg-27.2.2/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/demultiplexing/test_demux_results.py` & `cg-27.2.2/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/demultiplexing/test_flowcell_model.py` & `cg-27.2.2/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/mip/conftest.py` & `cg-27.2.2/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/mip/test_mip_analysis.py` & `cg-27.2.2/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/mip/test_mip_config.py` & `cg-27.2.2/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-27.2.2/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/mip/test_mip_sample_info.py` & `cg-27.2.2/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/nextflow/conftest.py` & `cg-27.2.2/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-27.2.2/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/observations/conftest.py` & `cg-27.2.2/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/observations/test_observations_input_files.py` & `cg-27.2.2/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/report/test_validators.py` & `cg-27.2.2/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/rnafusion/conftest.py` & `cg-27.2.2/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-27.2.2/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/test_cg_models.py` & `cg-27.2.2/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/test_compression_data.py` & `cg-27.2.2/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/test_file_data.py` & `cg-27.2.2/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/models/test_flowcell_class.py` & `cg-27.2.2/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/server/conftest.py` & `cg-27.2.2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/add/test_store_add_application_version.py` & `cg-27.2.2/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/add/test_store_add_base.py` & `cg-27.2.2/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/add/test_store_add_customer.py` & `cg-27.2.2/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/add/test_store_add_flow_celll.py` & `cg-27.2.2/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/conftest.py` & `cg-27.2.2/tests/store/api/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,14 +532,53 @@
             customer_id="".join(["cust00", str(number)]),
             no_invoice=False,
             delivered_at=timestamp_now,
         )
     yield store
 
 
+@pytest.fixture(name="store_with_analyses_for_cases")
+def fixture_store_with_analyses_for_cases(
+    analysis_store: Store,
+    helpers: StoreHelpers,
+    timestamp_now: dt.datetime,
+    timestamp_yesterday: dt.datetime,
+) -> Store:
+    """Return a store with two analyses for two cases."""
+    case_one = analysis_store.get_case_by_internal_id("yellowhog")
+    case_two = helpers.add_case(analysis_store, internal_id="test_case_1")
+
+    cases = [case_one, case_two]
+    for case in cases:
+        oldest_analysis = helpers.add_analysis(
+            analysis_store,
+            case=case,
+            started_at=timestamp_yesterday,
+            uploaded_at=timestamp_yesterday,
+            delivery_reported_at=None,
+            uploaded_to_vogue_at=timestamp_yesterday,
+            completed_at=timestamp_yesterday,
+        )
+        helpers.add_analysis(
+            analysis_store,
+            case=case,
+            started_at=timestamp_now,
+            uploaded_at=timestamp_now,
+            delivery_reported_at=None,
+            uploaded_to_vogue_at=None,
+            completed_at=timestamp_now,
+        )
+        sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
+        analysis_store.relate_sample(
+            family=oldest_analysis.family, sample=sample, status=PhenotypeStatus.UNKNOWN
+        )
+
+    return analysis_store
+
+
 @pytest.fixture(name="store_with_analyses_for_cases_not_uploaded_fluffy")
 def fixture_store_with_analyses_for_cases_not_uploaded_fluffy(
     analysis_store: Store,
     helpers: StoreHelpers,
     timestamp_now: dt.datetime,
     timestamp_yesterday: dt.datetime,
 ) -> Store:
@@ -578,14 +617,15 @@
 def fixture_store_with_analyses_for_cases_not_uploaded_microsalt(
     analysis_store: Store,
     helpers: StoreHelpers,
     timestamp_now: dt.datetime,
     timestamp_yesterday: dt.datetime,
 ) -> Store:
     """Return a store with two analyses for two cases and pipeline."""
+
     case_one = analysis_store.get_case_by_internal_id("yellowhog")
     case_two = helpers.add_case(analysis_store, internal_id="test_case_1")
 
     cases = [case_one, case_two]
     for case in cases:
         oldest_analysis = helpers.add_analysis(
             analysis_store,
```

### Comparing `cg-27.2.1/tests/store/api/delete/test_store_api_delete.py` & `cg-27.2.2/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/find/test_find_basic_data.py` & `cg-27.2.2/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-27.2.2/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/find/test_find_business_data.py` & `cg-27.2.2/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/find/test_find_business_data_analysis.py` & `cg-27.2.2/tests/store/api/test_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-"""Tests the findbusinessdata part of the Cg store API related to Analysis model."""
-from datetime import datetime
-from typing import List
-from cg.store import Store
-from cg.store.models import (
-    Analysis,
-)
-from tests.store_helpers import StoreHelpers
-from cg.constants import Pipeline
+"""Tests for the BaseHandle class."""
+from typing import Type
 
+import pytest
+from dataclasses import astuple
 
-def test_get_analysis_by_case(
-    store_with_case_and_analysis: Store, case_id: str = "test_case_internal_id"
-):
-    """Test that an analysis can be fetched by case."""
-    # GIVEN a database with an analysis and case
-    case = store_with_case_and_analysis.get_case_by_internal_id(internal_id=case_id)
-    assert case
-    # WHEN fetching the analysis by case
-    analyses: List[Analysis] = store_with_case_and_analysis.get_analyses_by_case_entry_id(
-        case_entry_id=case.id
-    )
-    # THEN one analysis should be returned
-    for analysis in analyses:
-        assert analysis
-        assert analysis.family == case
+from alchy import Query, ModelBase
+from cg.constants.subject import PhenotypeStatus
+from cg.store.api.base import BaseHandler
 
 
-def test_get_latest_nipt_analysis_to_upload(
-    store_with_analyses_for_cases_not_uploaded_fluffy: Store, timestamp_now: datetime
-):
-    # GIVEN an analysis that is not delivery reported but there exists a newer analysis
-
-    # WHEN calling the analyses_to_delivery_report
-    analyses = (
-        store_with_analyses_for_cases_not_uploaded_fluffy.get_latest_nipt_analysis_to_upload()
-    )
-
-    # THEN only the newest analysis should be returned
-    for analysis in analyses:
-        assert analysis.family.internal_id in ["test_case_1", "yellowhog"]
-        assert analysis.started_at == timestamp_now
-        assert analysis.uploaded_at is None
-        assert analysis.pipeline == Pipeline.FLUFFY
+@pytest.mark.parametrize("table", astuple(BaseHandler()))
+def test__get_query(base_store, table: Type[ModelBase]):
+    """Tests the _get_query function for all attributes of BaseHandler ie tables in the database."""
+    assert isinstance(base_store._get_query(table=table), Query)
 
 
-def test_get_latest_microsalt_analysis_to_upload(
-    store_with_analyses_for_cases_not_uploaded_microsalt: Store, timestamp_now: datetime
+def test_get_latest_analyses_for_cases_query(
+    analysis_store, helpers, timestamp_now, timestamp_yesterday
 ):
-    # GIVEN an analysis that is not delivery reported but there exists a newer analysis
+    """Tests that analyses that are not latest are not returned."""
 
-    # WHEN calling the analyses_to_delivery_report
-    analyses = (
-        store_with_analyses_for_cases_not_uploaded_microsalt.get_latest_microsalt_analysis_to_upload()
+    # GIVEN an analysis a newer analysis exists
+    case = helpers.add_case(analysis_store)
+    analysis_oldest = helpers.add_analysis(
+        analysis_store,
+        case=case,
+        started_at=timestamp_yesterday,
+        uploaded_at=timestamp_yesterday,
+        delivery_reported_at=None,
+    )
+    analysis_store.add_commit(analysis_oldest)
+    analysis_newest = helpers.add_analysis(
+        analysis_store,
+        case=case,
+        started_at=timestamp_now,
+        uploaded_at=timestamp_now,
+        delivery_reported_at=None,
+    )
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
+    analysis_store.relate_sample(
+        family=analysis_oldest.family, sample=sample, status=PhenotypeStatus.UNKNOWN
     )
 
+    # WHEN calling the analyses_to_delivery_report
+    analyses: Query = analysis_store._get_latest_analyses_for_cases_query()
+
+    # THEN analyses is a query
+    assert isinstance(analyses, Query)
+
     # THEN only the newest analysis should be returned
-    for analysis in analyses:
-        assert analysis.family.internal_id in ["test_case_1", "yellowhog"]
-        assert analysis.started_at == timestamp_now
-        assert analysis.uploaded_at is None
-        assert analysis.pipeline == Pipeline.MICROSALT
+    assert analysis_newest in analyses
+    assert analysis_oldest not in analyses
```

### Comparing `cg-27.2.1/tests/store/api/find/test_find_business_data_case.py` & `cg-27.2.2/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/find/test_find_business_data_sample.py` & `cg-27.2.2/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_analyses_to_clean.py` & `cg-27.2.2/tests/store/api/status/test_analyses_to_clean.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,136 @@
 """This file tests the analyses_to_clean part of the status api"""
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from cg.constants import Pipeline
 from cg.store import Store
 
 
-def test_analysis_included(analysis_store: Store, helpers):
-    """Tests that analyses that are uploaded are returned"""
+def test_analysis_included(
+    analysis_store: Store, helpers, timestamp_now: datetime, timestamp_yesterday: datetime
+):
+    """Tests that analyses that are uploaded are returned."""
 
     # GIVEN an analysis that is uploaded
-    timestamp = datetime.now()
     analysis = helpers.add_analysis(
-        analysis_store, started_at=timestamp, uploaded_at=timestamp, cleaned_at=None
+        analysis_store,
+        started_at=timestamp_yesterday,
+        uploaded_at=timestamp_yesterday,
+        cleaned_at=None,
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_yesterday)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean
-    analyses_to_clean = analysis_store.analyses_to_clean(before=analysis.started_at).all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean(before=timestamp_now)
 
-    # THEN this analyse should be returned
+    # THEN this analysis should be returned
     assert analysis in analyses_to_clean
 
 
-def test_analysis_excluded(analysis_store: Store, helpers):
-    """Tests that analyses that are completed but lacks delivery report are returned"""
+def test_analysis_excluded(analysis_store: Store, helpers, timestamp_now: datetime):
+    """Tests that analyses that are completed but lacks delivery report are returned."""
 
     # GIVEN an analysis that is not uploaded
-    timestamp = datetime.now()
     analysis = helpers.add_analysis(
-        analysis_store, started_at=timestamp, uploaded_at=None, cleaned_at=None
+        analysis_store, started_at=timestamp_now, uploaded_at=None, cleaned_at=None
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean
-    analyses_to_clean = analysis_store.analyses_to_clean().all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean()
 
-    # THEN this analyse should be returned
+    # THEN this analysis should be returned
     assert analysis not in analyses_to_clean
 
 
-def test_pipeline_included(analysis_store: Store, helpers):
-    """Tests that analyses that are included depending on pipeline"""
+def test_pipeline_included(
+    analysis_store: Store, helpers, timestamp_now: datetime, timestamp_yesterday: datetime
+):
+    """Tests that analyses that are included depending on pipeline."""
 
     # GIVEN an analysis that is uploaded and pipeline is specified
-    timestamp = datetime.now()
     pipeline = Pipeline.BALSAMIC
     analysis = helpers.add_analysis(
         analysis_store,
         pipeline=pipeline,
-        started_at=timestamp,
-        uploaded_at=timestamp,
+        started_at=timestamp_yesterday,
+        uploaded_at=timestamp_yesterday,
         cleaned_at=None,
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_yesterday)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean specifying the used pipeline
-    analyses_to_clean = analysis_store.analyses_to_clean(pipeline=pipeline, before=timestamp).all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean(
+        pipeline=pipeline, before=timestamp_now
+    )
 
-    # THEN this analyse should be returned
+    # THEN this analysis should be returned
     assert analysis in analyses_to_clean
 
 
-def test_pipeline_excluded(analysis_store: Store, helpers):
-    """Tests that analyses are excluded depending on pipeline"""
+def test_pipeline_excluded(analysis_store: Store, helpers, timestamp_now: datetime):
+    """Tests that analyses are excluded depending on pipeline."""
 
     # GIVEN an analysis that is uploaded
-    timestamp = datetime.now()
+
     used_pipeline = Pipeline.BALSAMIC
     wrong_pipeline = Pipeline.MIP_DNA
     analysis = helpers.add_analysis(
         analysis_store,
         pipeline=used_pipeline,
-        started_at=timestamp,
-        uploaded_at=timestamp,
+        started_at=timestamp_now,
+        uploaded_at=timestamp_now,
         cleaned_at=None,
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean specifying another pipeline
-    analyses_to_clean = analysis_store.analyses_to_clean(pipeline=wrong_pipeline).all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean(pipeline=wrong_pipeline)
 
-    # THEN this analyse should not be returned
+    # THEN this analysis should not be returned
     assert analysis not in analyses_to_clean
 
 
-def test_non_cleaned_included(analysis_store: Store, helpers):
-    """Tests that analyses that are included depending on cleaned_at"""
+def test_non_cleaned_included(
+    analysis_store: Store, helpers, timestamp_now: datetime, timestamp_yesterday: datetime
+):
+    """Tests that analyses that are included depending on cleaned_at."""
 
     # GIVEN an analysis that is uploaded but not cleaned
-    timestamp = datetime.now()
     analysis = helpers.add_analysis(
-        analysis_store, started_at=timestamp, uploaded_at=timestamp, cleaned_at=None
+        analysis_store,
+        started_at=timestamp_yesterday,
+        uploaded_at=timestamp_yesterday,
+        cleaned_at=None,
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_yesterday)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean
-    analyses_to_clean = analysis_store.analyses_to_clean(before=timestamp).all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean(before=timestamp_now)
 
-    # THEN this analyse should be returned
+    # THEN this analysis should be returned
     assert analysis in analyses_to_clean
 
 
-def test_cleaned_excluded(analysis_store: Store, helpers):
-    """Tests that analyses are excluded depending on cleaned_at"""
+def test_cleaned_excluded(analysis_store: Store, helpers, timestamp_now: datetime):
+    """Tests that analyses are excluded depending on cleaned_at."""
 
     # GIVEN an analysis that is cleaned
-    timestamp = datetime.now()
     analysis = helpers.add_analysis(
-        analysis_store, started_at=timestamp, uploaded_at=timestamp, cleaned_at=timestamp
+        analysis_store,
+        started_at=timestamp_now,
+        uploaded_at=timestamp_now,
+        cleaned_at=timestamp_now,
     )
-    sample = helpers.add_sample(analysis_store, delivered_at=timestamp)
+    sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
     analysis_store.relate_sample(family=analysis.family, sample=sample, status="unknown")
 
     # WHEN calling the analyses_to_clean
-    analyses_to_clean = analysis_store.analyses_to_clean().all()
+    analyses_to_clean = analysis_store.get_analyses_to_clean()
 
-    # THEN this analyse should not be returned
+    # THEN this analysis should not be returned
     assert analysis not in analyses_to_clean
```

### Comparing `cg-27.2.1/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-27.2.2/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,21 +186,41 @@
     )
     sample = helpers.add_sample(analysis_store, delivered_at=timestamp_now)
     analysis_store.relate_sample(
         family=analysis_oldest.family, sample=sample, status=PhenotypeStatus.UNKNOWN
     )
 
     # WHEN calling the analyses_to_delivery_report
-    analyses = analysis_store.latest_analyses().all()
+    analyses: List[
+        Analysis
+    ] = analysis_store.get_analyses_for_each_case_with_latest_started_at_date()
 
     # THEN only the newest analysis should be returned
     assert analysis_newest in analyses
     assert analysis_oldest not in analyses
 
 
+def test_multiple_analyses_and_cases(
+    store_with_analyses_for_cases, helpers, timestamp_now, timestamp_yesterday
+):
+    """Tests that analyses that are not latest are not returned."""
+
+    # GIVEN an analysis that is not delivery reported but there exists a newer analysis
+
+    # WHEN calling the analyses_to_delivery_report
+    analyses: List[
+        Analysis
+    ] = store_with_analyses_for_cases.get_analyses_for_each_case_with_latest_started_at_date()
+
+    # THEN only the newest analysis should be returned
+    for analysis in analyses:
+        assert analysis.family.internal_id in ["test_case_1", "yellowhog"]
+        assert analysis.started_at == timestamp_now
+
+
 def test_set_case_action(analysis_store, case_id):
     """Tests if actions of cases are changed to analyze."""
     # Given a store with a case with action None
     action = analysis_store.Family.query.filter(Family.internal_id == case_id).first().action
 
     assert action == None
```

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status_analysis.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status_cases.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status_customer.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status_pool.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/status/test_store_api_status_sample.py` & `cg-27.2.2/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/api/test_store_import_func.py` & `cg-27.2.2/tests/store/api/test_store_import_func.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/conftest.py` & `cg-27.2.2/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_analyses_filters.py` & `cg-27.2.2/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_application_filters.py` & `cg-27.2.2/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_application_version_filters.py` & `cg-27.2.2/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_bed_filters.py` & `cg-27.2.2/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-27.2.2/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-27.2.2/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_cases_filters.py` & `cg-27.2.2/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-27.2.2/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_customer_filters.py` & `cg-27.2.2/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-27.2.2/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_invoice_filters.py` & `cg-27.2.2/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_organism_filters.py` & `cg-27.2.2/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_panel_filters.py` & `cg-27.2.2/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_pool_filters.py` & `cg-27.2.2/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_samples_filters.py` & `cg-27.2.2/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/filters/test_status_user_filters.py` & `cg-27.2.2/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/test_delivery.py` & `cg-27.2.2/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store/test_store_models.py` & `cg-27.2.2/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/store_helpers.py` & `cg-27.2.2/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/test_store_helpers.py` & `cg-27.2.2/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/conftest.py` & `cg-27.2.2/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/test_commands.py` & `cg-27.2.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/test_date.py` & `cg-27.2.2/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/test_dict.py` & `cg-27.2.2/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/test_dispatcher.py` & `cg-27.2.2/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-27.2.1/tests/utils/test_utils.py` & `cg-27.2.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

