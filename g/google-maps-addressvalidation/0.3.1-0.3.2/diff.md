# Comparing `tmp/google-maps-addressvalidation-0.3.1.tar.gz` & `tmp/google-maps-addressvalidation-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-addressvalidation-0.3.1.tar", last modified: Mon Mar 27 14:58:55 2023, max compression
+gzip compressed data, was "google-maps-addressvalidation-0.3.2.tar", last modified: Tue Apr 11 16:32:47 2023, max compression
```

## Comparing `google-maps-addressvalidation-0.3.1.tar` & `google-maps-addressvalidation-0.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4820 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3894 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.485861 google-maps-addressvalidation-0.3.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.485861 google-maps-addressvalidation-0.3.1/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/
--rw-rw-r--   0 root         (0)     1003     1974 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/
--rw-rw-r--   0 root         (0)     1003     1671 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1505 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/__init__.py
--rw-rw-r--   0 root         (0)     1003    15687 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/async_client.py
--rw-rw-r--   0 root         (0)     1003    24571 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6718 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13582 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13812 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18770 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.489861 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/
--rw-rw-r--   0 root         (0)     1003     1343 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9109 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/address.py
--rw-rw-r--   0 root         (0)     1003    15058 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/address_validation_service.py
--rw-rw-r--   0 root         (0)     1003     4435 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/geocode.py
--rw-rw-r--   0 root         (0)     1003     2059 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003    11484 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/usps_data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/
--rw-r--r--   0 root         (0)     1003     4820 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1931 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      348 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:55.000000 google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3001 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:55.493862 google-maps-addressvalidation-0.3.1/tests/unit/gapic/addressvalidation_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/tests/unit/gapic/addressvalidation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    76826 2023-03-27 14:55:35.000000 google-maps-addressvalidation-0.3.1/tests/unit/gapic/addressvalidation_v1/test_address_validation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4820 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3894 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.856226 google-maps-addressvalidation-0.3.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.856226 google-maps-addressvalidation-0.3.2/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/
+-rw-rw-r--   0 root         (0)     1003     1974 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/
+-rw-rw-r--   0 root         (0)     1003     1671 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1505 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/
+-rw-rw-r--   0 root         (0)     1003      781 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15687 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24571 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6718 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13582 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13812 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18770 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.860226 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1343 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9240 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/address.py
+-rw-rw-r--   0 root         (0)     1003    15189 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/address_validation_service.py
+-rw-rw-r--   0 root         (0)     1003     4435 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/geocode.py
+-rw-rw-r--   0 root         (0)     1003     2175 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003    11749 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/usps_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/
+-rw-r--r--   0 root         (0)     1003     4820 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1931 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      348 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-11 16:32:47.000000 google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3001 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:47.864227 google-maps-addressvalidation-0.3.2/tests/unit/gapic/addressvalidation_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/tests/unit/gapic/addressvalidation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76826 2023-04-11 16:30:19.000000 google-maps-addressvalidation-0.3.2/tests/unit/gapic/addressvalidation_v1/test_address_validation.py
```

### Comparing `google-maps-addressvalidation-0.3.1/LICENSE` & `google-maps-addressvalidation-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/MANIFEST.in` & `google-maps-addressvalidation-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/PKG-INFO` & `google-maps-addressvalidation-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-addressvalidation
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Maps Addressvalidation API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-addressvalidation-0.3.1/README.rst` & `google-maps-addressvalidation-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation/gapic_version.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/gapic_metadata.json` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/gapic_version.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/async_client.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/async_client.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/client.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/base.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/__init__.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/address.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,21 @@
         "AddressComponent",
         "ComponentName",
     },
 )
 
 
 class Address(proto.Message):
-    r"""Details of the address parsed from the input.
+    r"""Details of the post-processed address. Post-processing
+    includes correcting misspelled parts of the address, replacing
+    incorrect parts, and inferring missing parts.
 
     Attributes:
         formatted_address (str):
-            The corrected address, formatted as a
+            The post-processed address, formatted as a
             single-line address following the address
             formatting rules of the region where the address
             is located.
         postal_address (google.type.postal_address_pb2.PostalAddress):
             The validated address represented as a postal
             address.
         address_components (MutableSequence[google.maps.addressvalidation_v1.types.AddressComponent]):
```

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/address_validation_service.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/address_validation_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,17 @@
         address (google.maps.addressvalidation_v1.types.Address):
             Information about the address itself as
             opposed to the geocode.
         geocode (google.maps.addressvalidation_v1.types.Geocode):
             Information about the location and place that
             the address geocoded to.
         metadata (google.maps.addressvalidation_v1.types.AddressMetadata):
-            Other information relevant to deliverability.
+            Other information relevant to deliverability. ``metadata``
+            is not guaranteed to be fully populated for every address
+            sent to the Address Validation API.
         usps_data (google.maps.addressvalidation_v1.types.UspsData):
             Extra deliverability flags provided by USPS. Only provided
             in region ``US`` and ``PR``.
     """
 
     verdict: "Verdict" = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/geocode.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/geocode.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/metadata_.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/metadata_.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     manifest={
         "AddressMetadata",
     },
 )
 
 
 class AddressMetadata(proto.Message):
-    r"""The metadata for the address.
+    r"""The metadata for the address. ``metadata`` is not guaranteed to be
+    fully populated for every address sent to the Address Validation
+    API.
+
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         business (bool):
             Indicates that this is the address of a
             business. If unset, indicates that the value is
```

### Comparing `google-maps-addressvalidation-0.3.1/google/maps/addressvalidation_v1/types/usps_data.py` & `google-maps-addressvalidation-0.3.2/google/maps/addressvalidation_v1/types/usps_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,19 @@
     zip_code_extension: str = proto.Field(
         proto.STRING,
         number=9,
     )
 
 
 class UspsData(proto.Message):
-    r"""The USPS data for the address.
+    r"""The USPS data for the address. ``uspsData`` is not guaranteed to be
+    fully populated for every US or PR address sent to the Address
+    Validation API. It's recommended to integrate the backup address
+    fields in the response if you utilize uspsData as the primary part
+    of the response.
 
     Attributes:
         standardized_address (google.maps.addressvalidation_v1.types.UspsAddress):
             USPS standardized address.
         delivery_point_code (str):
             2 digit delivery point code
         delivery_point_check_digit (str):
```

### Comparing `google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/PKG-INFO` & `google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-addressvalidation
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Maps Addressvalidation API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-addressvalidation-0.3.1/google_maps_addressvalidation.egg-info/SOURCES.txt` & `google-maps-addressvalidation-0.3.2/google_maps_addressvalidation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/setup.py` & `google-maps-addressvalidation-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/tests/__init__.py` & `google-maps-addressvalidation-0.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/tests/unit/__init__.py` & `google-maps-addressvalidation-0.3.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/tests/unit/gapic/__init__.py` & `google-maps-addressvalidation-0.3.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/tests/unit/gapic/addressvalidation_v1/__init__.py` & `google-maps-addressvalidation-0.3.2/tests/unit/gapic/addressvalidation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.1/tests/unit/gapic/addressvalidation_v1/test_address_validation.py` & `google-maps-addressvalidation-0.3.2/tests/unit/gapic/addressvalidation_v1/test_address_validation.py`

 * *Files identical despite different names*

