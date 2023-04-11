# Comparing `tmp/apitest_ezgo-0.0.5-py2-none-any.whl.zip` & `tmp/apitest_ezgo-0.0.6-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13459 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat     5077 b- defN 23-Feb-22 10:16 apitest_ezgo/Compare.py
--rw-rw-rw-  2.0 fat     9464 b- defN 23-Mar-31 07:29 apitest_ezgo/DbHelper.py
--rw-rw-rw-  2.0 fat     3681 b- defN 23-Mar-09 10:25 apitest_ezgo/FastRequest.py
--rw-rw-rw-  2.0 fat      237 b- defN 23-Mar-31 07:28 apitest_ezgo/__about__.py
+Zip file size: 13955 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat     5235 b- defN 23-Apr-10 07:11 apitest_ezgo/Compare.py
+-rw-rw-rw-  2.0 fat     9947 b- defN 23-Apr-10 06:34 apitest_ezgo/DbHelper.py
+-rw-rw-rw-  2.0 fat     4035 b- defN 23-Apr-10 07:13 apitest_ezgo/FastRequest.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Apr-11 07:29 apitest_ezgo/__about__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Feb-09 11:57 apitest_ezgo/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-16 03:14 apitest_ezgo/Har2Template/__init__.py
--rw-rw-rw-  2.0 fat     1654 b- defN 23-Mar-09 10:31 apitest_ezgo/Har2Template/cli.py
--rw-rw-rw-  2.0 fat      930 b- defN 23-Feb-28 02:01 apitest_ezgo/Har2Template/compat.py
--rw-rw-rw-  2.0 fat     6383 b- defN 23-Mar-01 02:29 apitest_ezgo/Har2Template/core.py
--rw-rw-rw-  2.0 fat     3184 b- defN 23-Mar-09 10:31 apitest_ezgo/Har2Template/utils.py
--rw-rw-rw-  2.0 fat      371 b- defN 23-Mar-31 07:30 apitest_ezgo-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-31 07:30 apitest_ezgo-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       69 b- defN 23-Mar-31 07:30 apitest_ezgo-0.0.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Mar-31 07:30 apitest_ezgo-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1274 b- defN 23-Mar-31 07:30 apitest_ezgo-0.0.5.dist-info/RECORD
-15 files, 32482 bytes uncompressed, 11323 bytes compressed:  65.1%
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-Mar-31 09:43 apitest_ezgo/Har2Template/cli.py
+-rw-rw-rw-  2.0 fat      931 b- defN 23-Mar-31 10:00 apitest_ezgo/Har2Template/compat.py
+-rw-rw-rw-  2.0 fat     6467 b- defN 23-Apr-07 03:11 apitest_ezgo/Har2Template/core.py
+-rw-rw-rw-  2.0 fat     3519 b- defN 23-Apr-07 03:47 apitest_ezgo/Har2Template/utils.py
+-rw-rw-rw-  2.0 fat      371 b- defN 23-Apr-11 07:29 apitest_ezgo-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 07:29 apitest_ezgo-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-11 07:29 apitest_ezgo-0.0.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-11 07:29 apitest_ezgo-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1274 b- defN 23-Apr-11 07:29 apitest_ezgo-0.0.6.dist-info/RECORD
+15 files, 34097 bytes uncompressed, 11819 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: apitest_ezgo/Har2Template/core.py
 Comment: 
 
 Filename: apitest_ezgo/Har2Template/utils.py
 Comment: 
 
-Filename: apitest_ezgo-0.0.5.dist-info/METADATA
+Filename: apitest_ezgo-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: apitest_ezgo-0.0.5.dist-info/WHEEL
+Filename: apitest_ezgo-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: apitest_ezgo-0.0.5.dist-info/entry_points.txt
+Filename: apitest_ezgo-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: apitest_ezgo-0.0.5.dist-info/top_level.txt
+Filename: apitest_ezgo-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: apitest_ezgo-0.0.5.dist-info/RECORD
+Filename: apitest_ezgo-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apitest_ezgo/Compare.py

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 import json
 import logging
 import jsonpath
+from datetime import datetime, date
 from deepdiff import DeepDiff
 from tabulate import tabulate
 
 
 def compare_json(json1, json2, exclude_paths=None, significant_digits=4, format_value=True, **kwargs):
     """
         对比组件
@@ -36,21 +37,21 @@
     @return: path
     """
     if isinstance(japths, str):
         japths = japths.split(",")
     elif isinstance(japths, set):
         japths = list(japths)
     elif not isinstance(japths, (list, tuple)):
