# Comparing `tmp/ccsdspy-1.0.0.tar.gz` & `tmp/ccsdspy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsdspy-1.0.0.tar", last modified: Thu Feb  2 16:26:20 2023, max compression
+gzip compressed data, was "ccsdspy-1.1.0.tar", last modified: Tue Apr 11 15:17:49 2023, max compression
```

## Comparing `ccsdspy-1.0.0.tar` & `ccsdspy-1.1.0.tar`

### file list

```diff
@@ -1,175 +1,182 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.440078 ccsdspy-1.0.0/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.249486 ccsdspy-1.0.0/.github/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.272929 ccsdspy-1.0.0/.github/workflows/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/.github/workflows/ccsdspy-ci.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/.github/workflows/doc-build.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/.gitignore
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1220 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/CHANGELOG.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/LICENSE.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4739 2023-02-02 16:26:20.440078 ccsdspy-1.0.0/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2200 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.278558 ccsdspy-1.0.0/ccsdspy/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      501 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/__main__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      160 2023-02-02 16:26:19.000000 ccsdspy-1.0.0/ccsdspy/_version.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13263 2023-02-02 16:24:40.000000 ccsdspy-1.0.0/ccsdspy/decode.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5911 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    16804 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/packet_types.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.291649 ccsdspy-1.0.0/ccsdspy/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.260103 ccsdspy-1.0.0/ccsdspy/tests/data/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.291649 ccsdspy-1.0.0/ccsdspy/tests/data/hs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.294641 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid001/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid001/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.296670 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid010/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid010/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.299629 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid035/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1191 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid035/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.301654 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid130/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid130/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.305644 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid251/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid251/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.311596 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid895/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid895/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.313622 ccsdspy-1.0.0/ccsdspy/tests/data/hs/attic/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2116 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/hs/attic/expand_mnemnonics.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.317772 ccsdspy-1.0.0/ccsdspy/tests/data/packet_def/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/packet_def/simple_csv_3col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/packet_def/simple_csv_4col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.327220 ccsdspy-1.0.0/ccsdspy/tests/data/split/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first100pkts.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00384.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00386.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00391.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00392.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00393.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00394.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/apid01313.tlm
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.396976 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Conventions.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_HI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/LIMITS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Overview.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Revision History.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_META.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.401130 ccsdspy-1.0.0/ccsdspy/tests/data/var_length/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/var_length/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/var_length/var_length_packets.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1213 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/var_length/var_length_packets.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4602 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_hs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1486 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6245 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_packet_types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4197 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_primary_header.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_split.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2244 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/tests/test_var_length.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1912 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/ccsdspy/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.284130 ccsdspy-1.0.0/ccsdspy.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4739 2023-02-02 16:26:20.000000 ccsdspy-1.0.0/ccsdspy.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6117 2023-02-02 16:26:20.000000 ccsdspy-1.0.0/ccsdspy.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-02-02 16:26:20.000000 ccsdspy-1.0.0/ccsdspy.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2023-02-02 16:26:20.000000 ccsdspy-1.0.0/ccsdspy.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-02-02 16:26:20.000000 ccsdspy-1.0.0/ccsdspy.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.409076 ccsdspy-1.0.0/docs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/Makefile
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.409076 ccsdspy-1.0.0/docs/_static/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/logo.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.421142 ccsdspy-1.0.0/docs/_static/used-by/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/goes-r.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/hermes.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/mms.jpg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/punch.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/resize.sh
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.425160 ccsdspy-1.0.0/docs/_static/used-by/small/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/small/goes-r.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/small/hermes.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/small/mms.jpg
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_static/used-by/small/punch.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.428143 ccsdspy-1.0.0/docs/_templates/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_templates/github.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/_templates/logo.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)       99 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/api.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7611 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/conf.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.428964 ccsdspy-1.0.0/docs/dev-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7282 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/dev-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2731 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/make.bat
--rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.437086 ccsdspy-1.0.0/docs/user-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3411 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/ccsds.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3224 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/fixedlength.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      228 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1824 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/packetfields.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      997 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/utils.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1521 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/user-guide/variablelength.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-02 16:26:20.439116 ccsdspy-1.0.0/docs/whatsnew/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/whatsnew/changelog.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/docs/whatsnew/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2620 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      542 2023-02-02 16:14:56.000000 ccsdspy-1.0.0/readthedocs.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2023-02-02 16:26:20.441107 ccsdspy-1.0.0/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.897923 ccsdspy-1.1.0/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.594823 ccsdspy-1.1.0/.github/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.746812 ccsdspy-1.1.0/.github/workflows/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.github/workflows/ccsdspy-ci.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.github/workflows/doc-build.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.gitignore
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2588 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/LICENSE.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-11 15:17:49.903884 ccsdspy-1.1.0/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2546 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.824060 ccsdspy-1.1.0/ccsdspy/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      526 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/__main__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      160 2023-04-11 15:17:46.000000 ccsdspy-1.1.0/ccsdspy/_version.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      166 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/constants.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9270 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19073 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/decode.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6540 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    24216 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/packet_types.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.943268 ccsdspy-1.1.0/ccsdspy/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.656934 ccsdspy-1.1.0/ccsdspy/tests/data/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.949858 ccsdspy-1.1.0/ccsdspy/tests/data/hs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.967831 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.980799 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.994356 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1159 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.015908 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.040843 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.099735 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.115676 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2116 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.138978 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_3col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_4col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.198488 ccsdspy-1.1.0/ccsdspy/tests/data/split/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00384.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00386.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00391.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00392.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00393.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00394.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid01313.tlm
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.705382 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Conventions.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_HI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/LIMITS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Overview.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Revision History.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.731861 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1213 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2015 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      590 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11320 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/tests/test_converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4837 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_hs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3103 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7600 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_packet_types.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8837 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/tests/test_primary_header.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_split.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4756 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4182 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_var_length.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7887 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:48.865178 ccsdspy-1.1.0/ccsdspy.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-11 15:17:47.000000 ccsdspy-1.1.0/ccsdspy.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6402 2023-04-11 15:17:48.000000 ccsdspy-1.1.0/ccsdspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-11 15:17:47.000000 ccsdspy-1.1.0/ccsdspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2023-04-11 15:17:47.000000 ccsdspy-1.1.0/ccsdspy.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-04-11 15:17:47.000000 ccsdspy-1.1.0/ccsdspy.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.760821 ccsdspy-1.1.0/docs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/Makefile
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.764777 ccsdspy-1.1.0/docs/_static/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/logo.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.805701 ccsdspy-1.1.0/docs/_static/used-by/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/goes-r.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/hermes.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/mms.jpg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/punch.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/resize.sh
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.827779 ccsdspy-1.1.0/docs/_static/used-by/small/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/goes-r.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/hermes.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/mms.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/punch.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.840744 ccsdspy-1.1.0/docs/_templates/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-03-18 01:24:52.000000 ccsdspy-1.1.0/docs/_templates/github.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_templates/logo.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      134 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/api.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7670 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/conf.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.845566 ccsdspy-1.1.0/docs/dev-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7281 2023-03-18 01:25:20.000000 ccsdspy-1.1.0/docs/dev-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2830 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/make.bat
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.883779 ccsdspy-1.1.0/docs/user-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3411 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/ccsds.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3995 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/user-guide/converters.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3253 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/fixedlength.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      243 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/user-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1853 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/packetfields.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/utils.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3777 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/variablelength.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:17:49.892756 ccsdspy-1.1.0/docs/whatsnew/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/whatsnew/changelog.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/whatsnew/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2716 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      542 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/readthedocs.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2023-04-11 15:17:49.906756 ccsdspy-1.1.0/setup.cfg
```

### Comparing `ccsdspy-1.0.0/.github/workflows/ccsdspy-ci.yml` & `ccsdspy-1.1.0/.github/workflows/ccsdspy-ci.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/.github/workflows/doc-build.yml` & `ccsdspy-1.1.0/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/.gitignore` & `ccsdspy-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/LICENSE.rst` & `ccsdspy-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/PKG-INFO` & `ccsdspy-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.0.0
+Version: 1.1.0
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -44,24 +44,24 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 CCSDSPy - IO Interface for Reading CCSDS Data in Python.
 ========================================================
 
