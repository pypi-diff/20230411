# Comparing `tmp/cnocr-2.2.2.2.tar.gz` & `tmp/cnocr-2.2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnocr-2.2.2.2.tar", last modified: Sat Feb 11 15:49:34 2023, max compression
+gzip compressed data, was "dist/cnocr-2.2.2.3.tar", last modified: Tue Apr 11 15:22:31 2023, max compression
```

## Comparing `cnocr-2.2.2.2.tar` & `cnocr-2.2.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.752413 cnocr-2.2.2.2/
--rw-r--r--   0 king       (501) staff       (20)    19838 2023-02-11 15:49:34.750530 cnocr-2.2.2.2/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    15891 2023-02-11 15:49:08.000000 cnocr-2.2.2.2/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.481470 cnocr-2.2.2.2/cnocr/
--rw-r--r--   0 king       (501) staff       (20)     1259 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      893 2023-02-11 15:49:08.000000 cnocr-2.2.2.2/cnocr/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     7025 2022-10-24 08:33:21.000000 cnocr-2.2.2.2/cnocr/app.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.500214 cnocr-2.2.2.2/cnocr/classification/
--rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/classification/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/classification/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/classification/image_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/clf_cli.py
--rw-r--r--   0 king       (501) staff       (20)    18161 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/cli.py
--rw-r--r--   0 king       (501) staff       (20)    17817 2022-09-16 16:03:16.000000 cnocr-2.2.2.2/cnocr/cn_ocr.py
--rw-r--r--   0 king       (501) staff       (20)     7439 2022-07-25 14:40:28.000000 cnocr-2.2.2.2/cnocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.509169 cnocr-2.2.2.2/cnocr/data_utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.2.2.2/cnocr/data_utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/data_utils/aug.py
--rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.2.2.2/cnocr/data_utils/block_shuffle.py
--rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.2.2.2/cnocr/data_utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     4295 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/dataset.py
--rw-r--r--   0 king       (501) staff       (20)    26689 2021-08-26 09:54:36.000000 cnocr-2.2.2.2/cnocr/label_cn.txt
--rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.2.2.2/cnocr/line_split.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.2.2.2/cnocr/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.519159 cnocr-2.2.2.2/cnocr/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.2.2.2/cnocr/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.2.2.2/cnocr/models/ctc.py
--rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.2.2.2/cnocr/models/densenet.py
--rw-r--r--   0 king       (501) staff       (20)     6877 2023-02-11 15:49:08.000000 cnocr-2.2.2.2/cnocr/models/mobilenet.py
--rw-r--r--   0 king       (501) staff       (20)    11059 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/models/ocr_model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.529757 cnocr-2.2.2.2/cnocr/ppocr/
--rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.534139 cnocr-2.2.2.2/cnocr/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     9675 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/ppocr/pp_recognizer.py
--rw-r--r--   0 king       (501) staff       (20)    20044 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/utility.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.740375 cnocr-2.2.2.2/cnocr/ppocr/utils/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/utils/chinese_cht_dict.txt
--rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/utils/en_dict.txt
--rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.2.2.2/cnocr/ppocr/utils/ppocr_keys_v1.txt
--rw-r--r--   0 king       (501) staff       (20)    16147 2023-02-11 15:49:08.000000 cnocr-2.2.2.2/cnocr/recognizer.py
--rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.2.2.2/cnocr/serve.py
--rw-r--r--   0 king       (501) staff       (20)    12496 2023-02-11 15:48:37.000000 cnocr-2.2.2.2/cnocr/trainer.py
--rw-r--r--   0 king       (501) staff       (20)    14819 2022-07-25 14:40:28.000000 cnocr-2.2.2.2/cnocr/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-11 15:49:34.497564 cnocr-2.2.2.2/cnocr.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    19838 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     1134 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       71 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.2.2.2/cnocr.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      238 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-02-11 15:49:34.000000 cnocr-2.2.2.2/cnocr.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-02-11 15:49:34.752653 cnocr-2.2.2.2/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3195 2023-02-11 15:49:08.000000 cnocr-2.2.2.2/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.343070 cnocr-2.2.2.3/
+-rw-r--r--   0 king       (501) staff       (20)    19838 2023-04-11 15:22:31.342154 cnocr-2.2.2.3/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    15891 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.211761 cnocr-2.2.2.3/cnocr/
+-rw-r--r--   0 king       (501) staff       (20)     1259 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      893 2023-04-09 11:55:18.000000 cnocr-2.2.2.3/cnocr/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     7025 2022-10-24 08:33:21.000000 cnocr-2.2.2.3/cnocr/app.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.281894 cnocr-2.2.2.3/cnocr/classification/
+-rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/image_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/clf_cli.py
+-rw-r--r--   0 king       (501) staff       (20)    18161 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    17817 2022-09-16 16:03:16.000000 cnocr-2.2.2.3/cnocr/cn_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)     7439 2022-07-25 14:40:28.000000 cnocr-2.2.2.3/cnocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.290602 cnocr-2.2.2.3/cnocr/data_utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.2.2.3/cnocr/data_utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/data_utils/aug.py
+-rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/data_utils/block_shuffle.py
+-rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/data_utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     4295 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)    26689 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/label_cn.txt
+-rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/line_split.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.301794 cnocr-2.2.2.3/cnocr/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/models/ctc.py
+-rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/models/densenet.py
+-rw-r--r--   0 king       (501) staff       (20)     6877 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/cnocr/models/mobilenet.py
+-rw-r--r--   0 king       (501) staff       (20)    11059 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/models/ocr_model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.312914 cnocr-2.2.2.3/cnocr/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.316938 cnocr-2.2.2.3/cnocr/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     9675 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/ppocr/pp_recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)    20044 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utility.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.326884 cnocr-2.2.2.3/cnocr/ppocr/utils/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/en_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt
+-rw-r--r--   0 king       (501) staff       (20)    16147 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/cnocr/recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.2.2.3/cnocr/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    12496 2023-03-22 14:23:07.000000 cnocr-2.2.2.3/cnocr/trainer.py
+-rw-r--r--   0 king       (501) staff       (20)    14819 2022-07-25 14:40:28.000000 cnocr-2.2.2.3/cnocr/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.276307 cnocr-2.2.2.3/cnocr.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    19838 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     1134 2023-04-11 15:22:31.000000 cnocr-2.2.2.3/cnocr.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       71 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.2.2.3/cnocr.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      233 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-04-11 15:22:31.343265 cnocr-2.2.2.3/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3190 2023-04-09 11:52:59.000000 cnocr-2.2.2.3/setup.py
```

### Comparing `cnocr-2.2.2.2/PKG-INFO` & `cnocr-2.2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.2.2.2
+Version: 2.2.2.3
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Description: <div align="center">
           <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
