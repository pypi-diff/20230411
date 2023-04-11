# Comparing `tmp/depthcharge-0.4.0.tar.gz` & `tmp/depthcharge-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-0.4.0.tar", last modified: Fri Aug  5 21:52:40 2022, max compression
+gzip compressed data, was "depthcharge-0.5.0.tar", last modified: Tue Apr 11 20:13:53 2023, max compression
```

## Comparing `depthcharge-0.4.0.tar` & `depthcharge-0.5.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.690440 depthcharge-0.4.0/
--rw-rw-r--   0 jon       (1000) jon       (1000)     4513 2022-03-05 23:20:23.000000 depthcharge-0.4.0/Depthcharge.md
--rw-rw-r--   0 jon       (1000) jon       (1000)       49 2022-03-05 23:20:23.000000 depthcharge-0.4.0/MANIFEST.in
--rw-rw-r--   0 jon       (1000) jon       (1000)     5615 2022-08-05 21:52:40.690440 depthcharge-0.4.0/PKG-INFO
--rw-rw-r--   0 jon       (1000) jon       (1000)     2068 2022-03-05 23:20:23.000000 depthcharge-0.4.0/README.md
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.642439 depthcharge-0.4.0/depthcharge/
--rw-rw-r--   0 jon       (1000) jon       (1000)     1116 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/__init__.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.650439 depthcharge-0.4.0/depthcharge/arch/
--rw-rw-r--   0 jon       (1000) jon       (1000)      259 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/arch/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     4339 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/arch/aarch64.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    11411 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/arch/arch.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     3279 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/arch/arm.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     1438 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/arch/generic.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     7619 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/builtin_payloads.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.650439 depthcharge-0.4.0/depthcharge/checker/
--rw-rw-r--   0 jon       (1000) jon       (1000)      432 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/__init__.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.654439 depthcharge-0.4.0/depthcharge/checker/_builtins/
--rw-rw-r--   0 jon       (1000) jon       (1000)      946 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      624 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/arch.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    16891 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/cmdline.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     7891 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/env.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     8900 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/fit.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    10501 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/fs.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2673 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/lib.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    20346 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/_builtins/net.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     9275 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/config_checker.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    12681 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/report.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    12873 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/checker/security_risk.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2129 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/uboot_config.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     8366 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/checker/uboot_header.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    23206 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/cmdline.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    12289 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/companion.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    14216 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/console.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    59750 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/context.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.654439 depthcharge-0.4.0/depthcharge/executor/
--rw-rw-r--   0 jon       (1000) jon       (1000)     1497 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/executor/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      992 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/executor/executor.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     1424 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/executor/go.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.662439 depthcharge-0.4.0/depthcharge/hunter/
--rw-rw-r--   0 jon       (1000) jon       (1000)      708 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    15344 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/cmdtbl.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      889 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/constant.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5165 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/cp.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     7988 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/env.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     6003 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/fdt.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    15954 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/hunter.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    25942 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/revcrc32.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     4074 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/hunter/string.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     8637 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/log.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.670440 depthcharge-0.4.0/depthcharge/memory/
--rw-rw-r--   0 jon       (1000) jon       (1000)     2256 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2802 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/cp.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     6131 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/crc32.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5016 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/data_abort.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5797 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/go.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     8460 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/i2c.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2207 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/itest.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5422 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/load.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    11570 2022-03-17 22:42:38.000000 depthcharge-0.4.0/depthcharge/memory/memcmds.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5618 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/patch.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     7660 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/reader.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2050 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/setexpr.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     3412 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/stratagem.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     6062 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/memory/writer.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     9460 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/monitor.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    22142 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/operation.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5036 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/payload_map.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     5260 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/progress.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.678440 depthcharge-0.4.0/depthcharge/register/
--rw-rw-r--   0 jon       (1000) jon       (1000)      978 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     1477 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/cp.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      869 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/crc32.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     3063 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/data_abort.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      946 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/fdt.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      858 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/itest.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2409 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/memcmds.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     1340 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/reader.py
--rw-rw-r--   0 jon       (1000) jon       (1000)      867 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/register/setexpr.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2301 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/revcrc32.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     9043 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/stratagem.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     7033 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/string.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.682440 depthcharge-0.4.0/depthcharge/uboot/
--rw-rw-r--   0 jon       (1000) jon       (1000)      338 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/__init__.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     3461 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/board.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     2902 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/cmd_table.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    11835 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/env.py
--rw-rw-r--   0 jon       (1000) jon       (1000)    12710 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/jump_table.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     4838 2022-03-05 23:20:23.000000 depthcharge-0.4.0/depthcharge/uboot/version.py
--rw-rw-r--   0 jon       (1000) jon       (1000)       64 2022-08-05 21:41:10.000000 depthcharge-0.4.0/depthcharge/version.py
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.646439 depthcharge-0.4.0/depthcharge.egg-info/
--rw-rw-r--   0 jon       (1000) jon       (1000)     5615 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/PKG-INFO
--rw-rw-r--   0 jon       (1000) jon       (1000)     2770 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/SOURCES.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)        1 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/dependency_links.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)        1 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/not-zip-safe
--rw-rw-r--   0 jon       (1000) jon       (1000)       80 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/requires.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)       12 2022-08-05 21:52:40.000000 depthcharge-0.4.0/depthcharge.egg-info/top_level.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)       50 2022-03-05 23:20:23.000000 depthcharge-0.4.0/pyproject.toml
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2022-08-05 21:52:40.690440 depthcharge-0.4.0/scripts/
--rwxrwxr-x   0 jon       (1000) jon       (1000)    12951 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-audit-config
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3770 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-find-cmd
--rwxrwxr-x   0 jon       (1000) jon       (1000)     6252 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-find-env
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3557 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-find-fdt
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3005 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-inspect
--rwxrwxr-x   0 jon       (1000) jon       (1000)     2900 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-mkenv
--rwxrwxr-x   0 jon       (1000) jon       (1000)     7002 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-print
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3462 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-read-mem
--rwxrwxr-x   0 jon       (1000) jon       (1000)     5686 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-stratagem
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3997 2022-03-05 23:20:23.000000 depthcharge-0.4.0/scripts/depthcharge-write-mem
--rw-rw-r--   0 jon       (1000) jon       (1000)       38 2022-08-05 21:52:40.690440 depthcharge-0.4.0/setup.cfg
--rwxrwxr-x   0 jon       (1000) jon       (1000)     3127 2022-03-17 22:44:08.000000 depthcharge-0.4.0/setup.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.103842 depthcharge-0.5.0/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     4513 2023-04-11 20:11:55.000000 depthcharge-0.5.0/Depthcharge.md
+-rw-rw-r--   0 jon       (1000) jon       (1000)       49 2023-04-11 20:11:55.000000 depthcharge-0.5.0/MANIFEST.in
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5615 2023-04-11 20:13:53.103842 depthcharge-0.5.0/PKG-INFO
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2068 2023-04-11 20:11:55.000000 depthcharge-0.5.0/README.md
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.063845 depthcharge-0.5.0/depthcharge/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1116 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/__init__.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.067845 depthcharge-0.5.0/depthcharge/arch/
+-rw-rw-r--   0 jon       (1000) jon       (1000)      259 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/arch/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     4339 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/arch/aarch64.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    11411 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/arch/arch.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3279 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/arch/arm.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1438 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/arch/generic.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     7619 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/builtin_payloads.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.071844 depthcharge-0.5.0/depthcharge/checker/
+-rw-rw-r--   0 jon       (1000) jon       (1000)      432 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/__init__.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.075844 depthcharge-0.5.0/depthcharge/checker/_builtins/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1012 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      624 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/arch.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    16891 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/cmdline.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     7891 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/env.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     8900 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/fit.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    10501 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/fs.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2673 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/lib.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    20346 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/net.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3093 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/_builtins/usb.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     9275 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/config_checker.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    12681 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/report.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    12873 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/security_risk.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2129 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/uboot_config.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     8366 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/checker/uboot_header.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    23206 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/cmdline.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    12289 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/companion.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    14216 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/console.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    59946 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/context.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.079844 depthcharge-0.5.0/depthcharge/executor/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1497 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/executor/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      992 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/executor/executor.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1424 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/executor/go.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.083844 depthcharge-0.5.0/depthcharge/hunter/
+-rw-rw-r--   0 jon       (1000) jon       (1000)      708 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    15344 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/cmdtbl.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      889 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/constant.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5165 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/cp.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     7988 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/env.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     6003 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/fdt.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    15954 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/hunter.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    25942 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/revcrc32.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     4074 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/hunter/string.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     8637 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/log.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.091843 depthcharge-0.5.0/depthcharge/memory/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2256 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2802 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/cp.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     6131 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/crc32.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5016 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/data_abort.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5797 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/go.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     8460 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/i2c.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2207 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/itest.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5422 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/load.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    11570 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/memcmds.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5618 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/patch.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     7660 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/reader.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2050 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/setexpr.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3412 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/stratagem.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     6062 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/memory/writer.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     9460 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/monitor.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    22142 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/operation.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5036 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/payload_map.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5260 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/progress.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.095843 depthcharge-0.5.0/depthcharge/register/
+-rw-rw-r--   0 jon       (1000) jon       (1000)      978 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1477 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/cp.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      869 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/crc32.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3063 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/data_abort.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      946 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/fdt.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      858 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/itest.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2409 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/memcmds.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1340 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/reader.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      867 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/register/setexpr.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2301 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/revcrc32.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     9043 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/stratagem.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     7033 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/string.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.095843 depthcharge-0.5.0/depthcharge/uboot/
+-rw-rw-r--   0 jon       (1000) jon       (1000)      338 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/__init__.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3461 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/board.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2902 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/cmd_table.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    11835 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/env.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)    12710 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/jump_table.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)     4838 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/uboot/version.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)       64 2023-04-11 20:11:55.000000 depthcharge-0.5.0/depthcharge/version.py
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.067845 depthcharge-0.5.0/depthcharge.egg-info/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     5615 2023-04-11 20:13:52.000000 depthcharge-0.5.0/depthcharge.egg-info/PKG-INFO
+-rw-rw-r--   0 jon       (1000) jon       (1000)     2807 2023-04-11 20:13:53.000000 depthcharge-0.5.0/depthcharge.egg-info/SOURCES.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)        1 2023-04-11 20:13:52.000000 depthcharge-0.5.0/depthcharge.egg-info/dependency_links.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)        1 2023-04-11 20:13:52.000000 depthcharge-0.5.0/depthcharge.egg-info/not-zip-safe
+-rw-rw-r--   0 jon       (1000) jon       (1000)       80 2023-04-11 20:13:52.000000 depthcharge-0.5.0/depthcharge.egg-info/requires.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)       12 2023-04-11 20:13:52.000000 depthcharge-0.5.0/depthcharge.egg-info/top_level.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)       50 2023-04-11 20:11:55.000000 depthcharge-0.5.0/pyproject.toml
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-04-11 20:13:53.103842 depthcharge-0.5.0/scripts/
+-rwxrwxr-x   0 jon       (1000) jon       (1000)    12951 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-audit-config
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3770 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-find-cmd
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     6252 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-find-env
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3557 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-find-fdt
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3005 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-inspect
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     2900 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-mkenv
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     7002 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-print
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3462 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-read-mem
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     5686 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-stratagem
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3997 2023-04-11 20:11:55.000000 depthcharge-0.5.0/scripts/depthcharge-write-mem
+-rw-rw-r--   0 jon       (1000) jon       (1000)       38 2023-04-11 20:13:53.103842 depthcharge-0.5.0/setup.cfg
+-rwxrwxr-x   0 jon       (1000) jon       (1000)     3127 2023-04-11 20:11:55.000000 depthcharge-0.5.0/setup.py
```

### Comparing `depthcharge-0.4.0/Depthcharge.md` & `depthcharge-0.5.0/Depthcharge.md`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/PKG-INFO` & `depthcharge-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge
-Version: 0.4.0
+Version: 0.5.0
 Summary: A U-Boot toolkit for security researchers and tinkerers
 Home-page: https://github.com/nccgroup/depthcharge
 Author: Jon Szymaniak (NCC Group)
 Author-email: jon.szymaniak.foss@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Source, https://github.com/nccgroup/depthcharge
```

