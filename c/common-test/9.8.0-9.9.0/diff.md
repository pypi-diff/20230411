# Comparing `tmp/common-test-9.8.0.tar.gz` & `tmp/common-test-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-9.8.0.tar", last modified: Wed Apr 13 09:57:34 2022, max compression
+gzip compressed data, was "common-test-9.9.0.tar", last modified: Wed Apr 13 10:01:14 2022, max compression
```

## Comparing `common-test-9.8.0.tar` & `common-test-9.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.422422 common-test-9.8.0/
--rw-r--r--   0 edz        (502) staff       (20)      156 2022-04-13 09:57:34.422546 common-test-9.8.0/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.407863 common-test-9.8.0/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:20.000000 common-test-9.8.0/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.409101 common-test-9.8.0/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:14.000000 common-test-9.8.0/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8761 2022-04-13 05:20:34.000000 common-test-9.8.0/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     1071 2022-04-12 07:36:43.000000 common-test-9.8.0/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)     3106 2022-04-13 03:32:12.000000 common-test-9.8.0/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.409667 common-test-9.8.0/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:39.000000 common-test-9.8.0/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7264 2022-04-12 12:44:23.000000 common-test-9.8.0/common/common/constant.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.410241 common-test-9.8.0/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.8.0/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2246 2022-04-12 12:14:49.000000 common-test-9.8.0/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.411343 common-test-9.8.0/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:37.000000 common-test-9.8.0/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     6511 2022-04-13 09:57:28.000000 common-test-9.8.0/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     5301 2022-04-13 05:20:34.000000 common-test-9.8.0/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.412325 common-test-9.8.0/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.8.0/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1751 2022-04-13 04:04:56.000000 common-test-9.8.0/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1305 2022-03-29 02:29:55.000000 common-test-9.8.0/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.415288 common-test-9.8.0/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4142 2022-04-07 05:49:45.000000 common-test-9.8.0/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:53.000000 common-test-9.8.0/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8140 2022-04-12 05:17:09.000000 common-test-9.8.0/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2128 2022-04-08 03:50:05.000000 common-test-9.8.0/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1630 2022-03-31 16:11:39.000000 common-test-9.8.0/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2158 2022-03-30 16:43:46.000000 common-test-9.8.0/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1026 2022-03-31 12:53:48.000000 common-test-9.8.0/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.415897 common-test-9.8.0/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.8.0/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2898 2022-03-29 02:29:55.000000 common-test-9.8.0/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.419616 common-test-9.8.0/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:42.000000 common-test-9.8.0/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)        1 2022-04-08 03:29:33.000000 common-test-9.8.0/common/plugin/common_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     3660 2022-04-13 09:50:31.000000 common-test-9.8.0/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     2336 2022-04-12 07:41:05.000000 common-test-9.8.0/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     4297 2022-04-13 04:19:31.000000 common-test-9.8.0/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:18.000000 common-test-9.8.0/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     4114 2022-04-12 12:42:58.000000 common-test-9.8.0/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 09:57:34.421821 common-test-9.8.0/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      156 2022-04-13 09:57:34.000000 common-test-9.8.0/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1035 2022-04-13 09:57:34.000000 common-test-9.8.0/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2022-04-13 09:57:34.000000 common-test-9.8.0/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)      261 2022-04-13 09:57:34.000000 common-test-9.8.0/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2022-04-13 09:57:34.000000 common-test-9.8.0/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      431 2022-04-13 09:57:34.423170 common-test-9.8.0/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)       69 2022-03-29 04:37:04.000000 common-test-9.8.0/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.465441 common-test-9.9.0/
+-rw-r--r--   0 edz        (502) staff       (20)      156 2022-04-13 10:01:14.465547 common-test-9.9.0/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.453973 common-test-9.9.0/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:20.000000 common-test-9.9.0/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.454999 common-test-9.9.0/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:14.000000 common-test-9.9.0/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8761 2022-04-13 05:20:34.000000 common-test-9.9.0/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     1071 2022-04-12 07:36:43.000000 common-test-9.9.0/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)     3106 2022-04-13 03:32:12.000000 common-test-9.9.0/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.455609 common-test-9.9.0/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:39.000000 common-test-9.9.0/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7264 2022-04-12 12:44:23.000000 common-test-9.9.0/common/common/constant.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.456128 common-test-9.9.0/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.9.0/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2246 2022-04-12 12:14:49.000000 common-test-9.9.0/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.457045 common-test-9.9.0/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:37.000000 common-test-9.9.0/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     6541 2022-04-13 10:00:10.000000 common-test-9.9.0/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     5301 2022-04-13 05:20:34.000000 common-test-9.9.0/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.458044 common-test-9.9.0/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.9.0/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1751 2022-04-13 04:04:56.000000 common-test-9.9.0/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1305 2022-03-29 02:29:55.000000 common-test-9.9.0/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.460539 common-test-9.9.0/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4142 2022-04-07 05:49:45.000000 common-test-9.9.0/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:53.000000 common-test-9.9.0/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8140 2022-04-12 05:17:09.000000 common-test-9.9.0/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2128 2022-04-08 03:50:05.000000 common-test-9.9.0/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1630 2022-03-31 16:11:39.000000 common-test-9.9.0/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2158 2022-03-30 16:43:46.000000 common-test-9.9.0/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1026 2022-03-31 12:53:48.000000 common-test-9.9.0/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.461196 common-test-9.9.0/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-9.9.0/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2898 2022-03-29 02:29:55.000000 common-test-9.9.0/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.463483 common-test-9.9.0/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:42.000000 common-test-9.9.0/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)        1 2022-04-08 03:29:33.000000 common-test-9.9.0/common/plugin/common_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     3692 2022-04-13 10:00:32.000000 common-test-9.9.0/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     2336 2022-04-12 07:41:05.000000 common-test-9.9.0/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     4297 2022-04-13 04:19:31.000000 common-test-9.9.0/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:18.000000 common-test-9.9.0/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     4114 2022-04-12 12:42:58.000000 common-test-9.9.0/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2022-04-13 10:01:14.465155 common-test-9.9.0/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      156 2022-04-13 10:01:14.000000 common-test-9.9.0/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1035 2022-04-13 10:01:14.000000 common-test-9.9.0/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2022-04-13 10:01:14.000000 common-test-9.9.0/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)      261 2022-04-13 10:01:14.000000 common-test-9.9.0/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2022-04-13 10:01:14.000000 common-test-9.9.0/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      431 2022-04-13 10:01:14.466108 common-test-9.9.0/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)       69 2022-03-29 04:37:04.000000 common-test-9.9.0/setup.py
```

### Comparing `common-test-9.8.0/common/autotest/base_requests.py` & `common-test-9.9.0/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/autotest/handle_allure.py` & `common-test-9.9.0/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/autotest/handle_assert.py` & `common-test-9.9.0/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/common/constant.py` & `common-test-9.9.0/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/config/config.py` & `common-test-9.9.0/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/data/data_process.py` & `common-test-9.9.0/common/data/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,27 +88,27 @@
     @classmethod
     def handle_data_fromat(cls, _template, data=None):
         if isinstance(_template, str):
             if isinstance(data, list):
                 _dict = []
                 for _index in range(len(data)):
                     if isinstance(data[_index], dict):
