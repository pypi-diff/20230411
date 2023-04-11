# Comparing `tmp/spark_quality_rules_tools-0.2.2.tar.gz` & `tmp/spark_quality_rules_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.2.tar", last modified: Fri Apr  7 23:30:08 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.2.4.tar", last modified: Tue Apr 11 12:29:06 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.2.tar` & `spark_quality_rules_tools-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.014212 spark_quality_rules_tools-0.2.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      155 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4481 2023-04-07 23:30:08.014212 spark_quality_rules_tools-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3672 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-07 23:30:08.015210 spark_quality_rules_tools-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-04-07 23:29:06.000000 spark_quality_rules_tools-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.934192 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2263 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.963199 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    31605 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.994205 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      216 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2472 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.999207 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/
--rw-rw-rw-   0        0        0    71803 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/folder_process.png
--rw-rw-rw-   0        0        0     1056 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/memory.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.008208 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    17801 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     2894 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.013210 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/table.html
-drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.955196 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4481 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      155 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3846 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-04-08 05:49:00.000000 spark_quality_rules_tools-0.2.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-04-11 12:19:40.000000 spark_quality_rules_tools-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.966518 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     1728 2023-04-10 14:18:27.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    19489 2023-04-08 05:39:17.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      216 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2472 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/
+-rw-rw-rw-   0        0        0    71803 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/folder_process.png
+-rw-rw-rw-   0        0        0     1056 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/memory.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    16245 2023-04-10 23:11:39.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     2475 2023-04-11 12:15:42.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/table.html
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.966518 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     3846 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.2/LICENSE` & `spark_quality_rules_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/PKG-INFO` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: spark_quality_rules_tools
-Version: 0.2.2
+Name: spark-quality-rules-tools
+Version: 0.2.4
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 Keywords: spark,dq,rules,hammurabies
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spark_quality_rules_tools
 
 [![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
@@ -36,89 +35,75 @@
 
 ## Usage
 
 wrapper run hammurabies
 
 ![Process](./spark_quality_rules_tools/utils/external/folder_process.png)
 
-## Local
+
+## Sandbox
 
 ```sh
 import os
-from spark_quality_rules_tools import get_quality_run_repo_local
-
-## add user register
-os.environ['JPY_USER'] = 'PXXXXX'
-
-project_sda="CDD"
-repo_urls= ["ssh://git@globaldevtools.bbva.com:7999/vbsuu/vbsuu_skynet_products_services_administration.git",
-            "ssh://git@globaldevtools.bbva.com:7999/vbsuu/vbsuu_skynet_xdkq.git",
-            "ssh://git@globaldevtools.bbva.com:7999/vbsuu/vbsuu_skynet_risk.git"]
-            
-## quality run_sandbox
-get_quality_run_repo_local(project_sda=project_sda,
-                           repo_urls=repo_urls)
 
-```
+from spark_quality_rules_tools.functions.generator import dq_path_workspace
+from spark_quality_rules_tools.functions.generator import dq_download_jar
+from spark_quality_rules_tools.functions.generator import dq_extract_parameters
+from spark_quality_rules_tools.functions.generator import dq_run_sandbox
+from spark_quality_rules_tools.functions.generator import dq_spark_session
+from spark_quality_rules_tools.functions.generator import dq_validate_conf
+from spark_quality_rules_tools.functions.generator import dq_validate_rules
 
-## Sandbox
+project_sda="SDA_37036"
+url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
 
-```sh
-import os
-from spark_quality_rules_tools import get_path_workspace
-from spark_quality_rules_tools import get_creating_directory_txt_file_empty
-from spark_quality_rules_tools import quality_rules_get_conf_parameter
-from spark_quality_rules_tools import get_quality_run_sandbox
-
-project_sda="CDD"
-uuaa_name = "ksan"
-table_name = "eomassetsliabilities"
-conf_name = "eomassetsliabilities-01"
 
 ## Create workspace