```

### Comparing `cnocr-2.2.2.2/README.md` & `cnocr-2.2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/__init__.py` & `cnocr-2.2.2.3/cnocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/__version__.py` & `cnocr-2.2.2.3/cnocr/__version__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '2.2.2.2'
+__version__ = '2.2.2.3'
```

### Comparing `cnocr-2.2.2.2/cnocr/app.py` & `cnocr-2.2.2.3/cnocr/app.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/classification/__init__.py` & `cnocr-2.2.2.3/cnocr/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/classification/dataset.py` & `cnocr-2.2.2.3/cnocr/classification/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/classification/image_classifier.py` & `cnocr-2.2.2.3/cnocr/classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/clf_cli.py` & `cnocr-2.2.2.3/cnocr/clf_cli.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/cli.py` & `cnocr-2.2.2.3/cnocr/cli.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/cn_ocr.py` & `cnocr-2.2.2.3/cnocr/cn_ocr.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/consts.py` & `cnocr-2.2.2.3/cnocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/data_utils/aug.py` & `cnocr-2.2.2.3/cnocr/data_utils/aug.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/data_utils/block_shuffle.py` & `cnocr-2.2.2.3/cnocr/data_utils/block_shuffle.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/data_utils/utils.py` & `cnocr-2.2.2.3/cnocr/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/dataset.py` & `cnocr-2.2.2.3/cnocr/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/label_cn.txt` & `cnocr-2.2.2.3/cnocr/label_cn.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/line_split.py` & `cnocr-2.2.2.3/cnocr/line_split.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/lr_scheduler.py` & `cnocr-2.2.2.3/cnocr/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/models/ctc.py` & `cnocr-2.2.2.3/cnocr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/models/densenet.py` & `cnocr-2.2.2.3/cnocr/models/densenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/models/mobilenet.py` & `cnocr-2.2.2.3/cnocr/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/models/ocr_model.py` & `cnocr-2.2.2.3/cnocr/models/ocr_model.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/consts.py` & `cnocr-2.2.2.3/cnocr/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/postprocess/__init__.py` & `cnocr-2.2.2.3/cnocr/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/postprocess/rec_postprocess.py` & `cnocr-2.2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/pp_recognizer.py` & `cnocr-2.2.2.3/cnocr/ppocr/pp_recognizer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/utility.py` & `cnocr-2.2.2.3/cnocr/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/utils/chinese_cht_dict.txt` & `cnocr-2.2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/ppocr/utils/ppocr_keys_v1.txt` & `cnocr-2.2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/recognizer.py` & `cnocr-2.2.2.3/cnocr/recognizer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/serve.py` & `cnocr-2.2.2.3/cnocr/serve.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/trainer.py` & `cnocr-2.2.2.3/cnocr/trainer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr/utils.py` & `cnocr-2.2.2.3/cnocr/utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/cnocr.egg-info/PKG-INFO` & `cnocr-2.2.2.3/cnocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.2.2.2
+Version: 2.2.2.3
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Description: <div align="center">
           <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
```

### Comparing `cnocr-2.2.2.2/cnocr.egg-info/SOURCES.txt` & `cnocr-2.2.2.3/cnocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.2/setup.py` & `cnocr-2.2.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ),
     about,
 )
 
 required = [
     "click",
     "tqdm",
-    "torch>=1.8.0,<2.0",
+    "torch>=1.8.0",
     "torchvision>=0.9.0",
     'numpy',
     "pytorch-lightning>=1.6.0",
     "torchmetrics",
     "pillow>=5.3.0",
     "onnx",
     "onnxruntime",
```