-.. image:: https://github.com/ddasilva/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
-    :target: https://github.com/ddasilva/ccsdspy/actions
+.. image:: https://github.com/ccsdspy/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
+    :target: https://github.com/ccsdspy/ccsdspy/actions
     :alt: CI Status
 
 
-.. image:: https://codecov.io/gh/ddasilva/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
-    :target: https://codecov.io/gh/ddasilva/ccsdspy
+.. image:: https://codecov.io/gh/ccsdspy/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
+    :target: https://codecov.io/gh/ccsdspy/ccsdspy
     :alt: Code Coverage	  
 	  
-This package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions.
+This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
  
 Installation
 ============
 To install ccsdspy
 
 .. code::
 
@@ -93,14 +93,18 @@
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
 
+Getting Help
+============
+For more information or to ask questions about the library or CCSDS data in general, check out the `CCSDSPy Discussion Board <https://github.com/ccsdspy/ccsdspy/discussions>`__ hosted through GitHub.
+
 Acknowledging or Citing ccsdspy
 ===============================
 If you use ccsdspy, it would be appreciated if you let us know and mention it in your publications. The continued growth and development of this package is dependent on the community being aware of it.
 
 Code of Conduct
 ===============
 When interacting with this package please behave consistent with the following `Code of Conduct <https://www.contributor-covenant.org/version/2/1/code_of_conduct/>`__.
```

### Comparing `ccsdspy-1.0.0/README.rst` & `ccsdspy-1.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 CCSDSPy - IO Interface for Reading CCSDS Data in Python.
 ========================================================
 
-.. image:: https://github.com/ddasilva/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
-    :target: https://github.com/ddasilva/ccsdspy/actions
+.. image:: https://github.com/ccsdspy/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
+    :target: https://github.com/ccsdspy/ccsdspy/actions
     :alt: CI Status
 
 
-.. image:: https://codecov.io/gh/ddasilva/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
-    :target: https://codecov.io/gh/ddasilva/ccsdspy
+.. image:: https://codecov.io/gh/ccsdspy/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
+    :target: https://codecov.io/gh/ccsdspy/ccsdspy
     :alt: Code Coverage	  
 	  
-This package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions.
+This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
  
 Installation
 ============
 To install ccsdspy
 
 .. code::
 
@@ -46,14 +46,18 @@
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
 
+Getting Help
+============
+For more information or to ask questions about the library or CCSDS data in general, check out the `CCSDSPy Discussion Board <https://github.com/ccsdspy/ccsdspy/discussions>`__ hosted through GitHub.
+
 Acknowledging or Citing ccsdspy
 ===============================
 If you use ccsdspy, it would be appreciated if you let us know and mention it in your publications. The continued growth and development of this package is dependent on the community being aware of it.
 
 Code of Conduct
 ===============
 When interacting with this package please behave consistent with the following `Code of Conduct <https://www.contributor-covenant.org/version/2/1/code_of_conduct/>`__.
```

### Comparing `ccsdspy-1.0.0/ccsdspy/__main__.py` & `ccsdspy-1.1.0/ccsdspy/__main__.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/packet_fields.py` & `ccsdspy-1.1.0/ccsdspy/packet_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 - packet_types.VariableLength
 """
 
 __author__ = "Daniel da Silva <mail@danieldasilva.org>"
 
 import numpy as np
 
+from .converters import Converter
+
 
 class PacketField:
     """A field contained in a packet."""
 
     def __init__(self, name, data_type, bit_length, bit_offset=None, byte_order="big"):
         """
         Parameters
@@ -63,20 +65,29 @@
 
         self._field_type = "element"
         self._array_shape = None
         self._array_order = None
 
     def __repr__(self):
         values = {k: repr(v) for (k, v) in self.__dict__.items()}
+        values["cls_name"] = self.__class__.__name__
 