-get_path_workspace(project_sda=project_sda)
+dq_path_workspace(project_sda=project_sda)
 
-## Create file conf local
-get_creating_directory_txt_file_empty(uuaa_name=uuaa_name,
-                                      table_name=table_name,
-                                      confs_list=[conf_name])
-                                      
+## Download Jar Haas
+dq_download_jar(haas_version="4.8.0",
+                force=False)
+                                                      
 ## Extract y Show Parameter                                 
-quality_rules_get_conf_parameter(uuaa_name=uuaa_name,
-                                 table_name=table_name,
-                                 confs_list=[conf_name])
+dq_extract_parameters(url_conf=url_conf)
+
 
 parameter_conf_list = [
- {
-   "ENTIFIC_ID": "PE",
-   "INFORMATION_ORIGIN_ID": "SKCO",
-   "SCHEMAS_REPOSITORY": "da-datio/schemas/pe/kgug/master/t_kgug_guarantees/latest/",
-   "LAST_CUTOFF_DATE": "2022-05-31",
-   "ODATE_DATE": "2022-06-30",
-   "SCHEMA_PATH": "t_ksan_eom_assets_liabilities.output.schema",
-   "CUTOFF_DATE": "2022-06-30",
-   "ARTIFACTORY_UNIQUE_CACHE": "https://globaldevtools.bbva.com"
+ {      
+    "ARTIFACTORY_UNIQUE_CACHE": "https://globaldevtools.bbva.com",
+    "ODATE_DATE": "2022-11-11",
+    "COUNTRY_ID": "PE",
+    "SCHEMA_PATH": "t_kcog_branch.output.schema",
+    "CUTOFF_DATE": "2022-11-11",
+    "SCHEMAS_REPOSITORY": "da-datio/schemas/pe/kcog/master/t_kcog_branch/latest/"
  }
 ]
-
-                         
+                  
 ## quality run_sandbox
-get_quality_run_sandbox(project_sda=project_sda,
-                        spark=spark,
-                        sc=sc,
-                        uuaa_name=uuaa_name,
-                        table_name=table_name,
-                        conf_name=conf_name,
-                        parameter_conf_list=parameter_conf_list,
-                        is_download_jar=True,
-                        jar_url=None,
-                        is_report_compress=False)
+dq_run_sandbox(parameter_conf_list=parameter_conf_list,
+               url_conf=url_conf))
+
+```
+
+## Validations
+
+```sh
+url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
+
+## validate conf
+dq_validate_conf(url_conf=url_conf)
+
+## validate rules
+dq_validate_rules(url_conf=url_conf)
 
 ```
 
+
+
 ## License
 
 [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
 
 ## New features v1.0
 
 ## BugFix
```

### Comparing `spark_quality_rules_tools-0.2.2/setup.py` & `spark_quality_rules_tools-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 from distutils.core import setup
+
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.2',
+    version='0.2.4',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
@@ -21,11 +22,10 @@
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
     ],
 )
