# Comparing `tmp/sl4p-1.4.2-py3-none-win_amd64.whl.zip` & `tmp/sl4p-1.4.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 22740 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     1386 b- defN 23-Mar-28 05:53 sl4p/__init__.py
+Zip file size: 22821 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat     1473 b- defN 23-Apr-11 05:32 sl4p/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 23-Mar-06 08:48 sl4p/sl4p_config.eg.json
 -rw-rw-rw-  2.0 fat     1593 b- defN 23-Mar-06 08:47 sl4p/sl4p_config.eg_professional.json
 -rw-rw-rw-  2.0 fat      983 b- defN 23-Mar-23 08:46 sl4p/mconfigs/apps_cfg.json
 -rw-rw-rw-  2.0 fat     1736 b- defN 23-Mar-27 10:24 sl4p/mconfigs/apps_default.json
 -rw-rw-rw-  2.0 fat     1733 b- defN 23-Mar-27 10:24 sl4p/mconfigs/cfgf_default.json
 -rw-rw-rw-  2.0 fat       23 b- defN 23-Mar-23 08:46 sl4p/src/__init__.py
 -rw-rw-rw-  2.0 fat      825 b- defN 23-Mar-23 08:46 sl4p/src/api.py
 -rw-rw-rw-  2.0 fat     7961 b- defN 23-Mar-23 08:46 sl4p/src/config.py
 -rw-rw-rw-  2.0 fat      707 b- defN 23-Mar-23 08:46 sl4p/src/const.py
 -rw-rw-rw-  2.0 fat     6397 b- defN 23-Mar-23 08:46 sl4p/src/context.py
 -rw-rw-rw-  2.0 fat     3806 b- defN 23-Mar-23 08:46 sl4p/src/decorators.py
 -rw-rw-rw-  2.0 fat     4215 b- defN 23-Mar-28 05:42 sl4p/src/embedding.py
--rw-rw-rw-  2.0 fat     8253 b- defN 23-Mar-28 05:48 sl4p/src/getter.py
+-rw-rw-rw-  2.0 fat     8431 b- defN 23-Apr-11 05:30 sl4p/src/getter.py
 -rw-rw-rw-  2.0 fat     3264 b- defN 23-Mar-23 08:48 sl4p/src/stats_performance.py
 -rw-rw-rw-  2.0 fat     2313 b- defN 23-Mar-23 08:48 sl4p/src/utils.py
--rw-rw-rw-  2.0 fat    13977 b- defN 23-Apr-10 07:16 sl4p-1.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 07:16 sl4p-1.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-10 07:16 sl4p-1.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1554 b- defN 23-Apr-10 07:16 sl4p-1.4.2.dist-info/RECORD
-20 files, 61130 bytes uncompressed, 20242 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat    14040 b- defN 23-Apr-11 05:39 sl4p-1.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-11 05:39 sl4p-1.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-11 05:39 sl4p-1.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1554 b- defN 23-Apr-11 05:39 sl4p-1.4.3.dist-info/RECORD
+20 files, 61464 bytes uncompressed, 20323 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: sl4p/src/stats_performance.py
 Comment: 
 
 Filename: sl4p/src/utils.py
 Comment: 
 
-Filename: sl4p-1.4.2.dist-info/METADATA
+Filename: sl4p-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: sl4p-1.4.2.dist-info/WHEEL
+Filename: sl4p-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: sl4p-1.4.2.dist-info/top_level.txt
+Filename: sl4p-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sl4p-1.4.2.dist-info/RECORD
+Filename: sl4p-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sl4p/__init__.py

```diff
@@ -2,22 +2,23 @@
 from .src.api import sl4p, sl4p_try, sl4p_try_exit, sl4p_time, register_post_exception_terminationf
 from .src.api import stat_start, stat_stop, example_config_dict
 
 __all__ = ['sl4p', 'sl4p_try', 'sl4p_time', 'sl4p_try_exit', 'register_post_exception_terminationf',
            'stat_start', 'stat_stop', 'example_config_dict']
 
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
 __author__ = 'surfhawk@github.com'
 
 __doc__ = " Package 'sl4p' for make logging your python application easy." + \
           " In config.json file, you can find lot's of useful options for production."
 
 __version_changes__ = '\n @ Release Note @' \
                       '\n 1.0.0 :: First deployed release version' \
                       '\n 1.3.1 :: Add log_level for @sl4p_time decorator' \
                       '\n 1.3.2 :: Add log_level for SimpleTimer: logger.create_simpleTimer(), config bugfix' \
                       '\n 1.3.3 :: override_dict bugfix (support python 3.9+)' \
                       '\n 1.4.0 :: Layered apps-config, Support console level&format, IndLogger, Enhance stability' \
                       '\n 1.4.1 :: Correct the docs, Change default config (console config has no initial values)' \
                       '\n 1.4.2 :: Coloring console log (by colorlog) and add related configs, Support console stdout' \
+                      '\n 1.4.3 :: Prevented logfile name starting with . (period)' \
                       '\n @@- Note End -@@'
```