-        logging.warning("jsonpath 参数格式不正确，多个使用列表，元组，或可使用英文逗号分割的字符串")
+        logging.warning(u"jsonpath 参数格式不正确，多个使用列表，元组，或可使用英文逗号分割的字符串")
     paths = []
     for jpath in japths:
         _paths = jsonpath.jsonpath(json_obj, jpath.strip(), result_type='PATH')
         if not _paths:
-            logging.warning("使用jsonpath: {jpath} 无法中获取到值，请检查jsonpath是否正确! json对象: {json_obj} ".format(jpath=jpath,
-                                                                                                      json_obj=json_obj))
+            # logging.warning(u"使用jsonpath: {jpath} 无法中获取到值，请检查jsonpath是否正确! json对象: {json_obj} ".
+            #                 format(jpath=jpath, json_obj=json.dumps(json_obj, ensure_ascii=False)))
             continue
         paths.extend([path.replace("$", "root") for path in _paths])
     return paths
 
 
 def table_log_result(diff_res):
     """
@@ -63,14 +64,15 @@
         diff_values = []
         for item in diff_res.items():
             for i in item:
                 if isinstance(i, set):
                     for ele in list(i):
                         diff_values.append([ele.report_type, ele.t1, ele.t2, ele])
         logging.warning(tabulate(diff_values, headers=header, tablefmt='grid'))
+        raise Exception, "结果比对失败"
 
 
 def values_format(obj, significant_digits):
     if isinstance(obj, (list, set)):
         for item in obj:
             values_format(item, significant_digits)
     elif isinstance(obj, dict):
@@ -81,20 +83,21 @@
                 try:
                     v = json.loads(v)
                     obj[k] = values_format(v, significant_digits)
                 except Exception:
                     obj[k] = str(v)
             elif isinstance(v, (int, float)):
                 obj[k] = round(v, significant_digits)
+            elif isinstance(v, (datetime, date)):
+                obj[k] = v.strftime('%Y-%m-%d %H:%M:%S')
             else:
                 obj[k] = values_format(v, significant_digits)
     return obj
 
 
-
 if __name__ == '__main__':
     json1 = {
         "url": "https://miao.baidu.com/abdr",
         "headers": {
             "Sec-Fetch-Site": "same-site",
             "Sec-Fetch-Mode": "cors",
             "User-Agent": "new agent",
@@ -127,8 +130,8 @@
         },
         "method": "POST",
         "data": {"a": 3.141592, "b": {"c": [2, 3]}, "d": "1234"},
         "test1": """{"aa":11, "bb":22}"""
     }
     compare_json(json1, json2, exclude_paths="$.data.b.c")
     # values_format(json2, 2)
-    # print json.dumps(json2)
+    # print json.dumps(json2)
```

## apitest_ezgo/DbHelper.py

```diff
@@ -1,13 +1,14 @@
 # coding:utf-8
 """
 @date: 2023/2/23
 @author: mawengang
 """
 from DBUtils.PooledDB import PooledDB
+from robot.api import logger
 
 
 class Config():
     # 数据库连接编码
     # DB_CHARSET = "utf-8"
 
     # mincached : 启动时开启的闲置连接数量(缺省值 0 开始时不创建连接)
@@ -100,14 +101,15 @@
             "port": '5434',
             "user": 'postgres',
             "password": 'login@6123',
             "database": 'scanner',
             "cursor_factory": psycopg2.extras.RealDictCursor
         }
         """
+        self.cursor_factory = db_config.get("cursor_factory", None)
         self.db = DbConnectionPool(creator, db_config)  # 从数据池中获取连接
 
     # def __new__(cls, *args, **kwargs):
     #     if not hasattr(cls, 'inst'):  # 单例
     #         cls.inst = super(SqLHelper, cls).__new__(cls, *args, **kwargs)
     #     return cls.inst
 
