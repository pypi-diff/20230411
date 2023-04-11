# Comparing `tmp/pymedquery-2.9.0b0.tar.gz` & `tmp/pymedquery-2.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymedquery-2.9.0b0.tar", max compression
+gzip compressed data, was "pymedquery-2.9.1b0.tar", max compression
```

## Comparing `pymedquery-2.9.0b0.tar` & `pymedquery-2.9.1b0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      226 2022-10-26 16:35:54.860924 pymedquery-2.9.0b0/LICENSE.md
--rw-r--r--   0        0        0     9414 2022-10-26 16:35:54.860924 pymedquery-2.9.0b0/README.md
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.860924 pymedquery-2.9.0b0/pymedquery/__init__.py
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.860924 pymedquery-2.9.0b0/pymedquery/config/__init__.py
--rw-r--r--   0        0        0     3308 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/config/config.py
--rw-r--r--   0        0        0      236 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/config/exceptions.py
--rw-r--r--   0        0        0     2641 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/config/logger.py
--rw-r--r--   0        0        0     1779 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/config/logger_object.py
--rw-r--r--   0        0        0        2 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/data/processed/images_uids.gz
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/data/processed/images_uids.pkl
--rw-r--r--   0        0        0      218 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/data/sql/create.sql
--rw-r--r--   0        0        0      385 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/data/sql/test.sql
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/docs/__init__.py
--rw-r--r--   0        0        0      904 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/docs/coverage.svg
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/docs/proj_logging/.gitkeep
--rwxr-xr-x   0        0        0     5358 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/medqueryInit.sh
--rw-r--r--   0        0        0    13033 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/minio_data_handler.py
--rw-r--r--   0        0        0      216 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/mqInit.py
--rw-r--r--   0        0        0    18388 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/pg_crud_handler.py
--rw-r--r--   0        0        0    23145 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/pymq.py
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/sql/default/__init__.py
--rw-r--r--   0        0        0      114 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/sql/default/col_query.sql
--rw-r--r--   0        0        0     1274 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/sql/default/image_affine_default_query.sql
--rw-r--r--   0        0        0     1195 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/sql/default/image_default_query.sql
--rw-r--r--   0        0        0        0 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/src/__init__.py
--rw-r--r--   0        0        0     9272 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/src/helpers.py
--rw-r--r--   0        0        0     5492 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pymedquery/src/utils.py
--rw-r--r--   0        0        0      734 2022-10-26 16:35:54.864925 pymedquery-2.9.0b0/pyproject.toml
--rw-r--r--   0        0        0    10793 2022-10-26 16:36:29.373170 pymedquery-2.9.0b0/setup.py
--rw-r--r--   0        0        0    10260 2022-10-26 16:36:29.373900 pymedquery-2.9.0b0/PKG-INFO
+-rw-r--r--   0        0        0      226 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/LICENSE.md
+-rw-r--r--   0        0        0     9325 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/pymedquery/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/pymedquery/config/__init__.py
+-rw-r--r--   0        0        0     3308 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/pymedquery/config/config.py
+-rw-r--r--   0        0        0      235 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/pymedquery/config/exceptions.py
+-rw-r--r--   0        0        0     2641 2022-11-16 15:04:37.287272 pymedquery-2.9.1b0/pymedquery/config/logger.py
+-rw-r--r--   0        0        0     1779 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/config/logger_object.py
+-rw-r--r--   0        0        0        2 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/data/processed/images_uids.gz
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/data/processed/images_uids.pkl
+-rw-r--r--   0        0        0      218 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/data/sql/create.sql
+-rw-r--r--   0        0        0      385 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/data/sql/test.sql
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/docs/__init__.py
+-rw-r--r--   0        0        0      904 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/docs/coverage.svg
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/docs/proj_logging/.gitkeep
+-rwxr-xr-x   0        0        0     5358 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/medqueryInit.sh
+-rw-r--r--   0        0        0    13033 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/minio_data_handler.py
+-rw-r--r--   0        0        0      216 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/mqInit.py
+-rw-r--r--   0        0        0    18388 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/pg_crud_handler.py
+-rw-r--r--   0        0        0    23106 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/pymq.py
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/sql/default/__init__.py
+-rw-r--r--   0        0        0      114 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/sql/default/col_query.sql
+-rw-r--r--   0        0        0     1274 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/sql/default/image_affine_default_query.sql
+-rw-r--r--   0        0        0     1195 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/sql/default/image_default_query.sql
+-rw-r--r--   0        0        0        0 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/src/__init__.py
+-rw-r--r--   0        0        0     9563 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/src/helpers.py
+-rw-r--r--   0        0        0     5492 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pymedquery/src/utils.py
+-rw-r--r--   0        0        0      734 2022-11-16 15:04:37.291272 pymedquery-2.9.1b0/pyproject.toml
+-rw-r--r--   0        0        0    10704 2022-11-16 15:05:05.692775 pymedquery-2.9.1b0/setup.py
+-rw-r--r--   0        0        0    10171 2022-11-16 15:05:05.693472 pymedquery-2.9.1b0/PKG-INFO
```

### Comparing `pymedquery-2.9.0b0/README.md` & `pymedquery-2.9.1b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# pyMedQuery <img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">
+# pyMedQuery [<img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">](https://neomedsys.io/)
 
 [![py-medquery](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml/badge.svg)](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml) <img src="./pymedquery/docs/coverage.svg"> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 <br>
 
 *pyMedQuery* is the sweet sweet database client for python that allows authenticated users to access medical data in the database MedQuery. The main reason for *pyMedQuery* to exist is to efficiently enable database access via python code that can be integrated into machine learning projects, production systems and data analysis pipelines. We are using SSL/TLS for safe connections and client certifications for authentication in order to keep the database connection highly secure. 
 
 The average user is expected to instantiate the `PyMedQuery()` class and run the methods `extract` or `batch_extract` to extract the necessary data for their given project. If the user wants to use the default SQL script then set the argument `get_all` to true in the `(batch_)extract` method and specify which projectID the data should relate to. The method will then extract all the data belonging to that projectID. Other users might find it usefull to write custom SQL scripts where the argument `format_params` can be passed into the extraction for flexible formating of SQL queries. This is especially useful for applications and pipelines.
 