### Comparing `depthcharge-0.4.0/README.md` & `depthcharge-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/__init__.py` & `depthcharge-0.5.0/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/arch/aarch64.py` & `depthcharge-0.5.0/depthcharge/arch/aarch64.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/arch/arch.py` & `depthcharge-0.5.0/depthcharge/arch/arch.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/arch/arm.py` & `depthcharge-0.5.0/depthcharge/arch/arm.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/arch/generic.py` & `depthcharge-0.5.0/depthcharge/arch/generic.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/builtin_payloads.py` & `depthcharge-0.5.0/depthcharge/builtin_payloads.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/__init__.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 
 from .cmdline   import _BUILTIN_DEFS as _CMDLINE_DEFS
 from .env       import _BUILTIN_DEFS as _ENV_DEFS
 from .fit       import _BUILTIN_DEFS as _FIT_DEFS
 from .fs        import _BUILTIN_DEFS as _FS_DEFS
 from .lib       import _BUILTIN_DEFS as _LIB_DEFS
 from .net       import _BUILTIN_DEFS as _NET_DEFS
+from .usb       import _BUILTIN_DEFS as _USB_DEFS
 
 # Aggregate builtins into a main set of definitions
 _BUILTIN_DEFS = (
     _CMDLINE_DEFS +
     _ENV_DEFS +
     _FIT_DEFS +
     _FS_DEFS +
     _LIB_DEFS +
-    _NET_DEFS
+    _NET_DEFS +
+    _USB_DEFS
 )
 
 # Fill empty source field.
 # Required by SecurityRisk constructor, but excessive to require in _BUILTIN_DEFS
 for entry in _BUILTIN_DEFS:
     entry[2]['source'] = ''
