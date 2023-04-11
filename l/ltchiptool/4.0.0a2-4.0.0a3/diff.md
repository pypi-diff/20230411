# Comparing `tmp/ltchiptool-4.0.0a2.tar.gz` & `tmp/ltchiptool-4.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool-4.0.0a2.tar", max compression
+gzip compressed data, was "ltchiptool-4.0.0a3.tar", max compression
```

## Comparing `ltchiptool-4.0.0a2.tar` & `ltchiptool-4.0.0a3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0        0        0     1076 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/LICENSE
--rw-r--r--   0        0        0     2378 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/README.md
--rw-r--r--   0        0        0      376 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/__init__.py
--rw-r--r--   0        0        0     2339 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/__main__.py
--rw-r--r--   0        0        0     2517 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/dumptool.py
--rw-r--r--   0        0        0      896 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/elf2bin.py
--rw-r--r--   0        0        0      451 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/flash/__main__.py
--rw-r--r--   0        0        0     1724 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/flash/_utils.py
--rw-r--r--   0        0        0     1610 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/flash/file.py
--rw-r--r--   0        0        0     3157 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/flash/read.py
--rw-r--r--   0        0        0     7143 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/flash/write.py
--rw-r--r--   0        0        0      881 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/link2bin.py
--rw-r--r--   0        0        0     2331 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/list.py
--rw-r--r--   0        0        0      423 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/commands/soc.py
--rw-r--r--   0        0        0      127 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/__init__.py
--rw-r--r--   0        0        0     1459 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/__main__.py
--rw-r--r--   0        0        0     9477 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool-192x192.png
--rw-r--r--   0        0        0    15406 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.ico
--rw-r--r--   0        0        0    15226 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.wxui
--rw-r--r--   0        0        0    19626 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.xrc
--rw-r--r--   0        0        0     6048 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/main.py
--rw-r--r--   0        0        0       48 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/panels/__init__.py
--rw-r--r--   0        0        0     2017 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/panels/about.py
--rw-r--r--   0        0        0     3977 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/panels/base.py
--rw-r--r--   0        0        0    17061 2023-03-26 17:36:23.718975 ltchiptool-4.0.0a2/ltchiptool/gui/panels/flash.py
--rw-r--r--   0        0        0     6937 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/panels/log.py
--rw-r--r--   0        0        0      789 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/utils.py
--rw-r--r--   0        0        0       47 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/work/__init__.py
--rw-r--r--   0        0        0      950 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/work/base.py
--rw-r--r--   0        0        0     6069 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/work/flash.py
--rw-r--r--   0        0        0     2528 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/gui/work/ports.py
--rw-r--r--   0        0        0      263 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/models/__init__.py
--rw-r--r--   0        0        0     3041 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/models/board.py
--rw-r--r--   0        0        0      155 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/models/enums.py
--rw-r--r--   0        0        0     5966 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/models/family.py
--rw-r--r--   0        0        0      185 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/__init__.py
--rw-r--r--   0        0        0      111 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/__init__.py
--rw-r--r--   0        0        0     6043 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/binary.py
--rw-r--r--   0        0        0     6871 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/flash.py
--rw-r--r--   0        0        0      721 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/main.py
--rw-r--r--   0        0        0       48 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/util/__init__.py
--rw-r--r--   0        0        0    18071 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz/util/rtltool.py
--rw-r--r--   0        0        0      114 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/__init__.py
--rw-r--r--   0        0        0     2780 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/flash.py
--rw-r--r--   0        0        0      595 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/main.py
--rw-r--r--   0        0        0       49 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/util/__init__.py
--rw-r--r--   0        0        0    13040 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/util/ambz2tool.py
--rw-r--r--   0        0        0      111 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/__init__.py
--rw-r--r--   0        0        0     8734 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/binary.py
--rw-r--r--   0        0        0     8305 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/bkpackager.py
--rw-r--r--   0        0        0     6820 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/flash.py
--rw-r--r--   0        0        0      723 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/main.py
--rw-r--r--   0        0        0      317 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/__init__.py
--rw-r--r--   0        0        0     7467 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/binary.py
--rw-r--r--   0        0        0     6175 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/crypto.py
--rw-r--r--   0        0        0      515 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/models.py
--rw-r--r--   0        0        0     2940 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/rbl.py
--rw-r--r--   0        0        0     2784 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/common.py
--rw-r--r--   0        0        0     6434 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/soc/interface.py
--rw-r--r--   0        0        0       48 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/__init__.py
--rw-r--r--   0        0        0     2408 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/bitint.py
--rw-r--r--   0        0        0     2727 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/cli.py
--rw-r--r--   0        0        0     5642 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/crc16.py
--rw-r--r--   0        0        0     6631 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/detection.py
--rw-r--r--   0        0        0     1987 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/dict.py
--rw-r--r--   0        0        0      346 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/env.py
--rw-r--r--   0        0        0     2420 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/fileio.py
--rw-r--r--   0        0        0     3591 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/flash.py
--rw-r--r--   0        0        0     6105 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/intbin.py
--rw-r--r--   0        0        0     4806 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/logging.py
--rw-r--r--   0        0        0     6683 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/lvm.py
--rw-r--r--   0        0        0     1368 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/misc.py
--rw-r--r--   0        0        0     1878 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/obj.py
--rw-r--r--   0        0        0      866 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/slice.py
--rw-r--r--   0        0        0     1612 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/util/toolchain.py
--rw-r--r--   0        0        0      772 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/ltchiptool/version.py
--rw-r--r--   0        0        0     1031 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/__init__.py
--rw-r--r--   0        0        0      251 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/binpatch/__init__.py
--rw-r--r--   0        0        0      471 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/binpatch/apply.py
--rw-r--r--   0        0        0     1027 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/binpatch/bindiff.py
--rw-r--r--   0        0        0     1666 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/binpatch/diff32.py
--rw-r--r--   0        0        0     4306 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/cli.py
--rw-r--r--   0        0        0      360 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/__init__.py
--rw-r--r--   0        0        0     4805 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/block.py
--rw-r--r--   0        0        0     5803 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/context.py
--rw-r--r--   0        0        0     2210 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/enums.py
--rw-r--r--   0        0        0     1256 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/flags.py
--rw-r--r--   0        0        0     3311 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/image.py
--rw-r--r--   0        0        0      778 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/partition.py
--rw-r--r--   0        0        0     4562 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/models/uf2.py
--rw-r--r--   0        0        0      124 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/upload/__init__.py
--rw-r--r--   0        0        0     4846 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/upload/esphome.py
--rw-r--r--   0        0        0     7219 2023-03-26 17:36:23.722975 ltchiptool-4.0.0a2/uf2tool/writer.py
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 ltchiptool-4.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/README.md
+-rw-r--r--   0        0        0      376 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/__init__.py
+-rw-r--r--   0        0        0     2339 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/__main__.py
+-rw-r--r--   0        0        0     2517 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/dumptool.py
+-rw-r--r--   0        0        0      908 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/elf2bin.py
+-rw-r--r--   0        0        0      451 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/flash/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/flash/_utils.py
+-rw-r--r--   0        0        0     1610 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/flash/file.py
+-rw-r--r--   0        0        0     3157 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/flash/read.py
+-rw-r--r--   0        0        0     7143 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/flash/write.py
+-rw-r--r--   0        0        0      881 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/link2bin.py
+-rw-r--r--   0        0        0     2331 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/list.py
+-rw-r--r--   0        0        0      423 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/commands/soc.py
+-rw-r--r--   0        0        0      127 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/__main__.py
+-rw-r--r--   0        0        0     9477 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool-192x192.png
+-rw-r--r--   0        0        0    15406 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.ico
+-rw-r--r--   0        0        0    15226 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.wxui
+-rw-r--r--   0        0        0    19626 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.xrc
+-rw-r--r--   0        0        0     6048 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/main.py
+-rw-r--r--   0        0        0       48 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/panels/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/panels/about.py
+-rw-r--r--   0        0        0     3977 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/panels/base.py
+-rw-r--r--   0        0        0    17080 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/panels/flash.py
+-rw-r--r--   0        0        0     6937 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/panels/log.py
+-rw-r--r--   0        0        0      789 2023-04-11 15:50:53.394868 ltchiptool-4.0.0a3/ltchiptool/gui/utils.py
+-rw-r--r--   0        0        0       47 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/gui/work/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/gui/work/base.py
+-rw-r--r--   0        0        0     6069 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/gui/work/flash.py
+-rw-r--r--   0        0        0     2528 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/gui/work/ports.py
+-rw-r--r--   0        0        0      263 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/models/__init__.py
+-rw-r--r--   0        0        0     3041 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/models/board.py
+-rw-r--r--   0        0        0      155 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/models/enums.py
+-rw-r--r--   0        0        0     5966 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/models/family.py
+-rw-r--r--   0        0        0      185 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/__init__.py
+-rw-r--r--   0        0        0     6198 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/binary.py
+-rw-r--r--   0        0        0     6871 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/flash.py
+-rw-r--r--   0        0        0      721 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/main.py
+-rw-r--r--   0        0        0       48 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/util/__init__.py
+-rw-r--r--   0        0        0    18071 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz/util/rtltool.py
+-rw-r--r--   0        0        0      114 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/__init__.py
+-rw-r--r--   0        0        0     2780 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/flash.py
+-rw-r--r--   0        0        0      595 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/main.py
+-rw-r--r--   0        0        0       49 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/util/__init__.py
+-rw-r--r--   0        0        0    13040 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/util/ambz2tool.py
+-rw-r--r--   0        0        0      111 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/__init__.py
+-rw-r--r--   0        0        0     9025 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/binary.py
+-rw-r--r--   0        0        0     8305 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/bkpackager.py
+-rw-r--r--   0        0        0     6820 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/flash.py
+-rw-r--r--   0        0        0      723 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/main.py
+-rw-r--r--   0        0        0      317 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/__init__.py
+-rw-r--r--   0        0        0     7467 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/binary.py
+-rw-r--r--   0        0        0     6175 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/crypto.py
+-rw-r--r--   0        0        0      515 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/models.py
+-rw-r--r--   0        0        0     2940 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/rbl.py
+-rw-r--r--   0        0        0     2827 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/common.py
+-rw-r--r--   0        0        0     6478 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/soc/interface.py
+-rw-r--r--   0        0        0       48 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/bitint.py
+-rw-r--r--   0        0        0     2727 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/cli.py
+-rw-r--r--   0        0        0     5642 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/crc16.py
+-rw-r--r--   0        0        0     6631 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/detection.py
+-rw-r--r--   0        0        0     1987 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/dict.py
+-rw-r--r--   0        0        0      346 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/env.py
+-rw-r--r--   0        0        0     2420 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/fileio.py
+-rw-r--r--   0        0        0     3591 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/flash.py
+-rw-r--r--   0        0        0     3296 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/fwbinary.py
+-rw-r--r--   0        0        0     6105 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/intbin.py
+-rw-r--r--   0        0        0     4806 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/logging.py
+-rw-r--r--   0        0        0     6683 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/lvm.py
+-rw-r--r--   0        0        0     1368 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/misc.py
+-rw-r--r--   0        0        0     1878 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/obj.py
+-rw-r--r--   0        0        0      866 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/slice.py
+-rw-r--r--   0        0        0     1612 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/util/toolchain.py
+-rw-r--r--   0        0        0      772 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/ltchiptool/version.py
+-rw-r--r--   0        0        0     1031 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/binpatch/__init__.py
+-rw-r--r--   0        0        0      471 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/binpatch/apply.py
+-rw-r--r--   0        0        0     1027 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/binpatch/bindiff.py
+-rw-r--r--   0        0        0     1666 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/binpatch/diff32.py
+-rw-r--r--   0        0        0     4306 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/cli.py
+-rw-r--r--   0        0        0      360 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/__init__.py
+-rw-r--r--   0        0        0     4805 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/block.py
+-rw-r--r--   0        0        0     5803 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/context.py
+-rw-r--r--   0        0        0     2210 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/enums.py
+-rw-r--r--   0        0        0     1256 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/flags.py
+-rw-r--r--   0        0        0     3311 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/image.py
+-rw-r--r--   0        0        0      778 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/partition.py
+-rw-r--r--   0        0        0     4562 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/models/uf2.py
+-rw-r--r--   0        0        0      124 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/upload/__init__.py
+-rw-r--r--   0        0        0     4846 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/upload/esphome.py
+-rw-r--r--   0        0        0     7219 2023-04-11 15:50:53.398867 ltchiptool-4.0.0a3/uf2tool/writer.py
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 ltchiptool-4.0.0a3/PKG-INFO
```

### Comparing `ltchiptool-4.0.0a2/LICENSE` & `ltchiptool-4.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/README.md` & `ltchiptool-4.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/__main__.py` & `ltchiptool-4.0.0a3/ltchiptool/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/dumptool.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/dumptool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/elf2bin.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/elf2bin.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,12 +22,12 @@
       INPUT    ELF input file
       OTA_IDX  OTA index of the input file
     """
     soc = SocInterface.get(board.family)
     soc.set_board(board)
     files = soc.elf2bin(input, ota_idx)
     info("Generated files:")
-    for name, offset in files.items():
-        if offset is None:
-            info(f" - {name}")
+    for file in files:
+        if file.offset is None:
+            info(f" - {file.filename}")
         else:
-            info(f" - {name} - flashable at 0x{offset:X}")
+            info(f" - {file.filename} - flashable at 0x{file.offset:X}")
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/flash/_utils.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/flash/_utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/flash/file.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/flash/file.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/flash/read.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/flash/read.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/flash/write.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/flash/write.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/link2bin.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/link2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/commands/list.py` & `ltchiptool-4.0.0a3/ltchiptool/commands/list.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/__main__.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool-192x192.png` & `ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool-192x192.png`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.ico` & `ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.ico`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.wxui` & `ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.0.0a3/ltchiptool/gui/ltchiptool.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/main.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/panels/about.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/panels/about.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/panels/base.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/panels/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/panels/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/panels/flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,15 @@
             operation=self.operation,
             file=self.file,
             soc=soc,
             offset=self.offset,
             skip=self.skip,
             length=self.length,
             verify=True,
-            ctx=self.detection.get_uf2_ctx(),
+            ctx=self.detection and self.detection.get_uf2_ctx(),
             on_chip_info=self.Start.SetNote,
         )
         self.start_work(work, freeze_ui=True)
         self.Start.SetNote("")
         self.Cancel.Enable()
 
     @on_event
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/panels/log.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/panels/log.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/utils.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/work/base.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/work/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/work/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/work/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/gui/work/ports.py` & `ltchiptool-4.0.0a3/ltchiptool/gui/work/ports.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/models/board.py` & `ltchiptool-4.0.0a3/ltchiptool/models/board.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/models/family.py` & `ltchiptool-4.0.0a3/ltchiptool/models/family.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz/binary.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz/binary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright (c) Kuba Szczodrzyński 2022-07-29.
 
 from abc import ABC
-from os.path import basename
 from struct import unpack
-from typing import IO, Dict, Optional, Tuple
+from typing import IO, List, Optional, Tuple
 
 from ltchiptool import SocInterface
 from ltchiptool.util.detection import Detection
-from ltchiptool.util.fileio import chname, isnewer, peek, readbin
+from ltchiptool.util.fileio import peek, readbin
+from ltchiptool.util.fwbinary import FirmwareBinary
 from ltchiptool.util.intbin import inttole32
-from ltchiptool.util.logging import graph
 
 
 def write_header(f: IO[bytes], start: int, end: int):
     f.write(b"81958711")
     f.write(inttole32(end - start))
     f.write(inttole32(start))
     f.write(b"\xff" * 16)
@@ -32,21 +31,16 @@
 
 
 def check_bootloader_binary(data: bytes) -> Optional[Tuple[int, int, bytes]]:
     return check_xip_binary(data, header=b"\x99\x99\x96\x96\x3F\xCC\x66\xFC")
 
 
 class AmebaZBinary(SocInterface, ABC):
-    def elf2bin(
-        self,
-        input: str,
-        ota_idx: int,
-    ) -> Dict[str, Optional[int]]:
+    def elf2bin(self, input: str, ota_idx: int) -> List[FirmwareBinary]:
         toolchain = self.board.toolchain
-        result: Dict[str, Optional[int]] = {}
 
         sections_ram = [
             ".ram_image2.entry",
             ".ram_image2.data",
             ".ram_image2.bss",
             ".ram_image2.skb.bss",
             ".ram_heap.data",
@@ -54,52 +48,67 @@
         sections_xip = [".xip_image2.text"]
         sections_rdp = [".ram_rdp.text"]
         nmap = toolchain.nm(input)
         ram_start = nmap["__ram_image2_text_start__"]
         ram_end = nmap["__ram_image2_text_end__"]
         xip_start = nmap["__flash_text_start__"] - 0x8000020
         # build output name
-        output = chname(input, f"image_ota{ota_idx}.0x{xip_start:06X}.bin")
-        out_ram = chname(input, f"image_ota{ota_idx}.ram_2.r.bin")
-        out_xip = chname(input, f"image_ota{ota_idx}.xip_image2.bin")
-        out_rdp = chname(input, f"image_ota{ota_idx}.rdp.bin")
+        output = FirmwareBinary(
+            location=input,
+            name=f"ota{ota_idx}",
+            offset=xip_start,
+            title=f"OTA{ota_idx} XIP image",
+            public=True,
+        )
+        out_ram = FirmwareBinary(
+            location=input,
+            name=f"ota{ota_idx}",
+            subname="ram_2.r",
+            title="Raw RAM image",
+        )
+        out_xip = FirmwareBinary(
+            location=input,
+            name=f"ota{ota_idx}",
+            subname="xip_image2",
+            title="Raw XIP image",
+        )
+        out_rdp = FirmwareBinary(
+            location=input,
+            name=f"ota{ota_idx}",
+            subname="rdp",
+            title="Raw RDP image",
+        )
         # print graph element
-        graph(1, basename(output))
+        output.graph(1)
         # objcopy required images
-        ram = toolchain.objcopy(input, out_ram, sections_ram)
-        xip = toolchain.objcopy(input, out_xip, sections_xip)
-        toolchain.objcopy(input, out_rdp, sections_rdp)
-        # add to outputs
-        result[out_ram] = None
-        result[out_xip] = None
-        result[out_rdp] = None
+        ram = toolchain.objcopy(input, out_ram.path, sections_ram)
+        xip = toolchain.objcopy(input, out_xip.path, sections_xip)
+        toolchain.objcopy(input, out_rdp.path, sections_rdp)
         # return if images are up-to-date
-        if not isnewer(ram, output) and not isnewer(xip, output):
-            result[output] = xip_start
-            return result
+        if output.isnewer(than=ram) and output.isnewer(than=xip):
+            return output.group_get()
 
         # read and trim RAM image
         ram = readbin(ram).rstrip(b"\x00")
         # read XIP image
         xip = readbin(xip)
         # align images to 4 bytes
         ram += b"\x00" * (((((len(ram) - 1) // 4) + 1) * 4) - len(ram))
         xip += b"\x00" * (((((len(xip) - 1) // 4) + 1) * 4) - len(xip))
         # write output file
-        with open(output, "wb") as f:
+        with output.write() as f:
             # write XIP header
             write_header(f, 0, len(xip))
             # write XIP image
             f.write(xip)
             # write RAM header
             write_header(f, ram_start, ram_end)
             # write RAM image
             f.write(ram)
-        result[output] = xip_start
-        return result
+        return output.group()
 
     def detect_file_type(
         self,
         file: IO[bytes],
         length: int,
     ) -> Optional[Detection]:
         data = peek(file, size=64)
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz/main.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz/util/rtltool.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz/util/rtltool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/main.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/ambz2/util/ambz2tool.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/ambz2/util/ambz2tool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/binary.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/binary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright (c) Kuba Szczodrzyński 2022-07-29.
 
 from abc import ABC
 from datetime import datetime
 from io import SEEK_SET, BytesIO
 from logging import warning
 from os import stat
-from os.path import basename
-from typing import IO, Dict, Optional, Union
+from typing import IO, List, Optional, Union
 
 from ltchiptool import SocInterface
 from ltchiptool.util.crc16 import CRC16
 from ltchiptool.util.detection import Detection
-from ltchiptool.util.fileio import chext, chname, isnewer, peek
+from ltchiptool.util.fileio import chext, peek
+from ltchiptool.util.fwbinary import FirmwareBinary
 from ltchiptool.util.intbin import betoint, gen2bytes, inttobe32, pad_data
-from ltchiptool.util.logging import graph
 from ltchiptool.util.obj import str2enum
 
 from .util import RBL, BekenBinary, DataType, OTACompression, OTAEncryption
 
 
 def to_offset(addr: int) -> int:
     return int(addr + (addr // 32) * 2)
@@ -37,17 +36,16 @@
             return True
         warning("File CRC16 invalid. Considering as non-CRC file.")
         return
     return None
 
 
 class BK72XXBinary(SocInterface, ABC):
-    def elf2bin(self, input: str, ota_idx: int) -> Dict[str, Optional[int]]:
+    def elf2bin(self, input: str, ota_idx: int) -> List[FirmwareBinary]:
         toolchain = self.board.toolchain
-        result: Dict[str, Optional[int]] = {}
 
         mcu = self.board["build.mcu"]
         coeffs = self.board["build.bkcrypt_coeffs"] or ("0" * 32)
         rbl_size = self.board["build.bkrbl_size_app"]
         ota_encryption = self.board["build.bkota.encryption"]
         ota_compression = self.board["build.bkota.compression"]
         ota_key = self.board["build.bkota.key"]
@@ -65,49 +63,77 @@
         if app_offs != app_part_offs:
             raise ValueError(
                 f"App partition offset (0x{app_part_offs:06X}) doesn't match "
                 f"the generated binary offset (0x{app_offs:06X})"
             )
 
         # build output names
-        out_rbl = chname(input, f"image_{mcu}_app.0x{app_offs:06X}.rbl")
-        out_crc = chname(input, f"image_{mcu}_app.0x{app_offs:06X}.crc")
-        out_rblh = chname(input, f"image_{mcu}_app.0x{rbl_offs:06X}.rblh")
-        out_ota = chname(input, f"image_{mcu}_app.ota.rbl")
-        out_ug = chname(input, f"image_{mcu}_app.ota.ug.bin")
+        out_ug = FirmwareBinary(
+            location=input,
+            name=f"{mcu}_app",
+            subname="ota.ug",
+            ext="bin",
+            title="Cloudcutter Image",
+            description="UG Image for flashing with tuya-cloudcutter",
+            public=True,
+        )
+        out_ota = FirmwareBinary(
+            location=input,
+            name=f"{mcu}_app",
+            subname="ota",
+            ext="rbl",
+            title="Beken OTA Image",
+            description="For flashing using Beken or OpenBeken OTA",
+            public=True,
+        )
+        out_rbl = FirmwareBinary(
+            location=input,
+            name=f"{mcu}_app",
+            offset=app_offs,
+            ext="rbl",
+            title="Beken Application Image",
+            public=True,
+        )
+        out_crc = FirmwareBinary(
+            location=input,
+            name=f"{mcu}_app",
+            offset=app_offs,
+            ext="crc",
+            title="Beken CRC/UA App",
+        )
+        out_rblh = FirmwareBinary(
+            location=input,
+            name=f"{mcu}_app",
+            offset=rbl_offs,
+            ext="rblh",
+            title="Beken Application RBL Header",
+        )
         fw_bin = chext(input, "bin")
-        outputs = [out_rbl, out_crc, out_rblh, out_ota, out_ug]
         # print graph element
-        graph(1, basename(out_rbl))
+        out_rbl.graph(1)
         # objcopy ELF -> raw BIN
         toolchain.objcopy(input, fw_bin)
-        result[fw_bin] = None
         # return if all outputs are up-to-date
-        if all(map(lambda f: isnewer(f, fw_bin), outputs)):
-            result[out_rbl] = app_offs
-            result[out_crc] = None
-            result[out_rblh] = rbl_offs
-            result[out_ota] = None
-            result[out_ug] = None
-            return result
+        if all(binary.isnewer(than=fw_bin) for binary in out_rbl.group_get()):
+            return out_rbl.group()
 
         bk = BekenBinary(coeffs)
         rbl = RBL(
             name="app",
             version=f"{version}-{mcu}",
             container_size=app_size,
         )
 
         fw_size = stat(fw_bin).st_size
         raw = open(fw_bin, "rb")
-        out = open(out_rbl, "wb")
+        out = out_rbl.write()
 
         # open encrypted+CRC binary output
-        graph(1, basename(out_crc))
-        crc = open(out_crc, "wb")
+        out_crc.graph(1)
+        crc = out_crc.write()
 
         # get partial (type, bytes) data generator
         package_gen = bk.package(raw, app_addr, fw_size, rbl, partial=True)
 
         # write all BINARY blocks
         for data_type, data in package_gen:
             if data_type != DataType.BINARY:
@@ -116,73 +142,67 @@
             crc.write(data)
 
         # skip PADDING_SIZE bytes for RBL header, write it to main output
         if data_type == DataType.PADDING_SIZE:
             out.write(b"\xff" * data)
 
         # open RBL header output
-        graph(1, basename(out_rblh))
-        rblh = open(out_rblh, "wb")
+        out_rblh.graph(1)
+        rblh = out_rblh.write()
 
         # write all RBL blocks
         for data_type, data in package_gen:
             if data_type != DataType.RBL:
                 break
             out.write(data)
             rblh.write(data)
 
-        result[out_rbl] = app_offs
-        result[out_crc] = None
-        result[out_rblh] = rbl_offs
-
         # write OTA package
         rbl = RBL(
             name="app",
             version=f"{version}-{mcu}",
             encryption=str2enum(OTAEncryption, ota_encryption) or OTAEncryption.NONE,
             compression=str2enum(OTACompression, ota_compression)
             or OTACompression.NONE,
         )
-        graph(1, basename(out_ota))
+        out_ota.graph(1)
         # seek back to start
         raw.seek(0, SEEK_SET)
         ota_gen = bk.ota_package(raw, rbl, key=ota_key, iv=ota_iv)
         ota_data = BytesIO()
-        ota = open(out_ota, "wb")
+        ota = out_ota.write()
         for data in ota_gen:
             ota.write(data)
             ota_data.write(data)
         if rbl.data_size > ota_size:
             warning(
                 f"OTA size too large: {rbl.data_size} > {ota_size} (0x{ota_size:X})"
             )
-        result[out_ota] = None
 
         # write Tuya OTA package (UG)
-        graph(1, basename(out_ug))
-        with open(out_ug, "wb") as ug:
+        out_ug.graph(1)
+        with out_ug.write() as ug:
             hdr = BytesIO()
             ota_bin = ota_data.getvalue()
             hdr.write(b"\x55\xAA\x55\xAA")
             hdr.write(pad_data(version.encode(), 12, 0x00))
             hdr.write(inttobe32(len(ota_bin)))
             hdr.write(inttobe32(sum(ota_bin)))
             ug.write(hdr.getvalue())
             ug.write(inttobe32(sum(hdr.getvalue())))
             ug.write(b"\xAA\x55\xAA\x55")
             ug.write(ota_bin)
-        result[out_ug] = None
 
         # close all files
         raw.close()
         out.close()
         crc.close()
         rblh.close()
         ota.close()
-        return result
+        return out_rbl.group()
 
     def detect_file_type(
         self,
         file: IO[bytes],
         length: int,
     ) -> Optional[Detection]:
         data = peek(file, size=96)
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/bkpackager.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/bkpackager.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/main.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/binary.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/crypto.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/models.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/models.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/bk72xx/util/rbl.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/bk72xx/util/rbl.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/common.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os import stat, unlink
 from os.path import basename, isfile
 from shutil import copyfile
 from typing import Dict, List, Optional, Tuple
 
 from ltchiptool.models import OTAType
 from ltchiptool.util.fileio import chext
+from ltchiptool.util.fwbinary import FirmwareBinary
 from ltchiptool.util.logging import graph
 
 from .interface import SocInterface
 
 
 def ldargs_parse(
     args: List[str],
@@ -77,16 +78,16 @@
         return {ota_idx + 1: elf for ota_idx, (elf, _) in enumerate(elfs)}
 
     def link2bin(
         self,
         ota1: str,
         ota2: str,
         args: List[str],
-    ) -> Dict[str, Optional[int]]:
+    ) -> List[FirmwareBinary]:
         elfs = self.link2elf(ota1, ota2, args)
-        output = {}
+        output = []
 
         for ota_idx, elf in elfs.items():
             # generate a set of binaries for the SoC
             bins = self.elf2bin(elf, ota_idx)
-            output.update(bins)
+            output += bins
         return output
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/soc/interface.py` & `ltchiptool-4.0.0a3/ltchiptool/soc/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from abc import ABC
 from typing import IO, Dict, Generator, List, Optional, Union
 
 from ltchiptool import Board, Family
 from ltchiptool.models import OTAType
 from ltchiptool.util.flash import FlashConnection, ProgressCallback
+from ltchiptool.util.fwbinary import FirmwareBinary
 from uf2tool import UploadContext
 
 
 class SocInterface(ABC):
     family: Family = None
     board: Board = None
     conn: FlashConnection = None
@@ -73,23 +74,23 @@
     ) -> Dict[int, str]:
         raise NotImplementedError()
 
     def elf2bin(
         self,
         input: str,
         ota_idx: int,
-    ) -> Dict[str, Optional[int]]:
+    ) -> List[FirmwareBinary]:
         raise NotImplementedError()
 
     def link2bin(
         self,
         ota1: str,
         ota2: str,
         args: List[str],
-    ) -> Dict[str, Optional[int]]:
+    ) -> List[FirmwareBinary]:
         raise NotImplementedError()
 
     def detect_file_type(
         self,
         file: IO[bytes],
         length: int,
     ) -> Optional["Detection"]:
```

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/bitint.py` & `ltchiptool-4.0.0a3/ltchiptool/util/bitint.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/cli.py` & `ltchiptool-4.0.0a3/ltchiptool/util/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/crc16.py` & `ltchiptool-4.0.0a3/ltchiptool/util/crc16.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/detection.py` & `ltchiptool-4.0.0a3/ltchiptool/util/detection.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/dict.py` & `ltchiptool-4.0.0a3/ltchiptool/util/dict.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/fileio.py` & `ltchiptool-4.0.0a3/ltchiptool/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/flash.py` & `ltchiptool-4.0.0a3/ltchiptool/util/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/intbin.py` & `ltchiptool-4.0.0a3/ltchiptool/util/intbin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/logging.py` & `ltchiptool-4.0.0a3/ltchiptool/util/logging.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/lvm.py` & `ltchiptool-4.0.0a3/ltchiptool/util/lvm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/misc.py` & `ltchiptool-4.0.0a3/ltchiptool/util/misc.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/obj.py` & `ltchiptool-4.0.0a3/ltchiptool/util/obj.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/slice.py` & `ltchiptool-4.0.0a3/ltchiptool/util/slice.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/util/toolchain.py` & `ltchiptool-4.0.0a3/ltchiptool/util/toolchain.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/ltchiptool/version.py` & `ltchiptool-4.0.0a3/ltchiptool/version.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/pyproject.toml` & `ltchiptool-4.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ltchiptool"
-version = "4.0.0a2"
+version = "4.0.0a3"
 description = "Universal flashing and binary manipulation tool for IoT chips"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 packages = [
     { include = "ltchiptool" },
     { include = "uf2tool" },
 ]
```

### Comparing `ltchiptool-4.0.0a2/uf2tool/binpatch/bindiff.py` & `ltchiptool-4.0.0a3/uf2tool/binpatch/bindiff.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/binpatch/diff32.py` & `ltchiptool-4.0.0a3/uf2tool/binpatch/diff32.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/cli.py` & `ltchiptool-4.0.0a3/uf2tool/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/block.py` & `ltchiptool-4.0.0a3/uf2tool/models/block.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/context.py` & `ltchiptool-4.0.0a3/uf2tool/models/context.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/enums.py` & `ltchiptool-4.0.0a3/uf2tool/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/flags.py` & `ltchiptool-4.0.0a3/uf2tool/models/flags.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/image.py` & `ltchiptool-4.0.0a3/uf2tool/models/image.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/partition.py` & `ltchiptool-4.0.0a3/uf2tool/models/partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/models/uf2.py` & `ltchiptool-4.0.0a3/uf2tool/models/uf2.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/upload/esphome.py` & `ltchiptool-4.0.0a3/uf2tool/upload/esphome.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/uf2tool/writer.py` & `ltchiptool-4.0.0a3/uf2tool/writer.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.0.0a2/PKG-INFO` & `ltchiptool-4.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool
-Version: 4.0.0a2
+Version: 4.0.0a3
 Summary: Universal flashing and binary manipulation tool for IoT chips
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

