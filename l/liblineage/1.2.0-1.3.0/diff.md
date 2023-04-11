# Comparing `tmp/liblineage-1.2.0.tar.gz` & `tmp/liblineage-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblineage-1.2.0.tar", max compression
+gzip compressed data, was "liblineage-1.3.0.tar", max compression
```

## Comparing `liblineage-1.2.0.tar` & `liblineage-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      386 2022-08-26 23:24:36.752356 liblineage-1.2.0/README.md
--rw-r--r--   0        0        0      237 2023-03-06 15:42:12.465614 liblineage-1.2.0/liblineage/__init__.py
--rw-r--r--   0        0        0      198 2022-08-30 13:21:57.046166 liblineage-1.2.0/liblineage/constants/infra.py
--rw-r--r--   0        0        0      657 2023-03-06 00:37:23.199983 liblineage-1.2.0/liblineage/constants/versions.py
--rw-r--r--   0        0        0      746 2023-03-06 15:41:20.302137 liblineage-1.2.0/liblineage/device.py
--rw-r--r--   0        0        0     2212 2022-09-10 22:11:52.475553 liblineage-1.2.0/liblineage/hudson/build_target.py
--rw-r--r--   0        0        0      222 2022-09-10 16:59:53.229174 liblineage-1.2.0/liblineage/hudson/period.py
--rw-r--r--   0        0        0     2360 2023-03-06 15:35:33.081202 liblineage-1.2.0/liblineage/ota/full_update_info.py
--rw-r--r--   0        0        0      219 2023-03-06 13:45:03.612525 liblineage-1.2.0/liblineage/updater/__init__.py
--rw-r--r--   0        0        0      463 2023-03-06 13:57:45.253121 liblineage-1.2.0/liblineage/updater/http_utils.py
--rw-r--r--   0        0        0     2008 2023-03-06 15:15:22.908220 liblineage-1.2.0/liblineage/updater/v1/__init__.py
--rw-r--r--   0        0        0      479 2023-03-06 15:15:13.344857 liblineage-1.2.0/liblineage/updater/v1/_deserializer.py
--rw-r--r--   0        0        0     1249 2023-03-06 15:13:58.101291 liblineage-1.2.0/liblineage/updater/v1/build.py
--rw-r--r--   0        0        0     1726 2023-03-06 15:15:46.388292 liblineage-1.2.0/liblineage/updater/v2/__init__.py
--rw-r--r--   0        0        0      527 2023-03-06 15:16:02.488342 liblineage-1.2.0/liblineage/updater/v2/_deserializer.py
--rw-r--r--   0        0        0      943 2023-03-06 13:43:39.422459 liblineage-1.2.0/liblineage/updater/v2/build.py
--rw-r--r--   0        0        0      971 2023-03-06 00:38:14.543370 liblineage-1.2.0/liblineage/updater/v2/build_file.py
--rw-r--r--   0        0        0     1189 2023-03-06 00:38:14.543370 liblineage-1.2.0/liblineage/updater/v2/device.py
--rw-r--r--   0        0        0      681 2023-03-06 13:30:12.755159 liblineage-1.2.0/liblineage/updater/v2/oem.py
--rw-r--r--   0        0        0      543 2023-03-06 13:30:12.755159 liblineage-1.2.0/liblineage/updater/v2/oem_device.py
--rw-r--r--   0        0        0      879 2022-08-27 23:27:58.787099 liblineage-1.2.0/liblineage/wiki/data_types/architecture_data.py
--rw-r--r--   0        0        0      582 2022-08-27 01:08:57.416656 liblineage-1.2.0/liblineage/wiki/data_types/base_data.py
--rw-r--r--   0        0        0     1259 2022-08-27 01:09:06.536770 liblineage-1.2.0/liblineage/wiki/data_types/battery_data.py
--rw-r--r--   0        0        0      898 2022-08-27 01:06:35.222893 liblineage-1.2.0/liblineage/wiki/data_types/bluetooth_data.py
--rw-r--r--   0        0        0      890 2022-08-28 00:15:02.394760 liblineage-1.2.0/liblineage/wiki/data_types/camera_data.py
--rw-r--r--   0        0        0     1204 2022-08-27 01:14:08.700546 liblineage-1.2.0/liblineage/wiki/data_types/dimension_data.py
--rw-r--r--   0        0        0      819 2022-08-27 23:08:32.653911 liblineage-1.2.0/liblineage/wiki/data_types/peripherals_data.py
--rw-r--r--   0        0        0     1141 2022-08-27 23:23:04.207708 liblineage-1.2.0/liblineage/wiki/data_types/release_data.py
--rw-r--r--   0        0        0     1352 2022-08-27 01:06:45.855025 liblineage-1.2.0/liblineage/wiki/data_types/screen_data.py
--rw-r--r--   0        0        0      877 2022-08-28 00:22:25.188025 liblineage-1.2.0/liblineage/wiki/data_types/sdcard_data.py
--rw-r--r--   0        0        0    11092 2022-08-30 13:38:18.795667 liblineage-1.2.0/liblineage/wiki/device_data.py
--rw-r--r--   0        0        0      520 2023-03-06 15:42:07.612268 liblineage-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      386 2022-08-26 23:24:36.752356 liblineage-1.3.0/README.md
+-rw-r--r--   0        0        0      237 2023-04-11 15:31:46.030989 liblineage-1.3.0/liblineage/__init__.py
+-rw-r--r--   0        0        0      198 2022-08-30 13:21:57.046166 liblineage-1.3.0/liblineage/constants/infra.py
+-rw-r--r--   0        0        0      657 2023-03-06 00:37:23.199983 liblineage-1.3.0/liblineage/constants/versions.py
+-rw-r--r--   0        0        0      746 2023-03-06 15:41:20.302137 liblineage-1.3.0/liblineage/device.py
+-rw-r--r--   0        0        0     2212 2022-09-10 22:11:52.475553 liblineage-1.3.0/liblineage/hudson/build_target.py
+-rw-r--r--   0        0        0      222 2022-09-10 16:59:53.229174 liblineage-1.3.0/liblineage/hudson/period.py
+-rw-r--r--   0        0        0     2360 2023-03-06 15:35:33.081202 liblineage-1.3.0/liblineage/ota/full_update_info.py
+-rw-r--r--   0        0        0      219 2023-03-06 13:45:03.612525 liblineage-1.3.0/liblineage/updater/__init__.py
+-rw-r--r--   0        0        0      463 2023-03-06 13:57:45.253121 liblineage-1.3.0/liblineage/updater/http_utils.py
+-rw-r--r--   0        0        0     2008 2023-03-06 15:15:22.908220 liblineage-1.3.0/liblineage/updater/v1/__init__.py
+-rw-r--r--   0        0        0      479 2023-03-06 15:15:13.344857 liblineage-1.3.0/liblineage/updater/v1/_deserializer.py
+-rw-r--r--   0        0        0     1249 2023-03-06 15:13:58.101291 liblineage-1.3.0/liblineage/updater/v1/build.py
+-rw-r--r--   0        0        0     1726 2023-03-06 15:15:46.388292 liblineage-1.3.0/liblineage/updater/v2/__init__.py
+-rw-r--r--   0        0        0      527 2023-03-06 15:16:02.488342 liblineage-1.3.0/liblineage/updater/v2/_deserializer.py
+-rw-r--r--   0        0        0      943 2023-03-06 13:43:39.422459 liblineage-1.3.0/liblineage/updater/v2/build.py
+-rw-r--r--   0        0        0      971 2023-03-06 00:38:14.543370 liblineage-1.3.0/liblineage/updater/v2/build_file.py
+-rw-r--r--   0        0        0     1049 2023-04-11 15:28:06.745781 liblineage-1.3.0/liblineage/updater/v2/device.py
+-rw-r--r--   0        0        0      681 2023-03-06 13:30:12.755159 liblineage-1.3.0/liblineage/updater/v2/oem.py
+-rw-r--r--   0        0        0      543 2023-03-06 13:30:12.755159 liblineage-1.3.0/liblineage/updater/v2/oem_device.py
+-rw-r--r--   0        0        0      879 2022-08-27 23:27:58.787099 liblineage-1.3.0/liblineage/wiki/data_types/architecture_data.py
+-rw-r--r--   0        0        0      582 2022-08-27 01:08:57.416656 liblineage-1.3.0/liblineage/wiki/data_types/base_data.py
+-rw-r--r--   0        0        0     1259 2022-08-27 01:09:06.536770 liblineage-1.3.0/liblineage/wiki/data_types/battery_data.py
+-rw-r--r--   0        0        0      898 2022-08-27 01:06:35.222893 liblineage-1.3.0/liblineage/wiki/data_types/bluetooth_data.py
+-rw-r--r--   0        0        0      890 2022-08-28 00:15:02.394760 liblineage-1.3.0/liblineage/wiki/data_types/camera_data.py
+-rw-r--r--   0        0        0     1204 2022-08-27 01:14:08.700546 liblineage-1.3.0/liblineage/wiki/data_types/dimension_data.py
+-rw-r--r--   0        0        0      819 2022-08-27 23:08:32.653911 liblineage-1.3.0/liblineage/wiki/data_types/peripherals_data.py
+-rw-r--r--   0        0        0     1141 2022-08-27 23:23:04.207708 liblineage-1.3.0/liblineage/wiki/data_types/release_data.py
+-rw-r--r--   0        0        0     1352 2022-08-27 01:06:45.855025 liblineage-1.3.0/liblineage/wiki/data_types/screen_data.py
+-rw-r--r--   0        0        0      877 2022-08-28 00:22:25.188025 liblineage-1.3.0/liblineage/wiki/data_types/sdcard_data.py
+-rw-r--r--   0        0        0    11092 2022-08-30 13:38:18.795667 liblineage-1.3.0/liblineage/wiki/device_data.py
+-rw-r--r--   0        0        0      520 2023-04-11 15:31:52.194374 liblineage-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.3.0/PKG-INFO
```

### Comparing `liblineage-1.2.0/liblineage/constants/versions.py` & `liblineage-1.3.0/liblineage/constants/versions.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/device.py` & `liblineage-1.3.0/liblineage/device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/hudson/build_target.py` & `liblineage-1.3.0/liblineage/hudson/build_target.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/ota/full_update_info.py` & `liblineage-1.3.0/liblineage/ota/full_update_info.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v1/__init__.py` & `liblineage-1.3.0/liblineage/updater/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v1/build.py` & `liblineage-1.3.0/liblineage/updater/v1/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/__init__.py` & `liblineage-1.3.0/liblineage/updater/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/_deserializer.py` & `liblineage-1.3.0/liblineage/updater/v2/_deserializer.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/build.py` & `liblineage-1.3.0/liblineage/updater/v2/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/build_file.py` & `liblineage-1.3.0/liblineage/updater/v2/build_file.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/device.py` & `liblineage-1.3.0/liblineage/updater/v2/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,37 @@
 	"""LineageOS device informations.
 
 	Attributes:
 	- name (str): The name of the device
 	- model (str): The model name of the device
 	- oem (str): The OEM name
 	- info_url (str): The URL of the device information page
-	- install_url (str): The URL of the installation instructions
 	- versions (list[str]): The LineageOS versions for this device (e.g. 18.1)
 	- dependencies (list[str]): The list of repositories used to build this device
 	"""
 	def __init__(
 		self,
 		name: str,
 		model: str,
 		oem: str,
 		info_url: str,
-		install_url: str,
 		versions: List[str],
 		dependencies: List[str],
 	) -> None:
 		self.name = name
 		self.model = model
 		self.oem = oem
 		self.info_url = info_url