@@ -118,14 +120,16 @@
         :param sql: 字符串类型，sql语句
         :param param: sql语句中要替换的参数"select %s from tab where id=%s" 其中的%s就是参数
         :param autoclose: 是否关闭连接
         :return: 返回连接conn和游标cursor
         """
         cursor, conn = self.db.get_conn()  # 从连接池获取连接
         count = 0
+        logger.info(u"执行sql为： %s" % sql)
+        logger.info(u"执行sql 参数为： %s" % param)
         try:
             # count : 为改变的数据条数
             if param:
                 count = cursor.execute(sql, param)
             else:
                 count = cursor.execute(sql)
             conn.commit()
@@ -138,18 +142,21 @@
     # 执行多条命令
     def executemany(self, lis):
         """
         :param lis: 是一个列表，里面放的是每个sql的字典'[{"sql":"xxx","param":"xx"}....]'
         :return:
         """
         cursor, conn = self.db.get_conn()
+
         try:
             for order in lis:
                 sql = order['sql']
                 param = order['param']
+                logger.info(u"执行sql为： %s" % sql)
+                logger.info(u"执行sql 参数为： %s" % param)
                 if param:
                     cursor.execute(sql, param)
                 else:
                     cursor.execute(sql)
             conn.commit()
             self.close(cursor, conn)
             return True
@@ -163,39 +170,43 @@
     def close(self, cursor, conn):
         """释放连接归还给连接池"""
         cursor.close()
         conn.close()
 
     # 查询所有， 应该是最常用的了
     def select_all(self, sql, param=None):
+        cursor, conn, count = self.execute(sql, param)
         try:
-            cursor, conn, count = self.execute(sql, param)
             res = cursor.fetchall()
+            if self.cursor_factory:
+                return [dict(i) for i in res]
             return res
         except Exception as e:
             print(e)
             self.close(cursor, conn)
             return count
 
     # 查询单条
     def select_one(self, sql, param=None):
+        cursor, conn, count = self.execute(sql, param)
         try:
-            cursor, conn, count = self.execute(sql, param)
             res = cursor.fetchone()
             self.close(cursor, conn)
+            if self.cursor_factory:
+                return [dict(i) for i in res]
             return res
         except Exception as e:
             print("error_msg:", e.args)
             self.close(cursor, conn)
             return count
 
     # 增加
     def insert_one(self, sql, param):
+        cursor, conn, count = self.execute(sql, param)
         try:
-            cursor, conn, count = self.execute(sql, param)
             # _id = cursor.lastrowid()  # 获取当前插入数据的主键id，该id应该为自动生成为好
             conn.commit()
             self.close(cursor, conn)
             return count
             # 防止表中没有id返回0
             # if _id == 0:
             #     return True
@@ -222,28 +233,28 @@
             print(e)
             conn.rollback()
             self.close(cursor, conn)
             return count
 
     # 删除
     def delete(self, sql, param=None):
+        cursor, conn, count = self.execute(sql, param)
         try:
-            cursor, conn, count = self.execute(sql, param)
             self.close(cursor, conn)
             return count
         except Exception as e:
             print(e)
             conn.rollback()
             self.close(cursor, conn)
             return count
 
     # 更新
     def update(self, sql, param=None):
+        cursor, conn, count = self.execute(sql, param)
         try:
-            cursor, conn, count = self.execute(sql, param)
             conn.commit()
             self.close(cursor, conn)
             return count
         except Exception as e:
             print(e)
             conn.rollback()
             self.close(cursor, conn)
```

## apitest_ezgo/FastRequest.py

```diff
@@ -18,22 +18,21 @@
     需要更新请求参数，传入对应jpath 和 值，如果需要将某个参数从请求中删除，将值更新为{REMOVE}
     例如{"$.headers.User-Agent": "new agent", "$..sec-ch-ua": '{REMOVE}'}
 
     @replace_dict: 需要变更的组装字典，KEY为jsonpath，value为需要替换的新值，如{"$.headers.User-Agent": "new agent"}
     @req_info: 原始请求参数
     """
     if not isinstance(replace_dict, dict):
-        logging.error("jsonpath 格式输入不合法")
-        raise "jsonpath 格式输入不合法: %s" % replace_dict
+        logging.error(u"jsonpath 格式输入不合法")
+        raise u"jsonpath 格式输入不合法: %s" % replace_dict
 
     # 更新请求参数
     for k, v in replace_dict.items():
         parser = jsonpath_ng.parse(k)
         parser.update_or_create(req_info, v)
-    print ("after update %s" % json.dumps(req_info))
 
     # 删除请求参数为{REMOVE}的
     parser = jsonpath_ng.parse("$..*")
     parser.filter(lambda x: x == '{REMOVE}', req_info)
 
 
 def load_req_info(file_path):