-        return (
-            "PacketField(name={_name}, data_type={_data_type}, "
-            "bit_length={_bit_length}, bit_offset={_bit_offset}, "
-            "byte_order={_byte_order})".format(**values)
-        )
+        if values["cls_name"] == "PacketArray":
+            return (
+                "{cls_name}(name={_name}, data_type={_data_type}, "
+                "bit_length={_bit_length}, bit_offset={_bit_offset}, "
+                "byte_order={_byte_order}, array_shape={_array_shape}, "
+                "array_order={_array_order})".format(**values)
+            )
+        else:
+            return (
+                "{cls_name}(name={_name}, data_type={_data_type}, "
+                "bit_length={_bit_length}, bit_offset={_bit_offset}, "
+                "byte_order={_byte_order}".format(**values)
+            )
 
     def __iter__(self):
         return iter(
             [
                 ("name", self._name),
                 ("dataType", self._data_type),
                 ("bitLength", self._bit_length),
@@ -98,36 +109,37 @@
         name : str
             String identifier for the field. The name specified how you may
             call upon this data later.
         data_type : {'uint', 'int', 'float', 'str', 'fill'}
             Data type of the field.
         bit_length : int
             Number of bits contained in the field.
-        array_shape : int, tuple of ints, or 'expand'
+        array_shape : int, tuple of ints, str, 'expand'
             Shape of the array as a tuple. For a 1-dimensional array, a single integer
-            can be supplied. For details on expanding arrays, see the
-            :py:class:`~ccsdspy.VariableLength` class.
+            can be supplied. To use another field's value, pass the name of that field. To
+            grow to fill the packet, use "expand". For details on variable length fields, see
+            the :py:class:`~ccsdspy.VariableLength` class.
         array_order  {'C', 'F'}
             Row-major (C-style) or column-major (Fortran-style) order.
         bit_offset : int, optional
             Bit offset into packet, including the primary header which is 48 bits long.
             If this is not specified, than the bit offset will the be calculated automatically
             from its position inside the packet definition.
         byte_order : {'big', 'little'}, optional
             Byte order of the field. Defaults to big endian.
 
         Raises
         ------
         TypeError
              If one of the arguments is not of the correct type.
         ValueError
-             data_type or byte_order is invalid
+             array_shape, array_order, data_type, or byte_order is invalid
         """
-        if array_shape == "expand":
-            if kwargs["data_type"] is None:
+        if isinstance(array_shape, str):
+            if "data_type" not in kwargs:
                 kwargs["data_type"] = "uint"
             elif kwargs["data_type"] != "uint":
                 raise ValueError("Expanding arrays must be data_type='uint'")
         else:
             if isinstance(array_shape, int):
                 array_shape = (array_shape,)
             if not isinstance(array_shape, tuple):
```

### Comparing `ccsdspy-1.0.0/ccsdspy/packet_types.py` & `ccsdspy-1.1.0/ccsdspy/packet_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """High-level Object-oriented API for the different types of packets
 (FixedLength and VariableLength) supported by the package.
 """
 
 import csv
 import os
+import warnings
 
 import numpy as np
 
+from .converters import Converter
 from .decode import _decode_fixed_length, _decode_variable_length
 from .packet_fields import PacketField, PacketArray
 
 
 __author__ = "Daniel da Silva <mail@danieldasilva.org>"
 
 
@@ -22,16 +24,20 @@
     def _init(self, fields):
         """
         Parameters
         ----------
         fields : list of `ccsdspy.PacketField`
             Layout of packet fields contained in the definition.
         """
+        # List of PacketField instances
         self._fields = fields[:]
 
+        # Dictionary mapping input name to tuple (output_name: str, Converter instance)
+        self._converters = {}
+
     @classmethod
     def from_file(cls, file):
         """
         Parameters
         ----------
         file : str
            Path to file on the local file system that defines the packet fields.
@@ -47,14 +53,69 @@
         if file_extension[1] == ".csv":
             fields = _get_fields_csv_file(file)
         else:
             raise ValueError(f"File type {file_extension[1]} not supported.")
 
         return cls(fields)
 
+    def add_converted_field(self, input_field_name, output_field_name, converter):
+        """Add a converteed field to the packet definition, used to apply
+        post-processing transformatons of decoded fields.
+
+        Parameters
+        ----------
+        input_field_name : str or list/tuple
+           Name of input field, or list/tuple of names of fields. There must be field(s)
+           which exists in the packet definition corresponding to these name(s).
+        output_field_name : str
+           Name of output field. When the packet is decoded using `pkt.load()`,
+           a new field named this will be present in the output dictionary.
+        converter : instance of subclass of `:py:class:~ccsdspy.converters.Converter`
+           A converter object to apply post-processing conversions, such as
+           calibration curves or value replacement. Converter objects
+           can be found in`:py:mod:~ccsdspy.converters`.
+
+        Raises
+        ------
+        TypeError
+           If one of the arguments is not of the correct type.
+        ValueError
+           The provided `input_field_name` is not present in the packet definition
+        """
+        if not isinstance(output_field_name, str):
+            raise TypeError("output_field_name must be a str")
+        if not isinstance(converter, Converter):
+            raise TypeError("converter must be an instance of a Converter subclass")
+
+        # Get tuple of input field names for storing; this handles the input_field_name
+        # argument being either a str, or list/tuple
+        if isinstance(input_field_name, str):
+            input_field_names = (input_field_name,)
+        elif isinstance(input_field_name, (list, tuple)):
+            input_field_names = tuple(input_field_name)
+        else:
+            raise TypeError("input_field_name must be either str, list, or tuple")
+
+        del input_field_name  # don't use the variable again in this function
+
+        # Check that each of the input field names exists in the packet, and report
+        # the missing fields if not
+        fields_in_packet_set = {field._name for field in self._fields}
+        input_field_names_set = set(input_field_names)
+        all_fields_present = input_field_names_set <= fields_in_packet_set  # subset
+
+        if not all_fields_present:
+            missing_fields = input_field_names_set - fields_in_packet_set  # set op A \ B
+            raise ValueError(
+                "Some fields specified as inputs to converters were missing: "
+                f"{sorted(missing_fields)}"
+            )
+
+        self._converters[input_field_names] = (output_field_name, converter)
+
 
 class FixedLength(_BasePacket):
     """Define a fixed length packet to decode binary data.
 
     Fixed length packets correspond to packats that are the same length and
     layout every time. A common example of this is housekeeping or status
     messages.
@@ -68,19 +129,18 @@
             Layout of packet fields contained in the definition.
 
         Raises
         ------
         ValueError
             one or more of the arguments are invalid
         """
-        if any(field._bit_length == "expand" for field in fields):
+        if any(isinstance(field._array_shape, str) for field in fields):
             raise ValueError(
-                "The FixedLength class does not support fields with "
-                "bit_length='expand'. Instead, use the VariableLength "
-                "class."
+                "The FixedLength class does not support variable fields. "
+                "Instead, use the VariableLength class."
             )
 
         self._init(fields)
 
     def load(self, file, include_primary_header=False):
         """Decode a file-like object containing a sequence of these packets.
 
@@ -92,35 +152,57 @@
            If True, provides the primary header in the output
 
         Returns
         -------
         field_arrays : dict, string to NumPy array
             dictionary mapping field names to NumPy arrays, with key order matching
             the order of fields in the packet.
+
+        Warns
+        -----
+        UserWarning
+            If the ccsds sequence count is not in order
+        UserWarning
+            If the ccsds sequence count is missing packets
+        UserWarning
+            If there are more than one APID
         """
-        return _load(
+        packet_arrays = _load(
             file,
             self._fields,
+            self._converters,
             "fixed_length",
-            include_primary_header=include_primary_header,
+            include_primary_header=True,
         )
 
+        # inspect the primary header and issue warning if appropriate
+        _inspect_primary_header_fields(packet_arrays)
+
+        if not include_primary_header:
+            _delete_primary_header_fields(packet_arrays)
+
+        return packet_arrays
+
 
 class VariableLength(_BasePacket):
     """Define a variable length packet to decode binary data.
 
     Variable length packets are packets which have a different length each
-    time. Each variable length packet should have a single `~ccsdspy.PacketArray` with
-    the `array_shape='expand'`, which will grow to fill the packet.
+    time.  Variable length fields are defined as `~ccsdspy.PacketArray` fields
+    where `array_shape="expand"` (causing the field to grow to fill the packet) or
+    `array_shape="other_field"` (causes the field named `other_field` to set the number
+    of elements in this array).
 
     Please note that while this class is able to parse fixed length packets, it
     is much slower. Use the :py:class:`~ccsdspy.FixedLength` class instead.
 
     Rules for variable length packets:
-      * Do provide only one one expanding `~ccsdspy.PacketArray` with `array_shape='expand'`.
+      * Do only specify a `~ccsdspy.PacketArray` with the `array_shape="other_field"`
+        when `other_field` precedes it in the packet definition
+      * Do not provide more than one expanding `~ccsdspy.PacketArray` with `array_shape="expand"`
       * Do not specify the primary header fields manually
       * Do not specify explicit bit_offsets (they will be computed automatically)
     """
 
     def __init__(self, fields):
         """
         Parameters
@@ -132,27 +214,46 @@
 
         Raises
         ------
         ValueError
             one or more of the arguments are invalid, or do not follow the
             specified rules.
         """
+        # Check there is only one expanding field in the packet definition
         expand_arrays = [
             field
             for field in fields
             if isinstance(field, PacketArray) and field._array_shape == "expand"
         ]
 
         if len(expand_arrays) > 1:
             raise ValueError(
                 "The VariableLength class does not support more than one field "
                 "with array_shape='expand', as the decoding process becomes "
                 "ambiguous."
             )
 
+        # Check variable fields with their sizes set by other fields only do so when
+        # the previous field precedes it
+        field_names = [field._name for field in fields]
+
+        for i, field in enumerate(fields):
+            if (
+                isinstance(field, PacketArray)
+                and isinstance(field._array_shape, str)
+                and field._array_shape != "expand"
+                and field._array_shape not in field_names[:i]
+            ):
+                raise ValueError(
+                    "The VariableLength class requires that variable fields with "
+                    "their sizes set by other fields only do so when the "
+                    "previous field precedes it."
+                )
+
+        # Check that bit offsets are not set
         if not all(field._bit_offset is None for field in fields):
             raise ValueError(
                 "The VariableLength class does not support explicit bit "
                 "offsets. You must specify the entire packet so they can be "
                 "determined automatically."
             )
 
@@ -169,26 +270,70 @@
            If True, provides the primary header in the output
 
         Returns
         -------
         field_arrays : dict, string to NumPy array
             dictionary mapping field names to NumPy arrays, with key order matching
             the order of fields in the packet.
+
+        Warns
+        -----
+        UserWarning
+            If the ccsds sequence count is not in order
+        UserWarning
+            If the ccsds sequence count is missing packets
+        UserWarning
+            If there are more than one APID
         """
         # The variable length decoder requires the full packet definition, so if
         # they didn't want the primary header fields, we parse for them and then
         # remove them after.
-        packet_arrays = _load(file, self._fields, "variable_length", include_primary_header=True)
+        packet_arrays = _load(
+            file, self._fields, self._converters, "variable_length", include_primary_header=True
+        )
+
+        # inspect the primary header and issue warning if appropriate
+        _inspect_primary_header_fields(packet_arrays)
 
         if not include_primary_header:
             _delete_primary_header_fields(packet_arrays)
 
         return packet_arrays
 
 
+def _inspect_primary_header_fields(packet_arrays):
+    """Inspects the primary header fields.
+
+    Checks for the following issues
+    * all apids are the same
+    * sequence count is not missing any values
+    * sequence count is in order
+
+    Parameters
+    -----------
+    packet_arrays
+        dictionary mapping field names to NumPy arrays, with key order matching
+        the order fields in the packet. Modified in place
+    """
+    seq_counts = packet_arrays["CCSDS_SEQUENCE_COUNT"]
+    start, end = seq_counts[0], seq_counts[-1]
+    missing_elements = sorted(set(range(start, end + 1)).difference(seq_counts))
+    if len(missing_elements) != 0:
+        warnings.warn(f"Missing packets found {missing_elements}.", UserWarning)
+
+    if not np.all(seq_counts == np.sort(seq_counts)):
+        warnings.warn("Sequence count are out of order.", UserWarning)
+
+    individual_ap_ids = set(packet_arrays["CCSDS_APID"])
+    if len(individual_ap_ids) != 1:
+        warnings.warn(f"Found multiple AP IDs {individual_ap_ids}.", UserWarning)
+
+    return None
+
+
 def _delete_primary_header_fields(packet_arrays):
     """Modifies in place the packet arrays dictionary to delete primary
     header fields.
 
     Parameters
     -----------
     packet_arrays
@@ -220,15 +365,15 @@
     expand_history : dict
       Dictionary mapping array name with shape/data-type and field expansions
     """
     return_fields = []
     expand_history = {}
 
     for existing_field in existing_fields:
-        if existing_field._field_type != "array" or existing_field._array_shape == "expand":
+        if existing_field._field_type != "array" or isinstance(existing_field._array_shape, str):
             return_fields.append(existing_field)
             continue
 
         array_shape = existing_field._array_shape
         array_order = existing_field._array_order
 
         index_vecs = [np.arange(dim) for dim in array_shape]
@@ -432,23 +577,26 @@
                             bit_offset=int(row["bit_offset"]),
                         )
                     )
 
     return fields
 
 
-def _load(file, fields, decoder_name, include_primary_header=False):
+def _load(file, fields, converters, decoder_name, include_primary_header=False):
     """Decode a file-like object containing a sequence of these packets.
 
     Parameters
     ----------
     file: str
        Path to file on the local file system, or file-like object
     fields : list of `ccsdspy.PacketField`
        Layout of packet fields contained in the definition.
+    converters : dict, str to tuple (str, Converter)
+       Dictionary of post-processing conversions. keys are input field names,
+       values are tuples of (output_field_name, Converter instance)
     decoder_name: {'fixed_length', 'variable_length'}
        String identifying which decoder to use.
     include_primary_header: bool
        If True, provides the primary header in the output
 
     Returns
     -------
@@ -477,9 +625,43 @@
     else:
         raise ValueError(
             f"Invalid decoder_name 'f{decoder_name}' specified. Must be "
             "either 'fixed_length', or 'variable_length'"
         )
 
     field_arrays = _unexpand_field_arrays(field_arrays, expand_history)
+    field_arrays = _apply_converters(field_arrays, converters)
 
     return field_arrays
+
+
+def _apply_converters(field_arrays, converters):
+    """Apply post-processing converters in place to a dictionary of field
+    arrays.
+
+    Parameters
+    ----------
+    field_arrays : dict of string to NumPy arrays
+       The decoded packet field arrays without any post-processing applied
+    converters : dict, str to tuple (str, Converter)
+       Dictionary of post-processing conversions. keys are input field names,
+       values are tuples of (output_field_name, Converter instance)
+
+    Returns
+    -------
+    converted_field_arrays : dict of string to NumPy arrays
+       The converted decoded packet field arrays, as a dictionary with the same
+       key as the passed `field_arrays`.
+    """
+    converted = field_arrays.copy()
+
+    for input_field_names, (output_field_name, converter) in converters.items():
+        # Collect list of input arrays to pass as *args to converter function
+        input_arrays = []
+
+        for input_field_name in input_field_names:
+            input_arrays.append(field_arrays[input_field_name])
+
+        # Call converter function
+        converted[output_field_name] = converter.convert(*input_arrays)
+
+    return converted
```

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid001/defs.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid010/defs.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid035/defs.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/defs.csv`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 name,data_type,bit_offset,bit_length,calibration
 pkt35_time_secs,uint,0,32,
 pkt35_time_msecs,uint,32,16,
 pkt35_int8_cnt,int,48,8,
-pkt35_uint16_bitfld,uint,56,16,
 pkt35_cntoverflow,uint,56,1,"{""0"":""NO_OVERFLOW"",""1"":""OVERFLOW""}"
 pkt35_notused,uint,57,7,
 pkt35_sine0status,uint,64,1,"{""0"":""NEGATIVE"",""1"":""POSITIVE""}"
 pkt35_sine1status,uint,65,1,"{""0"":""NEGATIVE"",""1"":""POSITIVE""}"
 pkt35_sine2status,uint,66,1,"{""0"":""NEGATIVE"",""1"":""POSITIVE""}"
 pkt35_sine3status,uint,67,1,"{""0"":""NEGATIVE"",""1"":""POSITIVE""}"
 pkt35_sine4status,uint,68,1,"{""0"":""NEGATIVE"",""1"":""POSITIVE""}"
```

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/hs/attic/expand_mnemnonics.py` & `ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first100pkts.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00384.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00384.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00392.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00392.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00393.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00393.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/apid00394.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00394.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/apid01313.tlm` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid01313.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Conventions.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Conventions.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_HI.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_HI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Overview.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Overview.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/Revision History.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Revision History.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_META.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv` & `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/var_length/README.md` & `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/README.md`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/data/var_length/var_length_packets.py` & `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/test_hs.py` & `ccsdspy-1.1.0/ccsdspy/tests/test_hs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import glob
 import os
 import numpy as np
 
 import pytest
 
 from .. import FixedLength, VariableLength, PacketField, PacketArray
+from ..constants import BITS_PER_BYTE
 
 
 def _run_apid_test(apid, cls):
     """Driver for running an APID test. Each apidXXX directory under
     `data/hs` contains:
 
             defs.csv     -- packet definition with conversions.
@@ -130,16 +131,15 @@
 
     for key, data_type, bit_length in zip(*tmp):
         pkt_fields.append(PacketField(name=key, data_type=data_type, bit_length=bit_length))
 
     normal_pkt = FixedLength(pkt_fields)
 
     # Make FixedLength for array packet
-    fill_length = sum(dict_normal_defs["bit_length"])
-    fill_length = 8 * 32  # 8 float32s at end
+    fill_length = sum(f._bit_length for f in pkt_fields if "[" not in f._name)
 
     array_pkt = FixedLength(
         [
             PacketField(name="unused", data_type="fill", bit_length=fill_length),
             PacketArray(name="PKT35_FLT_SIN_2H", data_type="float", bit_length=32, array_shape=8),
         ]
     )
@@ -149,7 +149,10 @@
     normal_result = normal_pkt.load(ccsds_file_path)
     array_result = array_pkt.load(ccsds_file_path)
 
     for i in range(8):
         assert np.all(
             normal_result[f"PKT35_FLT_SIN_2H[{i}]"] == array_result["PKT35_FLT_SIN_2H"][:, i]
         )
+        # These sin values should be between [0, 1]
+        assert np.abs(normal_result[f"PKT35_FLT_SIN_2H[{i}]"].min() - -1.0) < 1e-3
+        assert np.abs(normal_result[f"PKT35_FLT_SIN_2H[{i}]"].max() - +1.0) < 1e-3
```

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/test_packet_types.py` & `ccsdspy-1.1.0/ccsdspy/tests/test_packet_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 import os.path
 import struct
 
 import numpy as np
 import pytest
 
 from .. import FixedLength, VariableLength, PacketField, PacketArray
+from ..constants import BITS_PER_BYTE
 from ..packet_types import _get_fields_csv_file
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 packet_def_dir = os.path.join(dir_path, "data", "packet_def")
 csv_file_4col = os.path.join(packet_def_dir, "simple_csv_4col.csv")
 csv_file_3col = os.path.join(packet_def_dir, "simple_csv_3col.csv")
 csv_file_4col_with_array = os.path.join(packet_def_dir, "simple_csv_4col_with_array.csv")
 csv_file_3col_with_array = os.path.join(packet_def_dir, "simple_csv_3col_with_array.csv")
 
 
 def test_FixedLength_initializer_copies_field_list():
     """Tests that the FixedLengthPacket initializer stores a copy of the
     provided fields list.
     """
-    fields = [PacketField(name="mnemonic", data_type="uint", bit_length=8)]
+    fields = [PacketField(name="mnemonic", data_type="uint", bit_length=BITS_PER_BYTE)]
     pkt = FixedLength(fields)
     assert pkt._fields is not fields
 
 
 def test_get_fields_csv_file_3col():
     """Test that the csv reader parses the 3 column test file correctly."""
 
@@ -175,7 +176,56 @@
     results = pkt.load(io.BytesIO(packet_stream))
 
     # Check results
     for k in range(num_packets):
         for i in range(32):
             for j in range(4):
                 assert results["array"][k, i, j] == k * (2 * i + j)
+
+
+def test_fixed_length_rejects_expanding():
+    with pytest.raises(ValueError):
+        FixedLength(
+            [
+                PacketArray(
+                    name="array",
+                    array_shape="expand",
+                    data_type="uint",
+                    bit_length=BITS_PER_BYTE,
+                )
+            ]
+        )
+
+
+def test_variable_length_rejects_multiple_expanding():
+    with pytest.raises(ValueError):
+        FixedLength(
+            [
+                PacketArray(
+                    name="array1",
+                    array_shape="expand",
+                    data_type="uint",
+                    bit_length=BITS_PER_BYTE,
+                ),
+                PacketArray(
+                    name="array2",
+                    array_shape="expand",
+                    data_type="uint",
+                    bit_length=BITS_PER_BYTE,
+                ),
+            ]
+        )
+
+
+def test_variable_length_rejects_bit_offset():
+    with pytest.raises(ValueError):
+        FixedLength(
+            [
+                PacketArray(
+                    name="array1",
+                    array_shape="expand",
+                    data_type="uint",
+                    bit_length=BITS_PER_BYTE,
+                    bit_offset=32,
+                ),
+            ]
+        )
```

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/test_split.py` & `ccsdspy-1.1.0/ccsdspy/tests/test_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def test_command_line_split():
     """Tests command line interface to the code"""
     # TemporaryDirectory() will delete itself when its garbage collected
     # or when the program ends
     tmp_dir = tempfile.TemporaryDirectory()
     dir_path = os.path.dirname(os.path.realpath(__file__))
     data_path = os.path.join(dir_path, "data", "split")
-    mixed_stream = os.path.join(data_path, "CYGNSS_F7_L0_2022_086_10_15_V01_F__first100pkts.tlm")
+    mixed_stream = os.path.join(data_path, "CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm")
     shutil.copy(mixed_stream, tmp_dir.name)
 
     # Call module_main() with fake argv and custom working directory
     module_main(
         argv=[
             "__tests__",
             "split",
@@ -114,15 +114,15 @@
             )
             fields.append(field)
 
         # drop first seven because are they primary header
         packet_by_apid[apid] = cls(fields[7:])
 
     # Do split and test result to ground truth
-    mixed_stream = os.path.join(data_path, "CYGNSS_F7_L0_2022_086_10_15_V01_F__first100pkts.tlm")
+    mixed_stream = os.path.join(data_path, "CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm")
     stream_by_apid = split_by_apid(mixed_stream, valid_apids=list(packet_by_apid.keys()))
 
     for apid, stream_from_split in stream_by_apid.items():
         if apid in [132, 134, 389, 391]:
             # Known to have problems for acceptable reasons (insufficient packet definition)
             continue
```

### Comparing `ccsdspy-1.0.0/ccsdspy/tests/test_var_length.py` & `ccsdspy-1.1.0/ccsdspy/tests/test_var_length.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,15 +29,21 @@
     assert field_arrays["data"].dtype == object
     assert field_arrays["data"].size == 10
     assert all([arr.itemsize == 2 for arr in field_arrays["data"]])
 
     sizes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
 
     for i in range(len(sizes)):
-        assert field_arrays["data"][i].shape == (sizes[i],)
+        try:
+            assert field_arrays["data"][i].shape == (sizes[i],)
+        except:
+            import pdb
+
+            pdb.set_trace()
+
         expected = np.arange(sizes[i], dtype="uint16") + sizes[i]
         assert np.all(field_arrays["data"][i] == expected)
 
 
 @pytest.mark.parametrize("include_primary_header", [True, False])
 def test_var_length_data_with_footer(include_primary_header):
     dir_path = os.path.dirname(os.path.realpath(__file__))
@@ -63,7 +69,60 @@
 
     sizes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
 
     for i in range(10):
         assert field_arrays["data"][i].shape == (sizes[i],)
         expected = np.arange(sizes[i], dtype="uint16") + sizes[i]
         assert np.all(field_arrays["data"][i] == expected)
+
+
+@pytest.mark.parametrize("include_primary_header", [True, False])
+def test_var_length_double_varfield_with_footer(include_primary_header):
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    bin_path = os.path.join(
+        dir_path, "data", "var_length", "var_length_packets_double_varfield_with_footer.bin"
+    )
+
+    pkt = VariableLength(
+        [
+            PacketField(name="data1_len", data_type="uint", bit_length=8),
+            PacketArray(
+                name="data1",
+                data_type="uint",
+                bit_length=16,
+                array_shape="data1_len",
+            ),
+            PacketField(name="data2_len", data_type="uint", bit_length=8),
+            PacketArray(
+                name="data2",
+                data_type="uint",
+                bit_length=16,
+                array_shape="data2_len",
+            ),
+            PacketField(name="footer", data_type="uint", bit_length=16),
+        ]
+    )
+
+    field_arrays = pkt.load(bin_path, include_primary_header=include_primary_header)
+
+    # Check footer
+    assert np.all(field_arrays["footer"] == 1)
+
+    # Check data1 array
+    assert field_arrays["data1"].dtype == object
+    assert field_arrays["data1"].size == 10
+    sizes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
+
+    for i in range(10):
+        assert field_arrays["data1"][i].shape == (sizes[i],)
+        expected = np.arange(sizes[i], dtype="uint16") + sizes[i]
+        assert np.all(field_arrays["data1"][i] == expected)
+
+    # Check data2 array
+    assert field_arrays["data2"].dtype == object
+    assert field_arrays["data2"].size == 10
+    sizes = [5, 7, 2, 8, 3, 41, 42, 1, 3, 4]
+
+    for i in range(10):
+        assert field_arrays["data2"][i].shape == (sizes[i],)
+        expected = np.arange(sizes[i], dtype="uint16")
+        assert np.all(field_arrays["data2"][i] == expected)
```

### Comparing `ccsdspy-1.0.0/ccsdspy.egg-info/PKG-INFO` & `ccsdspy-1.1.0/ccsdspy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.0.0
+Version: 1.1.0
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -44,24 +44,24 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 CCSDSPy - IO Interface for Reading CCSDS Data in Python.
 ========================================================
 
-.. image:: https://github.com/ddasilva/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
-    :target: https://github.com/ddasilva/ccsdspy/actions
+.. image:: https://github.com/ccsdspy/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
+    :target: https://github.com/ccsdspy/ccsdspy/actions
     :alt: CI Status
 
 
-.. image:: https://codecov.io/gh/ddasilva/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
-    :target: https://codecov.io/gh/ddasilva/ccsdspy
+.. image:: https://codecov.io/gh/ccsdspy/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
+    :target: https://codecov.io/gh/ccsdspy/ccsdspy
     :alt: Code Coverage	  
 	  
-This package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions.
+This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
  
 Installation
 ============
 To install ccsdspy
 
 .. code::
 
@@ -93,14 +93,18 @@
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
 
+Getting Help
+============
+For more information or to ask questions about the library or CCSDS data in general, check out the `CCSDSPy Discussion Board <https://github.com/ccsdspy/ccsdspy/discussions>`__ hosted through GitHub.
+
 Acknowledging or Citing ccsdspy
 ===============================
 If you use ccsdspy, it would be appreciated if you let us know and mention it in your publications. The continued growth and development of this package is dependent on the community being aware of it.
 
 Code of Conduct
 ===============
 When interacting with this package please behave consistent with the following `Code of Conduct <https://www.contributor-covenant.org/version/2/1/code_of_conduct/>`__.
```

### Comparing `ccsdspy-1.0.0/ccsdspy.egg-info/SOURCES.txt` & `ccsdspy-1.1.0/ccsdspy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 readthedocs.yml
 setup.cfg
 .github/workflows/ccsdspy-ci.yml
 .github/workflows/doc-build.yml
 ccsdspy/__init__.py
 ccsdspy/__main__.py
 ccsdspy/_version.py
+ccsdspy/constants.py
+ccsdspy/converters.py
 ccsdspy/decode.py
 ccsdspy/packet_fields.py
 ccsdspy/packet_types.py
 ccsdspy/utils.py
 ccsdspy.egg-info/PKG-INFO
 ccsdspy.egg-info/SOURCES.txt
 ccsdspy.egg-info/dependency_links.txt
 ccsdspy.egg-info/requires.txt
 ccsdspy.egg-info/top_level.txt
 ccsdspy/tests/__init__.py
+ccsdspy/tests/test_converters.py
 ccsdspy/tests/test_hs.py
 ccsdspy/tests/test_packet_fields.py
 ccsdspy/tests/test_packet_types.py
 ccsdspy/tests/test_primary_header.py
 ccsdspy/tests/test_split.py
+ccsdspy/tests/test_utils.py
 ccsdspy/tests/test_var_length.py
 ccsdspy/tests/data/hs/README.rst
 ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
 ccsdspy/tests/data/hs/apid001/defs.csv
 ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
 ccsdspy/tests/data/hs/apid010/defs.csv
 ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
@@ -36,20 +40,20 @@
 ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
 ccsdspy/tests/data/hs/apid130/defs.csv
 ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
 ccsdspy/tests/data/hs/apid251/defs.csv
 ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
 ccsdspy/tests/data/hs/apid895/defs.csv
 ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
-ccsdspy/tests/data/hs/attic/expand_mnemnonics.py
+ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
 ccsdspy/tests/data/packet_def/simple_csv_3col.csv
 ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
 ccsdspy/tests/data/packet_def/simple_csv_4col.csv
 ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
-ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first100pkts.tlm
+ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
 ccsdspy/tests/data/split/apid00384.tlm
 ccsdspy/tests/data/split/apid00386.tlm
 ccsdspy/tests/data/split/apid00391.tlm
 ccsdspy/tests/data/split/apid00392.tlm
 ccsdspy/tests/data/split/apid00393.tlm
 ccsdspy/tests/data/split/apid00394.tlm
 ccsdspy/tests/data/split/apid01313.tlm
@@ -113,14 +117,16 @@
 ccsdspy/tests/data/split/defs/SCI_META.csv
 ccsdspy/tests/data/split/defs/SCI_META_V2.csv
 ccsdspy/tests/data/split/defs/SCI_RAW.csv
 ccsdspy/tests/data/split/defs/SUPER_NOM.csv
 ccsdspy/tests/data/var_length/README.md
 ccsdspy/tests/data/var_length/var_length_packets.bin
 ccsdspy/tests/data/var_length/var_length_packets.py
+ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
+ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
 ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
@@ -134,14 +140,15 @@
 docs/_static/used-by/small/hermes.png
 docs/_static/used-by/small/mms.jpg
 docs/_static/used-by/small/punch.png
 docs/_templates/github.html
 docs/_templates/logo.html
 docs/dev-guide/index.rst
 docs/user-guide/ccsds.rst
+docs/user-guide/converters.rst
 docs/user-guide/fixedlength.rst
 docs/user-guide/index.rst
 docs/user-guide/packetfields.rst
 docs/user-guide/utils.rst
 docs/user-guide/variablelength.rst
 docs/whatsnew/changelog.rst
 docs/whatsnew/index.rst
```

### Comparing `ccsdspy-1.0.0/docs/Makefile` & `ccsdspy-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/logo.png` & `ccsdspy-1.1.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/goes-r.png` & `ccsdspy-1.1.0/docs/_static/used-by/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/hermes.png` & `ccsdspy-1.1.0/docs/_static/used-by/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/mms.jpg` & `ccsdspy-1.1.0/docs/_static/used-by/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/punch.png` & `ccsdspy-1.1.0/docs/_static/used-by/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/small/goes-r.png` & `ccsdspy-1.1.0/docs/_static/used-by/small/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/small/hermes.png` & `ccsdspy-1.1.0/docs/_static/used-by/small/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/small/mms.jpg` & `ccsdspy-1.1.0/docs/_static/used-by/small/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/_static/used-by/small/punch.png` & `ccsdspy-1.1.0/docs/_static/used-by/small/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/conf.py` & `ccsdspy-1.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
+from datetime import datetime
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath("../ccsdspy"))
 
 rawfiles = ["images/logo.png"]
 
@@ -64,25 +65,25 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # contents of docs/conf.py
 from importlib.metadata import version
-version = version('ccsdspy')
+
+version = version("ccsdspy")
 # for example take major/minor
 # The short X.Y version.
 # The full version, including alpha/beta/rc tags.
 
 # General information about the project.
 project = "CCSDSPy"
-copyright = f"2018, Daniel da Silva, version={version}"
-author = "Daniel da Silva"
-
-
+authors = "CCSDSPy Developers"
+copyright = f"{datetime.now().year}, {authors}, version={version}"
+author = "CCSDSPy Developers"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
@@ -111,19 +112,17 @@
 # documentation.
 #
 html_theme_options = {
     "description": "A Python package for reading CCSDS packet data.",
     "show_related": True,
     "github_banner": True,
     "github_button": False,
-    "github_user": "ddasilva",
+    "github_user": "ccsdspy",
     "github_repo": "ccsdspy",
-    "extra_nav_links": {
-        "CCSDS blue books": "https://public.ccsds.org/publications/bluebooks.aspx"
-    },
+    "extra_nav_links": {"CCSDS Blue Books": "https://public.ccsds.org/publications/bluebooks.aspx"},
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_logo = "_static/logo.png"
```

### Comparing `ccsdspy-1.0.0/docs/dev-guide/index.rst` & `ccsdspy-1.1.0/docs/dev-guide/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The following standards are based on those provided by the `sunpy <https://github.com/sunpy/sunpy>`__.
 We would like to thank their contribution to the community.
 
 Installing for development
 ==========================
 To install this package for local development, first clone this package from github using your favorite git gui or with the command::
 
-    git clone git@github.com:ddasilva/ccsdspy.git
+    git clone git@github.com:ccsdspy/ccsdspy.git
 
 Then go into the directory and install the package for editing with the following command::
 
     pip install -e '.[dev]'
 
 This will include all of the development dependencies. 
 If you also need to build the documentation locally use the following command::
```

### Comparing `ccsdspy-1.0.0/docs/index.rst` & `ccsdspy-1.1.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 CCSDSPy
 =======
 
-.. image:: https://github.com/ddasilva/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
-    :target: https://github.com/ddasilva/ccsdspy/actions
+.. image:: https://github.com/ccsdspy/ccsdspy/actions/workflows/ccsdspy-ci.yml/badge.svg
+    :target: https://github.com/ccsdspy/ccsdspy/actions
     :alt: CI Status
 
 .. image:: https://img.shields.io/pypi/pyversions/ccsdspy.svg
     :target: https://pypi.org/project/ccsdspy/
 
-.. image:: https://codecov.io/gh/ddasilva/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
-    :target: https://codecov.io/gh/ddasilva/ccsdspy
+.. image:: https://codecov.io/gh/ccsdspy/ccsdspy/branch/main/graph/badge.svg?token=Ia45f4cW8f
+    :target: https://codecov.io/gh/ccsdspy/ccsdspy
     :alt: Code Coverage
 
 CCSDSPy provides an IO Interface for reading CCSDS_ data in Python.
-The CCSDS format is used for many NASA and ESA missions for low-level telemetry, and often contains tightly packed bits to reduce downlink requirements.
+The CCSDS format is used for many NASA and ESA missions for low-level telemetry, and often contains tightly packed bits to reduce downlink requirements. The library is developed with requirements sourced from the community and extensive automated testing. 
 
 .. _CCSDS: https://public.ccsds.org/default.aspx
 
 .. toctree::
    :maxdepth: 2
 
    whatsnew/index
@@ -35,15 +35,15 @@
 .. image:: _static/used-by/small/punch.png
     :target: https://punch.space.swri.edu/
 .. image:: _static/used-by/small/mms.jpg
     :target: https://mms.gsfc.nasa.gov/
 
 Do you know of other missions that use CCSDSPy? Let us know `through a github issue`_!
 
-.. _through a github issue: https://github.com/ddasilva/ccsdspy/issues/new
+.. _through a github issue: https://github.com/ccsdspy/ccsdspy/issues/new
 
 Install ccsdspy
 ---------------
 To install ccsdspy from source, you can use
 
 .. code::
 
@@ -76,8 +76,8 @@
             data_type='uint',
             bit_length=16,
             array_shape=(32, 32),
             array_order='C'
 	),
    ])
 
