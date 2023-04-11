# Comparing `tmp/sensors_connectivity-1.3.3.tar.gz` & `tmp/sensors_connectivity-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensors_connectivity-1.3.3.tar", max compression
+gzip compressed data, was "sensors_connectivity-1.4.0.tar", max compression
```

## Comparing `sensors_connectivity-1.3.3.tar` & `sensors_connectivity-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1507 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/LICENSE
--rw-r--r--   0        0        0     6281 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/README.md
--rw-r--r--   0        0        0       24 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/__init__.py
--rw-r--r--   0        0        0     9099 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/config/README.md
--rw-r--r--   0        0        0       36 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/config/__init__.py
--rw-r--r--   0        0        0     1006 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/config/default.json
--rw-r--r--   0        0        0      938 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/config/logging.py
--rw-r--r--   0        0        0      824 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/config/logging_template.py
--rw-r--r--   0        0        0       94 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/constants.py
--rw-r--r--   0        0        0     5975 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/main.py
--rw-r--r--   0        0        0       51 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/drivers/__init__.py
--rw-r--r--   0        0        0      477 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/drivers/ping.py
--rw-r--r--   0        0        0     5754 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/drivers/sds011.py
--rw-r--r--   0        0        0      189 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/feeders/__init__.py
--rw-r--r--   0        0        0     8954 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/feeders/datalog_feeder.py
--rw-r--r--   0        0        0     1280 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/feeders/frontier_datalog.py
--rw-r--r--   0        0        0     1088 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/feeders/ifeeder.py
--rw-r--r--   0        0        0     2521 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/feeders/robonomics_feeder.py
--rw-r--r--   0        0        0      187 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/__init__.py
--rw-r--r--   0        0        0     1377 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/base.py
--rw-r--r--   0        0        0     2046 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/environmental_box.py
--rw-r--r--   0        0        0     1443 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/mobile_lab.py
--rw-r--r--   0        0        0     1427 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/sensor_sds011.py
--rw-r--r--   0        0        0      771 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/sensor_template.py
--rw-r--r--   0        0        0     2572 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/sensors/trackagro_sensor.py
--rw-r--r--   0        0        0      212 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/__init__.py
--rw-r--r--   0        0        0     2238 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/comstation.py
--rw-r--r--   0        0        0     4380 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/httpstation.py
--rw-r--r--   0        0        0     1639 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/istation.py
--rw-r--r--   0        0        0     3815 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/mqttstation.py
--rw-r--r--   0        0        0     3090 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/src/stations/trackargostation.py
--rw-r--r--   0        0        0       55 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/database.py
--rwxr-xr-x   0        0        0     3207 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/flash_firmware.py
--rwxr-xr-x   0        0        0     1825 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/generate_secrets.py
--rw-r--r--   0        0        0      391 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/get_mac.py
--rwxr-xr-x   0        0        0      553 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/py_generate_secrets.py
--rwxr-xr-x   0        0        0     2502 2023-03-01 13:33:54.625561 sensors_connectivity-1.3.3/connectivity/utils/virtual-sensor.py
--rw-r--r--   0        0        0     1150 2023-03-01 13:33:54.629561 sensors_connectivity-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 sensors_connectivity-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1507 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6281 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/README.md
+-rw-r--r--   0        0        0       24 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/__init__.py
+-rw-r--r--   0        0        0     9099 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/README.md
+-rw-r--r--   0        0        0       36 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/__init__.py
+-rw-r--r--   0        0        0     1006 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/default.json
+-rw-r--r--   0        0        0      938 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/logging.py
+-rw-r--r--   0        0        0      824 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/logging_template.py
+-rw-r--r--   0        0        0       94 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/constants.py
+-rw-r--r--   0        0        0     5975 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/main.py
+-rw-r--r--   0        0        0       51 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/ping.py
+-rw-r--r--   0        0        0     5754 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/sds011.py
+-rw-r--r--   0        0        0      189 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/__init__.py
+-rw-r--r--   0        0        0     8956 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/datalog_feeder.py
+-rw-r--r--   0        0        0     1280 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/frontier_datalog.py
+-rw-r--r--   0        0        0     1088 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/ifeeder.py
+-rw-r--r--   0        0        0     3166 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/robonomics_feeder.py
+-rw-r--r--   0        0        0      224 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/base.py
+-rw-r--r--   0        0        0     2046 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/environmental_box.py
+-rw-r--r--   0        0        0      643 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/lora_sensors.py
+-rw-r--r--   0        0        0     1443 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/mobile_lab.py
+-rw-r--r--   0        0        0     1427 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_sds011.py
+-rw-r--r--   0        0        0      771 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_template.py
+-rw-r--r--   0        0        0     2572 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/trackagro_sensor.py
+-rw-r--r--   0        0        0      212 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/comstation.py
+-rw-r--r--   0        0        0     4380 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/httpstation.py
+-rw-r--r--   0        0        0     1639 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/istation.py
+-rw-r--r--   0        0        0     4055 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/mqttstation.py
+-rw-r--r--   0        0        0     3089 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/trackargostation.py
+-rw-r--r--   0        0        0       55 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/database.py
+-rwxr-xr-x   0        0        0     3207 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/flash_firmware.py
+-rwxr-xr-x   0        0        0     1825 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/generate_secrets.py
+-rw-r--r--   0        0        0      391 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/get_mac.py
+-rwxr-xr-x   0        0        0      553 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/py_generate_secrets.py
+-rwxr-xr-x   0        0        0     2502 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/virtual-sensor.py
+-rw-r--r--   0        0        0     1174 2023-04-11 13:26:12.145418 sensors_connectivity-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7507 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.0/PKG-INFO
```

### Comparing `sensors_connectivity-1.3.3/LICENSE` & `sensors_connectivity-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/README.md` & `sensors_connectivity-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/config/README.md` & `sensors_connectivity-1.4.0/connectivity/config/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/config/default.json` & `sensors_connectivity-1.4.0/connectivity/config/default.json`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/config/logging.py` & `sensors_connectivity-1.4.0/connectivity/config/logging.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/config/logging_template.py` & `sensors_connectivity-1.4.0/connectivity/config/logging_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/main.py` & `sensors_connectivity-1.4.0/connectivity/main.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/drivers/sds011.py` & `sensors_connectivity-1.4.0/connectivity/src/drivers/sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/feeders/datalog_feeder.py` & `sensors_connectivity-1.4.0/connectivity/src/feeders/datalog_feeder.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging.config
 import os
 import threading
 import time
 import typing as tp
 from tempfile import NamedTemporaryFile
 
-import ipfshttpclient
+import ipfshttpclient2
 import requests
 from pinatapy import PinataPy
 from prometheus_client import Enum
 from robonomicsinterface import RWS, Account, Datalog
 
 from connectivity.config.logging import LOGGING_CONFIG
 from connectivity.utils.database import DataBase
@@ -85,15 +85,15 @@
         logger.debug(f"Created temp file: {temp.name}")
         temp.write(json.dumps(payload))
         temp.close()
         DATALOG_MEMORY_METRIC.state("success")
     except Exception as e:
         DATALOG_MEMORY_METRIC.state("error")
 
-    with ipfshttpclient.connect(endpoint) as client:
+    with ipfshttpclient2.connect(endpoint) as client:
         response = client.add(temp.name)
         db.add_data("not sent", response["Hash"], time.time(), json.dumps(payload))
         return (response["Hash"], temp.name)
 
 
 def _pin_to_pinata(file_path: str, config: dict) -> None:
     """Pin file to Pinata for for better accessibility.
```