@@ -56,35 +55,41 @@
         # http适配器，自动重试次数3
         adapter = HTTPAdapter(max_retries=3, pool_connections=3, pool_maxsize=5)
         # http和https都适用适配器
         self.session.mount('http://', adapter)
         self.session.mount('https://', adapter)
         # @TODO session管理器
 
-    def fast_request(self, file_path, request_name, resp_jpath=None, session=None, replace_dict=None):
+    def fast_request(self, request_name, file_path='', resp_jpath=None, session=None, **replace_dict):
         """
         支持各类请求方式各类content-type的请求入口
-        @param file_path: json文件路径，可为相对于template_path的相对路径
+        @param file_path: json文件路径，可为相对于template_path的相对路径，不传时template_path需要到文件
         @param request_name: json文件中请求的名称，即字典名称
         @param resp_jpath: 需要提取响应数据的jsonpath
         @param session: 支持临时session请求，不传默认使用实例session
         @param replace_dict:需要更新请求参数，传入对应jpath 和 值，如果需要将某个参数从请求中删除，将值更新为{REMOVE}
                             例如{"$.headers.User-Agent": "new agent", "$..sec-ch-ua": '{REMOVE}'}
         @return: 传入resp_jpath取对应数据，默认返回响应对象
         """
-        path = os.path.join(self.template_path, file_path) if self.template_path else file_path
+        path = os.path.join(self.template_path, file_path) if (self.template_path and file_path) \
+            else (file_path if file_path else self.template_path)
         req_info = load_req_info(path).get(request_name)
         replace_dict = replace_dict if replace_dict else {}
         if self.base_url:
+            if self.base_url.endswith("/"):
+                self.base_url = self.base_url[:-1]
             replace_dict.update({"$.host": self.base_url})
         update_req_info(replace_dict, req_info)
         url = req_info.get("host") + req_info.get("path")
         req_info.pop("host")
         req_info.pop("path")
         # 支持临时session请求，默认使用实例session
+        logging.info(u"请求信息：\n %s" % req_info)
         if session:
             resp = session.request(url=url, **req_info)
         else:
             resp = self.session.request(url=url, **req_info)
+        msg = u"请求status_code： %s" % resp.status_code
+        logging.info(msg) if resp.status_code == 200 else logging.warning(msg)
         return jsonpath(resp.json(), resp_jpath)[0] if resp_jpath else resp
```

## apitest_ezgo/__about__.py

```diff
@@ -1,8 +1,8 @@
 __title__ = 'apitest_ezgo'
 __description__ = 'easy http interface test frame'
 __url__ = ''
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 __author__ = 'Gawen'
 __author_email__ = '502286126@qq.com'
 __license__ = 'Apache-2.0'
 __copyright__ = 'Copyright 2022 Gawen'
```

## apitest_ezgo/Har2Template/cli.py

```diff
@@ -40,7 +40,15 @@
     print args
 
     HarParser(
         har_source_file, args.dest_file_path
     ).gen_template()
     return 0
 
+def test(har_source_file, dest_file_path):
+    HarParser(
+        har_source_file, dest_file_path
+    ).gen_template()
+
+
+if __name__ == '__main__':
+    test(r"C:\Users\nsfocus\Desktop\units.har", ".")
```

## apitest_ezgo/Har2Template/compat.py

```diff
@@ -32,15 +32,15 @@
 # Specifics
 # ---------
 
 if is_py2:
     import urlparse
     from urllib import unquote
 
-    ensure_ascii = True
+    ensure_ascii = False
     builtin_str = str
     bytes = str
     str = (unicode, bytes)
     basestring = basestring
     numeric_types = (int, long, float)
     integer_types = (int, long)
