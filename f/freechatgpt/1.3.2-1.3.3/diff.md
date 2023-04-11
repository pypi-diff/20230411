# Comparing `tmp/freechatgpt-1.3.2.tar.gz` & `tmp/freechatgpt-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/freechatgpt-1.3.2.tar", last modified: Fri Apr  7 15:34:42 2023, max compression
+gzip compressed data, was "dist/freechatgpt-1.3.3.tar", last modified: Tue Apr 11 16:29:20 2023, max compression
```

## Comparing `freechatgpt-1.3.2.tar` & `freechatgpt-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt/
--rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.2/freechatgpt/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     5023 2023-04-07 15:34:09.000000 freechatgpt-1.3.2/freechatgpt/free_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.2/README.md
--rw-r--r--   0 admin      (501) staff       (20)     1361 2023-04-07 15:34:09.000000 freechatgpt-1.3.2/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      244 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       33 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/freechatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-07 15:34:42.000000 freechatgpt-1.3.2/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt/
+-rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.3/freechatgpt/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4919 2023-04-11 16:28:11.000000 freechatgpt-1.3.3/freechatgpt/free_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.3/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     1361 2023-04-11 16:28:51.000000 freechatgpt-1.3.3/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      244 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       33 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/setup.cfg
```

### Comparing `freechatgpt-1.3.2/PKG-INFO` & `freechatgpt-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.2
+Version: 1.3.3
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

### Comparing `freechatgpt-1.3.2/freechatgpt/free_chatgpt.py` & `freechatgpt-1.3.3/freechatgpt/free_chatgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def retry_if_timeout_error(excep):
     return isinstance(excep, ReadTimeout)
 
 
 class FreeChatgpt(object):
 
     @staticmethod
-    def ask(question: str) -> dict:
+    def __ask(question: str) -> dict:
         try:
             @retrying.retry(stop_max_attempt_number=4, stop_max_delay=100000,
                             wait_fixed=1500, retry_on_exception=retry_if_timeout_error)
             def ask_q():
                 if not question or not question.strip():
                     return {'code': 0, 'error': 'question is null!'}
                 # url = f'https://api.wqwlkj.cn/wqwlapi/chatgpt.php?msg={question.strip()}&type=json'
@@ -33,29 +33,31 @@
                 # url = f"https://api.caonm.net/api/ai/o.php?msg={question.strip()}"
                 print('AI问题思考中=====')
                 res = requests.get(url, timeout=70)
                 answer_q = None
                 try:
                     if not res.text:
                         raise ReadTimeout()
+                    print(res.text)
                     res_json = json.loads(res.text)
+
                     answer_q = res_json.get("ChatGPT_Answer")
                     print(f'AI问题回答:{answer_q}')
                     # if res_json.get('info'):
                     #     del res_json['info']
                 except JSONDecodeError:
                     return {'code': 0, 'error': answer_q}
                 return {'code': 1, 'text': answer_q}
 
             return ask_q()
         except ReadTimeout:
             return {'code': 0, 'error': 'ReadTimeout,please retry'}
 
     @staticmethod
-    def __ask(question: str):
+    def ask(question: str):
         try:
             @retrying.retry(stop_max_attempt_number=4, stop_max_delay=100000,
                             wait_fixed=1500, retry_on_exception=retry_if_timeout_error)
             def ask_q():
                 if not question or not question.strip():
                     return {'code': 0, 'error': 'question is null!'}
                 print('AI问题思考中=====')
@@ -78,38 +80,38 @@
 
     def _get_chat_res(self) -> str:
         pass
 
 
 class PlatformGptStore(BasePlatform):
     def _get_chat_res(self) -> str:
-        url = "http://free-gpt.store/chatgpt.php"
+        url = "http://free-gpt.fun/chatgpt.php"
         msg = urllib.parse.quote(self.question)
-        payload = f'message={msg}&mychat_ip=43.200.91.235&user_uuid=CHAT-APIGPT-6q1y-3u1p1p-iqoj-3u1y9ut'
+        payload = f'message={msg}&mychat_ip=121.78.25.14&user_uuid=CHAT-APIGPT-oj3uoj-gxhg-3u9ut-oj6q'
         headers = {
             'Accept': '*/*',
             'Accept-Encoding': 'gzip, deflate',
             'Accept-Language': 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7',
             'Connection': 'keep-alive',
             'Content-Length': '83',
             'Content-Type': 'application/x-www-form-urlencoded',
-            'Cookie': 'vtins__JyvVgnc34VsbRCoA=%7B%22sid%22%3A%20%2268124e43-9986-5086-b776-96164ead8e8a%22%2C%20%22vd%22%3A%201%2C%20%22stt%22%3A%200%2C%20%22dr%22%3A%200%2C%20%22expires%22%3A%201680107892363%2C%20%22ct%22%3A%201680106092363%7D; __51uvsct__JyvVgnc34VsbRCoA=1; __51vcke__JyvVgnc34VsbRCoA=c8a8bfcd-bd47-529f-b14b-a195a473eb77; __51vuft__JyvVgnc34VsbRCoA=1680106092372; __gads=ID=0014e195aa647a4f-2295111fd1dc0088:T=1680106133:RT=1680106133:S=ALNI_MYvd73jS0gke9fGbravjygychOjqA; __gpi=UID=00000a35412fdd57:T=1680106133:RT=1680106133:S=ALNI_MZAzBmFwa0kUZj15iK6LCmKFAmaLw',
-            'Host': 'free-gpt.store',
-            'Origin': 'http://free-gpt.store',
-            'Referer': 'http://free-gpt.store/',
+            'Cookie': 'vtins__JyvVgnc34VsbRCoA=%7B%22sid%22%3A%20%22d464cbac-4c29-5db2-9aa4-97ad394b66f4%22%2C%20%22vd%22%3A%201%2C%20%22stt%22%3A%200%2C%20%22dr%22%3A%200%2C%20%22expires%22%3A%201681231922594%2C%20%22ct%22%3A%201681230122594%7D; __51uvsct__JyvVgnc34VsbRCoA=1; __51vcke__JyvVgnc34VsbRCoA=13fce5dc-d74d-50cc-b2c9-c4a588b479d6; __51vuft__JyvVgnc34VsbRCoA=1681230122602',
+            'Host': 'free-gpt.fun',
+            'Origin': 'http://free-gpt.fun',
+            'Referer': 'http://free-gpt.fun/',
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
             'X-Requested-With': 'XMLHttpRequest'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload, timeout=60)
         rs = response.text.split('答：')[1].strip('<br />').strip('<br />')
         return rs
 
 
 if __name__ == '__main__':
     # r = FreeChatgpt.ask(question='帮我优化这段话:pandas快速替换所有字符中的特殊字符')
     # print(r)
     # t = FreeChatgpt.ask(question='中国文化的特点是什么？')
     # print(t)
-    q = '俄罗斯最赚钱的公司是哪家？'
+    q = '根据我的预算2000元,风险偏好中等风险,预期收益率1.3%,请为我提供一种个人理财方案'
     s = FreeChatgpt.ask(question=q)
     print(s)
```

### Comparing `freechatgpt-1.3.2/setup.py` & `freechatgpt-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author abo123456789
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='freechatgpt',
-    version='1.3.2',
+    version='1.3.3',
     description=(
         'free chatgpt api, not need token'
     ),
     keywords=(
         "chatgpt,free"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `freechatgpt-1.3.2/freechatgpt.egg-info/PKG-INFO` & `freechatgpt-1.3.3/freechatgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.2
+Version: 1.3.3
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