```

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/arch.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/arch.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/cmdline.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/cmdline.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/env.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/env.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/fit.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/fit.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/fs.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/fs.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/lib.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/lib.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/_builtins/net.py` & `depthcharge-0.5.0/depthcharge/checker/_builtins/net.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/config_checker.py` & `depthcharge-0.5.0/depthcharge/checker/config_checker.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/report.py` & `depthcharge-0.5.0/depthcharge/checker/report.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/security_risk.py` & `depthcharge-0.5.0/depthcharge/checker/security_risk.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/uboot_config.py` & `depthcharge-0.5.0/depthcharge/checker/uboot_config.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/checker/uboot_header.py` & `depthcharge-0.5.0/depthcharge/checker/uboot_header.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/cmdline.py` & `depthcharge-0.5.0/depthcharge/cmdline.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/companion.py` & `depthcharge-0.5.0/depthcharge/companion.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/console.py` & `depthcharge-0.5.0/depthcharge/console.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/context.py` & `depthcharge-0.5.0/depthcharge/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,19 +291,21 @@
         self.commands(detailed=kwargs.get('detailed_help', False))
         self.environment()
 
         # Establish our payload base address by resolving either an environment
         # variable read from the target device or using a user-provided address
         try:
             payload_map_base = self._resolve_payload_base()
-        except OperationFailed:
+        except OperationFailed as e:
             self._allow_deploy_exec = False
             self._skip_deploy = False
             payload_map_base = 0
-            log.warning('Disabling payload deployemnt and execution due to error(s).')
+
+            # Be a bit more helpful when loadaddr isn't in the environment
+            log.warning('Disabling payload deployemnt and execution due to error: ' + str(e))
 
         self._payloads = PayloadMap(self.arch, payload_map_base,
                                     skip_deploy=self._skip_deployment)
 
         # Retrieve and cache version information, if not provided earlier
         self.version()
 
@@ -330,14 +332,15 @@
         """
         if isinstance(self._payload_base,  str):
             try:
                 expanded = uboot.env.expand_variable(self._env, self._payload_base)
                 self._payload_base = int(expanded, 0)
             except KeyError:
                 msg = 'Environment variable used for payload_base does not exist: {:s}'
+                msg += '\n    You will need to manually specify -X payload_base=<address> to address this.'
                 raise OperationFailed(msg.format(self._payload_base))
             except ValueError:
                 msg = 'Encountered invalid expansion of payload_base: ' + expanded
                 raise OperationFailed(msg)
 
         msg = 'Depthcharge payload base (0x{:08x}) + payload offset (0x{:08x}) => 0x{:08x}'
         actual_base = self._payload_base + self._payload_off
```

