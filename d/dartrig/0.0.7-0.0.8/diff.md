# Comparing `tmp/dartrig-0.0.7.tar.gz` & `tmp/dartrig-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.0.7.tar", last modified: Sat Mar 18 11:48:49 2023, max compression
+gzip compressed data, was "dist/dartrig-0.0.8.tar", last modified: Tue Apr 11 08:27:35 2023, max compression
```

## Comparing `dartrig-0.0.7.tar` & `dartrig-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-03-18 11:48:49.000000 dartrig-0.0.7/
--rw-r--r--   0 nezah      (501) staff       (20)      411 2023-03-18 11:48:49.000000 dartrig-0.0.7/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.0.7/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 dartrig-0.0.7/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      544 2023-03-18 11:48:45.000000 dartrig-0.0.7/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    10584 2023-03-18 11:47:55.000000 dartrig-0.0.7/dartrig/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      411 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      170 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-03-18 11:48:49.000000 dartrig-0.0.7/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-03-18 11:48:49.000000 dartrig-0.0.7/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-11 08:27:35.000000 dartrig-0.0.8/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.0.8/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.0.8/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      600 2023-04-11 08:26:59.000000 dartrig-0.0.8/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    11505 2023-04-11 01:58:31.000000 dartrig-0.0.8/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.0.8/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      193 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-11 08:27:35.000000 dartrig-0.0.8/setup.cfg
```

### Comparing `dartrig-0.0.7/LICENSE` & `dartrig-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.0.7/setup.py` & `dartrig-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.0.7",
+    version="0.0.8",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="dartrig api wrapper",
-    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
+    long_description=open('README.md', "r").read(),
     url="https://github.com/cheddars/dart_rigger",
     packages=setuptools.find_packages(),
     classifiers=[
         # 패키지에 대한 태그
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
```

### Comparing `dartrig-0.0.7/dartrig/__init__.py` & `dartrig-0.0.8/dartrig/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,89 @@
 import re
 import requests
 import logging
 import traceback
+import time
 from typing import List
 from datetime import datetime
 from bs4 import BeautifulSoup
+from cache import AdtCache
+from dartrig.annotations import memoize
 
-headers = {
+HEADERS = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 Safari/537.36"}
 
+URLS = {
+    "DART_BASE": "https://dart.fss.or.kr",
+    "DART_LIST": "https://dart.fss.or.kr/dsab007/detailSearch.ax",
+    "DART_VIEWER": "https://dart.fss.or.kr/report/viewer.do",
+    "DART_DSAF": "https://dart.fss.or.kr/dsaf001/main.do",
+}
+logger = logging.getLogger("dartrig")
+
 
 class DartWeb:
     def __init__(self):
-        self.rcp_dcm_map = {}
-        self.rcp_html_map = {}
+        self.session = requests.Session()
+        self.session.get(URLS["DART_BASE"], headers=HEADERS)
 
+    @memoize
     def request_detail(self, rcp_no: str, dtd: str, ele_id: int = 0, offset: int = 0) -> str:
         """
         :param rcp_no:
         :param dtd: html | dart3.xsd
         :param ele_id:
         :param offset:
         :return:
         """
         dcm_no = self.get_dcm_no_by_rcp_no(rcp_no)
-        key = f"{rcp_no}_{dcm_no}_{dtd}"
-        text = self.rcp_html_map.get(key)
-        if text is None:
-            url = f"https://dart.fss.or.kr/report/viewer.do?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
-            logging.info(f"request_detail url : {url}")
-            response = requests.get(url, headers=headers)
-            # response.encoding = "UTF-8"
-            text = response.text
-            self.rcp_html_map[key] = text
-        else:
-            logging.debug(f"use text in cache for key : {key}")
-        return text
+        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
+        logger.info(f"request_detail url : {url}")
+        response = self.session.get(url, headers=HEADERS)
+        # response.encoding = "UTF-8"
+        return response.text
 
+    @memoize
     def request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0):
-        key = f"{rcp_no}_{dcm_no}_{dtd}"
-        text = self.rcp_html_map.get(key)
-        if text is None:
-            url = f"https://dart.fss.or.kr/report/viewer.do?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
-            logging.info(f"request_detail_with_dcm url : {url}")
-            text = requests.get(url, headers=headers).text
-            self.rcp_html_map[key] = text
-        else:
-            logging.debug(f"use text in cache for key : {key}")
-        return text
+        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
+        logger.info(f"request_detail_with_dcm url : {url}")
+        return self.session.get(url, headers=HEADERS).text
 
+    @memoize
     def dsaf001_report(self, rcp_no):
-        logging.debug(f"dsaf001_report for rcp_no {rcp_no}")
-        key = f"{rcp_no}"
-        html_text = self.rcp_html_map.get(key)
-        if html_text is None:
-            html_text = requests.get(f"https://dart.fss.or.kr/dsaf001/main.do?rcpNo={rcp_no}", headers=headers).text
-            self.rcp_html_map[key] = html_text
-        else:
-            logging.debug(f"use text in cache for key : {key}")
-
-        return html_text
+        logger.debug(f"dsaf001_report for rcp_no {rcp_no}")
+        return self.session.get(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", headers=HEADERS).text
 
+    @memoize
     def get_dcm_no_by_rcp_no(self, rcp_no):
         try:
             html_text = self.dsaf001_report(rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
         except Exception as ex:
-            logging.exception(ex)
+            logger.exception(ex)
             raise ValueError(f"dcm number fetch failed for rcp_no : [{rcp_no}]")
 
         return dcm_no
 
     def get_document(self, rcp_no, dtd, ele_id=0, offset=0):
         """
         문서 리턴
         :param rcp_no:
         :param dtd:
         :param ele_id:
         :param offset:
         :return: (content_type, content)
         """
         dcm_no = self.get_dcm_no_by_rcp_no(rcp_no)
-        url = f"https://dart.fss.or.kr/report/viewer.do?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
-        response = requests.get(url, headers=headers)
+        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
+        response = self.session.get(url, headers=HEADERS)
         content_type = response.headers.get("Content-Type")
         return content_type, response.content
 
-
     def search_report(self, num, start, end, srch_txt):
         data = {
             'currentPage': str(num),
             'maxResults': '100',
             'maxLinks': '10',
             'sort': 'date',
             'series': 'desc',
@@ -112,129 +104,163 @@
             'endDate': end,
             'finalReport': 'recent',
             'businessNm': '전체',
             'corporationType': 'all',
             'closingAccountsMonth': 'all',
             'tocSrch2': ''
         }
-        headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 "
-                          "Safari/537.36"}
 
-        return requests.post('https://dart.fss.or.kr/dsab007/detailSearch.ax', data=data, headers=headers)
+        return self.session.post(URLS["DART_LIST"], data=data, headers=HEADERS)
+
 
 class DartAPI:
-    def __init__(self, keys: List):
+    def __init__(self, keys: List, cache: AdtCache):
+        """
+
+        :param keys: dart_api key
+        :param cache: MemoryCache or RedisCache
+        """
         self.keys: DartKeys = DartKeys(keys)
+        self.cache = cache
+        logger.info(f"cache keys : {self.cache.keys()}")
 
-    def get_disclosure_list(self, end_de, depth=1):
+    def get_disclosure_list(self, end_de, max_page=1, use_cache=False, pause=0.5):
         """
-        :param end_de:
-        :param depth:
-        :return: rcp_no 내림차순 순으로 정렬된 공시 리스트
+        :param end_de: YYYYMMDD 요청 종료일
+        :param max_page: 최대 요청 페이지 생략시 1
+        :param use_cache: 캐시 사용여부
+        :param pause: 요청간 쉬는 시간(단위 초)
+        :return: 공시목록
         """
         results = []
-        hasMore = True
         page = 1
         total_page = 1
         page_no = 0
 
-        while hasMore and depth > 0:
+        while page <= total_page:
+            response_items = None
             json_data = self.get_disclosure(end_de=end_de, page=page)
             status = json_data.get("status")
 
             if status == '013':  # 조회된 데이터가 없습니다
-                logging.info("no data")
+                logger.info("no data")
                 break
             elif status == '012':  # 접근할 수 없는 IP입니다.
-                logging.error(f"접근할 수 없는 IP key")
+                logger.error(f"접근할 수 없는 IP key")
                 # self.dart_api.disable_key(key)
                 # not increase page
             elif status == '020':  # API key 한도 초과
-                logging.error(f"{status} API key 한도 초과 key")
+                logger.error(f"{status} API key 한도 초과 key")
                 # self.dart_api.disable_key(key)
                 # not increase page
             elif status == '021':
-                logging.error(f"{status} 조회 가능한 회사 개수가 초과하였습니다.(최대 100건)")
+                logger.error(f"{status} 조회 가능한 회사 개수가 초과하였습니다.(최대 100건)")
             elif status == '100':
-                logging.error(f"{status} 조회 가능한 회사 개수가 초과하였습니다.(최대 100건)")
+                logger.error(f"{status} 조회 가능한 회사 개수가 초과하였습니다.(최대 100건)")
             elif status == '101':
-                logging.error(f"{status} 부적절한 접근입니다.")
+                logger.error(f"{status} 부적절한 접근입니다.")
             elif status == '800':
-                logging.error(f"{status} 조회 가능한 회사 개수가 초과하였습니다.(최대 100건)")
+                logger.error(f"{status} 시스템 점검으로 인한 서비스가 중지 중입니다.")
+                break
             elif status == '900':
-                logging.error(f"{status} 정의되지 않은 오류가 발생하였습니다.")
+                logger.error(f"{status} 정의되지 않은 오류가 발생하였습니다.")
             elif status == '901':
-                logging.error(f"{status} 사용자 계정의 개인정보 보유기간이 만료되어 사용할 수 없는 키입니다. 관리자 이메일(opendart@fss.or.kr)로 문의하시기 바랍니다.")
+                logger.error(f"{status} 사용자 계정의 개인정보 보유기간이 만료되어 사용할 수 없는 키입니다. 관리자 이메일(opendart@fss.or.kr)로 문의하시기 바랍니다.")
             elif status == '000':  # 정상조회
                 page_no = json_data.get("page_no")
                 page_count = json_data.get("page_count")
-                total_count = json_data.get("total_count")
-                total_page = json_data.get("total_page")
+                total_count = int(json_data.get("total_count"))
+                total_page = int(json_data.get("total_page"))
                 page = page + 1
-                logging.info(f"정상조회 total_count : {total_count}, total_page : {total_page}, page_count : {page_count}, page_no : {page_no}")
-                results.extend(json_data.get("list"))
+                logger.info(f"정상조회 total_count : {total_count}, total_page : {total_page}, page_count : {page_count}, page_no : {page_no}")
+                response_items = json_data.get("list")
             else:
-                logging.error(f"처리안된 예외 케이스 status : {status}")
+                logger.error(f"처리안된 예외 케이스 status : {status}")
 
-            depth = depth - 1
+            if use_cache:
+                cache_key = f"dartapi_list_{end_de}"
+                keys = [x.get("rcept_no") for x in response_items]
+                diff = self.cache.differential(cache_key, keys)
+                logger.debug(f"diff : {diff}, cached keys : {len(self.cache.keys())}")
+                diff_ratio = float(len(diff)) / float(len(response_items)) * 100
+                if diff_ratio == float(0):
+                    logger.info(f"diff ratio is {diff_ratio}% => break")
+                    break
+                else:
+                    logging.info(f"diff ratio is {diff_ratio}%")
+                    results.extend([x for x in response_items if x.get("rcept_no") in diff])
+                    self.cache.push_values(cache_key, keys)
+
+                    if diff_ratio < 80:
+                        logger.info(f"break")
+                        break
+                    else:
+                        logger.info(f"pause {pause} secs for continue")
+                        time.sleep(pause)
+                        continue
+            else:
+                results.extend(response_items)
 
             if total_page == page_no:
+                logger.info(f"total page reached {total_page}")
+                break
+
+            if max_page >= page_no:
+                logger.info(f"max page reached {max_page}")
                 break
 
         list_items = []
 
         for item in results:
-            # 각 항목별로 데이터 추출
-            rcept_dt = item.get('rcept_dt', '')
 
+            # 각 항목별로 데이터 추출
             data = {
                 "company": item.get('corp_name', ''),
                 "market": item.get('corp_cls', ''),
                 "title": item.get('report_nm', ''),
                 "code": item.get('stock_code', ''),
                 "rcp_no": item.get('rcept_no', ''),
-                "rcept_dt": rcept_dt[:4] + '.' + rcept_dt[4:6] + '.' + rcept_dt[6:],
+                "rcept_dt": item.get('rcept_dt', ''),
+                "remark": item.get('rm', ''),
+                "flr_nm": item.get('flr_nm', ''),
             }
             list_items.append(data)
 
-        list_items.sort(key=lambda x: int(x.get('rcp_no')[-4:]), reverse=True)  ## 내림차순 정렬
-        logging.debug(
-            f"sorted list_item rcp_no from : {list_items[0].get('rcp_no')}, to : {list_items[-1].get('rcp_no')}")
-
         return list_items
 
     def get_disclosure(self, end_de, page=1, page_count=100):
         key = self.keys.next_key()
-        logging.info(f"fetching data  date : {end_de}, page : {page}, withkey : {key}")
+        logger.info(f"fetching data  date : {end_de}, page : {page}, withkey : {key}")
         param = {
             'crtfc_key': key,
             'page_count': page_count,
             'page_no': page,
             'end_de': end_de
         }
         return requests.get("https://opendart.fss.or.kr/api/list.json", params=param).json()
 
     def get_document_zip_bytes(self, rcp_no):
         key = self.keys.next_key()
-        logging.info(f"fetching data  rcp_no : {rcp_no}, withkey : {key}")
+        logger.info(f"fetching data  rcp_no : {rcp_no}, withkey : {key}")
         param = {
             'crtfc_key': key,
             'rcept_no': rcp_no
         }
         response = requests.get("https://opendart.fss.or.kr/api/document.xml", params=param)
         content_type = response.headers.get("Content-Type")
         if "xml" in content_type:
+            logger.info(f"rcp_no : {rcp_no} Content-Type is XML")
             try:
                 soup = BeautifulSoup(response.text, "html.parser")
                 status = soup.find("status").text
                 message = soup.find("message").text
-                print(f"status : [{status}], message : {message}")
+                logger.info(f"status : [{status}], message : {message}")
             except Exception as ex:
                 traceback.print_exc()
+                logger.error(ex)
             return None
         else:
             return response.content
 
     def disable_key(self, key):
         self.keys.disable_key(key)
 
@@ -249,29 +275,29 @@
         return f"key : {self.key}, disabled : {self.disabled}, at : {self.disabledAt}"
 
 
 class DartKeys:
     def __init__(self, keys: List):
         self.current = 0
         self.keys = list(map(lambda key: DartKey(key), keys))
-        logging.info(f"keys {self}")
+        logger.info(f"keys {self}")
 
     def next_key(self):
         available_keys = list(filter(lambda x : not x.disabled, self.keys))
-        logging.debug(f"available keys : {(','.join([str(elem) for elem in available_keys]))}")
+        logger.debug(f"available keys : {(','.join([str(elem) for elem in available_keys]))}")
 
         if self.current >= len(available_keys) - 1:
             self.current = 0
 
         key = available_keys[self.current].key
         self.current = self.current + 1
         return key
 
     def disable_key(self, keycode):
         for dartkey in self.keys:
             if dartkey.key == keycode:
                 dartkey.disabled = True
                 dartkey.disabledAt = datetime.now()
-                logging.info(f"dart key {keycode} DISABLED")
+                logger.info(f"dart key {keycode} DISABLED")
 
     def __str__(self):
         return "\n".join(list(map(lambda key: f"{key}", self.keys)))
```