```

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/dataframe.py` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/folder_process.png` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/folder_process.png`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/memory.py` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/rules.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,67 +5,60 @@
 
 
 def get_validate_rules(hocons_dir=None):
     import os
     import sys
     import json
     from spark_quality_rules_tools.utils import BASE_DIR
-    from spark_quality_rules_tools.utils.color import get_color, get_color_b
     from pyhocon.converter import HOCONConverter
     from pyhocon import ConfigFactory
     from prettytable import PrettyTable
 
     is_windows = sys.platform.startswith('win')
-    dir_resource_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
+    dir_default_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
+    file_conf = hocons_dir
 
     if hocons_dir in ("", None):
         raise Exception(f'required variable hocons_dir')
 
     if is_windows:
-        dir_resource_rules = dir_resource_rules.replace("\\", "/")
-        hocons_dir = hocons_dir.replace("\\", "/")
+        dir_default_rules = dir_default_rules.replace("\\", "/")
+        file_conf = file_conf.replace("\\", "/")
 
-    with open(dir_resource_rules) as f:
-        parameter_conf = json.load(f)
+    with open(dir_default_rules) as f:
+        default_rules = json.load(f)
 
-    validate_rules_properties_columns = parameter_conf["rules_common_properties"][0]["rules_columns"]
-    validate_rules_properties_datatype = parameter_conf["rules_common_properties"][0]["rules_datatype"]
-    validate_rules_config = parameter_conf["rules_config"]
-
-    dir_confs_filename_parameters2 = hocons_dir
-    conf = ConfigFactory.parse_file(dir_confs_filename_parameters2)
-    res = HOCONConverter.to_json(conf)
-    res = json.loads(res)
-    rules = res["hammurabi"]["rules"]
-
-    for k in rules:
-        hocons_rules = str(k["class"])
-        hocons_config = k["config"]
-        hocons_rules_type = str(hocons_rules).split(".")[4]
-        hocons_rules_class = str(hocons_rules).split(".")[5]
-
-        validate_rules_class = validate_rules_config[hocons_rules_type][hocons_rules_class]
-        validate_rules_version = validate_rules_class[0]["rules_version"]
-        validate_rules_columns = validate_rules_class[0]["rules_columns"]
-        validate_rules_datatype = validate_rules_class[0]["rules_datatype"]
+    file_conf = ConfigFactory.parse_file(file_conf)
+    file_conf = HOCONConverter.to_json(file_conf)
+    file_conf = json.loads(file_conf)
+    haas_rules = file_conf["hammurabi"]["rules"]
+
+    rules_default_properties = default_rules["rules_common_properties"][0]
+
+    for haas_rule in haas_rules:
+        haas_class = str(haas_rule["class"])
+        haas_columns = haas_rule["config"]
+        haas_rules_type = str(haas_class).split(".")[4]
+        haas_rules_class = str(haas_class).split(".")[5]
+
+        rules_version = default_rules["rules_config"][haas_rules_type][haas_rules_class][0]["rules_version"]
+        rules_columns = default_rules["rules_config"][haas_rules_type][haas_rules_class][0]["rules_columns"][0]
+        rules_columns_all = {**rules_columns, **rules_default_properties}
 
-        validate_total_columns = validate_rules_properties_columns + validate_rules_columns
-        validate_total_datatype = dict(**validate_rules_properties_datatype, **validate_rules_datatype)
-
-        print("type=>", hocons_rules_type, "class=>", hocons_rules_class, "version=>", validate_rules_version)
+        print("type=>", haas_rules_type, "class=>", haas_rules_class, "version=>", rules_version)
 
         t = PrettyTable()
-        t.field_names = [f"Variable", "Dtype Actual", "Dtype Esperado", "Es correcto"]
+        t.field_names = [f"Variable", "Value", "Dtype Actual", "Dtype Esperado", "Es Obligatorio"]
 
-        if 'id' not in hocons_config.keys():
+        if 'id' not in haas_columns.keys():
             print("variable id: no existe")
         else:
-            print("variable id:", hocons_config["id"])
+            print("variable id:", haas_columns["id"])
 
-        for k, v in hocons_config.items():
-            if not str(k) in validate_total_columns:
-                t.add_row([k, str(type(k)), "Error", "NO"])
-
-        for k, v in hocons_config.items():
-            if str(k) in validate_total_columns:
-                t.add_row([k, str(type(k)), validate_total_datatype[k], "YES"])
+        for col, value in haas_columns.items():
+            if not str(col) in rules_columns_all.keys():
+                t.add_row([col, value, str(type(col)), "Deprecado", "false"])
+
+        for col, value in haas_columns.items():
+            if str(col) in rules_columns_all.keys():
+                t.add_row([col, value, str(type(value)), rules_columns_all[col][0], rules_columns_all[col][1]])
         print(t)
```

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/table.html` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