-   result = pkt.load('MyCCSDS.bin')
+   result = pkt.load('MyCCSDS.tlm')
```

### Comparing `ccsdspy-1.0.0/docs/make.bat` & `ccsdspy-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/user-guide/ccsds.rst` & `ccsdspy-1.1.0/docs/user-guide/ccsds.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.0.0/docs/user-guide/fixedlength.rst` & `ccsdspy-1.1.0/docs/user-guide/fixedlength.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 
 Overview
 ========
 Fixed length packets are one type of packet defined in the CCSDS packet standard.
 This kind of packet does not change in length and so is the easiest to parse quickly since the start of the next packet can easily be calculated.
 This packet type is in contrast to variable length packets which are also supported (see `ccsdspy.VariableLength`).
 
+.. contents::
+   :depth: 2
+
 Defining a packet
------------------
+=================
 Fixed length packets are ones that only include `~ccsdspy.PacketField` that do not vary in size.
 The only `~cccsds.PacketField` which has the option to be variable is `~ccsdspy.PacketArray`.
 The following code defines a simple fixed length packet
 
 .. code-block:: python
 
    import ccsdspy
@@ -38,15 +41,15 @@
 
 .. code-block:: python
 
    import ccsdspy
    pkt = ccsdspy.FixedLength.from_file('packet_definition.csv')
 
 Parsing a file
