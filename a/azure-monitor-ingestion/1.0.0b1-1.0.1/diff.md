# Comparing `tmp/azure-monitor-ingestion-1.0.0b1.zip` & `tmp/azure-monitor-ingestion-1.0.1.zip`

## zipinfo {}

```diff
@@ -1,55 +1,65 @@
-Zip file size: 44392 bytes, number of entries: 53
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/samples/
--rw-rw-r--  2.0 unx       38 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx    11659 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/LICENSE
--rw-rw-r--  2.0 unx     8679 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/README.md
--rw-rw-r--  2.0 unx      190 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     2931 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/setup.py
--rw-rw-r--  2.0 unx      513 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     2280 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx      508 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/tests/preparer.py
--rw-rw-r--  2.0 unx     1269 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/tests/test_logs_ingestion.py
--rw-rw-r--  2.0 unx     1327 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/tests/test_logs_ingestion_async.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    11659 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       41 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/requires.txt
--rw-rw-r--  2.0 unx     1433 b- defN 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/SOURCES.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/monitor/
--rw-rw-r--  2.0 unx       80 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/
--rw-rw-r--  2.0 unx       80 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/
--rw-rw-r--  2.0 unx      920 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_models.py
--rw-rw-r--  2.0 unx     3801 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_client.py
--rw-rw-r--  2.0 unx     1390 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_vendor.py
--rw-rw-r--  2.0 unx     1092 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_helpers.py
--rw-rw-r--  2.0 unx      939 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/__init__.py
--rw-rw-r--  2.0 unx       27 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/py.typed
--rw-rw-r--  2.0 unx     1824 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_patch.py
--rw-rw-r--  2.0 unx     3649 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_configuration.py
--rw-rw-r--  2.0 unx      494 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_version.py
--rw-rw-r--  2.0 unx      830 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/__init__.py
--rw-rw-r--  2.0 unx     3640 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_patch.py
--rw-rw-r--  2.0 unx    10103 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/
--rw-rw-r--  2.0 unx     3904 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_client.py
--rw-rw-r--  2.0 unx      979 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_vendor.py
--rw-rw-r--  2.0 unx      843 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/__init__.py
--rw-rw-r--  2.0 unx     1922 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_patch.py
--rw-rw-r--  2.0 unx     3669 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_configuration.py
--rw-rw-r--  2.0 unx      830 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/__init__.py
--rw-rw-r--  2.0 unx     2354 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/_patch.py
--rw-rw-r--  2.0 unx     8185 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-15 19:54 azure-monitor-ingestion-1.0.0b1/samples/async_samples/
--rw-rw-r--  2.0 unx      845 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/samples/sample_send_logs_max_concurrency.py
--rw-rw-r--  2.0 unx      915 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/samples/sample_send_small_logs.py
--rw-rw-r--  2.0 unx     1148 b- defN 22-Jul-15 19:53 azure-monitor-ingestion-1.0.0b1/samples/async_samples/sample_send_small_logs_async.py
-53 files, 98071 bytes uncompressed, 33694 bytes compressed:  65.6%
+Zip file size: 77880 bytes, number of entries: 63
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/samples/
+-rw-rw-r--  2.0 unx     3011 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/setup.py
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/CHANGELOG.md
+-rw-rw-r--  2.0 unx      190 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/MANIFEST.in
+-rw-rw-r--  2.0 unx    11675 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/README.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/LICENSE
+-rw-rw-r--  2.0 unx       50 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/pyproject.toml
+-rw-rw-r--  2.0 unx    13914 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/setup.cfg
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_serialization.py
+-rw-rw-r--  2.0 unx     3626 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py
+-rw-rw-r--  2.0 unx     1833 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py
+-rw-rw-r--  2.0 unx     3664 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_version.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py
+-rw-rw-r--  2.0 unx     1496 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/py.typed
+-rw-rw-r--  2.0 unx      998 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_models.py
+-rw-rw-r--  2.0 unx     1755 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_helpers.py
+-rw-rw-r--  2.0 unx     3979 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_patch.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py
+-rw-rw-r--  2.0 unx     6908 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/
+-rw-rw-r--  2.0 unx     3757 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py
+-rw-rw-r--  2.0 unx     1869 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py
+-rw-rw-r--  2.0 unx     3706 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py
+-rw-rw-r--  2.0 unx     1002 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py
+-rw-rw-r--  2.0 unx     5023 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/tests/perf_tests/
+-rw-rw-r--  2.0 unx     2164 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_helpers.py
+-rw-rw-r--  2.0 unx     6580 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion_async.py
+-rw-rw-r--  2.0 unx     5538 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion.py
+-rw-rw-r--  2.0 unx     3510 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/conftest.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/perf_tests/__init__.py
+-rw-rw-r--  2.0 unx     3679 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/tests/perf_tests/upload_logs.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       66 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    13914 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     1813 b- defN 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:07 azure-monitor-ingestion-1.0.1/samples/async_samples/
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_custom_error_callback.py
+-rw-rw-r--  2.0 unx     1889 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_send_small_logs.py
+-rw-rw-r--  2.0 unx     2516 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_upload_pandas_dataframe.py
+-rw-rw-r--  2.0 unx     2533 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/sample_upload_file_contents.py
+-rw-rw-r--  2.0 unx     3273 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_custom_error_callback_async.py
+-rw-rw-r--  2.0 unx     2993 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_file_contents_async.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_pandas_dataframe_async.py
+-rw-rw-r--  2.0 unx     2127 b- defN 23-Apr-11 18:06 azure-monitor-ingestion-1.0.1/samples/async_samples/sample_send_small_logs_async.py
+63 files, 216006 bytes uncompressed, 65258 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,160 +1,190 @@
-Filename: azure-monitor-ingestion-1.0.0b1/
+Filename: azure-monitor-ingestion-1.0.1/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/tests/
+Filename: azure-monitor-ingestion-1.0.1/azure/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/
+Filename: azure-monitor-ingestion-1.0.1/tests/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/samples/
+Filename: azure-monitor-ingestion-1.0.1/samples/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/setup.cfg
+Filename: azure-monitor-ingestion-1.0.1/setup.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/PKG-INFO
+Filename: azure-monitor-ingestion-1.0.1/CHANGELOG.md
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/LICENSE
+Filename: azure-monitor-ingestion-1.0.1/MANIFEST.in
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/README.md
+Filename: azure-monitor-ingestion-1.0.1/README.md
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/MANIFEST.in
+Filename: azure-monitor-ingestion-1.0.1/LICENSE
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/setup.py
+Filename: azure-monitor-ingestion-1.0.1/pyproject.toml
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/CHANGELOG.md
+Filename: azure-monitor-ingestion-1.0.1/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/tests/conftest.py
+Filename: azure-monitor-ingestion-1.0.1/setup.cfg
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/tests/preparer.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/tests/test_logs_ingestion.py
+Filename: azure-monitor-ingestion-1.0.1/azure/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/tests/test_logs_ingestion_async.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/not-zip-safe
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/PKG-INFO
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/top_level.txt
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/dependency_links.txt
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_serialization.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/requires.txt
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/SOURCES.txt
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_version.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/py.typed
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_models.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_models.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_helpers.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_client.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_vendor.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_helpers.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/py.typed
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_patch.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_configuration.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_version.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_patch.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_operations.py
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/
+Filename: azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_client.py
+Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_vendor.py
+Filename: azure-monitor-ingestion-1.0.1/tests/test_helpers.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion_async.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_patch.py
+Filename: azure-monitor-ingestion-1.0.1/tests/test_logs_ingestion.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_configuration.py
+Filename: azure-monitor-ingestion-1.0.1/tests/conftest.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/__init__.py
+Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/__init__.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/_patch.py
+Filename: azure-monitor-ingestion-1.0.1/tests/perf_tests/upload_logs.py
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/_operations.py
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/samples/async_samples/
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/samples/sample_send_logs_max_concurrency.py
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/samples/sample_send_small_logs.py
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/requires.txt
 Comment: 
 
-Filename: azure-monitor-ingestion-1.0.0b1/samples/async_samples/sample_send_small_logs_async.py
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/sample_custom_error_callback.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/sample_send_small_logs.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/sample_upload_pandas_dataframe.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/sample_upload_file_contents.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_custom_error_callback_async.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_file_contents_async.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_upload_pandas_dataframe_async.py
+Comment: 
+
+Filename: azure-monitor-ingestion-1.0.1/samples/async_samples/sample_send_small_logs_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-monitor-ingestion-1.0.0b1/LICENSE` & `azure-monitor-ingestion-1.0.1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-monitor-ingestion-1.0.0b1/README.md` & `azure-monitor-ingestion-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # Azure Monitor Ingestion client library for Python
 
-The Azure Monitor Ingestion client library is used to send custom logs to [Azure Monitor][azure_monitor_overview].
+The Azure Monitor Ingestion client library is used to send custom logs to [Azure Monitor][azure_monitor_overview] using the [Logs Ingestion API][ingestion_overview].
 
-This library allows you to send data from virtually any source to supported built-in tables or to custom tables 
-that you create in Log Analytics workspace. You can even extend the schema of built-in tables with custom columns.
+This library allows you to send data from virtually any source to supported built-in tables or to custom tables that you create in Log Analytics workspace. You can even extend the schema of built-in tables with custom columns.
 
 **Resources:**
 
 - [Source code][source]
 - [Package (PyPI)][package]
+- [Package (Conda)](https://anaconda.org/microsoft/azure-monitor-ingestion/)
 - [API reference documentation][python-ingestion-ref-docs]
 - [Service documentation][azure_monitor_overview]
 - [Samples][samples]
 - [Change log][changelog]
 
-## _Disclaimer_
-
-_Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
-
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.6 or later
+- Python 3.7 or later
 - An [Azure subscription][azure_subscription]
-- An [Azure Log Analytics workspace][azure_monitor_create_using_portal].
+- An [Azure Log Analytics workspace][azure_monitor_create_using_portal]
 - A [Data Collection Endpoint][data_collection_endpoint]
 - A [Data Collection Rule][data_collection_rule]
 
 ### Install the package
 
 Install the Azure Monitor Ingestion client library for Python with [pip][pip]:
 
 ```bash
 pip install azure-monitor-ingestion
 ```
 
-
 ### Create the client
 
 An authenticated client is required to upload Logs to Azure Monitor. The library includes both synchronous and asynchronous forms of the clients. To authenticate, create an instance of a token credential. Use that instance when creating a `LogsIngestionClient`. The following examples use `DefaultAzureCredential` from the [azure-identity](https://pypi.org/project/azure-identity/) package.
 
 #### Synchronous clients
 
 Consider the following example, which creates synchronous clients for uploading logs:
@@ -69,52 +64,52 @@
 logs_client = LogsIngestionClient(endpoint, credential)
 ```
 
 ## Key concepts
 
 ### Data Collection Endpoint
 