### Comparing `sensors_connectivity-1.3.3/connectivity/src/feeders/frontier_datalog.py` & `sensors_connectivity-1.4.0/connectivity/src/feeders/frontier_datalog.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/feeders/ifeeder.py` & `sensors_connectivity-1.4.0/connectivity/src/feeders/ifeeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/feeders/robonomics_feeder.py` & `sensors_connectivity-1.4.0/connectivity/src/feeders/robonomics_feeder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import logging
 import logging.config
+import os
+import tempfile
 import threading
 import typing as tp
 
-import ipfshttpclient
+import ipfshttpclient2
 
 from connectivity.config.logging import LOGGING_CONFIG
 
 from ...constants import PING_MODEL
 from .ifeeder import IFeeder
 
 logging.config.dictConfig(LOGGING_CONFIG)
@@ -51,15 +53,15 @@
 
     return json.dumps(message)
 
 
 class RobonomicsFeeder(IFeeder):
     """
     Publishes a result or demand message to IPFS pubsub channel
-    according to Robonomics communication protocol. 
+    according to Robonomics communication protocol.
     """
 
     def __init__(self, config: dict) -> None:
         """Initialize IPFS client.
 
         :param config: Dict with configuration.
         """
@@ -67,23 +69,38 @@
         super().__init__(config)
 
         endpoint: str = (
             config["robonomics"]["ipfs_provider"]
             if config["robonomics"]["ipfs_provider"]
             else "/ip4/127.0.0.1/tcp/5001/http"
         )
