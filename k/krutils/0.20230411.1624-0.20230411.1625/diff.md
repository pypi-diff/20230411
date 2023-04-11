# Comparing `tmp/krutils-0.20230411.1624.tar.gz` & `tmp/krutils-0.20230411.1625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1624.tar", last modified: Tue Apr 11 07:24:24 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1625.tar", last modified: Tue Apr 11 07:26:00 2023, max compression
```

## Comparing `krutils-0.20230411.1624.tar` & `krutils-0.20230411.1625.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:24:24.021708 krutils-0.20230411.1624/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:24:24.016898 krutils-0.20230411.1624/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1624/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:24:23.847590 krutils-0.20230411.1624/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1624/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1624/krutils/CONST.py
--rw-rw-rw-   0        0        0       93 2023-04-11 07:24:11.000000 krutils-0.20230411.1624/krutils/__init__.py
--rw-rw-rw-   0        0        0     5485 2023-04-11 07:16:33.000000 krutils-0.20230411.1624/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1624/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:24:23.982991 krutils-0.20230411.1624/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:24:24.024096 krutils-0.20230411.1624/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-04-11 07:24:22.000000 krutils-0.20230411.1624/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:26:00.011513 krutils-0.20230411.1625/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:25:59.976341 krutils-0.20230411.1625/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1625/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:25:59.923975 krutils-0.20230411.1625/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1625/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1625/krutils/CONST.py
+-rw-rw-rw-   0        0        0       93 2023-04-11 07:24:11.000000 krutils-0.20230411.1625/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5481 2023-04-11 07:25:57.000000 krutils-0.20230411.1625/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1625/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:25:59.972369 krutils-0.20230411.1625/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:26:00.012042 krutils-0.20230411.1625/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/setup.py
```

### Comparing `krutils-0.20230411.1624/krutils/CONST.py` & `krutils-0.20230411.1625/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1624/krutils/dbmgr.py` & `krutils-0.20230411.1625/krutils/dbmgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import os
 import pymysql
 from pymysql import Connection
-import utils
+from .krutils import utils
 
 
 # SQL PARAM 형식
 SQL_PARAM_PATTERN = "#\\{\\D[\\w]*\\}";
 
 # SELECT 기본 MAX 건수 : 500 (DBIO 조회 기본값)
 MAX_CNT = 10000;
@@ -21,26 +21,26 @@
     '''
     SQL을 실행, 결과를 반환한다.
     '''
 
     '''
     예를 들어 입력 SQL이 아래와 같다고 하면...
 
-    SELECT * 
+    SELECT *
     FROM TBTMP
     where k1 = #{k1}
     ;
     '''
 
     # CONNECTION
     juso_db = pymysql.connect(
-        user='root', 
-        passwd='{설정한 비밀번호}', 
-        host='127.0.0.1', 
-        db='juso-db', 
+        user='root',
+        passwd='{설정한 비밀번호}',
+        host='127.0.0.1',
+        db='juso-db',
         charset='utf8'
     )
 
 
     # CURSOR
     cursor = juso_db.cursor(pymysql.cursors.DictCursor)
 
@@ -57,15 +57,15 @@
     result = pd.DataFrame(result)
     result
 
 
 
     ##########################
     # INSERT
-    sql = '''INSERT INTO `busan-jibun` (관리번호, 일련번호, 시도명, 시군구명) 
+    sql = '''INSERT INTO `busan-jibun` (관리번호, 일련번호, 시도명, 시군구명)
     VALUES ('1234567891234567891234567', '1', '서울특별시', '강남구');'''
 
     cursor.execute(sql)
     juso_db.commit()
 
 
 
@@ -77,15 +77,15 @@
 
 
 
 def _get_connection() -> pymysql.Connection:
     '''
     DB Connection
     '''
-    
+
     # katis 메인 환경설정 읽기
     katis_env = utils.get_katis_env()
     logger.debug("katis_env[%%]", katis_env)
 
     # DB 설정 파일 읽기
     curr_dir = os.path.dirname(__file__)
     base_name = os.path.basename(__file__)
@@ -160,15 +160,15 @@
         new_key = str(f[2:-1]).upper()
         # logger.debug("new_key[%%]", new_key)
 
         try:
             new_val = new_kwargs[new_key]
         except Exception as e:
             new_val = None
-        
+
         new_args.append(new_val)
     # logger.dblog("new_args[%%]", new_args)
 
 
     # sql에서 변수 할당 치환
     new_sql = re.sub(SQL_PARAM_PATTERN, "%s", sql)
     # logger.dblog("new_sql[%%] new_args[%%]", new_sql, new_args)
```

### Comparing `krutils-0.20230411.1624/krutils/utils.py` & `krutils-0.20230411.1625/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1624/setup.py` & `krutils-0.20230411.1625/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1624",
+    version="0.20230411.1625",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