-Data Collection Endpoints (DCEs) allow you to uniquely configure ingestion settings for Azure Monitor. [This 
-article][data_collection_endpoint] provides an overview of data collection endpoints including their contents and 
-structure and how you can create and work with them.
+Data Collection Endpoints (DCEs) allow you to uniquely configure ingestion settings for Azure Monitor. [This article][data_collection_endpoint] provides an overview of data collection endpoints including their contents and structure and how you can create and work with them.
 
 ### Data Collection Rule
 
-Data collection rules (DCR) define data collected by Azure Monitor and specify how and where that data should be sent or
-stored. The REST API call must specify a DCR to use. A single DCE can support multiple DCRs, so you can specify a
-different DCR for different sources and target tables.
+Data collection rules (DCR) define data collected by Azure Monitor and specify how and where that data should be sent or stored. The REST API call must specify a DCR to use. A single DCE can support multiple DCRs, so you can specify a different DCR for different sources and target tables.
+
+The DCR must understand the structure of the input data and the structure of the target table. If the two don't match, it can use a transformation to convert the source data to match the target table. You may also use the transform to filter source data and perform any other calculations or conversions.
 
-The DCR must understand the structure of the input data and the structure of the target table. If the two don't match,
-it can use a transformation to convert the source data to match the target table. You may also use the transform to
-filter source data and perform any other calculations or conversions.
+For more details, see [Data collection rules in Azure Monitor][data_collection_rule]. For information on how to retrieve a DCR ID, see [this tutorial][data_collection_rule_tutorial].
 
