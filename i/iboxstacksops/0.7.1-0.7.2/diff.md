# Comparing `tmp/iboxstacksops-0.7.1.tar.gz` & `tmp/iboxstacksops-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.1.tar", last modified: Thu Mar 30 13:10:46 2023, max compression
+gzip compressed data, was "iboxstacksops-0.7.2.tar", last modified: Tue Apr 11 14:50:01 2023, max compression
```

## Comparing `iboxstacksops-0.7.1.tar` & `iboxstacksops-0.7.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.090116 iboxstacksops-0.7.1/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-03-30 13:10:46.090116 iboxstacksops-0.7.1/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.1/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.074116 iboxstacksops-0.7.1/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.074116 iboxstacksops-0.7.1/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.082116 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-03-30 13:10:45.000000 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-03-30 13:10:45.000000 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-03-30 13:10:45.000000 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-03-30 13:10:45.000000 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-03-30 13:10:45.000000 iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.090116 iboxstacksops-0.7.1/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.1/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.1/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.1/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4059 2023-03-30 09:41:57.000000 iboxstacksops-0.7.1/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5343 2023-03-30 13:07:04.000000 iboxstacksops-0.7.1/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.1/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.1/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.1/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.1/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.1/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-03-28 16:21:23.000000 iboxstacksops-0.7.1/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.1/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.1/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8546 2022-11-15 15:15:53.000000 iboxstacksops-0.7.1/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17095 2023-03-30 09:41:57.000000 iboxstacksops-0.7.1/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.1/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10003 2023-03-22 10:22:38.000000 iboxstacksops-0.7.1/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.1/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.1/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.1/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.1/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.1/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2081 2021-10-28 09:48:26.000000 iboxstacksops-0.7.1/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.1/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.1/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-30 13:10:46.090116 iboxstacksops-0.7.1/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.1/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-03-30 13:10:46.094117 iboxstacksops-0.7.1/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-03-30 13:10:35.000000 iboxstacksops-0.7.1/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.2/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.093030 iboxstacksops-0.7.2/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.093030 iboxstacksops-0.7.2/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.097030 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.2/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.2/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.2/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4059 2023-03-30 09:41:57.000000 iboxstacksops-0.7.2/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5343 2023-03-30 13:07:04.000000 iboxstacksops-0.7.2/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.2/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.2/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.2/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.2/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.2/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.2/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.2/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.2/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.2/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17122 2023-04-11 14:44:45.000000 iboxstacksops-0.7.2/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.2/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10003 2023-03-22 10:22:38.000000 iboxstacksops-0.7.2/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.2/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.2/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.2/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.2/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.2/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2081 2021-10-28 09:48:26.000000 iboxstacksops-0.7.2/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.2/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.2/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.2/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-04-11 14:49:46.000000 iboxstacksops-0.7.2/setup.py
```

### Comparing `iboxstacksops-0.7.1/PKG-INFO` & `iboxstacksops-0.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.1
+Version: 0.7.2
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.1
+Version: 0.7.2
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.1/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/actions.py` & `iboxstacksops-0.7.2/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/aws.py` & `iboxstacksops-0.7.2/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/cfg.py` & `iboxstacksops-0.7.2/iboxstacksops/cfg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/changeset.py` & `iboxstacksops-0.7.2/iboxstacksops/changeset.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/commands.py` & `iboxstacksops-0.7.2/iboxstacksops/commands.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/common.py` & `iboxstacksops-0.7.2/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/dashboard.py` & `iboxstacksops-0.7.2/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/events.py` & `iboxstacksops-0.7.2/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/i_region.py` & `iboxstacksops-0.7.2/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/i_stack.py` & `iboxstacksops-0.7.2/iboxstacksops/i_stack.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/msg.py` & `iboxstacksops-0.7.2/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/outputs.py` & `iboxstacksops-0.7.2/iboxstacksops/outputs.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/parameters.py` & `iboxstacksops-0.7.2/iboxstacksops/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,17 @@
         usage="Allowed Stack Params ... allowed values are in {}",
         formatter_class=argparse.RawTextHelpFormatter,
     )
 
     # for parameter in sorted(
     #    stack_parameters, key=lambda x: x['ParameterKey']):
     for p in sorted(istack.parameters):
+        # skip intrinsic cmd parameters already parsed
+        if hasattr(istack.cfg.cmd_args, p):
+            continue
         v = istack.parameters[p]
         allowed_values = v["AllowedValues"] if "AllowedValues" in v else []
         kwargs = {"type": str, "metavar": "\t%s" % v["Description"]}
 
         # If Parameter do not have Default value and is new or
         # current value is not allowed in new template,
         # enforce it as required
```

### Comparing `iboxstacksops-0.7.1/iboxstacksops/parser.py` & `iboxstacksops-0.7.2/iboxstacksops/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,8 +636,9 @@
     if cfg.all_stacks and not (cfg.stack or cfg.role or cfg.type):
         cfg.type = ["ALL"]
 
     if not cfg.no_stacks and not (cfg.stack or cfg.role or cfg.type):
         parser.print_help()
         exit(0)
 
+    cfg.cmd_args = args[0]
     cfg.stack_args = args[1]
```

### Comparing `iboxstacksops-0.7.1/iboxstacksops/replica.py` & `iboxstacksops-0.7.2/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/resolve.py` & `iboxstacksops-0.7.2/iboxstacksops/resolve.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/resources.py` & `iboxstacksops-0.7.2/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/route53.py` & `iboxstacksops-0.7.2/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/ssm.py` & `iboxstacksops-0.7.2/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/stacks.py` & `iboxstacksops-0.7.2/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/table.py` & `iboxstacksops-0.7.2/iboxstacksops/table.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/tags.py` & `iboxstacksops-0.7.2/iboxstacksops/tags.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/template.py` & `iboxstacksops-0.7.2/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/iboxstacksops/tools.py` & `iboxstacksops-0.7.2/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.1/setup.py` & `iboxstacksops-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.1",
+    version="0.7.2",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

