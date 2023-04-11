# Comparing `tmp/ami-val-0.2.4.tar.gz` & `tmp/ami-val-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ami-val-0.2.4.tar", last modified: Mon Mar 27 14:00:19 2023, max compression
+gzip compressed data, was "dist/ami-val-0.2.5.tar", last modified: Tue Apr 11 07:12:41 2023, max compression
```

## Comparing `ami-val-0.2.4.tar` & `ami-val-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-03-27 14:00:19.000000 ami-val-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-03-27 14:00:15.000000 ami-val-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/ami_val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/cfg/ami-val.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/libs/aws_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/libs/resource_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    39009 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/libs/utils_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/scripts/rhel-ha-aws-check.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/templates/sum.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/tests/test_stage0.py
--rw-r--r--   0 runner    (1001) docker     (123)    43399 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/tests/test_stage1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/tests/test_stage2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-03-27 14:00:15.000000 ami-val-0.2.4/ami_val/tests/test_stage3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 14:00:19.000000 ami-val-0.2.4/ami_val.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:00:19.000000 ami-val-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 14:00:15.000000 ami-val-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-11 07:12:41.000000 ami-val-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-11 07:12:24.000000 ami-val-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/ami_val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/cfg/ami-val.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/libs/aws_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/libs/resource_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39009 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/libs/utils_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/scripts/rhel-ha-aws-check.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/templates/sum.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/tests/test_stage0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43399 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/tests/test_stage1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/tests/test_stage2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-11 07:12:24.000000 ami-val-0.2.5/ami_val/tests/test_stage3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 07:12:41.000000 ami-val-0.2.5/ami_val.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:12:41.000000 ami-val-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-11 07:12:24.000000 ami-val-0.2.5/setup.py
```

### Comparing `ami-val-0.2.4/PKG-INFO` & `ami-val-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ami-val
-Version: 0.2.4
+Version: 0.2.5
 Summary: AMI validation tool
 Home-page: https://github.com/liangxiao1/ami-val
 Author: Xiao Liang
 Author-email: xiliang@redhat.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ami-val-0.2.4/README.md` & `ami-val-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/ami_val.py` & `ami-val-0.2.5/ami_val/ami_val.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/cfg/ami-val.yaml` & `ami-val-0.2.5/ami_val/cfg/ami-val.yaml`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/libs/aws_lib.py` & `ami-val-0.2.5/ami_val/libs/aws_lib.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/libs/resource_class.py` & `ami-val-0.2.5/ami_val/libs/resource_class.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/libs/utils_lib.py` & `ami-val-0.2.5/ami_val/libs/utils_lib.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/scripts/rhel-ha-aws-check.sh` & `ami-val-0.2.5/ami_val/scripts/rhel-ha-aws-check.sh`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/templates/sum.html` & `ami-val-0.2.5/ami_val/templates/sum.html`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/tests/test_stage0.py` & `ami-val-0.2.5/ami_val/tests/test_stage0.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/tests/test_stage1.py` & `ami-val-0.2.5/ami_val/tests/test_stage1.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/tests/test_stage2.py` & `ami-val-0.2.5/ami_val/tests/test_stage2.py`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/ami_val/tests/test_stage3.py` & `ami-val-0.2.5/ami_val/tests/test_stage3.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,26 @@
     cmd = "sudo yum repoinfo"
     if is_fedora(test_instance):
         # fedora updates repo Repo-pkgs is 0 maybe because of no updates in developing
         run_cmd(test_instance, cmd, expect_ret=0, timeout=1200, msg='try to get repo info')
     else:
         run_cmd(test_instance, cmd, expect_ret=0, expect_not_kw='Repo-pkgs          : 0', timeout=1200, msg='try to get repo info')
 
+def test_stage3_test_yum_package_install_kernel_debug(test_instance):
+    '''
+    rhbz: 2117700
+    kernel-debug, kernel-debug-devel matching current kernel version are avaiable in repo
+    '''
+    if 'ATOMIC' in test_instance.info['name'].upper():
+        test_instance.skipTest('skip in Atomic AMIs')
+    run_cmd(test_instance, "sudo yum clean all", expect_ret=0, timeout=180)
+    run_cmd(test_instance, "sudo yum repolist", expect_ret=0, timeout=1200)
+    run_cmd(test_instance, "sudo yum -y install install kernel-debug-devel-$(uname -r)", timeout=1200)
+    run_cmd(test_instance, "sudo yum -y install install kernel-debug-$(uname -r)", timeout=1200)
+
 def test_stage3_test_yum_package_install(test_instance):
     if 'ATOMIC' in test_instance.info['name'].upper():
         test_instance.skipTest('skip in Atomic AMIs')
     run_cmd(test_instance, "sudo yum clean all", expect_ret=0, timeout=180)
     run_cmd(test_instance, "sudo yum repolist", expect_ret=0, timeout=1200)
     run_cmd(test_instance, "sudo yum check-update", timeout=1200)
     run_cmd(test_instance, "sudo yum search zsh", expect_ret=0, timeout=180)
```

### Comparing `ami-val-0.2.4/ami_val.egg-info/PKG-INFO` & `ami-val-0.2.5/ami_val.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ami-val
-Version: 0.2.4
+Version: 0.2.5
 Summary: AMI validation tool
 Home-page: https://github.com/liangxiao1/ami-val
 Author: Xiao Liang
 Author-email: xiliang@redhat.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ami-val-0.2.4/ami_val.egg-info/SOURCES.txt` & `ami-val-0.2.5/ami_val.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ami-val-0.2.4/setup.py` & `ami-val-0.2.5/setup.py`

 * *Files identical despite different names*

