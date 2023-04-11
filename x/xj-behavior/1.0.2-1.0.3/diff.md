# Comparing `tmp/xj_behavior-1.0.2.tar.gz` & `tmp/xj_behavior-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_behavior-1.0.2.tar", last modified: Tue Mar 28 01:52:34 2023, max compression
+gzip compressed data, was "dist\xj_behavior-1.0.3.tar", last modified: Tue Apr 11 11:40:16 2023, max compression
```

## Comparing `xj_behavior-1.0.2.tar` & `xj_behavior-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/
--rw-rw-rw-   0        0        0     1440 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-03-28 01:52:26.000000 xj_behavior-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior/
--rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.2/xj_behavior/__init__.py
--rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.2/xj_behavior/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/apis/__init__.py
--rw-rw-rw-   0        0        0      682 2023-03-24 02:42:43.000000 xj_behavior-1.0.2/xj_behavior/apis/standing_book_apis.py
--rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.2/xj_behavior/apps.py
--rw-rw-rw-   0        0        0       32 2023-03-24 00:42:51.000000 xj_behavior-1.0.2/xj_behavior/models.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/services/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-03-28 01:51:46.000000 xj_behavior-1.0.2/xj_behavior/services/standing_book_services.py
--rw-rw-rw-   0        0        0      233 2023-03-24 02:10:22.000000 xj_behavior-1.0.2/xj_behavior/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/utils/custom_response.py
--rw-rw-rw-   0        0        0     7806 2022-10-31 08:53:23.000000 xj_behavior-1.0.2/xj_behavior/utils/custom_tool.py
--rw-rw-rw-   0        0        0      958 2022-10-25 06:03:08.000000 xj_behavior-1.0.2/xj_behavior/utils/j_dict.py
--rw-rw-rw-   0        0        0     8365 2022-10-17 06:55:25.000000 xj_behavior-1.0.2/xj_behavior/utils/j_recur.py
--rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/utils/join_list.py
--rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.2/xj_behavior/utils/model_handle.py
--rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_behavior-1.0.2/xj_behavior/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior.egg-info/
--rw-rw-rw-   0        0        0     1440 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-28 01:52:34.000000 xj_behavior-1.0.2/xj_behavior.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:16.000000 xj_behavior-1.0.3/
+-rw-rw-rw-   0        0        0     1440 2023-04-11 11:40:16.000000 xj_behavior-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 11:40:16.000000 xj_behavior-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-04-11 11:40:09.000000 xj_behavior-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior/
+-rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.3/xj_behavior/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.3/xj_behavior/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/apis/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-03-28 03:17:01.000000 xj_behavior-1.0.3/xj_behavior/apis/standing_book_apis.py
+-rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.3/xj_behavior/apps.py
+-rw-rw-rw-   0        0        0       32 2023-03-24 00:42:51.000000 xj_behavior-1.0.3/xj_behavior/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:16.000000 xj_behavior-1.0.3/xj_behavior/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/services/__init__.py
+-rw-rw-rw-   0        0        0     3783 2023-04-11 11:39:58.000000 xj_behavior-1.0.3/xj_behavior/services/standing_book_services.py
+-rw-rw-rw-   0        0        0      233 2023-03-24 02:10:22.000000 xj_behavior-1.0.3/xj_behavior/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:16.000000 xj_behavior-1.0.3/xj_behavior/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/utils/custom_response.py
+-rw-rw-rw-   0        0        0     7806 2022-10-31 08:53:23.000000 xj_behavior-1.0.3/xj_behavior/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      958 2022-10-25 06:03:08.000000 xj_behavior-1.0.3/xj_behavior/utils/j_dict.py
+-rw-rw-rw-   0        0        0     8365 2022-10-17 06:55:25.000000 xj_behavior-1.0.3/xj_behavior/utils/j_recur.py
+-rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/utils/join_list.py
+-rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.3/xj_behavior/utils/model_handle.py
+-rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_behavior-1.0.3/xj_behavior/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior.egg-info/
+-rw-rw-rw-   0        0        0     1440 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 11:40:15.000000 xj_behavior-1.0.3/xj_behavior.egg-info/top_level.txt
```

### Comparing `xj_behavior-1.0.2/PKG-INFO` & `xj_behavior-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_behavior
-Version: 1.0.2
+Version: 1.0.3
 Summary: 行为模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj-behavior
         
         #### 介绍
         行为模块