-More functionalities are coming to *pyMedQuery* in later beta version where `(batch_)upload` and `move_data` will be part of the release. If you have any feedback or ideas to new features or bugs then please get in contact with us.
+If you have any feedback or ideas to new features or bugs then please get in contact with us.
 
-*pyMedQuery* is meant to be a simple and friendly. We hope you'll like it! Check out the tutorial script for some examples. Also note that advanced user can directly connect to the RDBMS and data lake for more complex operations.   
+*pyMedQuery* is meant to be a simple and friendly. We hope you'll like it! Check out the tutorial script for some examples. 
 
 ### Quickstart Guide
 
 #### 1. installing and completing the settings (this is a one time procedure)
 
 1. Use poetry or any other kind of dependency manager to install the package.
 
@@ -90,18 +90,18 @@
         `project_id`. If the data has corresponding masks, then set `include_mask` to true
 
 ```python
 from pymedquery import pymq
         
 # instantiate the class
 mq = pymq.PyMedQuery()
-# User limit to set a maximum number of patients to include in the extraction
+# Use the limit argument to set a maximum number of patients to include in the extraction
 small_data_sample = mq.extract(get_all=True, get_affines=True, project_id='fancyID', limit=200, include_mask=False)
         # do more stuff here
-        # save processed data to your local disk with e.g. in HDF5 or pickle
+        # save processed data to your local disk with e.g. in HDF5 or pickle. Let go of big cluttering file systems!
 ```
 
 
 1.  Extracting a small data sample with a custom and formatable SQL script where data has corresponding masks.
         A mask in this case is a finished image segmentation.
 
 ```python
@@ -134,16 +134,16 @@
 
 ```python
 from pymedquery import pymq
 
 # instantiate the class
 mq = pymq.PyMedQuery()
 
-# Setting batch size to 400
-large_data = mq.batch_extract(get_all=True, project_id='fancyID', batch_size=400)
+# Setting batch size to 200 volumes with 150 slices each. That corresponds to 30000 2D images in each batch
+large_data = mq.batch_extract(get_all=True, project_id='fancyID', batch_size=200)
 for batch in large_data:
         # do more stuff here:
         # 1. process data
         # 2. split train, test and val
         # 3. save processed data to your local disk with e.g. HDF5
 ```
 ##### NOTE: it's advisable to save your processed data in a HDF5 file as it's easy to structure your data in the file and it can be lazy loaded into other scripts for subsequent analyses.
```

### Comparing `pymedquery-2.9.0b0/pymedquery/config/config.py` & `pymedquery-2.9.1b0/pymedquery/config/config.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/config/logger.py` & `pymedquery-2.9.1b0/pymedquery/config/logger.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/config/logger_object.py` & `pymedquery-2.9.1b0/pymedquery/config/logger_object.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/docs/coverage.svg` & `pymedquery-2.9.1b0/pymedquery/docs/coverage.svg`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/medqueryInit.sh` & `pymedquery-2.9.1b0/pymedquery/medqueryInit.sh`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/minio_data_handler.py` & `pymedquery-2.9.1b0/pymedquery/minio_data_handler.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/pg_crud_handler.py` & `pymedquery-2.9.1b0/pymedquery/pg_crud_handler.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/pymq.py` & `pymedquery-2.9.1b0/pymedquery/pymq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pymedquery.pg_crud_handler import CRUD
 from pymedquery.minio_data_handler import MinioHandler
 from pymedquery.config.logger_object import Logger
 from pymedquery.config import config