### Comparing `depthcharge-0.4.0/depthcharge/executor/__init__.py` & `depthcharge-0.5.0/depthcharge/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/executor/executor.py` & `depthcharge-0.5.0/depthcharge/executor/executor.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/executor/go.py` & `depthcharge-0.5.0/depthcharge/executor/go.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/__init__.py` & `depthcharge-0.5.0/depthcharge/hunter/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/cmdtbl.py` & `depthcharge-0.5.0/depthcharge/hunter/cmdtbl.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/constant.py` & `depthcharge-0.5.0/depthcharge/hunter/constant.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/cp.py` & `depthcharge-0.5.0/depthcharge/hunter/cp.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/env.py` & `depthcharge-0.5.0/depthcharge/hunter/env.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/fdt.py` & `depthcharge-0.5.0/depthcharge/hunter/fdt.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/hunter.py` & `depthcharge-0.5.0/depthcharge/hunter/hunter.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/revcrc32.py` & `depthcharge-0.5.0/depthcharge/hunter/revcrc32.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/hunter/string.py` & `depthcharge-0.5.0/depthcharge/hunter/string.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/log.py` & `depthcharge-0.5.0/depthcharge/log.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/__init__.py` & `depthcharge-0.5.0/depthcharge/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/cp.py` & `depthcharge-0.5.0/depthcharge/memory/cp.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/crc32.py` & `depthcharge-0.5.0/depthcharge/memory/crc32.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/data_abort.py` & `depthcharge-0.5.0/depthcharge/memory/data_abort.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/go.py` & `depthcharge-0.5.0/depthcharge/memory/go.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/i2c.py` & `depthcharge-0.5.0/depthcharge/memory/i2c.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/itest.py` & `depthcharge-0.5.0/depthcharge/memory/itest.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/load.py` & `depthcharge-0.5.0/depthcharge/memory/load.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/memcmds.py` & `depthcharge-0.5.0/depthcharge/memory/memcmds.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/patch.py` & `depthcharge-0.5.0/depthcharge/memory/patch.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/reader.py` & `depthcharge-0.5.0/depthcharge/memory/reader.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/setexpr.py` & `depthcharge-0.5.0/depthcharge/memory/setexpr.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/stratagem.py` & `depthcharge-0.5.0/depthcharge/memory/stratagem.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/memory/writer.py` & `depthcharge-0.5.0/depthcharge/memory/writer.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/monitor.py` & `depthcharge-0.5.0/depthcharge/monitor.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/operation.py` & `depthcharge-0.5.0/depthcharge/operation.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/payload_map.py` & `depthcharge-0.5.0/depthcharge/payload_map.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/progress.py` & `depthcharge-0.5.0/depthcharge/progress.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/__init__.py` & `depthcharge-0.5.0/depthcharge/register/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/cp.py` & `depthcharge-0.5.0/depthcharge/register/cp.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/crc32.py` & `depthcharge-0.5.0/depthcharge/register/crc32.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/data_abort.py` & `depthcharge-0.5.0/depthcharge/register/data_abort.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/fdt.py` & `depthcharge-0.5.0/depthcharge/register/fdt.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/itest.py` & `depthcharge-0.5.0/depthcharge/register/itest.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/memcmds.py` & `depthcharge-0.5.0/depthcharge/register/memcmds.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/reader.py` & `depthcharge-0.5.0/depthcharge/register/reader.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/register/setexpr.py` & `depthcharge-0.5.0/depthcharge/register/setexpr.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/revcrc32.py` & `depthcharge-0.5.0/depthcharge/revcrc32.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/stratagem.py` & `depthcharge-0.5.0/depthcharge/stratagem.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/string.py` & `depthcharge-0.5.0/depthcharge/string.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/uboot/board.py` & `depthcharge-0.5.0/depthcharge/uboot/board.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/uboot/cmd_table.py` & `depthcharge-0.5.0/depthcharge/uboot/cmd_table.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/uboot/env.py` & `depthcharge-0.5.0/depthcharge/uboot/env.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/uboot/jump_table.py` & `depthcharge-0.5.0/depthcharge/uboot/jump_table.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge/uboot/version.py` & `depthcharge-0.5.0/depthcharge/uboot/version.py`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/depthcharge.egg-info/PKG-INFO` & `depthcharge-0.5.0/depthcharge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge
-Version: 0.4.0
+Version: 0.5.0
 Summary: A U-Boot toolkit for security researchers and tinkerers
 Home-page: https://github.com/nccgroup/depthcharge
 Author: Jon Szymaniak (NCC Group)
 Author-email: jon.szymaniak.foss@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Source, https://github.com/nccgroup/depthcharge
