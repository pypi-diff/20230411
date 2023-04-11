# Comparing `tmp/flowtask-4.3.1.tar.gz` & `tmp/flowtask-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowtask-4.3.1.tar", last modified: Mon Apr 10 23:23:48 2023, max compression
+gzip compressed data, was "flowtask-4.3.2.tar", last modified: Tue Apr 11 01:37:17 2023, max compression
```

## Comparing `flowtask-4.3.1.tar` & `flowtask-4.3.2.tar`

### file list

```diff
@@ -1,192 +1,205 @@
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.346930 flowtask-4.3.1/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1305 2023-04-08 03:29:54.000000 flowtask-4.3.1/CONTRIBUTING.md
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       90 2023-04-08 00:40:06.000000 flowtask-4.3.1/INSTALL
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11357 2023-04-08 00:36:44.000000 flowtask-4.3.1/LICENSE
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      224 2023-04-08 03:21:18.000000 flowtask-4.3.1/MANIFEST.in
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      589 2023-04-08 03:21:13.000000 flowtask-4.3.1/Makefile
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4215 2023-04-10 23:23:48.346930 flowtask-4.3.1/PKG-INFO
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2819 2023-04-08 03:29:01.000000 flowtask-4.3.1/README.md
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.322930 flowtask-4.3.1/flowtask/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      474 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      994 2023-04-09 19:21:54.000000 flowtask-4.3.1/flowtask/__main__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.334930 flowtask-4.3.1/flowtask/components/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9238 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/AddDataset.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6146 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/Boto3Client.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      193 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CopyTo.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15289 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/CopyToPg.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.334930 flowtask-4.3.1/flowtask/components/CreateReport/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6589 2023-04-09 02:21:01.000000 flowtask-4.3.1/flowtask/components/CreateReport/CreateReport.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      148 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/__init__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.334930 flowtask-4.3.1/flowtask/components/CreateReport/charts/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      439 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/charts/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1816 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/charts/bar.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1994 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/charts/base.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2150 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/charts/pie.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      342 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/CreateReport/utils.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7120 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DataInput.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9519 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DateList.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6667 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DbClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14849 2023-04-09 01:56:59.000000 flowtask-4.3.1/flowtask/components/DownloadFrom.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6840 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DownloadFromFTP.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13178 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DownloadFromIMAP.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9693 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DownloadFromS3.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9272 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DownloadFromSFTP.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3131 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DownloadFromSharepoint.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4248 2023-04-09 02:05:04.000000 flowtask-4.3.1/flowtask/components/DownloadFromSmartSheet.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      227 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/DropboxClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      833 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/Dummy.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      150 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/Excel365.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9581 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/ExecuteSQL.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3823 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FTPClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6195 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileBase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5136 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileCopy.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3095 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileDelete.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7247 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileExists.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3025 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileIteratorDelete.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4072 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileList.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2037 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FileOpen.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.334930 flowtask-4.3.1/flowtask/components/FilterRows/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5340 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/FilterRows/FilterRows.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      147 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/FilterRows/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2211 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/FilterRows/functions.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3095 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/GoogleA4.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      213 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/GoogleClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15042 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/HTTPClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6167 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/IMAPClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6520 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/IteratorBase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    12740 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/MergeFiles.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3979 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/O365Client.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      149 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/OneDrive.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    20497 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/OpenWithBase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    22825 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/OpenWithPandas.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3451 2023-04-10 22:37:14.000000 flowtask-4.3.1/flowtask/components/OpenXML.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6239 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/PGPDecrypt.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5475 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/PandasIterator.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7077 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/PandasToFile.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3636 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/ParamIterator.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4483 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/PrintMessage.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5243 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/QSBase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10122 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/QueryIterator.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9495 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/QueryToInsert.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    25069 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/QueryToPandas.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7169 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/RESTClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2012 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/RunSSH.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2918 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/RunShell.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14081 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/SSHClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7071 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/SendNotify.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5263 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/SetVariables.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4177 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/Sharepoint.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4994 2023-04-09 02:20:14.000000 flowtask-4.3.1/flowtask/components/SubTask.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5808 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableBase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10618 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableDelete.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3316 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableInput.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.334930 flowtask-4.3.1/flowtask/components/TableOutput/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     8577 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableOutput/TableOutput.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       66 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/TableOutput/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4579 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableOutput/postgres.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    16499 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TableSchema.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/components/TransformRows/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11102 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/TransformRows/TransformRows.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      169 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/TransformRows/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    25492 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/TransformRows/functions.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2384 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/UPCDatabase.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7734 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/Uncompress.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4726 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UniqueRows.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5128 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UpdateOperationalVars.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11559 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UploadTo.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4331 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UploadToS3.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4516 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UploadToSFTP.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4041 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/UserFunc.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4349 2023-04-10 22:22:00.000000 flowtask-4.3.1/flowtask/components/WSDLClient.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7244 2023-04-10 22:35:02.000000 flowtask-4.3.1/flowtask/components/XMLtoPandas.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2908 2023-04-10 00:48:54.000000 flowtask-4.3.1/flowtask/components/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    22782 2023-04-09 01:54:08.000000 flowtask-4.3.1/flowtask/components/abstract.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3243 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/azureauth.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2729 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/functions.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5667 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/group.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13378 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/interfaces.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/components/py.typed
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3417 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/tConcat.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4748 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/tFilter.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6004 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/tJoin.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13098 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/tMap.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2372 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/tPluckCols.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    17830 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/components/user.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6085 2023-04-09 23:40:55.000000 flowtask-4.3.1/flowtask/conf.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3991 2023-04-10 00:06:08.000000 flowtask-4.3.1/flowtask/download.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14977 2023-04-09 01:38:24.000000 flowtask-4.3.1/flowtask/events.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   995657 2023-04-08 14:56:28.000000 flowtask-4.3.1/flowtask/exceptions.c
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/jobs/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       51 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/jobs/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5265 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/models.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/parsers/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      323 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/parsers/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   287490 2023-04-08 14:56:28.000000 flowtask-4.3.1/flowtask/parsers/_yaml.c
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7463 2023-04-09 19:20:55.000000 flowtask-4.3.1/flowtask/parsers/argparser.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   335612 2023-04-08 14:56:28.000000 flowtask-4.3.1/flowtask/parsers/base.c
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   286221 2023-04-08 14:56:28.000000 flowtask-4.3.1/flowtask/parsers/json.c
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1722 2023-04-09 21:51:45.000000 flowtask-4.3.1/flowtask/parsers/maps.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   286259 2023-04-08 14:56:28.000000 flowtask-4.3.1/flowtask/parsers/toml.c
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/plugins/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      417 2023-04-09 22:10:21.000000 flowtask-4.3.1/flowtask/plugins/__init__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/plugins/components/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-09 21:32:15.000000 flowtask-4.3.1/flowtask/plugins/components/__init__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/plugins/handler/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1655 2023-04-09 23:09:17.000000 flowtask-4.3.1/flowtask/plugins/handler/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1187 2023-04-09 21:34:02.000000 flowtask-4.3.1/flowtask/plugins/importer.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9290 2023-04-09 19:19:48.000000 flowtask-4.3.1/flowtask/runner.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/scheduler/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      166 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/scheduler/__init__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.338930 flowtask-4.3.1/flowtask/scheduler/handlers/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      128 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/scheduler/handlers/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10649 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/scheduler/handlers/manager.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2559 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/scheduler/handlers/service.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    28790 2023-04-09 02:21:08.000000 flowtask-4.3.1/flowtask/scheduler/scheduler.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.342930 flowtask-4.3.1/flowtask/tasks/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-09 01:24:52.000000 flowtask-4.3.1/flowtask/tasks/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15394 2023-04-09 02:23:08.000000 flowtask-4.3.1/flowtask/tasks/abstract.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3865 2023-04-09 01:15:38.000000 flowtask-4.3.1/flowtask/tasks/command.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9319 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/tasks/pile.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      887 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/tasks/run.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.342930 flowtask-4.3.1/flowtask/tasks/storages/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      286 2023-04-09 00:53:15.000000 flowtask-4.3.1/flowtask/tasks/storages/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      675 2023-04-09 01:53:02.000000 flowtask-4.3.1/flowtask/tasks/storages/abstract.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      756 2023-04-09 01:07:20.000000 flowtask-4.3.1/flowtask/tasks/storages/database.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2261 2023-04-09 01:50:45.000000 flowtask-4.3.1/flowtask/tasks/storages/filesystem.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      752 2023-04-09 01:05:52.000000 flowtask-4.3.1/flowtask/tasks/storages/row.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    24767 2023-04-09 02:04:44.000000 flowtask-4.3.1/flowtask/tasks/task.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.342930 flowtask-4.3.1/flowtask/template/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3986 2023-04-09 01:41:55.000000 flowtask-4.3.1/flowtask/template/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6810 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/tests.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.342930 flowtask-4.3.1/flowtask/types/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      166 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/types/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   298393 2023-04-08 03:26:09.000000 flowtask-4.3.1/flowtask/types/typedefs.c
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.346930 flowtask-4.3.1/flowtask/utils/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      527 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/utils/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14405 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/utils/_functions.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2126 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/utils/constants.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      485 2023-04-08 03:26:08.000000 flowtask-4.3.1/flowtask/utils/encoders.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2553 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/utils/executor.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   288527 2023-04-10 21:24:30.000000 flowtask-4.3.1/flowtask/utils/functions.cpp
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   306739 2023-04-08 14:45:00.000000 flowtask-4.3.1/flowtask/utils/json.cpp
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2002 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/utils/mail.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   369041 2023-04-08 03:26:09.000000 flowtask-4.3.1/flowtask/utils/parseqs.c
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7593 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/utils/stats.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1896 2023-04-08 01:12:31.000000 flowtask-4.3.1/flowtask/utils/validators.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      352 2023-04-10 23:23:43.000000 flowtask-4.3.1/flowtask/version.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.322930 flowtask-4.3.1/flowtask.egg-info/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4215 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/PKG-INFO
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5325 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/SOURCES.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        1 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/dependency_links.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       76 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/entry_points.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      768 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/requires.txt
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       17 2023-04-10 23:23:48.000000 flowtask-4.3.1/flowtask.egg-info/top_level.txt
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.346930 flowtask-4.3.1/plugins/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       35 2023-04-09 21:10:13.000000 flowtask-4.3.1/plugins/__init__.py
-drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-10 23:23:48.346930 flowtask-4.3.1/plugins/components/
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      538 2023-04-10 16:07:25.000000 flowtask-4.3.1/plugins/components/TestComponent.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      299 2023-04-10 16:12:33.000000 flowtask-4.3.1/plugins/components/Use1.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       68 2023-04-09 21:02:40.000000 flowtask-4.3.1/plugins/components/__init__.py
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1920 2023-04-08 03:22:00.000000 flowtask-4.3.1/pyproject.toml
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       38 2023-04-10 23:23:48.346930 flowtask-4.3.1/setup.cfg
--rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6258 2023-04-08 03:26:08.000000 flowtask-4.3.1/setup.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.170870 flowtask-4.3.2/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1305 2023-04-08 03:29:54.000000 flowtask-4.3.2/CONTRIBUTING.md
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       90 2023-04-08 00:40:06.000000 flowtask-4.3.2/INSTALL
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11357 2023-04-08 00:36:44.000000 flowtask-4.3.2/LICENSE
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      224 2023-04-08 03:21:18.000000 flowtask-4.3.2/MANIFEST.in
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      589 2023-04-08 03:21:13.000000 flowtask-4.3.2/Makefile
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4215 2023-04-11 01:37:17.170870 flowtask-4.3.2/PKG-INFO
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2819 2023-04-08 03:29:01.000000 flowtask-4.3.2/README.md
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.142871 flowtask-4.3.2/flowtask/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      474 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      994 2023-04-09 19:21:54.000000 flowtask-4.3.2/flowtask/__main__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9238 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/AddDataset.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6146 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/Boto3Client.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      193 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CopyTo.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15289 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/CopyToPg.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/CreateReport/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6589 2023-04-09 02:21:01.000000 flowtask-4.3.2/flowtask/components/CreateReport/CreateReport.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      148 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/CreateReport/charts/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      439 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/charts/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1816 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/charts/bar.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1994 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/charts/base.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2150 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/charts/pie.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      342 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/CreateReport/utils.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7120 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DataInput.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9519 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DateList.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6667 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DbClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14849 2023-04-09 01:56:59.000000 flowtask-4.3.2/flowtask/components/DownloadFrom.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6840 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DownloadFromFTP.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13178 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DownloadFromIMAP.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9693 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DownloadFromS3.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9272 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DownloadFromSFTP.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3131 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DownloadFromSharepoint.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4248 2023-04-09 02:05:04.000000 flowtask-4.3.2/flowtask/components/DownloadFromSmartSheet.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      227 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/DropboxClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      833 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/Dummy.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      150 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/Excel365.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9581 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/ExecuteSQL.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3823 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FTPClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6195 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileBase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5136 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileCopy.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3095 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileDelete.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7247 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileExists.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3025 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileIteratorDelete.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4072 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileList.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2037 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FileOpen.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/FilterRows/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5340 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/FilterRows/FilterRows.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      147 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/FilterRows/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1981 2023-04-11 00:07:27.000000 flowtask-4.3.2/flowtask/components/FilterRows/functions.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3095 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/GoogleA4.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      213 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/GoogleClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15042 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/HTTPClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6167 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/IMAPClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6520 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/IteratorBase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    12740 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/MergeFiles.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3979 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/O365Client.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      149 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/OneDrive.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    20497 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/OpenWithBase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    22825 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/OpenWithPandas.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3451 2023-04-10 22:37:14.000000 flowtask-4.3.2/flowtask/components/OpenXML.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6239 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/PGPDecrypt.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5475 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/PandasIterator.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7077 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/PandasToFile.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3636 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/ParamIterator.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4483 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/PrintMessage.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5243 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/QSBase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10122 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/QueryIterator.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9495 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/QueryToInsert.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    25069 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/QueryToPandas.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7169 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/RESTClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2012 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/RunSSH.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2918 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/RunShell.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14081 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/SSHClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7071 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/SendNotify.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5263 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/SetVariables.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4177 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/Sharepoint.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4994 2023-04-09 02:20:14.000000 flowtask-4.3.2/flowtask/components/SubTask.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5808 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableBase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10618 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableDelete.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3316 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableInput.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/TableOutput/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     8577 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableOutput/TableOutput.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       66 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/TableOutput/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4579 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableOutput/postgres.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    16499 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/TableSchema.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/components/TransformRows/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11103 2023-04-11 00:06:32.000000 flowtask-4.3.2/flowtask/components/TransformRows/TransformRows.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      169 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/TransformRows/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    25488 2023-04-11 00:06:24.000000 flowtask-4.3.2/flowtask/components/TransformRows/functions.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2384 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/UPCDatabase.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7734 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/Uncompress.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4726 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UniqueRows.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5128 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UpdateOperationalVars.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11559 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UploadTo.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4331 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UploadToS3.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4516 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UploadToSFTP.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4041 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/UserFunc.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4349 2023-04-10 22:22:00.000000 flowtask-4.3.2/flowtask/components/WSDLClient.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7244 2023-04-10 22:35:02.000000 flowtask-4.3.2/flowtask/components/XMLtoPandas.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2933 2023-04-11 01:11:43.000000 flowtask-4.3.2/flowtask/components/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    22782 2023-04-09 01:54:08.000000 flowtask-4.3.2/flowtask/components/abstract.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3243 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/azureauth.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2729 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/functions.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5667 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/group.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13378 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/interfaces.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/components/py.typed
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3417 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/tConcat.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4748 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/tFilter.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6004 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/tJoin.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    13098 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/tMap.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2372 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/tPluckCols.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    17830 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/components/user.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6085 2023-04-09 23:40:55.000000 flowtask-4.3.2/flowtask/conf.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3991 2023-04-10 00:06:08.000000 flowtask-4.3.2/flowtask/download.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14977 2023-04-09 01:38:24.000000 flowtask-4.3.2/flowtask/events.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   995657 2023-04-08 14:56:28.000000 flowtask-4.3.2/flowtask/exceptions.c
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.158871 flowtask-4.3.2/flowtask/jobs/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       51 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/jobs/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5265 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/models.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/parsers/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      323 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/parsers/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   287490 2023-04-08 14:56:28.000000 flowtask-4.3.2/flowtask/parsers/_yaml.c
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7463 2023-04-09 19:20:55.000000 flowtask-4.3.2/flowtask/parsers/argparser.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   335612 2023-04-08 14:56:28.000000 flowtask-4.3.2/flowtask/parsers/base.c
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   286221 2023-04-08 14:56:28.000000 flowtask-4.3.2/flowtask/parsers/json.c
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1722 2023-04-09 21:51:45.000000 flowtask-4.3.2/flowtask/parsers/maps.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   286259 2023-04-08 14:56:28.000000 flowtask-4.3.2/flowtask/parsers/toml.c
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/plugins/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      417 2023-04-11 01:04:55.000000 flowtask-4.3.2/flowtask/plugins/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/plugins/components/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-09 21:32:15.000000 flowtask-4.3.2/flowtask/plugins/components/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/plugins/handler/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1655 2023-04-09 23:09:17.000000 flowtask-4.3.2/flowtask/plugins/handler/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1187 2023-04-09 21:34:02.000000 flowtask-4.3.2/flowtask/plugins/importer.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/plugins/sources/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:09:23.000000 flowtask-4.3.2/flowtask/plugins/sources/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9290 2023-04-09 19:19:48.000000 flowtask-4.3.2/flowtask/runner.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/scheduler/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      166 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/scheduler/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/scheduler/handlers/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      128 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/scheduler/handlers/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    10649 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/scheduler/handlers/manager.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2559 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/scheduler/handlers/service.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    28790 2023-04-09 02:21:08.000000 flowtask-4.3.2/flowtask/scheduler/scheduler.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.162871 flowtask-4.3.2/flowtask/tasks/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-09 01:24:52.000000 flowtask-4.3.2/flowtask/tasks/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    15394 2023-04-09 02:23:08.000000 flowtask-4.3.2/flowtask/tasks/abstract.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3865 2023-04-09 01:15:38.000000 flowtask-4.3.2/flowtask/tasks/command.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9319 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/tasks/pile.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      887 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/tasks/run.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.166870 flowtask-4.3.2/flowtask/tasks/storages/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      286 2023-04-09 00:53:15.000000 flowtask-4.3.2/flowtask/tasks/storages/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      675 2023-04-09 01:53:02.000000 flowtask-4.3.2/flowtask/tasks/storages/abstract.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      756 2023-04-09 01:07:20.000000 flowtask-4.3.2/flowtask/tasks/storages/database.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2261 2023-04-09 01:50:45.000000 flowtask-4.3.2/flowtask/tasks/storages/filesystem.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      752 2023-04-09 01:05:52.000000 flowtask-4.3.2/flowtask/tasks/storages/row.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    24767 2023-04-09 02:04:44.000000 flowtask-4.3.2/flowtask/tasks/task.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.166870 flowtask-4.3.2/flowtask/template/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     3986 2023-04-09 01:41:55.000000 flowtask-4.3.2/flowtask/template/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6810 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/tests.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.166870 flowtask-4.3.2/flowtask/types/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      166 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/types/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   298393 2023-04-08 03:26:09.000000 flowtask-4.3.2/flowtask/types/typedefs.c
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.166870 flowtask-4.3.2/flowtask/utils/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      527 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/utils/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    14405 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/utils/_functions.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2126 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/utils/constants.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      485 2023-04-08 03:26:08.000000 flowtask-4.3.2/flowtask/utils/encoders.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2553 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/utils/executor.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   288527 2023-04-10 21:24:30.000000 flowtask-4.3.2/flowtask/utils/functions.cpp
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   306739 2023-04-08 14:45:00.000000 flowtask-4.3.2/flowtask/utils/json.cpp
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2002 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/utils/mail.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)   369041 2023-04-08 03:26:09.000000 flowtask-4.3.2/flowtask/utils/parseqs.c
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     7593 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/utils/stats.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1896 2023-04-08 01:12:31.000000 flowtask-4.3.2/flowtask/utils/validators.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      352 2023-04-11 01:34:51.000000 flowtask-4.3.2/flowtask/version.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.146871 flowtask-4.3.2/flowtask.egg-info/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     4215 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/PKG-INFO
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5640 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        1 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       76 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/entry_points.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      768 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/requires.txt
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       17 2023-04-11 01:37:17.000000 flowtask-4.3.2/flowtask.egg-info/top_level.txt
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.166870 flowtask-4.3.2/plugins/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       35 2023-04-09 21:10:13.000000 flowtask-4.3.2/plugins/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.170870 flowtask-4.3.2/plugins/components/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      538 2023-04-10 16:07:25.000000 flowtask-4.3.2/plugins/components/TestComponent.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)      299 2023-04-10 16:12:33.000000 flowtask-4.3.2/plugins/components/Use1.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       68 2023-04-09 21:02:40.000000 flowtask-4.3.2/plugins/components/__init__.py
+drwxrwxr-x   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:37:17.170870 flowtask-4.3.2/plugins/sources/
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)        0 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/__init__.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     2757 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/get_populartimes.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     5705 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/google.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    23000 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/hubspot.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    18326 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/icims.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    19826 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/mobileinsight.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     8154 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/newrelic.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     8587 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/uap.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     9592 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/venu.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)    11152 2023-04-11 01:10:29.000000 flowtask-4.3.2/plugins/sources/vocinity.py
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     1920 2023-04-08 03:22:00.000000 flowtask-4.3.2/pyproject.toml
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)       38 2023-04-11 01:37:17.170870 flowtask-4.3.2/setup.cfg
+-rw-rw-r--   0 jesuslara  (1000) jesuslara  (1000)     6258 2023-04-08 03:26:08.000000 flowtask-4.3.2/setup.py
```

### Comparing `flowtask-4.3.1/CONTRIBUTING.md` & `flowtask-4.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/LICENSE` & `flowtask-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/Makefile` & `flowtask-4.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/PKG-INFO` & `flowtask-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowtask
-Version: 4.3.1
+Version: 4.3.2
 Summary: Framework for building/running Tasks and from CLI and API for orchestation. Component-based Task builder/Runner for non-programmers.
 Home-page: https://github.com/phenobarbital/flowtask
 Author: Jesus Lara
 Author-email: "Jesus Lara G." <jesuslarag@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/phenobarbital/flowtask
 Project-URL: Funding, https://paypal.me/phenobarbital