---------------
+==============
 Once a `~ccsdspy.FixedLength` object is defined, it can be used to read a binary file containing those packets.
 
 .. code-block:: python
 
    import ccsdspy
    from ccsdspy import PacketField, PacketArray
 
@@ -61,26 +64,26 @@
             data_type='uint',
             bit_length=16,
             array_shape=(32, 32),
             array_order='C'
 	),
    ])
 
-   result = pkt.load('MyCCSDS.bin')
+   result = pkt.load('MyCCSDS.tlm')
 
 The result is returned as a dictionary, containing the names as keys and values are each a `~numpy.ndarray` of the interpreted data from each packet.
 The bit length of the `~numpy.ndarray` elements will be rounded up to the next nearest byte.
 
 .. _getting-header:
 
 Getting the CCSDS Header
-------------------------
+========================
 
 It is also possible to return the contents of the packet primary header.
 This may be important to determine the APID or check for packet loss by checking the packet sequence number.
 For a definition of the CCSDS primary header see :ref:`ccsds_standard`.
 
 .. code-block:: python
 
-    result = pkt.load('MyCCSDS.bin', include_primary_header=True)
+    result = pkt.load('MyCCSDS.tlm', include_primary_header=True)
 
-This adds the following fields to the result `CCSDS_VERSION_NUMBER`, `CCSDS_PACKET_TYPE`, `CCSDS_SECONDARY_FLAG`, `CCSDS_SEQUENCE_FLAG`, `CCSDS_SEQUENCE_COUNT`, `CCSDS_PACKET_LENGTH`.
+This adds the following fields to the result `CCSDS_VERSION_NUMBER`, `CCSDS_PACKET_TYPE`, `CCSDS_SECONDARY_FLAG`, `CCSDS_SEQUENCE_FLAG`, `CCSDS_SEQUENCE_COUNT`, `CCSDS_PACKET_LENGTH`.
```

### Comparing `ccsdspy-1.0.0/docs/user-guide/packetfields.rst` & `ccsdspy-1.1.0/docs/user-guide/packetfields.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 Defining Packet Fields
 **********************
 
 All fields in a packet including those in the packet primary header are defined by a name, bit length (if available), and data type.
 This is done by using one of the following objects `~ccsdspy.PacketField` and `~ccsdspy.PacketArray`.
 These objects are used by the packet objects `~ccsdspy.FixedLength` and `~ccsdspy.VariableLength`.
 