```

### Comparing `depthcharge-0.4.0/depthcharge.egg-info/SOURCES.txt` & `depthcharge-0.5.0/depthcharge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 depthcharge/checker/_builtins/arch.py
 depthcharge/checker/_builtins/cmdline.py
 depthcharge/checker/_builtins/env.py
 depthcharge/checker/_builtins/fit.py
 depthcharge/checker/_builtins/fs.py
 depthcharge/checker/_builtins/lib.py
 depthcharge/checker/_builtins/net.py
+depthcharge/checker/_builtins/usb.py
 depthcharge/executor/__init__.py
 depthcharge/executor/executor.py
 depthcharge/executor/go.py
 depthcharge/hunter/__init__.py
 depthcharge/hunter/cmdtbl.py
 depthcharge/hunter/constant.py
 depthcharge/hunter/cp.py
```

### Comparing `depthcharge-0.4.0/scripts/depthcharge-audit-config` & `depthcharge-0.5.0/scripts/depthcharge-audit-config`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-find-cmd` & `depthcharge-0.5.0/scripts/depthcharge-find-cmd`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-find-env` & `depthcharge-0.5.0/scripts/depthcharge-find-env`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-find-fdt` & `depthcharge-0.5.0/scripts/depthcharge-find-fdt`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-inspect` & `depthcharge-0.5.0/scripts/depthcharge-inspect`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-mkenv` & `depthcharge-0.5.0/scripts/depthcharge-mkenv`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-print` & `depthcharge-0.5.0/scripts/depthcharge-print`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-read-mem` & `depthcharge-0.5.0/scripts/depthcharge-read-mem`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-stratagem` & `depthcharge-0.5.0/scripts/depthcharge-stratagem`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/scripts/depthcharge-write-mem` & `depthcharge-0.5.0/scripts/depthcharge-write-mem`

 * *Files identical despite different names*

### Comparing `depthcharge-0.4.0/setup.py` & `depthcharge-0.5.0/setup.py`

 * *Files identical despite different names*