-For more details, refer to [Data collection rules in Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview).
+### Log Analytics workspace tables
 
-### Log Analytics Workspace Tables
+Custom logs can send data to any custom table that you create and to certain built-in tables in your Log Analytics workspace. The target table must exist before you can send data to it. The following built-in tables are currently supported:
 
-Custom logs can send data to any custom table that you create and to certain built-in tables in your Log Analytics 
-workspace. The target table must exist before you can send data to it. The following built-in tables are currently supported:
+- [CommonSecurityLog](https://learn.microsoft.com/azure/azure-monitor/reference/tables/commonsecuritylog)
+- [SecurityEvents](https://learn.microsoft.com/azure/azure-monitor/reference/tables/securityevent)
+- [Syslog](https://learn.microsoft.com/azure/azure-monitor/reference/tables/syslog)
+- [WindowsEvents](https://learn.microsoft.com/azure/azure-monitor/reference/tables/windowsevent)
 
-- [CommonSecurityLog](https://docs.microsoft.com/azure/azure-monitor/reference/tables/commonsecuritylog)
-- [SecurityEvents](https://docs.microsoft.com/azure/azure-monitor/reference/tables/securityevent)
-- [Syslog](https://docs.microsoft.com/azure/azure-monitor/reference/tables/syslog)
-- [WindowsEvents](https://docs.microsoft.com/azure/azure-monitor/reference/tables/windowsevent)
+### Logs retrieval
+
+The logs that were uploaded using this library can be queried using the [Azure Monitor Query][azure_monitor_query] client library.
 
 ## Examples
 
 - [Upload custom logs](#upload-custom-logs)
+- [Upload with custom error handling](#upload-with-custom-error-handling)
 
 ### Upload custom logs
 
-This example shows uploading logs to Azure monitor.
+This example shows uploading logs to Azure Monitor.
 
 ```python
 import os
-from azure.monitor.ingestion import LogsIngestionClient, UploadLogsStatus
+
+from azure.core.exceptions import HttpResponseError
 from azure.identity import DefaultAzureCredential
+from azure.monitor.ingestion import LogsIngestionClient
 
 endpoint = os.environ['DATA_COLLECTION_ENDPOINT']
 credential = DefaultAzureCredential()
 
 client = LogsIngestionClient(endpoint=endpoint, credential=credential, logging_enable=True)
 
 rule_id = os.environ['LOGS_DCR_RULE_ID']
@@ -127,18 +122,36 @@
       {
         "Time": "2021-12-08T23:51:14.1104269Z",
         "Computer": "Computer2",
         "AdditionalContext": "context"
       }
     ]
 
-response = client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body)
-if response.status != UploadLogsStatus.SUCCESS:
-    failed_logs = response.failed_logs_index
-    print(failed_logs)
+try:
+    client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body)
+except HttpResponseError as e:
+    print(f"Upload failed: {e}")
+```
+
+### Upload with custom error handling
+
+To upload logs with custom error handling, you can pass a callback function to the `on_error` parameter of the `upload` method. The callback function will be called for each error that occurs during the upload and should expect one argument that corresponds to an `LogsUploadError` object. This object contains the error encountered and the list of logs that failed to upload.
+
+```python
+# Example 1: Collect all logs that failed to upload.
+failed_logs = []
+def on_error(error):
+    print("Log chunk failed to upload with error: ", error.error)
+    failed_logs.extend(error.failed_logs)
+
+# Example 2: Ignore all errors.
+def on_error_pass(error):
+    pass
+
+client.upload(rule_id=rule_id, stream_name=os.environ['LOGS_DCR_STREAM_NAME'], logs=body, on_error=on_error)
 ```
 
 ## Troubleshooting
 
 Enable the `azure.monitor.ingestion` logger to collect traces from the library.
 
 ### General
@@ -159,37 +172,53 @@
 
 ### Samples
 
 The following code samples show common scenarios with the Azure Monitor Ingestion client library.
 
 #### Logs Ingestion samples
 
-- [Upload a list of logs](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/sample_send_small_logs.py) ([async sample](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/async_samples/sample_send_small_logs_async.py))
+- [Upload a list of logs][sample_send_small_logs] ([async sample][sample_send_small_logs_async])
+- [Upload a list of logs with custom error handling][sample_custom_error_callback] ([async sample][sample_custom_error_callback_async])
+- [Upload the contents of a file][sample_upload_file_contents] ([async sample][sample_upload_file_contents_async])
+- [Upload data in a pandas DataFrame][sample_upload_pandas_dataframe] ([async sample][sample_upload_pandas_dataframe_async])
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repositories using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
 
 <!-- LINKS -->
 
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
-[azure_monitor_overview]: https://docs.microsoft.com/azure/azure-monitor/
+[azure_monitor_create_using_portal]: https://learn.microsoft.com/azure/azure-monitor/logs/quick-create-workspace
+[azure_monitor_overview]: https://learn.microsoft.com/azure/azure-monitor/
+[azure_monitor_query]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query#readme
 [azure_subscription]: https://azure.microsoft.com/free/python/
 [changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/CHANGELOG.md
+[data_collection_endpoint]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-endpoint-overview
+[data_collection_rule]: https://learn.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview
+[data_collection_rule_tutorial]: https://learn.microsoft.com/azure/azure-monitor/logs/tutorial-logs-ingestion-portal#collect-information-from-the-dcr
+[ingestion_overview]: https://learn.microsoft.com/azure/azure-monitor/logs/logs-ingestion-api-overview
 [package]: https://aka.ms/azsdk-python-monitor-ingestion-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-ingestion-ref-docs]: https://aka.ms/azsdk/python/monitor-ingestion/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-ingestion/samples
 [source]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/
-[data_collection_endpoint]: https://docs.microsoft.com//azure/azure-monitor/essentials/data-collection-endpoint-overview
-[data_collection_rule]: https://docs.microsoft.com/azure/azure-monitor/essentials/data-collection-rule-overview
+
+[sample_send_small_logs]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/sample_send_small_logs.py
+[sample_send_small_logs_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/async_samples/sample_send_small_logs_async.py
+[sample_custom_error_callback]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/sample_custom_error_callback.py
+[sample_custom_error_callback_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/async_samples/sample_custom_error_callback_async.py
+[sample_upload_file_contents]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/sample_upload_file_contents.py
+[sample_upload_file_contents_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/async_samples/sample_upload_file_contents_async.py
+[sample_upload_pandas_dataframe]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/sample_upload_pandas_dataframe.py
+[sample_upload_pandas_dataframe_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-ingestion/samples/async_samples/sample_upload_pandas_dataframe_async.py
 
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
```

## Comparing `azure-monitor-ingestion-1.0.0b1/setup.py` & `azure-monitor-ingestion-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,31 +57,33 @@
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         'samples',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.monitor',
     ]),
+    include_package_data=True,
     install_requires=[
-        'msrest>=0.6.19',
         'azure-core<2.0.0,>=1.24.0',
+        'isodate>=0.6.0',
+        "typing-extensions>=4.0.1"
     ]
 )
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure_monitor_ingestion.egg-info/SOURCES.txt` & `azure-monitor-ingestion-1.0.1/azure_monitor_ingestion.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/monitor/__init__.py
 azure/monitor/ingestion/__init__.py
 azure/monitor/ingestion/_client.py
 azure/monitor/ingestion/_configuration.py
 azure/monitor/ingestion/_helpers.py
 azure/monitor/ingestion/_models.py
 azure/monitor/ingestion/_patch.py
+azure/monitor/ingestion/_serialization.py
 azure/monitor/ingestion/_vendor.py
 azure/monitor/ingestion/_version.py
 azure/monitor/ingestion/py.typed
 azure/monitor/ingestion/_operations/__init__.py
 azure/monitor/ingestion/_operations/_operations.py
 azure/monitor/ingestion/_operations/_patch.py
 azure/monitor/ingestion/aio/__init__.py
@@ -27,14 +29,21 @@
 azure/monitor/ingestion/aio/_operations/_patch.py
 azure_monitor_ingestion.egg-info/PKG-INFO
 azure_monitor_ingestion.egg-info/SOURCES.txt
 azure_monitor_ingestion.egg-info/dependency_links.txt
 azure_monitor_ingestion.egg-info/not-zip-safe
 azure_monitor_ingestion.egg-info/requires.txt
 azure_monitor_ingestion.egg-info/top_level.txt
-samples/sample_send_logs_max_concurrency.py
+samples/sample_custom_error_callback.py
 samples/sample_send_small_logs.py
+samples/sample_upload_file_contents.py
+samples/sample_upload_pandas_dataframe.py
+samples/async_samples/sample_custom_error_callback_async.py
 samples/async_samples/sample_send_small_logs_async.py
+samples/async_samples/sample_upload_file_contents_async.py
+samples/async_samples/sample_upload_pandas_dataframe_async.py
 tests/conftest.py
-tests/preparer.py
+tests/test_helpers.py
 tests/test_logs_ingestion.py
-tests/test_logs_ingestion_async.py
+tests/test_logs_ingestion_async.py
+tests/perf_tests/__init__.py
+tests/perf_tests/upload_logs.py
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_client.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,92 +5,76 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
-from msrest import Deserializer, Serializer
-
 from azure.core import PipelineClient
 from azure.core.rest import HttpRequest, HttpResponse
 
-from ._configuration import MonitorIngestionClientConfiguration
-from ._operations import MonitorIngestionClientOperationsMixin
+from ._configuration import LogsIngestionClientConfiguration
+from ._operations import LogsIngestionClientOperationsMixin
+from ._serialization import Deserializer, Serializer
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Dict
-
     from azure.core.credentials import TokenCredential
 
 
-class MonitorIngestionClient(
-    MonitorIngestionClientOperationsMixin
-):  # pylint: disable=client-accepts-api-version-keyword
+class LogsIngestionClient(LogsIngestionClientOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """Azure Monitor Data Collection Python Client.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "TokenCredential", **kwargs: Any
-    ) -> None:
+    def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
         _endpoint = "{endpoint}"
-        self._config = MonitorIngestionClientConfiguration(
-            endpoint=endpoint, credential=credential, **kwargs
-        )
-        self._client = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
+        self._config = LogsIngestionClientConfiguration(endpoint=endpoint, credential=credential, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client.send_request(request)
         <HttpResponse: 200 OK>
 
-        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         path_format_arguments = {
-            "endpoint": self._serialize.url(
-                "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
-            ),
+            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
-        request_copy.url = self._client.format_url(
-            request_copy.url, **path_format_arguments
-        )
+        request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         self._client.close()
 
-    def __enter__(self):
-        # type: () -> MonitorIngestionClient
+    def __enter__(self) -> "LogsIngestionClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_vendor.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_vendor.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
-from typing import TYPE_CHECKING
+from typing import List, TYPE_CHECKING, cast
 
-from ._configuration import MonitorIngestionClientConfiguration
+from ._configuration import LogsIngestionClientConfiguration
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from msrest import Deserializer, Serializer
-
     from azure.core import PipelineClient
 
+    from ._serialization import Deserializer, Serializer
+
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
-            components = [
-                c for c in formatted_components if "{}".format(key.args[0]) not in c
-            ]
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
+            components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
 
 
-class MixinABC(ABC):
+class LogsIngestionClientMixinABC(ABC):
     """DO NOT use this class. It is for internal typing use only."""
 
     _client: "PipelineClient"
-    _config: MonitorIngestionClientConfiguration
+    _config: LogsIngestionClientConfiguration
     _serialize: "Serializer"
     _deserialize: "Deserializer"
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/__init__.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import MonitorIngestionClient
-from ._models import UploadLogsResult, UploadLogsStatus
+from ._operations import LogsIngestionClientOperationsMixin
 
-try:
-    from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
-except ImportError:
-    _patch_all = []
+from ._patch import __all__ as _patch_all
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["MonitorIngestionClient", "UploadLogsResult", "UploadLogsStatus"]
+__all__ = [
+    "LogsIngestionClientOperationsMixin",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
-
 _patch_sdk()
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_patch.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 from typing import TYPE_CHECKING, Any
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
-from ._client import MonitorIngestionClient as GeneratedClient
+from ._client import LogsIngestionClient as GeneratedClient
+from ._models import LogsUploadError
 
 if TYPE_CHECKING:
     from azure.core.credentials import TokenCredential
 
 
 class LogsIngestionClient(GeneratedClient):
     """Azure Monitor Data Collection Python Client.
@@ -23,29 +24,25 @@
     :param credential: Credential needed for the client to connect to Azure.
     :type credential: ~azure.core.credentials.TokenCredential
     :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "TokenCredential", **kwargs: Any
-    ) -> None:
+    def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
         scope = "https://monitor.azure.com//.default"
         super().__init__(
             endpoint,
             credential,
-            authentication_policy=BearerTokenCredentialPolicy(
-                credential, scope, **kwargs
-            ),
+            authentication_policy=BearerTokenCredentialPolicy(credential, scope, **kwargs),
             **kwargs
         )
 
 
-__all__ = ["LogsIngestionClient"]
+__all__ = ["LogsIngestionClient", "LogsUploadError"]
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_configuration.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,84 +2,71 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 VERSION = "unknown"
 
 
-class MonitorIngestionClientConfiguration(
-    Configuration
-):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MonitorIngestionClient.
+class LogsIngestionClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for LogsIngestionClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "TokenCredential", **kwargs: Any
-    ) -> None:
-        super(MonitorIngestionClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2021-11-01-preview")  # type: str
+    def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
+        super(LogsIngestionClientConfiguration, self).__init__(**kwargs)
+        api_version: Literal["2023-01-01"] = kwargs.pop("api_version", "2023-01-01")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
         self.credential = credential
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["user_impersonation"])
-        kwargs.setdefault("sdk_moniker", "monitoringestionclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-ingestion/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        self.user_agent_policy = kwargs.get(
-            "user_agent_policy"
-        ) or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(
-            **kwargs
-        )
+    def _configure(self, **kwargs: Any) -> None:
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get(
-            "logging_policy"
-        ) or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get(
-            "http_logging_policy"
-        ) or policies.HttpLoggingPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
         self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get(
-            "custom_hook_policy"
-        ) or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(
-            **kwargs
-        )
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = policies.BearerTokenCredentialPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/__init__.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._operations import MonitorIngestionClientOperationsMixin
+from ._operations import LogsIngestionClientOperationsMixin
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "MonitorIngestionClientOperationsMixin",
+    "LogsIngestionClientOperationsMixin",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_patch.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_operations/_patch.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,87 +2,90 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
-import concurrent.futures
-from typing import List, Any, Optional
-from ._operations import MonitorIngestionClientOperationsMixin as GeneratedOps
-from .._models import UploadLogsStatus, UploadLogsResult
-from .._helpers import _create_gzip_requests
+from io import IOBase
+import logging
+import sys
+from typing import Callable, cast, List, Any, Awaitable, Optional, Union, IO
 
+from ._operations import LogsIngestionClientOperationsMixin as GeneratedOps
+from ..._helpers import _create_gzip_requests, GZIP_MAGIC_NUMBER
+from ..._models import LogsUploadError
 
-class MonitorIngestionClientOperationsMixin(GeneratedOps):
-    def upload( # pylint: disable=arguments-renamed, arguments-differ
+if sys.version_info >= (3, 9):
+    from collections.abc import Mapping, MutableMapping
+else:
+    from typing import Mapping, MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
+
+
+_LOGGER = logging.getLogger(__name__)
+JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
+
+
+class LogsIngestionClientOperationsMixin(GeneratedOps):
+    async def upload(  # type: ignore[override] # pylint: disable=arguments-renamed, arguments-differ
         self,
         rule_id: str,
         stream_name: str,
-        logs: List[Any],
+        logs: Union[List[JSON], IO],
         *,
-        max_concurrency: Optional[int] = None,
+        on_error: Optional[Callable[[LogsUploadError], Awaitable[None]]] = None,
         **kwargs: Any
-    ) -> UploadLogsResult:
+    ) -> None:
         """Ingestion API used to directly ingest data using Data Collection Rules.
 
-        See error response code and error response message for more detail.
+        A list of logs is divided into chunks of 1MB or less, then each chunk is gzip-compressed and uploaded.
+        If an I/O stream is passed in, the stream is uploaded as-is.
 
-        :param rule_id: The immutable Id of the Data Collection Rule resource.
+        :param rule_id: The immutable ID of the Data Collection Rule resource.
         :type rule_id: str
-        :param stream_name: The streamDeclaration name as defined in the Data Collection Rule.
-        :type stream_name: str
+        :param stream: The streamDeclaration name as defined in the Data Collection Rule.
+        :type stream: str
         :param logs: An array of objects matching the schema defined by the provided stream.
-        :type logs: list[any]
-        :keyword max_concurrency: Number of parallel threads to use when logs size is > 1mb.
-        :paramtype max_concurrency: int
-        :return: UploadLogsResult
-        :rtype: UploadLogsResult
+        :type logs: list[JSON] or IO
+        :keyword on_error: The callback function that is called when a chunk of logs fails to upload.
+            This function should expect one argument that corresponds to an "LogsUploadError" object.
+            If no function is provided, then the first exception encountered will be raised.
+        :paramtype on_error: Optional[Callable[[~azure.monitor.ingestion.LogsUploadError], None]]
+        :return: None
+        :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        requests = _create_gzip_requests(logs)
-        results = []
-        status = UploadLogsStatus.SUCCESS
-        parallel = max_concurrency and max_concurrency > 1 and len(requests) > 1
-        if parallel:
-            with concurrent.futures.ThreadPoolExecutor(max_concurrency) as executor:
-                future_to_req = {
-                    executor.submit(
-                        super(MonitorIngestionClientOperationsMixin, self).upload,
-                        rule_id,
-                        stream=stream_name,
-                        body=request,
-                        content_encoding="gzip",
-                        **kwargs
-                    ): request
-                    for request in requests
-                }
-                for future in concurrent.futures.as_completed(future_to_req):
-                    req = future_to_req[future]
-                    response = future.result()
-                    if response is not None:
-                        results.append(req)
-                        status = UploadLogsStatus.PARTIAL_FAILURE
-            return UploadLogsResult(failed_logs=results, status=status)
-        for request in requests:
-            response = super().upload(
-                rule_id,
-                stream=stream_name,
-                body=request,
-                content_encoding="gzip",
-                **kwargs
-            )
-            if response is not None:
-                results.append(request)
-                status = UploadLogsStatus.PARTIAL_FAILURE
-        return UploadLogsResult(failed_logs=results, status=status)
+        if isinstance(logs, IOBase):
+            if not logs.readable():
+                raise ValueError("The 'logs' stream must be readable.")
+            content_encoding = None
+            # Check if the stream is gzip-compressed if stream is seekable.
+            if logs.seekable():
+                if logs.read(2) == GZIP_MAGIC_NUMBER:
+                    content_encoding = "gzip"
+                logs.seek(0)
+
+            await super().upload(rule_id, stream=stream_name, body=logs, content_encoding=content_encoding, **kwargs)
+            return
+
+        for gzip_data, log_chunk in _create_gzip_requests(cast(List[JSON], logs)):
+            try:
+                await super().upload(
+                    rule_id, stream=stream_name, body=gzip_data, content_encoding="gzip", **kwargs  # type: ignore
+                )
+            except Exception as err:  # pylint: disable=broad-except
+                if on_error:
+                    await on_error(LogsUploadError(error=err, failed_logs=cast(List[Mapping[str, Any]], log_chunk)))
+                else:
+                    _LOGGER.error("Failed to upload chunk containing %d log entries", len(log_chunk))
+                    raise err
 
 
 __all__: List[str] = [
-    "MonitorIngestionClientOperationsMixin"
+    "LogsIngestionClientOperationsMixin"
 ]  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/_operations/_operations.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/_operations/_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,173 +3,89 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
-from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
-
-from msrest import Serializer
+from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
+    ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
-from .._vendor import MixinABC, _format_url_section
+from .._serialization import Serializer
+from .._vendor import LogsIngestionClientMixinABC, _format_url_section
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
-ClsType = Optional[
-    Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]
-]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_upload_request(rule_id: str, stream: str, **kwargs: Any) -> HttpRequest:
+def build_logs_ingestion_upload_request(
+    rule_id: str,
+    stream: str,
+    *,
+    content_encoding: Optional[str] = None,
+    x_ms_client_request_id: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-11-01-preview")
-    )  # type: str
-    content_encoding = kwargs.pop(
-        "content_encoding", _headers.pop("Content-Encoding", None)
-    )  # type: Optional[str]
-    x_ms_client_request_id = kwargs.pop(
-        "x_ms_client_request_id", _headers.pop("x-ms-client-request-id", None)
-    )  # type: Optional[str]
-    content_type = kwargs.pop(
-        "content_type", _headers.pop("Content-Type", None)
-    )  # type: Optional[str]
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    api_version: Literal["2023-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/dataCollectionRules/{ruleId}/streams/{stream}"
     path_format_arguments = {
         "ruleId": _SERIALIZER.url("rule_id", rule_id, "str"),
         "stream": _SERIALIZER.url("stream", stream, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_encoding is not None:
-        _headers["Content-Encoding"] = _SERIALIZER.header(
-            "content_encoding", content_encoding, "str"
-        )
+        _headers["Content-Encoding"] = _SERIALIZER.header("content_encoding", content_encoding, "str")
     if x_ms_client_request_id is not None:
-        _headers["x-ms-client-request-id"] = _SERIALIZER.header(
-            "x_ms_client_request_id", x_ms_client_request_id, "str"
-        )
+        _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
     if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header(
-            "content_type", content_type, "str"
-        )
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="POST", url=_url, params=_params, headers=_headers, **kwargs
-    )
-
-
-class MonitorIngestionClientOperationsMixin(MixinABC):
-    @overload
-    def upload(  # pylint: disable=inconsistent-return-statements
-        self,
-        rule_id: str,
-        stream: str,
-        body: List[JSON],
-        *,
-        content_encoding: Optional[str] = None,
-        x_ms_client_request_id: Optional[str] = None,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> None:
-        """Ingestion API used to directly ingest data using Data Collection Rules.
-
-        See error response code and error response message for more detail.
-
-        :param rule_id: The immutable Id of the Data Collection Rule resource. Required.
-        :type rule_id: str
-        :param stream: The streamDeclaration name as defined in the Data Collection Rule. Required.
-        :type stream: str
-        :param body: An array of objects matching the schema defined by the provided stream. Required.
-        :type body: list[JSON]
-        :keyword content_encoding: gzip. Default value is None.
-        :paramtype content_encoding: str
-        :keyword x_ms_client_request_id: Client request Id. Default value is None.
-        :paramtype x_ms_client_request_id: str
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: None
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # JSON input template you can fill out and use as your body input.
-                body = [
-                    {}  # Optional.
-                ]
-        """
-
-    @overload
-    def upload(  # pylint: disable=inconsistent-return-statements
-        self,
-        rule_id: str,
-        stream: str,
-        body: IO,
-        *,
-        content_encoding: Optional[str] = None,
-        x_ms_client_request_id: Optional[str] = None,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> None:
-        """Ingestion API used to directly ingest data using Data Collection Rules.
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
-        See error response code and error response message for more detail.
 
-        :param rule_id: The immutable Id of the Data Collection Rule resource. Required.
-        :type rule_id: str
-        :param stream: The streamDeclaration name as defined in the Data Collection Rule. Required.
-        :type stream: str
-        :param body: An array of objects matching the schema defined by the provided stream. Required.
-        :type body: IO
-        :keyword content_encoding: gzip. Default value is None.
-        :paramtype content_encoding: str
-        :keyword x_ms_client_request_id: Client request Id. Default value is None.
-        :paramtype x_ms_client_request_id: str
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: None
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+class LogsIngestionClientOperationsMixin(LogsIngestionClientMixinABC):
 
     @distributed_trace
     def upload(  # pylint: disable=inconsistent-return-statements
         self,
         rule_id: str,
         stream: str,
         body: Union[List[JSON], IO],
@@ -183,15 +99,15 @@
         See error response code and error response message for more detail.
 
         :param rule_id: The immutable Id of the Data Collection Rule resource. Required.
         :type rule_id: str
         :param stream: The streamDeclaration name as defined in the Data Collection Rule. Required.
         :type stream: str
         :param body: An array of objects matching the schema defined by the provided stream. Is either
-         a list type or a IO type. Required.
+         a [JSON] type or a IO type. Required.
         :type body: list[JSON] or IO
         :keyword content_encoding: gzip. Default value is None.
         :paramtype content_encoding: str
         :keyword x_ms_client_request_id: Client request Id. Default value is None.
         :paramtype x_ms_client_request_id: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
@@ -200,62 +116,55 @@
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: str
-        content_type = kwargs.pop(
-            "content_type", _headers.pop("Content-Type", None)
-        )  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_upload_request(
+        request = build_logs_ingestion_upload_request(
             rule_id=rule_id,
             stream=stream,
-            api_version=api_version,
             content_encoding=content_encoding,
             x_ms_client_request_id=x_ms_client_request_id,
             content_type=content_type,
+            api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
-            "endpoint": self._serialize.url(
-                "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
-            ),
+            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_client.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,93 +5,76 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
-from msrest import Deserializer, Serializer
-
 from azure.core import AsyncPipelineClient
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
-from ._configuration import MonitorIngestionClientConfiguration
-from ._operations import MonitorIngestionClientOperationsMixin
+from .._serialization import Deserializer, Serializer
+from ._configuration import LogsIngestionClientConfiguration
+from ._operations import LogsIngestionClientOperationsMixin
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Dict
-
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class MonitorIngestionClient(
-    MonitorIngestionClientOperationsMixin
-):  # pylint: disable=client-accepts-api-version-keyword
+class LogsIngestionClient(LogsIngestionClientOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """Azure Monitor Data Collection Python Client.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any
-    ) -> None:
+    def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
         _endpoint = "{endpoint}"
-        self._config = MonitorIngestionClientConfiguration(
-            endpoint=endpoint, credential=credential, **kwargs
-        )
-        self._client = AsyncPipelineClient(
-            base_url=_endpoint, config=self._config, **kwargs
-        )
+        self._config = LogsIngestionClientConfiguration(endpoint=endpoint, credential=credential, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
 
-    def send_request(
-        self, request: HttpRequest, **kwargs: Any
-    ) -> Awaitable[AsyncHttpResponse]:
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client.send_request(request)
         <AsyncHttpResponse: 200 OK>
 
-        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         path_format_arguments = {
-            "endpoint": self._serialize.url(
-                "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
-            ),
+            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
-        request_copy.url = self._client.format_url(
-            request_copy.url, **path_format_arguments
-        )
+        request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
         return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
-    async def __aenter__(self) -> "MonitorIngestionClient":
+    async def __aenter__(self) -> "LogsIngestionClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_vendor.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_vendor.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
-from ._configuration import MonitorIngestionClientConfiguration
+from ._configuration import LogsIngestionClientConfiguration
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from msrest import Deserializer, Serializer
-
     from azure.core import AsyncPipelineClient
 
+    from .._serialization import Deserializer, Serializer
+
 
-class MixinABC(ABC):
+class LogsIngestionClientMixinABC(ABC):
     """DO NOT use this class. It is for internal typing use only."""
 
     _client: "AsyncPipelineClient"
-    _config: MonitorIngestionClientConfiguration
+    _config: LogsIngestionClientConfiguration
     _serialize: "Serializer"
     _deserialize: "Deserializer"
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/__init__.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import MonitorIngestionClient
+from ._client import LogsIngestionClient
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["MonitorIngestionClient"]
+__all__ = [
+    "LogsIngestionClient",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_patch.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_patch.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 from typing import List, Any, TYPE_CHECKING
 from azure.core.pipeline.policies import AsyncBearerTokenCredentialPolicy
-from ._client import MonitorIngestionClient as GeneratedClient
+from ._client import LogsIngestionClient as GeneratedClient
 
 if TYPE_CHECKING:
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class LogsIngestionClient(GeneratedClient):
     """Azure Monitor Data Collection Python Client.
@@ -23,23 +23,18 @@
     :param credential: Credential needed for the client to connect to Azure.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any
-    ) -> None:
+    def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
         scope = "https://monitor.azure.com//.default"
         super().__init__(
-            endpoint,
-            credential,
-            authentication_policy=AsyncBearerTokenCredentialPolicy(credential, scope),
-            **kwargs
+            endpoint, credential, authentication_policy=AsyncBearerTokenCredentialPolicy(credential, scope), **kwargs
         )
 
 
 __all__: List[str] = [
     "LogsIngestionClient"
 ]  # Add all objects you want publicly available to users at this package level
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_configuration.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,83 +2,71 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 VERSION = "unknown"
 
 
-class MonitorIngestionClientConfiguration(
-    Configuration
-):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MonitorIngestionClient.
+class LogsIngestionClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for LogsIngestionClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The Data Collection Endpoint for the Data Collection Rule, for example
      https://dce-name.eastus-2.ingest.monitor.azure.com. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2021-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(
-        self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any
-    ) -> None:
-        super(MonitorIngestionClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2021-11-01-preview")  # type: str
+    def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
+        super(LogsIngestionClientConfiguration, self).__init__(**kwargs)
+        api_version: Literal["2023-01-01"] = kwargs.pop("api_version", "2023-01-01")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
         self.credential = credential
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["user_impersonation"])
-        kwargs.setdefault("sdk_moniker", "monitoringestionclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-ingestion/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
-        self.user_agent_policy = kwargs.get(
-            "user_agent_policy"
-        ) or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(
-            **kwargs
-        )
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get(
-            "logging_policy"
-        ) or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get(
-            "http_logging_policy"
-        ) or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(
-            **kwargs
-        )
-        self.custom_hook_policy = kwargs.get(
-            "custom_hook_policy"
-        ) or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get(
-            "redirect_policy"
-        ) or policies.AsyncRedirectPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = policies.AsyncBearerTokenCredentialPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-monitor-ingestion-1.0.0b1/azure/monitor/ingestion/aio/_operations/__init__.py` & `azure-monitor-ingestion-1.0.1/azure/monitor/ingestion/aio/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._operations import MonitorIngestionClientOperationsMixin
+from ._client import LogsIngestionClient
 
-from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+try:
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # pylint: disable=unused-wildcard-import
+except ImportError:
+    _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "MonitorIngestionClientOperationsMixin",
+    "LogsIngestionClient",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
+
 _patch_sdk()
```

