# Comparing `tmp/ytsaurus-spyt-1.69.3b436.post17234365.dev1.tar.gz` & `tmp/ytsaurus-spyt-1.69.3b438.post3932209.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.69.3b436.post17234365.dev1.tar", last modified: Mon Apr 10 15:30:53 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.69.3b438.post3932209.dev1.tar", last modified: Tue Apr 11 11:45:13 2023, max compression
```

## Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1.tar` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11036 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-10 15:29:49.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3493 2023-03-18 23:30:06.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35089 2023-04-10 11:54:30.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-04-10 15:30:23.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-10 15:30:53.000000 ytsaurus-spyt-1.69.3b436.post17234365.dev1/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11036 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-10 15:29:49.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3493 2023-03-18 23:30:06.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35113 2023-04-11 11:38:05.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-04-11 11:44:58.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-11 11:45:12.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-11 11:45:13.000000 ytsaurus-spyt-1.69.3b438.post3932209.dev1/setup.cfg
```

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/client.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/common.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/conf.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/enabler.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/standalone.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/standalone.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import uuid
 
 from spyt.dependency_utils import require_yt_client
 require_yt_client()
 
 from yt.wrapper.common import update_inplace, update
-from yt.wrapper.cypress_commands import exists, copy
+from yt.wrapper.cypress_commands import exists, copy as cypress_copy
 from yt.wrapper.acl_commands import check_permission
 from yt.wrapper.file_commands import upload_file_to_cache
 from yt.wrapper.http_helpers import get_token, get_user_name, get_proxy_url
 from yt.wrapper.operation_commands import TimeWatcher, process_operation_unsuccesful_finish_state, \
     abort_operation, get_operation_state
 from yt.wrapper.run_operation_commands import run_operation
 from yt.wrapper.spec_builders import VanillaSpecBuilder
@@ -220,15 +220,15 @@
         for spark_arg in spark_args:
             if spark_arg.startswith('local:/'):
                 if spark_arg not in remote_paths:
                     file_path = spark_arg[7:] # Drops prefix
                     _, file_extension = os.path.splitext(file_path)
                     destination = upload_file_to_cache(file_path, client=client)
                     destination_ext = "{}{}".format(destination, file_extension)
-                    copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
+                    cypress_copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
                     logger.info("%s has been uploaded to YT as %s", file_path, destination_ext)
                     remote_paths[spark_arg] = "yt:/{}".format(destination_ext)
                 new_spark_args.append(remote_paths[spark_arg])
             else:
                 new_spark_args.append(spark_arg)
         spark_args = new_spark_args
```

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/submit.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/types.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/spyt/utils.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.3b436.post17234365.dev1/setup.py` & `ytsaurus-spyt-1.69.3b438.post3932209.dev1/setup.py`

 * *Files identical despite different names*