```

### Comparing `flowtask-4.3.1/README.md` & `flowtask-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/__main__.py` & `flowtask-4.3.2/flowtask/__main__.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/AddDataset.py` & `flowtask-4.3.2/flowtask/components/AddDataset.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/Boto3Client.py` & `flowtask-4.3.2/flowtask/components/Boto3Client.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/CopyToPg.py` & `flowtask-4.3.2/flowtask/components/CopyToPg.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/CreateReport/CreateReport.py` & `flowtask-4.3.2/flowtask/components/CreateReport/CreateReport.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/CreateReport/charts/bar.py` & `flowtask-4.3.2/flowtask/components/CreateReport/charts/bar.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/CreateReport/charts/base.py` & `flowtask-4.3.2/flowtask/components/CreateReport/charts/base.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/CreateReport/charts/pie.py` & `flowtask-4.3.2/flowtask/components/CreateReport/charts/pie.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DataInput.py` & `flowtask-4.3.2/flowtask/components/DataInput.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DateList.py` & `flowtask-4.3.2/flowtask/components/DateList.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DbClient.py` & `flowtask-4.3.2/flowtask/components/DbClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFrom.py` & `flowtask-4.3.2/flowtask/components/DownloadFrom.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromFTP.py` & `flowtask-4.3.2/flowtask/components/DownloadFromFTP.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromIMAP.py` & `flowtask-4.3.2/flowtask/components/DownloadFromIMAP.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromS3.py` & `flowtask-4.3.2/flowtask/components/DownloadFromS3.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromSFTP.py` & `flowtask-4.3.2/flowtask/components/DownloadFromSFTP.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromSharepoint.py` & `flowtask-4.3.2/flowtask/components/DownloadFromSharepoint.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/DownloadFromSmartSheet.py` & `flowtask-4.3.2/flowtask/components/DownloadFromSmartSheet.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/Dummy.py` & `flowtask-4.3.2/flowtask/components/Dummy.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/ExecuteSQL.py` & `flowtask-4.3.2/flowtask/components/ExecuteSQL.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FTPClient.py` & `flowtask-4.3.2/flowtask/components/FTPClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileBase.py` & `flowtask-4.3.2/flowtask/components/FileBase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileCopy.py` & `flowtask-4.3.2/flowtask/components/FileCopy.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileDelete.py` & `flowtask-4.3.2/flowtask/components/FileDelete.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileExists.py` & `flowtask-4.3.2/flowtask/components/FileExists.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileIteratorDelete.py` & `flowtask-4.3.2/flowtask/components/FileIteratorDelete.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileList.py` & `flowtask-4.3.2/flowtask/components/FileList.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FileOpen.py` & `flowtask-4.3.2/flowtask/components/FileOpen.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FilterRows/FilterRows.py` & `flowtask-4.3.2/flowtask/components/FilterRows/FilterRows.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/FilterRows/functions.py` & `flowtask-4.3.2/flowtask/components/FilterRows/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Functions for FilterRows."""
-import pandas
 import re
 import numpy as np
 
 def drop_columns(dataframe, columns=[]):
     if columns and isinstance(columns, list):
         dataframe.drop(axis=1, columns=columns, inplace=True, errors='ignore')
     return dataframe
@@ -47,21 +46,12 @@
     if columns and isinstance(columns, list):
         for column in columns:
             dataframe[column] = dataframe[column].astype(str)
             dataframe[column] = dataframe[column].apply(clean_chars)
     return dataframe
 
 
-# def suppress_chars(field):
-#     name = str(field)
-#     if re.search(self.pattern, name):
-#         pos = re.search(self.pattern, name).start()
-#         return str(name)[:pos]
-#     else:
-#         return name
-
-
 def fill_na(df, columns:list = [], fill_value='', **kwargs):
     #df[columns].fillna(fill_value, inplace=True)
     df[columns] = df[columns].astype(str).replace(['nan', np.nan], fill_value, regex=True)
     #self.data[u.columns].replace({pandas.NaT: None})
     return df
```

### Comparing `flowtask-4.3.1/flowtask/components/GoogleA4.py` & `flowtask-4.3.2/flowtask/components/GoogleA4.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/HTTPClient.py` & `flowtask-4.3.2/flowtask/components/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/IMAPClient.py` & `flowtask-4.3.2/flowtask/components/IMAPClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/IteratorBase.py` & `flowtask-4.3.2/flowtask/components/IteratorBase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/MergeFiles.py` & `flowtask-4.3.2/flowtask/components/MergeFiles.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/O365Client.py` & `flowtask-4.3.2/flowtask/components/O365Client.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/OpenWithBase.py` & `flowtask-4.3.2/flowtask/components/OpenWithBase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/OpenWithPandas.py` & `flowtask-4.3.2/flowtask/components/OpenWithPandas.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/OpenXML.py` & `flowtask-4.3.2/flowtask/components/OpenXML.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/PGPDecrypt.py` & `flowtask-4.3.2/flowtask/components/PGPDecrypt.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/PandasIterator.py` & `flowtask-4.3.2/flowtask/components/PandasIterator.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/PandasToFile.py` & `flowtask-4.3.2/flowtask/components/PandasToFile.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/ParamIterator.py` & `flowtask-4.3.2/flowtask/components/ParamIterator.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/PrintMessage.py` & `flowtask-4.3.2/flowtask/components/PrintMessage.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/QSBase.py` & `flowtask-4.3.2/flowtask/components/QSBase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/QueryIterator.py` & `flowtask-4.3.2/flowtask/components/QueryIterator.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/QueryToInsert.py` & `flowtask-4.3.2/flowtask/components/QueryToInsert.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/QueryToPandas.py` & `flowtask-4.3.2/flowtask/components/QueryToPandas.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/RESTClient.py` & `flowtask-4.3.2/flowtask/components/RESTClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/RunSSH.py` & `flowtask-4.3.2/flowtask/components/RunSSH.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/RunShell.py` & `flowtask-4.3.2/flowtask/components/RunShell.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/SSHClient.py` & `flowtask-4.3.2/flowtask/components/SSHClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/SendNotify.py` & `flowtask-4.3.2/flowtask/components/SendNotify.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/SetVariables.py` & `flowtask-4.3.2/flowtask/components/SetVariables.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/Sharepoint.py` & `flowtask-4.3.2/flowtask/components/Sharepoint.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/SubTask.py` & `flowtask-4.3.2/flowtask/components/SubTask.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableBase.py` & `flowtask-4.3.2/flowtask/components/TableBase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableDelete.py` & `flowtask-4.3.2/flowtask/components/TableDelete.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableInput.py` & `flowtask-4.3.2/flowtask/components/TableInput.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableOutput/TableOutput.py` & `flowtask-4.3.2/flowtask/components/TableOutput/TableOutput.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableOutput/postgres.py` & `flowtask-4.3.2/flowtask/components/TableOutput/postgres.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TableSchema.py` & `flowtask-4.3.2/flowtask/components/TableSchema.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/TransformRows/TransformRows.py` & `flowtask-4.3.2/flowtask/components/TransformRows/TransformRows.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from flowtask.exceptions import ComponentError, DataNotFound
 # moving this outside of TranformRows
 import flowtask.components.TransformRows.functions as dffunctions
 from flowtask.utils.executor import getFunction
 from flowtask.utils import AttrDict
 from flowtask.utils.functions import check_empty
 
+
 class TransformRows(DtComponent):
     """TransformRows.
 
     Tranform, add or modify rows based on some criteria
     """
     def __init__(
             self,
```

### Comparing `flowtask-4.3.1/flowtask/components/TransformRows/functions.py` & `flowtask-4.3.2/flowtask/components/TransformRows/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import orjson
 import numpy as np
 import pandas
 from tzwhere import tzwhere
 from navconfig.logging import logging
 from pandas.tseries.offsets import MonthEnd
 from querysource.types import strtobool
-from settings.settings import DEFAULT_TIMEZONE
+from flowtask.conf import DEFAULT_TIMEZONE
 
 
 def explode(df: pandas.DataFrame, field: str, columns: list = None, is_string: bool = True, delimiter: str = ','):
     splitcols = [field]
     if columns is not None:
         splitcols = splitcols + columns
     ### first: convert all colums to list:
```

### Comparing `flowtask-4.3.1/flowtask/components/UPCDatabase.py` & `flowtask-4.3.2/flowtask/components/UPCDatabase.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/Uncompress.py` & `flowtask-4.3.2/flowtask/components/Uncompress.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UniqueRows.py` & `flowtask-4.3.2/flowtask/components/UniqueRows.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UpdateOperationalVars.py` & `flowtask-4.3.2/flowtask/components/UpdateOperationalVars.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UploadTo.py` & `flowtask-4.3.2/flowtask/components/UploadTo.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UploadToS3.py` & `flowtask-4.3.2/flowtask/components/UploadToS3.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UploadToSFTP.py` & `flowtask-4.3.2/flowtask/components/UploadToSFTP.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/UserFunc.py` & `flowtask-4.3.2/flowtask/components/UserFunc.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/WSDLClient.py` & `flowtask-4.3.2/flowtask/components/WSDLClient.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/XMLtoPandas.py` & `flowtask-4.3.2/flowtask/components/XMLtoPandas.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/__init__.py` & `flowtask-4.3.2/flowtask/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 def loadComponent(component, program: str = None):
     try:
         # Getting Basic Components
         classpath = f"flowtask.components.{component}"
         return importComponent(component, classpath, package='components')
     except ImportError as ex:
+        logger.error(ex)
         try:
             # another, check if task is an User-Defined Component
             classpath = f"flowtask.plugins.components.{component}"
             obj = importComponent(component, classpath, package='components')
             if issubclass(obj, (UserComponent, DtComponent)):
                 return obj
             raise ImportError(
```

### Comparing `flowtask-4.3.1/flowtask/components/abstract.py` & `flowtask-4.3.2/flowtask/components/abstract.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/azureauth.py` & `flowtask-4.3.2/flowtask/components/azureauth.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/functions.py` & `flowtask-4.3.2/flowtask/components/functions.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/group.py` & `flowtask-4.3.2/flowtask/components/group.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/interfaces.py` & `flowtask-4.3.2/flowtask/components/interfaces.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/tConcat.py` & `flowtask-4.3.2/flowtask/components/tConcat.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/tFilter.py` & `flowtask-4.3.2/flowtask/components/tFilter.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/tJoin.py` & `flowtask-4.3.2/flowtask/components/tJoin.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/tMap.py` & `flowtask-4.3.2/flowtask/components/tMap.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/tPluckCols.py` & `flowtask-4.3.2/flowtask/components/tPluckCols.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/components/user.py` & `flowtask-4.3.2/flowtask/components/user.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/conf.py` & `flowtask-4.3.2/flowtask/conf.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/download.py` & `flowtask-4.3.2/flowtask/download.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/events.py` & `flowtask-4.3.2/flowtask/events.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/exceptions.c` & `flowtask-4.3.2/flowtask/exceptions.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/models.py` & `flowtask-4.3.2/flowtask/models.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/_yaml.c` & `flowtask-4.3.2/flowtask/parsers/_yaml.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/argparser.py` & `flowtask-4.3.2/flowtask/parsers/argparser.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/base.c` & `flowtask-4.3.2/flowtask/parsers/base.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/json.c` & `flowtask-4.3.2/flowtask/parsers/json.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/maps.py` & `flowtask-4.3.2/flowtask/parsers/maps.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/parsers/toml.c` & `flowtask-4.3.2/flowtask/parsers/toml.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/plugins/handler/__init__.py` & `flowtask-4.3.2/flowtask/plugins/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/plugins/importer.py` & `flowtask-4.3.2/flowtask/plugins/importer.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/runner.py` & `flowtask-4.3.2/flowtask/runner.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/scheduler/handlers/manager.py` & `flowtask-4.3.2/flowtask/scheduler/handlers/manager.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/scheduler/handlers/service.py` & `flowtask-4.3.2/flowtask/scheduler/handlers/service.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/scheduler/scheduler.py` & `flowtask-4.3.2/flowtask/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/abstract.py` & `flowtask-4.3.2/flowtask/tasks/abstract.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/command.py` & `flowtask-4.3.2/flowtask/tasks/command.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/pile.py` & `flowtask-4.3.2/flowtask/tasks/pile.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/run.py` & `flowtask-4.3.2/flowtask/tasks/run.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/storages/abstract.py` & `flowtask-4.3.2/flowtask/tasks/storages/abstract.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/storages/database.py` & `flowtask-4.3.2/flowtask/tasks/storages/database.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/storages/filesystem.py` & `flowtask-4.3.2/flowtask/tasks/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/storages/row.py` & `flowtask-4.3.2/flowtask/tasks/storages/row.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tasks/task.py` & `flowtask-4.3.2/flowtask/tasks/task.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/template/__init__.py` & `flowtask-4.3.2/flowtask/template/__init__.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/tests.py` & `flowtask-4.3.2/flowtask/tests.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/types/typedefs.c` & `flowtask-4.3.2/flowtask/types/typedefs.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/__init__.py` & `flowtask-4.3.2/flowtask/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/_functions.py` & `flowtask-4.3.2/flowtask/utils/_functions.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/constants.py` & `flowtask-4.3.2/flowtask/utils/constants.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/executor.py` & `flowtask-4.3.2/flowtask/utils/executor.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/functions.cpp` & `flowtask-4.3.2/flowtask/utils/functions.cpp`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/json.cpp` & `flowtask-4.3.2/flowtask/utils/json.cpp`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/mail.py` & `flowtask-4.3.2/flowtask/utils/mail.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/parseqs.c` & `flowtask-4.3.2/flowtask/utils/parseqs.c`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/stats.py` & `flowtask-4.3.2/flowtask/utils/stats.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask/utils/validators.py` & `flowtask-4.3.2/flowtask/utils/validators.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/flowtask.egg-info/PKG-INFO` & `flowtask-4.3.2/flowtask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowtask
-Version: 4.3.1
+Version: 4.3.2
 Summary: Framework for building/running Tasks and from CLI and API for orchestation. Component-based Task builder/Runner for non-programmers.
 Home-page: https://github.com/phenobarbital/flowtask
 Author: Jesus Lara
 Author-email: "Jesus Lara G." <jesuslarag@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/phenobarbital/flowtask
 Project-URL: Funding, https://paypal.me/phenobarbital
```

### Comparing `flowtask-4.3.1/flowtask.egg-info/SOURCES.txt` & `flowtask-4.3.2/flowtask.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 flowtask/parsers/json.c
 flowtask/parsers/maps.py
 flowtask/parsers/toml.c
 flowtask/plugins/__init__.py
 flowtask/plugins/importer.py
 flowtask/plugins/components/__init__.py
 flowtask/plugins/handler/__init__.py
+flowtask/plugins/sources/__init__.py
 flowtask/scheduler/__init__.py
 flowtask/scheduler/scheduler.py
 flowtask/scheduler/handlers/__init__.py
 flowtask/scheduler/handlers/manager.py
 flowtask/scheduler/handlers/service.py
 flowtask/tasks/__init__.py
 flowtask/tasks/abstract.py
@@ -160,8 +161,18 @@
 flowtask/utils/mail.py
 flowtask/utils/parseqs.c
 flowtask/utils/stats.py
 flowtask/utils/validators.py
 plugins/__init__.py
 plugins/components/TestComponent.py
 plugins/components/Use1.py
-plugins/components/__init__.py
+plugins/components/__init__.py
+plugins/sources/__init__.py
+plugins/sources/get_populartimes.py
+plugins/sources/google.py
+plugins/sources/hubspot.py
+plugins/sources/icims.py
+plugins/sources/mobileinsight.py
+plugins/sources/newrelic.py
+plugins/sources/uap.py
+plugins/sources/venu.py
+plugins/sources/vocinity.py
```

### Comparing `flowtask-4.3.1/flowtask.egg-info/requires.txt` & `flowtask-4.3.2/flowtask.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/plugins/components/TestComponent.py` & `flowtask-4.3.2/plugins/components/TestComponent.py`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/pyproject.toml` & `flowtask-4.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flowtask-4.3.1/setup.py` & `flowtask-4.3.2/setup.py`

 * *Files identical despite different names*

