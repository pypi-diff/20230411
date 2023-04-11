# Comparing `tmp/automation_rest_server-3.6.4.tar.gz` & `tmp/automation_rest_server-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.6.4.tar", last modified: Mon Apr 10 10:02:29 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.6.5.tar", last modified: Tue Apr 11 03:21:46 2023, max compression
```

## Comparing `automation_rest_server-3.6.4.tar` & `automation_rest_server-3.6.5.tar`

### file list

```diff
@@ -1,153 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.4/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     3914 2023-04-10 08:49:21.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1992 2023-04-10 08:33:59.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10711 2023-03-31 07:34:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.4/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.4/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.4/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.4/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-04-10 10:02:07.000000 automation_rest_server-3.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.5/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.5/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.5/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+-rw-rw-rw-   0        0        0     2440 2023-04-11 02:41:45.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
+-rw-rw-rw-   0        0        0      669 2023-04-11 02:57:44.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1992 2023-04-10 08:33:59.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10711 2023-03-31 07:34:14.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.5/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.5/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.5/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.5/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.5/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.5/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.5/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-04-11 03:21:45.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6858 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 03:21:45.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-11 03:21:45.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-04-11 03:21:45.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-11 03:21:45.000000 automation_rest_server-3.6.5/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-04-11 03:21:46.000000 automation_rest_server-3.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-04-11 03:21:15.000000 automation_rest_server-3.6.5/setup.py
```

### Comparing `automation_rest_server-3.6.4/LICENSE.txt` & `automation_rest_server-3.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/MANIFEST.in` & `automation_rest_server-3.6.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/PKG-INFO` & `automation_rest_server-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.6.4
+Version: 3.6.5
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.4/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.6.5/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.6.5/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.6.5/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.6.5/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/run.py` & `automation_rest_server-3.6.5/automation_rest_server/run.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-
-import subprocess
 import os
-import time
 from utils.system import decorate_exception_result
 from utils.firmware_path import FirmwareBinPath
 from utils import log
-from test_framework.state import State, UpgradeType
 from utils.system import get_test_platform_version
 
 
-class OakgateDownload(object):
+class NVMeDownload(object):
 
     def __init__(self):
-        super(OakgateDownload, self).__init__()
         self.root_path = os.getcwd()
         self.script_path = os.path.join(self.root_path, "Utility")
         self.logs_path = os.path.join(self.root_path, "Logs")
         self.orig_log_folders = list()
         self.latest_log_folders = list()
         self.fw_path_manage = FirmwareBinPath()
 
@@ -35,21 +30,14 @@
         if version == 1:
             cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --image2={}".format(self.script_path, ogt, fw_path)
         else:
             cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --target_image={}".format(self.script_path, ogt, fw_path)
         log.INFO("oakgate download: {}".format(cmd))
         return cmd
 
-    def gen_two_step_cmd_line(self, fw_path, spi_fw, ogt, com):
-
-        cmd = f"cd /d {self.script_path} && python two_step_download.py --oakgate {ogt} --firmwarePath {fw_path} " \
-              f"--serialPort {com} --preBinPath {spi_fw}"
-        log.INFO("oakgate two step download: {}".format(cmd))
-        return cmd
-
     def get_orig_logs(self):
         log_dirs = os.listdir(self.logs_path)
         for item in log_dirs:
             if os.path.isdir(os.path.join(self.logs_path, item)):
                 self.orig_log_folders.append(os.path.join(self.logs_path, item))
 
     def get_new_log(self, oakgate):
@@ -63,28 +51,18 @@
                         if os.path.isfile(os.path.join(log_item, new_log_item)):
                             if oakgate in new_log_item:    # check if this log belong to correct oagkate
                                 new_logs.append(os.path.join(log_item, new_log_item))
         return new_logs
 
     @decorate_exception_result
     def run(self, parameters):
-        cmd = None
         oakgate = parameters.get("oakgate", None)
-        com = parameters.get("com", None)
         self.get_orig_logs()
-        if int(parameters.get("upgrade_type", 1)) == UpgradeType.NVMe[0]:
-            fw_path = self.fw_path_manage.get_fw_path_from_parameter(parameters)
-            if oakgate is not None and fw_path is not None:
-                cmd = self.gen_nvme_cmd_line(fw_path, oakgate)
-        else:
-            spi_path = self.fw_path_manage.get_spi_path(parameters)
-            cap_path = self.fw_path_manage.get_cap(parameters)
-            print(spi_path, cap_path, oakgate)
-            if spi_path is not None and cap_path is not None and oakgate is not None:
-                cmd = self.gen_two_step_cmd_line(cap_path, spi_path, oakgate, com)
+        fw_path = self.fw_path_manage.get_fw_path_from_parameter(parameters)
+        cmd = self.gen_nvme_cmd_line(fw_path, oakgate) if oakgate is not None and fw_path is not None else None
         if cmd is not None:
             ret = os.system(cmd)
             logs = self.get_new_log(oakgate)
         else:
             ret = -1
-            logs = f"OGT upgrade fail: com: {com},ogt:{oakgate}"
+            logs = f"OGT upgrade fail: cmd: {cmd},ogt:{oakgate}"
         return ret, logs
```

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/state.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_pool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.6.5/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.6.5/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.6.5/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/buf.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/firmware_path.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/log.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/process.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server/utils/system.py` & `automation_rest_server-3.6.5/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.4/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.6.5/automation_rest_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.6.4
+Version: 3.6.5
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.4/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.6.5/automation_rest_server.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 automation_rest_server/test_framework/engine/sse_engine.py
 automation_rest_server/test_framework/firmware_engine/__init__.py
 automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
 automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
 automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
 automation_rest_server/test_framework/reboot_engine/__init__.py
 automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
 automation_rest_server/tool/__init__.py
 automation_rest_server/tool/device/__init__.py
 automation_rest_server/tool/device/linux_nvme.py
 automation_rest_server/tool/device/dll/__init__.py
 automation_rest_server/tool/device/dll/buf.dll
```

### Comparing `automation_rest_server-3.6.4/setup.py` & `automation_rest_server-3.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.6.4',
+    version = '3.6.5',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
```