+.. contents::
+   :depth: 2
+
+
 PacketField
------------
+===========
 The `~ccsdspy.PacketField` is used to define most fields in a packet as well as the packet primary header.
 It can be defined simply, for example::
 
     PacketField(name='SHCOARSE', data_type='uint', bit_length=32)
 
 It requires a name, data type, as well as bit length.
 The name can be any string.
 This string is used as the index in the resulting dictionary once a packet is parsed.
 It is also possible to provide a bit offset to define precisely its position within the packet.
 This is typically not necessary because packet are defined in a list.
 Without a bit offset, its value is calculated automatically assuming that the order of packet fields is correct.
 
 PacketArray
------------
+===========
 The `~ccsdspy.PacketArray` provides a simple way to define multiple repeating packet fields.
 It is defined similarly to `~ccsdspy.PacketField` but adds a few new keywords, for example::
 
     PacketArray(name='SENSOR_GRID', data_type='uint', bit_length=16,
                 array_shape=(32, 32), array_order='C')
 
 The bit length is the value for each element in the array.
```

### Comparing `ccsdspy-1.0.0/pyproject.toml` & `ccsdspy-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -53,30 +53,33 @@
 
 [tool.setuptools]
 packages = ["ccsdspy"]
 
 [tool.setuptools_scm]
 write_to = "ccsdspy/_version.py"
 