-                        _dict.append(cls.get_data(_template, data[_index]))
+                        _dict.append(cls.handle_data_fromat(_template, data[_index]))
                 return _dict
             else:
                 return req_expr(_template, data)
         else:
             if isinstance(_template, list):
                 for _index in range(len(_template)):
-                    _template[_index] = cls.get_data(_template[_index], data)
+                    _template[_index] = cls.handle_data_fromat(_template[_index], data)
                 return _template
             else:
                 if isinstance(_template, dict):
                     for key in _template.keys():
-                        _template[key] = cls.get_data(_template[key], data)
+                        _template[key] = cls.handle_data_fromat(_template[key], data)
                 return _template
 
     @classmethod
     def handle_data(cls, variable: str, jsonformat:bool=True) -> dict:
         """请求数据处理
         :param variable: 请求数据，传入的是可转换字典/json的字符串,其中可以包含变量表达式
         return 处理之后的json/dict类型的字典数据
```

### Comparing `common-test-9.8.0/common/data/handle_common.py` & `common-test-9.9.0/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/db/handle_db.py` & `common-test-9.9.0/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/db/handle_sqlserver.py` & `common-test-9.9.0/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/ReadFile.py` & `common-test-9.9.0/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/handle_excel.py` & `common-test-9.9.0/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/handle_file.py` & `common-test-9.9.0/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/handle_reques.py` & `common-test-9.9.0/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/handle_system.py` & `common-test-9.9.0/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/file/handle_yaml.py` & `common-test-9.9.0/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/mq/handle_rabbit.py` & `common-test-9.9.0/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/plugin/data_bus.py` & `common-test-9.9.0/common/plugin/data_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         cls.save_yaml(cls.get_env())
 
 
 if __name__ == '__main__':
     # DataBus.set_key("env","test")
     # DataBus.set_key("test333","3343434")
     DataBus.set_key("JSESSIONID","3333")
-    print(get_yaml_config('$.common.request_headers'))
+    print(DataProcess.handle_data_fromat(get_yaml_config('$.common.request_headers')))
     # print(DataBus.get_data("${aaa}12343434${bb}883434",[{'aaa':'BBBBBB'},{'bb':'BBBBBBB'}])[0])
     # print(DataBus.get_key('test333'))
     # #DataBus.save_init_data()
     # #print(DataBus.get_data("{test333}3333${mysql-data}{test333}@get_current_time()@"))
     # dict=["${test333}","${mysql-data}"]
     # print(DataBus.get_data(dict))
     # # print(eval(DataBus.get_key("mysql-data"))['user'])
```

### Comparing `common-test-9.8.0/common/plugin/data_plugin.py` & `common-test-9.9.0/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/plugin/file_plugin.py` & `common-test-9.9.0/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/plugin/hooks_plugin.py` & `common-test-9.9.0/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common/plugin/pytest_plugin.py` & `common-test-9.9.0/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-9.8.0/common_test.egg-info/SOURCES.txt` & `common-test-9.9.0/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

