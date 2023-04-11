# Comparing `tmp/sog-devops-client-1.0.0.tar.gz` & `tmp/sog-devops-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sog-devops-client-1.0.0.tar", last modified: Thu Apr  6 09:17:26 2023, max compression
+gzip compressed data, was "sog-devops-client-1.0.1.tar", last modified: Tue Apr 11 05:53:26 2023, max compression
```

## Comparing `sog-devops-client-1.0.0.tar` & `sog-devops-client-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 09:17:26.463725 sog-devops-client-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-03-31 09:21:16.000000 sog-devops-client-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1544 2023-04-06 09:17:26.462723 sog-devops-client-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-04-06 07:46:50.000000 sog-devops-client-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 09:17:26.450723 sog-devops-client-1.0.0/generate/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:52:03.000000 sog-devops-client-1.0.0/generate/__init__.py
--rw-rw-rw-   0        0        0     3812 2023-04-06 08:39:49.000000 sog-devops-client-1.0.0/generate/generate.py
--rw-rw-rw-   0        0        0       88 2023-03-31 09:06:53.000000 sog-devops-client-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 09:17:26.463725 sog-devops-client-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-04-06 09:17:15.000000 sog-devops-client-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:17:26.461723 sog-devops-client-1.0.0/sog_devops_client.egg-info/
--rw-rw-rw-   0        0        0     1544 2023-04-06 09:17:26.000000 sog-devops-client-1.0.0/sog_devops_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-06 09:17:26.000000 sog-devops-client-1.0.0/sog_devops_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 09:17:26.000000 sog-devops-client-1.0.0/sog_devops_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-06 09:17:26.000000 sog-devops-client-1.0.0/sog_devops_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 09:17:26.000000 sog-devops-client-1.0.0/sog_devops_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 09:17:26.462723 sog-devops-client-1.0.0/test/
--rw-rw-rw-   0        0        0      987 2023-04-06 08:44:57.000000 sog-devops-client-1.0.0/test/test_generate.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:53:26.972518 sog-devops-client-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-03-31 09:21:16.000000 sog-devops-client-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1649 2023-04-11 05:53:26.972518 sog-devops-client-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-04-11 05:53:18.000000 sog-devops-client-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:53:26.958516 sog-devops-client-1.0.1/generate/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:52:03.000000 sog-devops-client-1.0.1/generate/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-04-11 05:50:38.000000 sog-devops-client-1.0.1/generate/generate_config.py
+-rw-rw-rw-   0        0        0       88 2023-03-31 09:06:53.000000 sog-devops-client-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:53:26.972518 sog-devops-client-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-04-11 02:38:01.000000 sog-devops-client-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:53:26.970516 sog-devops-client-1.0.1/sog_devops_client.egg-info/
+-rw-rw-rw-   0        0        0     1649 2023-04-11 05:53:26.000000 sog-devops-client-1.0.1/sog_devops_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-11 05:53:26.000000 sog-devops-client-1.0.1/sog_devops_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:53:26.000000 sog-devops-client-1.0.1/sog_devops_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-11 05:53:26.000000 sog-devops-client-1.0.1/sog_devops_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 05:53:26.000000 sog-devops-client-1.0.1/sog_devops_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 05:53:26.971517 sog-devops-client-1.0.1/test/
+-rw-rw-rw-   0        0        0      987 2023-04-11 05:51:02.000000 sog-devops-client-1.0.1/test/test_generate.py
```

### Comparing `sog-devops-client-1.0.0/LICENSE` & `sog-devops-client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sog-devops-client-1.0.0/PKG-INFO` & `sog-devops-client-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sog-devops-client
-Version: 1.0.0
+Version: 1.0.1
 Author: v-yangchao
 Author-email: v-yangchao@sinooceangroup.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -13,14 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # 简介
 海鸥Ⅱ根据模板生成配置文件