-[tool.pytest]
-minversion = 3.0
+[tool.pytest.ini_options]
+minversion = "6.0"
 testpaths = ["ccsdspy/tests", "docs"]
-norecursedirs = ["build", "docs/_build", "docs/generated", "*.egg-info"]
+norecursedirs = ["build", "docs/_build", "docs/generated", "*.egg-info", "attic"]
 doctest_plus = "enabled"
 text_file_format = "rst"
 addopts = "--doctest-modules"
+collect_ignore_glob= ['_*.py']
 filterwarnings = [
-    # This is due to dependencies building with a numpy version different from
-    # the local installed numpy version, but should be fine
-    # See https://github.com/numpy/numpy/issues/15748#issuecomment-598584838
-    "ignore:numpy.ufunc size changed:RuntimeWarning",
-    "ignore:numpy.ndarray size changed:RuntimeWarning",
-    # See https://github.com/astropy/extension-helpers/issues/23
-    "ignore:Distutils was imported before Setuptools"
- ]
+  "ignore::UserWarning",
+  "ignore::DeprecationWarning",
+  # This is due to dependencies building with a numpy version different from
+  # the local installed numpy version, but should be fine
+  # See https://github.com/numpy/numpy/issues/15748#issuecomment-598584838
+  "ignore:numpy.ufunc size changed:RuntimeWarning",
+  "ignore:numpy.ndarray size changed:RuntimeWarning",
+  # See https://github.com/astropy/extension-helpers/issues/23
+  "ignore:Distutils was imported before Setuptools"
+]
 
 
 [tool.coverage.run]
 omit = [
   'ccsdspy/__init*',
   'ccsdspy/conftest.py',
   'ccsdspy/*setup_package*',
```

### Comparing `ccsdspy-1.0.0/readthedocs.yml` & `ccsdspy-1.1.0/readthedocs.yml`

 * *Files identical despite different names*