-from pymedquery.config.exceptions import NoRecordsFound, CommitBounced
+from pymedquery.config.exceptions import NoRecordsFound, CommitBouncedError
 from pymedquery.src.helpers import (
-    batch_maker, encode_payload, make_uid_list, check_batch_size
+    batch_maker, encode_payload, make_uid_list, check_batch_size, timer
 )
 
 import os
 import psycopg2
 import numpy as np
 from minio.error import S3Error
 from time import sleep
@@ -186,14 +186,15 @@
             self.crud.close_connection()
         if colnames:
             return colnames
         else:
             self.log.error('I tried to fetch column names but got an empty result. Lordy lord!')
             raise psycopg2.OperationalError()
 
+    @timer
     def extract(
             self, get_all: bool, get_affines: bool = True, project_id: Optional[str] = None, limit: Optional[Union[int, str]] = 'NULL',
             include_mask: Optional[bool] = None, format_params: Optional[dict] = None, sql_file_path: Optional[str] = None,
             bucket_name: Optional[str] = 'multimodal-images', verbose: bool = False, image_extraction: bool = True,
             reset_connection: bool = False, post_close_connection: bool = False
     ) -> Union[Dict[str, List[np.ndarray]], Dict[str, List[any]]]:
         """extract is the public method that is exposed to the user for data extraction of small image quantites. The method is
@@ -241,15 +242,15 @@
                 batch_extract=False
             )
             if not all_uids[0]:
                 raise NoRecordsFound('Your query returned an empty result. Please check your query or projectID')
 
             if len(all_uids[0]) > 30:
                 self.log.warning(f"""
-                    Top of the morning! This is just a heads up my good man or woman; you are about to
+                    To
                     extract {len(all_uids)} 3D images in one go and you might run into a memory
                     allocation error. Consider using batch_extract with a specific batch size to mitigate
                     potential problems.
                     """)
                 sleep(5)
 
             if isinstance(all_uids[0], list) and len(all_uids[0]) > 1:
@@ -361,17 +362,18 @@
             sample: Generator[List[str], None, None] = batch_maker(iterable=all_uids[0], batch_size=batch_size)
 
             # run bathes out of the sample and yield them one at the time
             for _batch in sample:
                 # extract the images by using the MinioHandler class method
                 blobby: Dict[str, List[np.ndarray]] = self.mh.get_blobs(bucket_name=bucket_name, blob_list=_batch, image_extraction=image_extraction)
                 yield blobby
-        except(AttributeError, psycopg2.Error, S3Error) as e:
+        except (AttributeError, psycopg2.Error, S3Error) as e:
             self.log.error(f'failed to extract the following uids {all_uids} with the error: {e}')
 
+    @timer
     def upload(
             self, records: Dict[Union[str, int, float], Any], table_name: str,
             verbose: bool = False, meta: Union[Dict[str, str], None] = None,
             bucket_name: str = config.BUCKET_NAME, post_close_connection: bool = False,
             ignore_conflict: bool = False) -> NoReturn:
         """upload is the method that allows users to upload data to MedQuery without having to deal with
         two wrappers. You simply specify the name of the table you are writing to and include the data as
@@ -434,25 +436,26 @@
             """)
 
         self.log.info(f'Uploading records to {table_name} in MedQuery')
         try:
             self.crud.insert(columns=col_names, records=[record_values], table=table_name, ignore_conflict=ignore_conflict)
             self.crud.commit()
             if self.crud.log.error_log:
-                raise CommitBounced(f'{self.crud.log.error_log}')
+                raise CommitBouncedError(f'{self.crud.log.error_log}')
             # the index 1 in the tuple is supposed to be where the blob shoud be entered by the client
             for record_key, record_tuple in records.items():
                 if record_tuple[1] is not None:
                     record_value, record_blob = record_tuple
                     if isinstance(record_blob, np.ndarray):
                         meta: Dict[str, str] = {
                             'img_shape': str(record_blob.shape),
                             'dtype': str(record_blob.dtype)
                         }
                     payload, payload_size = encode_payload(payload=record_blob)
+
                     # Make sure that the bytes reading starts from the beginning
                     if hasattr(payload, 'getbuffer'):
                         payload.seek(0)
                     else:
                         raise ValueError('payload is not a IO object')
 
                     # NOTE! we need to make sure that the multimodal bucket dose not get cluttered with
```

### Comparing `pymedquery-2.9.0b0/pymedquery/sql/default/image_affine_default_query.sql` & `pymedquery-2.9.1b0/pymedquery/sql/default/image_affine_default_query.sql`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/sql/default/image_default_query.sql` & `pymedquery-2.9.1b0/pymedquery/sql/default/image_default_query.sql`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pymedquery/src/helpers.py` & `pymedquery-2.9.1b0/pymedquery/src/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,30 +242,32 @@
     dict_.clear()
     for list_ in payload:
         for idx, col in enumerate(colnames):
             dict_[col].append(list_[idx])
     return dict_
 
 
-def payload_transform(payload: bytes, shape_str: str, dtype_str: str, image_extraction: bool = True) -> Union[np.ndarray, bytes]:
+def payload_transform(payload: bytes, dtype_str: str, shape_str: Union[str, None] = None, image_extraction: bool = True) -> Union[np.ndarray, bytes]:
     """payload_transform takes an API response of an image as input and converts it back from bytes
     to a numpy array.
 
     Parameters
     ----------
     payload : bytes
         payload