-		self.install_url = install_url
 		self.versions = versions
 		self.dependencies = dependencies
 
 	@classmethod
 	def from_json(cls, json: Dict[str, Any]):
 		"""Create an object from a JSON object."""
 		return cls(
 			json["name"],
 			json["model"],
 			json["oem"],
 			json["info_url"],
-			json["install_url"],
 			json["versions"],
 			json["dependencies"],
 		)
```

### Comparing `liblineage-1.2.0/liblineage/updater/v2/oem.py` & `liblineage-1.3.0/liblineage/updater/v2/oem.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/updater/v2/oem_device.py` & `liblineage-1.3.0/liblineage/updater/v2/oem_device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/architecture_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/architecture_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/base_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/base_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/battery_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/battery_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/bluetooth_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/bluetooth_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/camera_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/camera_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/dimension_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/dimension_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/peripherals_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/peripherals_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/release_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/release_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/screen_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/screen_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/data_types/sdcard_data.py` & `liblineage-1.3.0/liblineage/wiki/data_types/sdcard_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/liblineage/wiki/device_data.py` & `liblineage-1.3.0/liblineage/wiki/device_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.2.0/pyproject.toml` & `liblineage-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liblineage"
-version = "1.2.0"
+version = "1.3.0"
 description = "LineageOS utils library"
 authors = ["Sebastiano Barezzi <barezzisebastiano@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sebaubuntu-python/liblineage"
 
 [tool.poetry.dependencies]
```

### Comparing `liblineage-1.2.0/PKG-INFO` & `liblineage-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblineage
-Version: 1.2.0
+Version: 1.3.0
 Summary: LineageOS utils library
 Home-page: https://github.com/sebaubuntu-python/liblineage
 License: LGPL-3.0-or-later
 Author: Sebastiano Barezzi
 Author-email: barezzisebastiano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