```

## apitest_ezgo/Har2Template/core.py

```diff
@@ -11,21 +11,21 @@
 try:
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
 IGNORE_REQUEST_HEADERS = [
     "host",
-    "accept",
+    # "accept",
     "content-length",
     "connection",
-    "accept-encoding",
-    "accept-language",
+    # "accept-encoding",
+    # "accept-language",
     "origin",
-    "referer",
+    # "referer",
     "cache-control",
     "pragma",
     "cookie",
     "upgrade-insecure-requests",
     ":authority",
     ":method",
     ":scheme",
@@ -37,15 +37,15 @@
 
     def __init__(self, har_file_path, dest_file_path, filter_str=None, exclude_str=None):
         self.har_file_path = har_file_path
         self.dest_file_path = dest_file_path
         self.filter_str = filter_str
         self.exclude_str = exclude_str or ""
 
-    def __make_request_url(self, path, requst_dict, entry_json):
+    def __make_request_url(self, name, path, requst_dict, entry_json):
         """ parse HAR entry request url and queryString, and make requst url and params
 
         Args:
             entry_json (dict):
                 {
                     "request": {
                         "url": "https://httprunner.top/home?v=1&w=2",
@@ -66,55 +66,55 @@
                 }
             }
 
         """
         request_params = utils.convert_list_to_dict(
             entry_json["request"].get("queryString", [])
         )
-        requst_dict[path]["path"] = path
+        requst_dict[name]["path"] = path
         full_url = entry_json["request"].get("url")
         if not full_url:
             logging.exception("url missed in request.")
             sys.exit(1)
 
         parsed_object = urlparse.urlparse(full_url)
         if request_params:
             parsed_object = parsed_object._replace(query='')
             url = parsed_object.geturl()
-            requst_dict[path]["params"] = request_params
+            requst_dict[name]["params"] = request_params
         else:
             url = full_url
-        requst_dict[path]["host"] = url.replace(path, "")
+        requst_dict[name]["host"] = url.replace(path, "")
 
 
-    def __make_request_method(self, path, requst_dict, entry_json):
+    def __make_request_method(self, name, requst_dict, entry_json):
         """ parse HAR entry request method, and make requst method.
         """
         method = entry_json["request"].get("method")
         if not method:
             logging.exception("method missed in request.")
             sys.exit(1)
 
-        requst_dict[path]["method"] = method
+        requst_dict[name]["method"] = method
 
-    def __make_request_headers(self, path, requst_dict, entry_json):
+    def __make_request_headers(self, name, requst_dict, entry_json):
         """ parse HAR entry request headers, and make requst headers.
             header in IGNORE_REQUEST_HEADERS will be ignored.
         """
         requst_headers = {}
         for header in entry_json["request"].get("headers", []):
             if header["name"].lower() in IGNORE_REQUEST_HEADERS:
                 continue
 
             requst_headers[header["name"]] = header["value"]
 
         if requst_headers:
-            requst_dict[path]["headers"] = requst_headers
+            requst_dict[name]["headers"] = requst_headers
 
-    def _make_request_data(self, path, requst_dict, entry_json):
+    def _make_request_data(self, name, requst_dict, entry_json):
         """ parse HAR entry request data, and make requst request data
         """
         method = entry_json["request"].get("method")
         if method in ["POST", "PUT", "PATCH"]:
             postData = entry_json["request"].get("postData", {})
             mimeType = postData.get("mimeType")
 
@@ -136,33 +136,34 @@
                     pass
             elif mimeType.startswith("application/x-www-form-urlencoded"):
                 post_data = utils.convert_x_www_form_urlencoded_to_dict(post_data)
             else:
                 # TODO: make compatible with more mimeType
                 pass
 
-            requst_dict[path][request_data_key] = post_data
+            requst_dict[name][request_data_key] = post_data
 
     def _prepare_requst(self, entry_json):
         """ extract info from entry dict and make requst
         """
         url = entry_json["request"].get("url")
         if not url:
             logging.exception("url missed in request.")
             sys.exit(1)
 
         parsed_object = urlparse.urlparse(url)
         path = parsed_object.path
+        name = entry_json["request"].get("method") + "_" + path
         requst_dict = {
-            path: {},
+            name: {},
         }
-        self.__make_request_url(path, requst_dict, entry_json)
-        self.__make_request_method(path, requst_dict, entry_json)
-        self.__make_request_headers(path, requst_dict, entry_json)
-        self._make_request_data(path, requst_dict, entry_json)
+        self.__make_request_url(name, path, requst_dict, entry_json)
+        self.__make_request_method(name, requst_dict, entry_json)
+        self.__make_request_headers(name, requst_dict, entry_json)
+        self._make_request_data(name, requst_dict, entry_json)
 
         return requst_dict
 
     def _prepare_requst_info(self, fmt_version):
         """ make requst list.
             requst_info list are parsed from HAR log entries list.
```

## apitest_ezgo/Har2Template/utils.py

```diff
@@ -1,15 +1,26 @@
 import io
 import json
 import logging
 import sys
 import yaml
+import datetime
 from apitest_ezgo.Har2Template.compat import bytes, ensure_ascii, str, unquote
 
 
+class ComplexEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime):
+            return obj.strftime('%Y-%m-%d %H:%M:%S')
+        elif isinstance(obj, datetime.date):
+            return obj.strftime('%Y-%m-%d')
+        else:
+            return json.JSONEncoder.default(self, obj)
+
+
 def load_har_log_entries(file_path):
     """ load HAR file and return log entries list
 
     Args:
         file_path (str)
 
     Returns:
```

## Comparing `apitest_ezgo-0.0.5.dist-info/RECORD` & `apitest_ezgo-0.0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-apitest_ezgo/Compare.py,sha256=1JDU_uVD9uo4VB6FqEDgLdzHjyMn3MJ1xFKMOQaRD3A,5077
-apitest_ezgo/DbHelper.py,sha256=HRq75ScG5KhGtU30IDVGyE6gfA9w5-6T7OeDY51rYc4,9464
-apitest_ezgo/FastRequest.py,sha256=9XepQBd8-NbhcEOW3ZdSdVIezda6X-D4l9-BlmdFLwg,3681
-apitest_ezgo/__about__.py,sha256=ixahm2tcwaaofKgzRxUUJdfTDWwXRarCYE1L9dEiVtQ,237
+apitest_ezgo/Compare.py,sha256=aA1rCXKEtZhzsU0UlMxTN2t_tBs-nzQdy9GSK5Nyjts,5235
+apitest_ezgo/DbHelper.py,sha256=QUjjVKXJ8idMNeD0ruJakiCd77Fx_JZrkuW79RVvxSk,9947
+apitest_ezgo/FastRequest.py,sha256=dJURPhlq_7npDkEY2VrRy9s04aQ51qV5hIGZL-6-qYA,4035
+apitest_ezgo/__about__.py,sha256=vIUinmANX4OTBnmhqpP5DVMRHJnZcmEi8MHVsc8_4QI,237
 apitest_ezgo/__init__.py,sha256=uM6HTTSwSziyZus-ubqZ-VKNG3KKd4kBHOlj7lR2OhQ,53
 apitest_ezgo/Har2Template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-apitest_ezgo/Har2Template/cli.py,sha256=H9vEtD_UTtfa0OGursOZc3dDnjRf8-Wq2cezCUk801s,1654
-apitest_ezgo/Har2Template/compat.py,sha256=xxl3BpN5OBYI2jJLe0CBxJpoWVF4I_sZNieu89VOQBg,930
-apitest_ezgo/Har2Template/core.py,sha256=_O5ZddUSajsp3NM5hb375jJyFur2pc2q22Y69RySUrw,6383
-apitest_ezgo/Har2Template/utils.py,sha256=w9dJv513jH8dueGvOp-uWJyx2d-Vf015gr3QTP9iPec,3184
-apitest_ezgo-0.0.5.dist-info/METADATA,sha256=PZZC6BeEWfCLJtyEj6XYPDHjcdlVfqC-IqEj1lF9x5s,371
-apitest_ezgo-0.0.5.dist-info/WHEEL,sha256=1VPi6hfNQaRRNuEdK_3dv9o8COtLGnHWJghhj4CQ28k,92
-apitest_ezgo-0.0.5.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
-apitest_ezgo-0.0.5.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
-apitest_ezgo-0.0.5.dist-info/RECORD,,
+apitest_ezgo/Har2Template/cli.py,sha256=ZCRAPECXeISO_SW53N0oyxO-B-9lYBWUPGJfDaqX1QA,1854
+apitest_ezgo/Har2Template/compat.py,sha256=WuUsCFx7TLCiAN-u3CPWILWnMmEaKJdcofD-ZRPJRdE,931
+apitest_ezgo/Har2Template/core.py,sha256=4ZV_gSPfatFL_iCuPOf0GWmZxsylBgX5x6gYjFSeuEk,6467
+apitest_ezgo/Har2Template/utils.py,sha256=oU22kMbbvWKw8s30Gifo3PW-dgFUMWsdl1PFEoEcomk,3519
+apitest_ezgo-0.0.6.dist-info/METADATA,sha256=z_O8qJaMZjfdtp_xy199tuVCmbjm8adyouu8sxrB4Es,371
+apitest_ezgo-0.0.6.dist-info/WHEEL,sha256=1VPi6hfNQaRRNuEdK_3dv9o8COtLGnHWJghhj4CQ28k,92
+apitest_ezgo-0.0.6.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
+apitest_ezgo-0.0.6.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
+apitest_ezgo-0.0.6.dist-info/RECORD,,
```