## sl4p/src/getter.py

```diff
@@ -101,14 +101,17 @@
     root_logger = logging.getLogger(logger_name if logger_name else _root_logger_name)
 
     if not len(root_logger.handlers):
         logCfg = config.defaultConfig
         msgFormats = config.msgFormats
 
         logfile_name = '{}.{}.{}'.format(logCfg.logfile_name.format(get_now_dtStr()), _root_logger_name, _logfile_ext)
+        if logfile_name.startswith('.'):
+            logfile_name = logfile_name[1:]
+
         logfile_savedir = logCfg.logfile_savedir
         logfile_savedir = os.path.abspath(logfile_savedir)
         timestamp_tpl = logCfg.logging_timestamp_tpl
 
         logfile_path = os.path.join(logfile_savedir, logfile_name)
 
         make_foldertree_if_not_exists(logfile_savedir)
@@ -160,14 +163,17 @@
     # assigning custom_logger_name as root-logger-name dot pre-fixed, does logging both root and custom.
     custom_logger_name = '{}.{}'.format(_root_logger_name, snippet.replace('/', '-'))
     custom_logger = logging.getLogger(custom_logger_name)
 
     if not len(custom_logger.handlers):
         logfile_name = '{}.{}.{}'.format(defaultConfig.logfile_name.format(get_now_dtStr()),
                                          '{}.{}'.format(snippet.replace('/', '-'), _root_logger_name), _logfile_ext)
+        if logfile_name.startswith('.'):
+            logfile_name = logfile_name[1:]
+
         custom_savedir = customConfig.use_custom_savedir
         logfile_savedir = custom_savedir if custom_savedir else defaultConfig.logfile_savedir
         logfile_savedir = os.path.abspath(logfile_savedir)
         timestamp_tpl = defaultConfig.logging_timestamp_tpl
         logfile_path = os.path.join(logfile_savedir, logfile_name)
 
         make_foldertree_if_not_exists(logfile_savedir)
```

## Comparing `sl4p-1.4.2.dist-info/METADATA` & `sl4p-1.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sl4p
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple logger for python. Easy configuration and Multiprocess supported.
 Home-page: https://github.com/surfhawk/sl4p
 Author: surfhawk
 Author-email: surfhawk@naver.com
 License: S-BSD
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Logging
@@ -15,15 +15,15 @@
 Requires-Dist: psutil
 Requires-Dist: colorlog (==6.7.0)
 Requires-Dist: pywin32
 Requires-Dist: colorama
 
 # SL4P : simplest logging for your python
 