-        self.ipfs_client = ipfshttpclient.connect(endpoint, session=True)
+        self.ipfs_client = ipfshttpclient2.connect(endpoint, session=True)
         self.topic: str = config["robonomics"]["ipfs_topic"]
 
+    def _publish_to_topic(self, payload):
+
+        if int(self.ipfs_client.version()["Version"].split(".")[1]) < 11:
+            return self.ipfs_client.pubsub.publish_old(self.topic, payload)
+
+        if isinstance(payload, str) and not os.path.exists(payload):
+            payload = payload.encode()
+        if isinstance(payload, bytes) or isinstance(payload, bytearray):
+            with tempfile.NamedTemporaryFile() as tp:
+                tp.write(payload)
+                tp.flush()
+                self.ipfs_client.pubsub.publish(self.topic, tp.name)
+        else:
+            self.ipfs_client.pubsub.publish(self.topic, payload)
+
     def feed(self, data: tp.List[dict]) -> None:
         """Send data to IPFS pubsub in the topic from config.
 
         :param data: Data from the stations.
         """
         if self.config["robonomics"]["enable"]:
             for d in data:
                 if d.public and d.model != PING_MODEL:
                     pubsub_payload = _to_pubsub_message(d)
                 else:
                     pubsub_payload = _to_ping_message(d)
                 logger.info(f"RobonomicsFeeder: {pubsub_payload}")
-                self.ipfs_client.pubsub.publish(self.topic, pubsub_payload)
+                self._publish_to_topic(pubsub_payload)
```

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/base.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/base.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/environmental_box.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/environmental_box.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/mobile_lab.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/mobile_lab.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/sensor_sds011.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/sensor_template.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/sensors/trackagro_sensor.py` & `sensors_connectivity-1.4.0/connectivity/src/sensors/trackagro_sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/stations/comstation.py` & `sensors_connectivity-1.4.0/connectivity/src/stations/comstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/stations/httpstation.py` & `sensors_connectivity-1.4.0/connectivity/src/stations/httpstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/stations/istation.py` & `sensors_connectivity-1.4.0/connectivity/src/stations/istation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/src/stations/mqttstation.py` & `sensors_connectivity-1.4.0/connectivity/src/stations/mqttstation.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing as tp
 
 import paho.mqtt.client as mqtt
 
 from connectivity.config.logging import LOGGING_CONFIG
 
 from ...constants import STATION_VERSION
-from ..sensors import EnvironmentalBox, MobileLab
+from ..sensors import EnvironmentalBox, LoraSensor, MobileLab
 from .istation import IStation
 
 logging.config.dictConfig(LOGGING_CONFIG)
 logger = logging.getLogger("sensors-connectivity")
 
 thlock = threading.RLock()
 sessions = dict()
@@ -65,21 +65,25 @@
         global thlock
         global sessions
         data = json.loads(msg.payload.decode())
         if "esp8266id" in data.keys():
             meas = EnvironmentalBox(data)
         elif "ID" in data.keys():
             meas = MobileLab(data)
+        elif "decoded_payload" in data["uplink_message"]:
+            id = data["end_device_ids"]["device_id"]
+            meas = LoraSensor(id=id, data=data["uplink_message"]["decoded_payload"])
+        else:
+            return
         with thlock:
             if meas:
                 sessions[meas.id] = meas
 
     def on_subscribe(self, client, userdata, mid, granted_qos) -> None:
         """Subscription callback."""
-
         logger.info(f"Subscribed {str(mid)} to topic {self.topic}")
 
     def run(self) -> None:
         """Service function for MQTT handler."""
 
         self.connect_async(self.host, self.port, 60)
         self.loop_start()
```

