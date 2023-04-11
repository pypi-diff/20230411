# Comparing `tmp/NetGsm-0.0.5.tar.gz` & `tmp/NetGsm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetGsm-0.0.5.tar", last modified: Mon Apr 10 19:31:35 2023, max compression
+gzip compressed data, was "NetGsm-0.0.6.tar", last modified: Tue Apr 11 18:34:52 2023, max compression
```

## Comparing `NetGsm-0.0.5.tar` & `NetGsm-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.599268 NetGsm-0.0.5/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.5/LICENSE
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.597733 NetGsm-0.0.5/NetGsm.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      253 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2023-04-10 19:31:35.000000 NetGsm-0.0.5/NetGsm.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1832 2023-04-10 19:31:35.599127 NetGsm-0.0.5/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1328 2022-11-20 10:57:16.000000 NetGsm-0.0.5/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-10 19:31:35.598808 NetGsm-0.0.5/netgsm/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.5/netgsm/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1096 2023-04-10 19:15:27.000000 NetGsm-0.0.5/netgsm/error_code.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.5/netgsm/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2492 2023-04-10 19:31:01.000000 NetGsm-0.0.5/netgsm/service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-10 19:31:35.599313 NetGsm-0.0.5/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2023-04-10 19:31:01.000000 NetGsm-0.0.5/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.285769 NetGsm-0.0.6/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.6/LICENSE
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.284305 NetGsm-0.0.6/NetGsm.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      253 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 18:34:52.285638 NetGsm-0.0.6/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1430 2023-04-10 19:34:03.000000 NetGsm-0.0.6/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.285344 NetGsm-0.0.6/netgsm/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.6/netgsm/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1096 2023-04-10 19:15:27.000000 NetGsm-0.0.6/netgsm/error_code.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.6/netgsm/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2628 2023-04-11 18:33:32.000000 NetGsm-0.0.6/netgsm/service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-11 18:34:52.285813 NetGsm-0.0.6/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2023-04-11 18:34:45.000000 NetGsm-0.0.6/setup.py
```

### Comparing `NetGsm-0.0.5/LICENSE` & `NetGsm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.5/NetGsm.egg-info/PKG-INFO` & `NetGsm-0.0.6/NetGsm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.5
+Version: 0.0.6
 Summary: NetGsm Sms Client Python package
-Home-page: https://github.com/blueromans/netgsm.git
+Home-page: https://github.com/blueromans/NetGsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
-Project-URL: Bug Tracker, https://github.com/blueromans/netgsm/issues
+Project-URL: Bug Tracker, https://github.com/blueromans/NetGsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/NetGsm.svg)](https://pypi.python.org/pypi/NetGsm)
+
 # NetGsm Python PyPackage
 
 NetGsm is the most popular sms provider at Turkey. NetGsm client is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
@@ -42,15 +44,15 @@
     # you can also set user code from environment.
     'user_code': 'net gsm user code', # Default value : None
     # you can also set user password from environment.
     'user_password': 'net gsm user password',  # Default value : None
     'api_url': 'net gsm api url'  # Default value : 'https://api.netgsm.com.tr/sms/send/get'
 }
 sms_service = SmsService(**kwargs)
-sms_service.send(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
+sms_service.send_sms(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
 # header default value : None if you don't pass this value your header is your user code
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `NetGsm-0.0.5/PKG-INFO` & `NetGsm-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.5
+Version: 0.0.6
 Summary: NetGsm Sms Client Python package
-Home-page: https://github.com/blueromans/netgsm.git
+Home-page: https://github.com/blueromans/NetGsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
-Project-URL: Bug Tracker, https://github.com/blueromans/netgsm/issues
+Project-URL: Bug Tracker, https://github.com/blueromans/NetGsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/NetGsm.svg)](https://pypi.python.org/pypi/NetGsm)
+
 # NetGsm Python PyPackage
 
 NetGsm is the most popular sms provider at Turkey. NetGsm client is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
@@ -42,15 +44,15 @@
     # you can also set user code from environment.
     'user_code': 'net gsm user code', # Default value : None
     # you can also set user password from environment.
     'user_password': 'net gsm user password',  # Default value : None
     'api_url': 'net gsm api url'  # Default value : 'https://api.netgsm.com.tr/sms/send/get'
 }
 sms_service = SmsService(**kwargs)
-sms_service.send(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
+sms_service.send_sms(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
 # header default value : None if you don't pass this value your header is your user code
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `NetGsm-0.0.5/README.md` & `NetGsm-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://img.shields.io/pypi/v/NetGsm.svg)](https://pypi.python.org/pypi/NetGsm)
+
 # NetGsm Python PyPackage
 
 NetGsm is the most popular sms provider at Turkey. NetGsm client is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
@@ -27,15 +29,15 @@
     # you can also set user code from environment.
     'user_code': 'net gsm user code', # Default value : None
     # you can also set user password from environment.
     'user_password': 'net gsm user password',  # Default value : None
     'api_url': 'net gsm api url'  # Default value : 'https://api.netgsm.com.tr/sms/send/get'
 }
 sms_service = SmsService(**kwargs)
-sms_service.send(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
+sms_service.send_sms(phone='Phone Number (5551234567)', message='Your Message', header='Your header')
 # header default value : None if you don't pass this value your header is your user code
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `NetGsm-0.0.5/netgsm/error_code.py` & `NetGsm-0.0.6/netgsm/error_code.py`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.5/netgsm/service.py` & `NetGsm-0.0.6/netgsm/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,30 +31,32 @@
                                 'message': message,
                                 'msgheader': header})
             response = requests.get(
                 f'{self.API_URL}{url}',
                 params=self.params,
             )
             self.check_sms_status(response)
-            return True
+            response = response.text.split(" ")
+            return response[0], response[1]
         except Exception as e:
             raise NetGsmException(e.__str__())
 
     def send_otp(self, phone, message, url='/sms/send/otp', header=None):
         try:
             if header is None:
                 header = self.user_code
             xmlData = f'<?xml version="1.0"?><mainbody><header><usercode>{self.user_code}</usercode><password>{self.user_password}</password><msgheader>{header}</msgheader></header><body><msg><![CDATA[{message}]] ></msg><no>{phone}</no></body></mainbody>'
             headers = {'Content-Type': 'application/xml'}
             response = requests.post(
                 f'{self.API_URL}{url}',
                 data=xmlData, headers=headers
             )
             self.check_sms_status(response)
-            return True
+            response = response.text.split(" ")
+            return response[0], response[1]
         except Exception as e:
             raise NetGsmException(e.__str__())
 
     def check_sms_status(self, response):
         response = response.text
         response_code = re.search('[0-9]+', response).group()
         self.is_sms_send = int(response_code) not in ErrorCode.sms_error_codes
```

### Comparing `NetGsm-0.0.5/setup.py` & `NetGsm-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='NetGsm',
-    version="0.0.5",
+    version="0.0.6",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='NetGsm Sms Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/blueromans/netgsm.git',
+    url='https://github.com/blueromans/NetGsm.git',
     project_urls={
-        "Bug Tracker": "https://github.com/blueromans/netgsm/issues",
+        "Bug Tracker": "https://github.com/blueromans/NetGsm/issues",
     },
     install_requires=['requests'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