-[![](https://img.shields.io/badge/pypi-1.4.2-007ec6?logo=PyPI&logoColor=white)](https://pypi.org/project/sl4p/)
+[![](https://img.shields.io/badge/pypi-1.4.3-007ec6?logo=PyPI&logoColor=white)](https://pypi.org/project/sl4p/)
 [![](https://img.shields.io/badge/python-Min%203.0%20%7C%20Rec'd%203.6%2B-blue?logo=Python&logoColor=white)](https://pypi.org/project/sl4p/)
 [![](https://img.shields.io/badge/license-BSD%20License-lightgrey)](https://pypi.org/project/sl4p/)
 [![](https://img.shields.io/badge/build-passing-brightgreen)](https://pypi.org/project/sl4p/)  
 
 **sl4p** is a logging library that makes it easy to introduce more production-focused logging into your python applications.    
 sl4p users need not know anything about the slightly complex built-in python logging, although sl4p uses built-in Python's logging internally.  
 Quite simply, **you can start logging right in any code with the three lines** below.
@@ -249,15 +249,16 @@
 Right here, please be active in this GitHub repository.  
 All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  
 <br/>
 
 ***
 ## Release Note
 
-**(*) ver 1.4.2 :: Coloring console log (by colorlog) and add related configs, Support console stdout'**  
+**(*) ver 1.4.3 :: Prevented logfile name starting with . (period)**  
+ver 1.4.2 :: Coloring console log (by colorlog) and add related configs, Support console stdout'  
 ver 1.4.1 :: Correct the docs, Change default config (console config has no initial values)  
 ver 1.4.0 :: Layered apps-config, Support console level&format, IndLogger, Enhance stability  
 ver 1.3.3linux :: excluding 'psutil' in requires for linux   
 ver 1.3.3 :: override_dict bugfix (support python 3.9+)  
 ver 1.3.2 :: Add log_level for SimpleTimer: logger.create_simpleTimer(), config bugfix  
 ver 1.3.1 :: Add log_level for @sl4p_time decorator  
 ver 1.2.0 :: Add stopwatch(SimpleTimer), Profiling stats(CPU & MEM), Recording TimeZone
```

## Comparing `sl4p-1.4.2.dist-info/RECORD` & `sl4p-1.4.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-sl4p/__init__.py,sha256=1FnvPmyvP43k6ro2937OQb_1CzVzOO8KitUZvc60rc0,1386
+sl4p/__init__.py,sha256=U__c4i84RpcHScx2hRIIg_QyEtM1YLTPrdw6rMWTq7Y,1473
 sl4p/sl4p_config.eg.json,sha256=uTKKgpupcz_FoAzBA7ZJG-G_xTUXKxdnJ82rfi-BRQ4,307
 sl4p/sl4p_config.eg_professional.json,sha256=8ETdRVHX42lttiPMb_ds-LQlVxLmpfjHeDHJcawIh3Y,1593
 sl4p/mconfigs/apps_cfg.json,sha256=aot9SSPjR-H6a3AziVW2XKL0sZp_7C9GLkkL1ftErk8,983
 sl4p/mconfigs/apps_default.json,sha256=4OEUEVB-UvPQM3HIvCBLtOLGtbh-cUV_FShv9dJTqcg,1736
 sl4p/mconfigs/cfgf_default.json,sha256=d5zX7oJ6b_MY1-vR0rEpBSDjfYxhgrClpNO1C7_SeGg,1733
 sl4p/src/__init__.py,sha256=5FQ0s_2rPa2Vpj_dOhp6usXXAHPT9X-MBVVZLP2Uoqo,23
 sl4p/src/api.py,sha256=QSPmmda-uU-a6035_C4FpfHBhISIYAzVMSiTH0Fdz4A,825
 sl4p/src/config.py,sha256=f4HjqiixvXCsP7tQDEcV9gwdCZ-xVOhUV0HPmoDZt0Y,7961
 sl4p/src/const.py,sha256=ARTzDSYRRHoOeQ4TozUhCUohKJwkHNe1aNVi-rMO5Kw,707
 sl4p/src/context.py,sha256=Lvx4eEvRrZgQ6BqMwb5LXJjr9jGnHQOjctlDmRllFic,6397
 sl4p/src/decorators.py,sha256=E6XPV8KEHNI9XPc47A2VZtsXc5_JwNEHsiEupT1V4dU,3806
 sl4p/src/embedding.py,sha256=J1hYBSEoFHfVtVGeG2v7oZgoRbyFr8ptFlg9gX9wxlA,4215
-sl4p/src/getter.py,sha256=GTPVuGp1bhfS2SvzDlViMOF9KQ7mJNa-8JxPCwpTMVI,8253
+sl4p/src/getter.py,sha256=p9dSm88SPMEHsCqj9hdacGnuEvUJIGAPUkMrvk3faZM,8431
 sl4p/src/stats_performance.py,sha256=Gjsmp6plMwFDk1su7bvMw8R9KwAVXJHo1m8ebN2AUEU,3264
 sl4p/src/utils.py,sha256=QVkeq7YE6ZOInZjm6GdvupU2V-HFRh9YxGcToXJBic8,2313
-sl4p-1.4.2.dist-info/METADATA,sha256=jRVqOkCMKlJiK_A7Wu6F9iZQ2KW39wLoxzyM7k89Lgc,13977
-sl4p-1.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sl4p-1.4.2.dist-info/top_level.txt,sha256=2qwy-uf7rRCkxD2oourdWZ1WOOydVM8KI37dyVsILks,5
-sl4p-1.4.2.dist-info/RECORD,,
+sl4p-1.4.3.dist-info/METADATA,sha256=rSp00g-TPIDZo6RmotuRRH_9SOoxKOSLlifPePTIMKw,14040
+sl4p-1.4.3.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+sl4p-1.4.3.dist-info/top_level.txt,sha256=2qwy-uf7rRCkxD2oourdWZ1WOOydVM8KI37dyVsILks,5
+sl4p-1.4.3.dist-info/RECORD,,
```