### Comparing `sensors_connectivity-1.3.3/connectivity/src/stations/trackargostation.py` & `sensors_connectivity-1.4.0/connectivity/src/stations/trackargostation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 import logging.config
 import ssl
 import threading
 import time
 import typing as tp
 import urllib.request as ur
-
 # from os import times
 from urllib import error, parse
 
 from connectivity.config.logging import LOGGING_CONFIG
 
 from ...constants import STATION_VERSION
 from ..sensors import TrackAgro
```

### Comparing `sensors_connectivity-1.3.3/connectivity/utils/database.py` & `sensors_connectivity-1.4.0/connectivity/utils/database.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/utils/flash_firmware.py` & `sensors_connectivity-1.4.0/connectivity/utils/flash_firmware.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/utils/generate_secrets.py` & `sensors_connectivity-1.4.0/connectivity/utils/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/utils/py_generate_secrets.py` & `sensors_connectivity-1.4.0/connectivity/utils/py_generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/connectivity/utils/virtual-sensor.py` & `sensors_connectivity-1.4.0/connectivity/utils/virtual-sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.3.3/pyproject.toml` & `sensors_connectivity-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensors_connectivity"
-version = "1.3.3"
+version = "1.4.0"
 description = "Robonomics package to read data from sensors and publish to different output channels"
 authors = [
     "Vadim Manaenko <vadim.razorq@gmail.com>",
     "Mariia Bystramovich <m.bystramovich@gmail.com>",
 ]
 license = "BSD 3-Clause License"
 
@@ -29,14 +29,15 @@
 robonomics-interface = "^1.6.0"
 ipfshttpclient = "0.8.0a2"
 pinatapy-vourhey = "^0.1.3"
 netifaces = "^0.11.0"
 paho-mqtt = "^1.6.1"
 prometheus-client = "^0.13.1"
 py-sr25519-bindings = "^0.2.0"
+IPFS-Toolkit = "^0.4.4"
 
 [tool.poetry.scripts]
 sensors_connectivity = "connectivity.main:run"
 test_environmental_box = "tests.environmental_box_test:main"
 test_mobile_lab = "tests.mobile_lab_test:main"
 test_many_sensors = "tests.many_environmental_boxes:main"
```

### Comparing `sensors_connectivity-1.3.3/PKG-INFO` & `sensors_connectivity-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sensors-connectivity
-Version: 1.3.3
+Version: 1.4.0
 Summary: Robonomics package to read data from sensors and publish to different output channels
 Home-page: https://github.com/airalab/sensors-connectivity
 License: BSD 3-Clause License
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: IPFS-Toolkit (>=0.4.4,<0.5.0)
 Requires-Dist: ipfshttpclient (==0.8.0a2)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: pinatapy-vourhey (>=0.1.3,<0.2.0)
 Requires-Dist: prometheus-client (>=0.13.1,<0.14.0)
 Requires-Dist: py-sr25519-bindings (>=0.2.0,<0.3.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
```