-    shape_str : str
-        shape_str
+    shape_str : str | None
+        shape_str is the shape of the image that you are extracting
     dtype_str : str
-        dtype_str
+        dtype_str referst to the datatype of your blob, e.g. int8 or float64
+    image_extraction : bool
+        image_extraction is a boolean flag that will either set the processing to image or blob transform
 
     Returns
     -------
-    np.ndarray
+    np.ndarray | bytes
 
     """
     # decompress the payload
     payload_decomp = blosc.decompress(payload)
     if image_extraction:
         if not shape_str:
             raise TypeError(f'I expected a shape string for the image but got {shape_str}')
@@ -304,15 +306,15 @@
     try:
         bytes_compressed = blosc.compress(bytes(payload), cname='zstd')
     except OverflowError as e:
         log.warning(f"""
         We are getting an overflow error on the payload: {e}.
         Shifting to pkl.dumps to see if it solves the problem.""")
         bytes_compressed = blosc.compress(pkl.dumps(payload), cname='zstd')
-    except ValueError as e:
+    except (TypeError, ValueError) as e:
         log.warning(f'We are getting an error {e}. I will try to json dump your payload for bytes conversion.')
         bytes_compressed = blosc.compress(bytes(json.dumps(payload)), cname='zstd')
     finally:
         byte_buffer = io.BytesIO(bytes_compressed)
         return byte_buffer, byte_buffer.getbuffer().nbytes
```

### Comparing `pymedquery-2.9.0b0/pymedquery/src/utils.py` & `pymedquery-2.9.1b0/pymedquery/src/utils.py`

 * *Files identical despite different names*

### Comparing `pymedquery-2.9.0b0/pyproject.toml` & `pymedquery-2.9.1b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymedquery"
-version = "v2.9.0-beta"
+version = "v2.9.1-beta"
 
 description = "This is a python client for the medical-database MedQuery"
 authors = ["Jon E Nesvold <jon.nesvold@pm.me>"]
 license = "LICENSE.md"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pymedquery-2.9.0b0/setup.py` & `pymedquery-2.9.1b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'tqdm>=4.61.2,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['pymq-init = pymedquery.mqInit:run_setup']}
 
 setup_kwargs = {
     'name': 'pymedquery',
-    'version': '2.9.0b0',
+    'version': '2.9.1b0',
     'description': 'This is a python client for the medical-database MedQuery',
-    'long_description': '# pyMedQuery <img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">\n\n[![py-medquery](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml/badge.svg)](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml) <img src="./pymedquery/docs/coverage.svg"> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)\n[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)\n[![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)\n\n<br>\n\n*pyMedQuery* is the sweet sweet database client for python that allows authenticated users to access medical data in the database MedQuery. The main reason for *pyMedQuery* to exist is to efficiently enable database access via python code that can be integrated into machine learning projects, production systems and data analysis pipelines. We are using SSL/TLS for safe connections and client certifications for authentication in order to keep the database connection highly secure. \n\nThe average user is expected to instantiate the `PyMedQuery()` class and run the methods `extract` or `batch_extract` to extract the necessary data for their given project. If the user wants to use the default SQL script then set the argument `get_all` to true in the `(batch_)extract` method and specify which projectID the data should relate to. The method will then extract all the data belonging to that projectID. Other users might find it usefull to write custom SQL scripts where the argument `format_params` can be passed into the extraction for flexible formating of SQL queries. This is especially useful for applications and pipelines.\n\nMore functionalities are coming to *pyMedQuery* in later beta version where `(batch_)upload` and `move_data` will be part of the release. If you have any feedback or ideas to new features or bugs then please get in contact with us.\n\n*pyMedQuery* is meant to be a simple and friendly. We hope you\'ll like it! Check out the tutorial script for some examples. Also note that advanced user can directly connect to the RDBMS and data lake for more complex operations.   \n\n### Quickstart Guide\n\n#### 1. installing and completing the settings (this is a one time procedure)\n\n1. Use poetry or any other kind of dependency manager to install the package.\n\n```$ poetry add pymedquery```\n\n2. If you are using poetry then run `poetry run pymq-init` and follow the setup of the database authentication. (A valid username, password and cert files are currently required in forehand) The setup script will guide you through the authentication. A more streamlined way to authenticate via a MedQuery\'s CLI is in the roadmap for 2022.\n\n<details>\n<summary>Open this drop down if you want to do the authentication manually or you are on Windows with no bash in power shell:</summary>\n<br>\n\n2. Store the certification and key files for postgres somwhere safe on your machine. (you will receive the database credentials from the admins)\n\n3. Set environment variables on your system for the file paths that point to the cert and key files you received for the database. We recommended to put the commands in your .zshrc or .bashrc.\n\n```\n$ echo \'export PGSSLCERT=file_path_to_client_crt\' >> ~/<.your_rc_file>\n$ echo \'export PGSSLROOTCERT=file_path_to_ca_crt\' >> ~/<.your_rc_file>\n$ echo \'export PGSSLKEY=file_path_to_client_key\' >> ~/<.your_rc_file>\n```\n\nSet correct permissions on your client key in order for the database to read it.\n```\n$ chmod 600 $PGSSLKEY\n```\n\nDo the equivalent on windows with\n\n```\nsetx PGSSLCERT file_path_to_client_crt\nsetx PPGSSLROOTCERT file_path_to_ca_crt\nsetx PGSSLKEY file_path_to_client_key\n```\n\n<details>\n<summary>Windows is not a straight forward when setting 600 permission but you can follow these steps:</summary>\n<br>\n\n- Right-click on the target file and select properties then select Security Tab\n\n- Click Advanced and then make sure inheritance is disabled.\n\n- Click apply and then click Edit in the security menu\n\n- Remove all users except Admin user, which should have full control *Admin account should have all checkboxes checked on Allow column except special permission.\n\n- Click Apply and then click OK :)\n        \n<br>\n</details>\n\n\n4. Also include the username and password in your rc file as environment variables:\n\n```\n<your-rc-file>\n# (env vars to fill out that pyMedQuery will pick up on)\nexport MQUSER=\'username-to-medquery\'\nexport MQPWD=\'password-to-medquery\'\nexport DATABASE=\'medquery\'\n```\n##### NOTE! The env var names is a strict convention. The program will not work if you use other names.\n\n<br>\n</details>\n\n#### 2. Examples of how to run the basics\n\n0.  Extracting a small data sample by using the default SQL script and a certain `project_id`. Given that `get_all` is true then you can adjust\n        how many patients to include in your query by filling in limit. If you leave it blank then the query will retrieve all records in the\n        `project_id`. If the data has corresponding masks, then set `include_mask` to true\n\n```python\nfrom pymedquery import pymq\n        \n# instantiate the class\nmq = pymq.PyMedQuery()\n# User limit to set a maximum number of patients to include in the extraction\nsmall_data_sample = mq.extract(get_all=True, get_affines=True, project_id=\'fancyID\', limit=200, include_mask=False)\n        # do more stuff here\n        # save processed data to your local disk with e.g. in HDF5 or pickle\n```\n\n\n1.  Extracting a small data sample with a custom and formatable SQL script where data has corresponding masks.\n        A mask in this case is a finished image segmentation.\n\n```python\nfrom pymedquery import pymq\nfrom config import config\n\nsql_file_path =  # file-path-to-the-pre-written-sql-script\n# instantiate the class\nmq = pymq.PyMedQuery()\n        \n# The formatable parameters will be inserted into the custom SQL scrip and thus extracting data belonging to\n# \'fancy_id\' from only the year 2012 and for only women between 40 and 49. The SQL script must include the\n# format syntax {project_id}, {start_time}..., etc. for the filtering to happen.\nFORMAT_PARAMS = {\n        \'project_id\': \'fancy_id\',\n        \'start_time\': \'2012-01-01\',\n        \'end_time\': \'2012-12-31\',\n        \'gender\': \'F\',\n        \'age_group\': \'40-49\'\n        }\n        \n# Note that the SQL file path is given by a configuartion script called config\n# Lets set get_affines to False in order to include the affine matrices as well\nsmall_data_sample = mq.extract(get_all=False, get_affines=False, format_params=FORMAT_PARAMS, sql_file_path=config.SQL_FILE_PATH, include_mask=True)\n        # do more stuff\n        # save processed data to local disk with e.g. in HDF5 orpickle\n```\n        \n2. Extracting large amounts of data (this step could either be done with a custom SQL file or without. The example is given with the default SQL file for brevity.\n\n```python\nfrom pymedquery import pymq\n\n# instantiate the class\nmq = pymq.PyMedQuery()\n\n# Setting batch size to 400\nlarge_data = mq.batch_extract(get_all=True, project_id=\'fancyID\', batch_size=400)\nfor batch in large_data:\n        # do more stuff here:\n        # 1. process data\n        # 2. split train, test and val\n        # 3. save processed data to your local disk with e.g. HDF5\n```\n##### NOTE: it\'s advisable to save your processed data in a HDF5 file as it\'s easy to structure your data in the file and it can be lazy loaded into other scripts for subsequent analyses.\n        \n3. Uploading data into MedQuery. You can either create your own table in a specific part of MedQuery or use a pre-existing table (there will be tables for the data and model versioning and storing)\n\n```python\nfrom pymedquery import pymq\n\n# instantiate the class\nmq = mq.PyMedQuery()\n \n# load the model file into the program\nmodel_file = load_model()\n\n# We are done with a model and I we want to save it back to MedQuery with the proper version for other researchers and applications to use.\n# Befor we make the upload, we need to have dictionary containing the records to upload. The dictionary keys must align with sorting of the table coulumns. Make sure that this is correct befor uploading. Use the \'verbose\' argument if you want to make sure that you structure is correct.\n# the structure of the records dict should be: {key: (record_value, blob),....}\nrecords Dict[str, Tuple[Any, Any]: = {\n        # record_value: blob (not all record_values have a corresponding blob)\n        \'timestamp\': (datetime.datetime.now(), None),\n        \'model_id\': (\'model_fasde32r345t45c324xd\', model_file),\n        \'model_version\': (\'modelw_v1.1.0\', None),\n        \'project_owner\': (\'Schlomo Cohen\': None)\n        }\n\n \n# Upload the records with pymedquery\nmq.upload(records=records, table_name=\'model_artifacts\', verbose=True, image_extraction=False)\n          \n# NOTE! Blobs for record_values are not supported at the moment\n```\n\n##### The records dict aligns with the `model_artifacts` table which has the following columns:\n        \n      | time | model_id | model_version | project_owner |\n\n##### The project pyMedQuery is currently in Beta and we are looking for Beta tester. You have to be affiliated or employed at UHO to take part in the Beta release\n',
+    'long_description': '# pyMedQuery [<img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">](https://neomedsys.io/)\n\n[![py-medquery](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml/badge.svg)](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml) <img src="./pymedquery/docs/coverage.svg"> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)\n[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)\n[![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)\n\n<br>\n\n*pyMedQuery* is the sweet sweet database client for python that allows authenticated users to access medical data in the database MedQuery. The main reason for *pyMedQuery* to exist is to efficiently enable database access via python code that can be integrated into machine learning projects, production systems and data analysis pipelines. We are using SSL/TLS for safe connections and client certifications for authentication in order to keep the database connection highly secure. \n\nThe average user is expected to instantiate the `PyMedQuery()` class and run the methods `extract` or `batch_extract` to extract the necessary data for their given project. If the user wants to use the default SQL script then set the argument `get_all` to true in the `(batch_)extract` method and specify which projectID the data should relate to. The method will then extract all the data belonging to that projectID. Other users might find it usefull to write custom SQL scripts where the argument `format_params` can be passed into the extraction for flexible formating of SQL queries. This is especially useful for applications and pipelines.\n\nIf you have any feedback or ideas to new features or bugs then please get in contact with us.\n\n*pyMedQuery* is meant to be a simple and friendly. We hope you\'ll like it! Check out the tutorial script for some examples. \n\n### Quickstart Guide\n\n#### 1. installing and completing the settings (this is a one time procedure)\n\n1. Use poetry or any other kind of dependency manager to install the package.\n\n```$ poetry add pymedquery```\n\n2. If you are using poetry then run `poetry run pymq-init` and follow the setup of the database authentication. (A valid username, password and cert files are currently required in forehand) The setup script will guide you through the authentication. A more streamlined way to authenticate via a MedQuery\'s CLI is in the roadmap for 2022.\n\n<details>\n<summary>Open this drop down if you want to do the authentication manually or you are on Windows with no bash in power shell:</summary>\n<br>\n\n2. Store the certification and key files for postgres somwhere safe on your machine. (you will receive the database credentials from the admins)\n\n3. Set environment variables on your system for the file paths that point to the cert and key files you received for the database. We recommended to put the commands in your .zshrc or .bashrc.\n\n```\n$ echo \'export PGSSLCERT=file_path_to_client_crt\' >> ~/<.your_rc_file>\n$ echo \'export PGSSLROOTCERT=file_path_to_ca_crt\' >> ~/<.your_rc_file>\n$ echo \'export PGSSLKEY=file_path_to_client_key\' >> ~/<.your_rc_file>\n```\n\nSet correct permissions on your client key in order for the database to read it.\n```\n$ chmod 600 $PGSSLKEY\n```\n\nDo the equivalent on windows with\n\n```\nsetx PGSSLCERT file_path_to_client_crt\nsetx PPGSSLROOTCERT file_path_to_ca_crt\nsetx PGSSLKEY file_path_to_client_key\n```\n\n<details>\n<summary>Windows is not a straight forward when setting 600 permission but you can follow these steps:</summary>\n<br>\n\n- Right-click on the target file and select properties then select Security Tab\n\n- Click Advanced and then make sure inheritance is disabled.\n\n- Click apply and then click Edit in the security menu\n\n- Remove all users except Admin user, which should have full control *Admin account should have all checkboxes checked on Allow column except special permission.\n\n- Click Apply and then click OK :)\n        \n<br>\n</details>\n\n\n4. Also include the username and password in your rc file as environment variables:\n\n```\n<your-rc-file>\n# (env vars to fill out that pyMedQuery will pick up on)\nexport MQUSER=\'username-to-medquery\'\nexport MQPWD=\'password-to-medquery\'\nexport DATABASE=\'medquery\'\n```\n##### NOTE! The env var names is a strict convention. The program will not work if you use other names.\n\n<br>\n</details>\n\n#### 2. Examples of how to run the basics\n\n0.  Extracting a small data sample by using the default SQL script and a certain `project_id`. Given that `get_all` is true then you can adjust\n        how many patients to include in your query by filling in limit. If you leave it blank then the query will retrieve all records in the\n        `project_id`. If the data has corresponding masks, then set `include_mask` to true\n\n```python\nfrom pymedquery import pymq\n        \n# instantiate the class\nmq = pymq.PyMedQuery()\n# Use the limit argument to set a maximum number of patients to include in the extraction\nsmall_data_sample = mq.extract(get_all=True, get_affines=True, project_id=\'fancyID\', limit=200, include_mask=False)\n        # do more stuff here\n        # save processed data to your local disk with e.g. in HDF5 or pickle. Let go of big cluttering file systems!\n```\n\n\n1.  Extracting a small data sample with a custom and formatable SQL script where data has corresponding masks.\n        A mask in this case is a finished image segmentation.\n\n```python\nfrom pymedquery import pymq\nfrom config import config\n\nsql_file_path =  # file-path-to-the-pre-written-sql-script\n# instantiate the class\nmq = pymq.PyMedQuery()\n        \n# The formatable parameters will be inserted into the custom SQL scrip and thus extracting data belonging to\n# \'fancy_id\' from only the year 2012 and for only women between 40 and 49. The SQL script must include the\n# format syntax {project_id}, {start_time}..., etc. for the filtering to happen.\nFORMAT_PARAMS = {\n        \'project_id\': \'fancy_id\',\n        \'start_time\': \'2012-01-01\',\n        \'end_time\': \'2012-12-31\',\n        \'gender\': \'F\',\n        \'age_group\': \'40-49\'\n        }\n        \n# Note that the SQL file path is given by a configuartion script called config\n# Lets set get_affines to False in order to include the affine matrices as well\nsmall_data_sample = mq.extract(get_all=False, get_affines=False, format_params=FORMAT_PARAMS, sql_file_path=config.SQL_FILE_PATH, include_mask=True)\n        # do more stuff\n        # save processed data to local disk with e.g. in HDF5 orpickle\n```\n        \n2. Extracting large amounts of data (this step could either be done with a custom SQL file or without. The example is given with the default SQL file for brevity.\n\n```python\nfrom pymedquery import pymq\n\n# instantiate the class\nmq = pymq.PyMedQuery()\n\n# Setting batch size to 200 volumes with 150 slices each. That corresponds to 30000 2D images in each batch\nlarge_data = mq.batch_extract(get_all=True, project_id=\'fancyID\', batch_size=200)\nfor batch in large_data:\n        # do more stuff here:\n        # 1. process data\n        # 2. split train, test and val\n        # 3. save processed data to your local disk with e.g. HDF5\n```\n##### NOTE: it\'s advisable to save your processed data in a HDF5 file as it\'s easy to structure your data in the file and it can be lazy loaded into other scripts for subsequent analyses.\n        \n3. Uploading data into MedQuery. You can either create your own table in a specific part of MedQuery or use a pre-existing table (there will be tables for the data and model versioning and storing)\n\n```python\nfrom pymedquery import pymq\n\n# instantiate the class\nmq = mq.PyMedQuery()\n \n# load the model file into the program\nmodel_file = load_model()\n\n# We are done with a model and I we want to save it back to MedQuery with the proper version for other researchers and applications to use.\n# Befor we make the upload, we need to have dictionary containing the records to upload. The dictionary keys must align with sorting of the table coulumns. Make sure that this is correct befor uploading. Use the \'verbose\' argument if you want to make sure that you structure is correct.\n# the structure of the records dict should be: {key: (record_value, blob),....}\nrecords Dict[str, Tuple[Any, Any]: = {\n        # record_value: blob (not all record_values have a corresponding blob)\n        \'timestamp\': (datetime.datetime.now(), None),\n        \'model_id\': (\'model_fasde32r345t45c324xd\', model_file),\n        \'model_version\': (\'modelw_v1.1.0\', None),\n        \'project_owner\': (\'Schlomo Cohen\': None)\n        }\n\n \n# Upload the records with pymedquery\nmq.upload(records=records, table_name=\'model_artifacts\', verbose=True, image_extraction=False)\n          \n# NOTE! Blobs for record_values are not supported at the moment\n```\n\n##### The records dict aligns with the `model_artifacts` table which has the following columns:\n        \n      | time | model_id | model_version | project_owner |\n\n##### The project pyMedQuery is currently in Beta and we are looking for Beta tester. You have to be affiliated or employed at UHO to take part in the Beta release\n',
     'author': 'Jon E Nesvold',
     'author_email': 'jon.nesvold@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pymedquery-2.9.0b0/PKG-INFO` & `pymedquery-2.9.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymedquery
-Version: 2.9.0b0
+Version: 2.9.1b0
 Summary: This is a python client for the medical-database MedQuery
 License: LICENSE.md
 Author: Jon E Nesvold
 Author-email: jon.nesvold@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,29 +17,29 @@
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: python-dotenv (>=0.18.0,<0.19.0)
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
 Description-Content-Type: text/markdown
 
-# pyMedQuery <img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">
+# pyMedQuery [<img align="right" width="120" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/183247351-53e45de2-09cf-4344-be30-120d8a744d5f.png">](https://neomedsys.io/)
 
 [![py-medquery](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml/badge.svg)](https://github.com/CRAI-OUS/py-medquery/actions/workflows/pymedquery.yaml) <img src="./pymedquery/docs/coverage.svg"> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 <br>
 
 *pyMedQuery* is the sweet sweet database client for python that allows authenticated users to access medical data in the database MedQuery. The main reason for *pyMedQuery* to exist is to efficiently enable database access via python code that can be integrated into machine learning projects, production systems and data analysis pipelines. We are using SSL/TLS for safe connections and client certifications for authentication in order to keep the database connection highly secure. 
 
 The average user is expected to instantiate the `PyMedQuery()` class and run the methods `extract` or `batch_extract` to extract the necessary data for their given project. If the user wants to use the default SQL script then set the argument `get_all` to true in the `(batch_)extract` method and specify which projectID the data should relate to. The method will then extract all the data belonging to that projectID. Other users might find it usefull to write custom SQL scripts where the argument `format_params` can be passed into the extraction for flexible formating of SQL queries. This is especially useful for applications and pipelines.
 
-More functionalities are coming to *pyMedQuery* in later beta version where `(batch_)upload` and `move_data` will be part of the release. If you have any feedback or ideas to new features or bugs then please get in contact with us.
+If you have any feedback or ideas to new features or bugs then please get in contact with us.
 
-*pyMedQuery* is meant to be a simple and friendly. We hope you'll like it! Check out the tutorial script for some examples. Also note that advanced user can directly connect to the RDBMS and data lake for more complex operations.   
+*pyMedQuery* is meant to be a simple and friendly. We hope you'll like it! Check out the tutorial script for some examples. 
 
 ### Quickstart Guide
 
 #### 1. installing and completing the settings (this is a one time procedure)
 
 1. Use poetry or any other kind of dependency manager to install the package.
 
@@ -113,18 +113,18 @@
         `project_id`. If the data has corresponding masks, then set `include_mask` to true
 
 ```python
 from pymedquery import pymq
         
 # instantiate the class
 mq = pymq.PyMedQuery()
-# User limit to set a maximum number of patients to include in the extraction
+# Use the limit argument to set a maximum number of patients to include in the extraction
 small_data_sample = mq.extract(get_all=True, get_affines=True, project_id='fancyID', limit=200, include_mask=False)
         # do more stuff here
-        # save processed data to your local disk with e.g. in HDF5 or pickle
+        # save processed data to your local disk with e.g. in HDF5 or pickle. Let go of big cluttering file systems!
 ```
 
 
 1.  Extracting a small data sample with a custom and formatable SQL script where data has corresponding masks.
         A mask in this case is a finished image segmentation.
 
 ```python
@@ -157,16 +157,16 @@
 
 ```python
 from pymedquery import pymq
 
 # instantiate the class
 mq = pymq.PyMedQuery()
 
-# Setting batch size to 400
-large_data = mq.batch_extract(get_all=True, project_id='fancyID', batch_size=400)
+# Setting batch size to 200 volumes with 150 slices each. That corresponds to 30000 2D images in each batch
+large_data = mq.batch_extract(get_all=True, project_id='fancyID', batch_size=200)
 for batch in large_data:
         # do more stuff here:
         # 1. process data
         # 2. split train, test and val
         # 3. save processed data to your local disk with e.g. HDF5
 ```
 ##### NOTE: it's advisable to save your processed data in a HDF5 file as it's easy to structure your data in the file and it can be lazy loaded into other scripts for subsequent analyses.
```