```

### Comparing `xj_behavior-1.0.2/README.md` & `xj_behavior-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/setup.py` & `xj_behavior-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_behavior',  # 模块名称
-    version='1.0.2',  # 模块版本
+    version='1.0.3',  # 模块版本
     description='行为模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     license="apache 3.0",
     install_requires=[]
 )
```

### Comparing `xj_behavior-1.0.2/xj_behavior/apis/standing_book_apis.py` & `xj_behavior-1.0.3/xj_behavior/apis/standing_book_apis.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/services/standing_book_services.py` & `xj_behavior-1.0.3/xj_behavior/services/standing_book_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,29 +38,30 @@
         enroll_record_list, err = EnrollRecordServices.record_list(params={"enroll_id_list": enroll_id_list}, need_pagination=False)
         enroll_record_map = {}
         for i in enroll_record_list:
             if enroll_record_map.get(i["enroll"]):
                 enroll_record_map[i["enroll"]].append(i["user_info"].get("full_name", "该用户不存在"))
             else:
                 enroll_record_map[i["enroll"]] = [i["user_info"].get("full_name", "该用户不存在")]
+
         current_index = (page - 1) * size
         # 获取发票相关的信息
         for item in enroll_list:
             # 添加
             group_names_str = ""
-            for i in group_names.get(item["user_id"], []):
+            for i in group_names.get(item.get("user_id", ""), []):
                 group_names_str = group_names_str + ("," if len(group_names_str) > 0 else "") + i["group_name"]
             item["group_name"] = "游客" if not group_names_str else group_names_str  # 分组字符串
 
             current_index += 1
             item["index"] = current_index  # 序号
-            item["beneficiary"] = beneficiary_user_map.get(item["user_id"], "非业务人员邀请用户")  # 邀请用户
-            item["total"] = item["count"] * item["price"]  # 小计
-            item["beneficiary_amount"] = float(item["amount"]) * 0.6  # 业务员提成
-            item["urge_free"] = 50 if isinstance(item["is_urgent"], str) and int(item["is_urgent"]) else 0  # 加急费用
+            item["beneficiary"] = beneficiary_user_map.get(item.get("user_id"), "非业务人员邀请用户")  # 邀请用户
+            item["total"] = item.get("count", 0) * item.get("price", 0)  # 小计
+            item["beneficiary_amount"] = float(item.get("amount", 0)) * 0.6  # 业务员提成
+            item["urge_free"] = 50 if isinstance(item.get("is_urgent", None), str) and int(item["is_urgent"]) else 0  # 加急费用
             item["other_money"] = '-'  # 其他款项
 
             enroll_user_name_str = ""
             for i in enroll_record_map.get(item["id"], []):
                 enroll_user_name_str = enroll_user_name_str + ("," if len(enroll_user_name_str) > 0 else "") + i
             item["enroll_user_names"] = enroll_user_name_str  # 报名名称
```

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/custom_authorization.py` & `xj_behavior-1.0.3/xj_behavior/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/custom_response.py` & `xj_behavior-1.0.3/xj_behavior/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/custom_tool.py` & `xj_behavior-1.0.3/xj_behavior/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/j_dict.py` & `xj_behavior-1.0.3/xj_behavior/utils/j_dict.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/j_recur.py` & `xj_behavior-1.0.3/xj_behavior/utils/j_recur.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/model_handle.py` & `xj_behavior-1.0.3/xj_behavior/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior/utils/validator.py` & `xj_behavior-1.0.3/xj_behavior/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.2/xj_behavior.egg-info/PKG-INFO` & `xj_behavior-1.0.3/xj_behavior.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-behavior
-Version: 1.0.2
+Version: 1.0.3
 Summary: 行为模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj-behavior
         
         #### 介绍
         行为模块
```

### Comparing `xj_behavior-1.0.2/xj_behavior.egg-info/SOURCES.txt` & `xj_behavior-1.0.3/xj_behavior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