+
 # 工具准备
 ## 安装打包工具
 ```
  python -m pip install --user --upgrade setuptools wheel
  ```
 ## 安装上传工具
 ```
@@ -56,7 +57,16 @@
 ```
 pip install seagull2_generate_config_template
 ```
 # 更新
 ````
 pip install -U seagull2_generate_config_template  
 ````
+# 项目版本更新记录
+
+1.0.1
+
+* 调整模块名称
+
+1.0.0
+
+* 配置文件模板化封装
```

### Comparing `sog-devops-client-1.0.0/README.md` & `sog-devops-client-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # 简介
 海鸥Ⅱ根据模板生成配置文件
+
 # 工具准备
 ## 安装打包工具
 ```
  python -m pip install --user --upgrade setuptools wheel
  ```
 ## 安装上传工具
 ```
@@ -40,7 +41,16 @@
 ```
 pip install seagull2_generate_config_template
 ```
 # 更新
 ````
 pip install -U seagull2_generate_config_template  
 ````
+# 项目版本更新记录
+
+1.0.1
+
+* 调整模块名称
+
+1.0.0
+
+* 配置文件模板化封装
```

### Comparing `sog-devops-client-1.0.0/generate/generate.py` & `sog-devops-client-1.0.1/generate/generate_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     else:
         raise Exception(response)
     return
 
 # 生成配置
 
 
-def generate_config(user, env, token, publish, synApollo,  generateConfigUrl, apolloUrl, configTemplates, request_data):
+def generate(user, env, token, publish, synApollo,  generateConfigUrl, apolloUrl, configTemplates, request_data):
     host = ''
     if env == 'DEV':
         host = 'https://workflow-dev.sinoocean-test.com'
     elif env == 'FAT':
         host = 'https://workflow.sinoocean-test.com'
     elif env == 'UAT':
         host = 'https://workflow.sinoocean-uat.com'
```

### Comparing `sog-devops-client-1.0.0/setup.py` & `sog-devops-client-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = "sog-devops-client",
-	version = '1.0.0',
+	version = '1.0.1',
   author ="v-yangchao",
   author_email = "v-yangchao@sinooceangroup.com",
   long_description_content_type="text/markdown",
 	long_description = open('README.md',encoding="utf-8").read(),
   python_requires=">=3.6",
   install_requires=['requests>=2.26.0', 'tenacity>=8.2.1'],
 	packages = find_packages(),
```

### Comparing `sog-devops-client-1.0.0/sog_devops_client.egg-info/PKG-INFO` & `sog-devops-client-1.0.1/sog_devops_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sog-devops-client
-Version: 1.0.0
+Version: 1.0.1
 Author: v-yangchao
 Author-email: v-yangchao@sinooceangroup.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -13,14 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # 简介
 海鸥Ⅱ根据模板生成配置文件
+
 # 工具准备
 ## 安装打包工具
 ```
  python -m pip install --user --upgrade setuptools wheel
  ```
 ## 安装上传工具
 ```
@@ -56,7 +57,16 @@
 ```
 pip install seagull2_generate_config_template
 ```
 # 更新
 ````
 pip install -U seagull2_generate_config_template  
 ````
+# 项目版本更新记录
+
+1.0.1
+
+* 调整模块名称
+
+1.0.0
+
+* 配置文件模板化封装
```

### Comparing `sog-devops-client-1.0.0/test/test_generate.py` & `sog-devops-client-1.0.1/test/test_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from generate_config import generate
+from generate import generate_config
 
 # 构建参数
 request_data = {
     'publicAppId': 'WebApi',  # 公共应用appid
     'appId': 'TestAPI'  # 当前应用id
 }
 config_result = 'config_result.txt'
@@ -12,15 +12,15 @@
 
 
 class TestGenerate(unittest.TestCase):
 
     def test_generate(self):
         config_result_path = "./%s" % config_result
         try:
-            generate.generate_config('apollo', 'DEV', '', False,
+            generate_config.generate('apollo', 'DEV', '', False,
                                      False, '', '', configTemplates, request_data)
             file_object = open(config_result_path, encoding='utf-8')
             all_the_text = file_object.read()  # 结果为str类型
             print(all_the_text)
             file_object.close()
             self.assertEqual(all_the_text, '我是"Development"环境')
         finally:
```

