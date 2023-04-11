# Comparing `tmp/touch_sdk-0.6.3.tar.gz` & `tmp/touch_sdk-0.6.4.tar.gz`

## Comparing `touch_sdk-0.6.3.tar` & `touch_sdk-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/.gitlab-ci.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/.pylintrc
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/basic.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/custom_data.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/magnetometer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/osc.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/plotter.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/raycasting.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/examples/sensors.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/basic.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/pressure.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/gatt_scanner.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/uuids.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/watch.py
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/watch_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/protobuf/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/protobuf/vec_pb2.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/protobuf/watch_input_pb2.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/src/touch_sdk/protobuf/watch_output_pb2.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/.gitignore
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/LICENSE
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.pylintrc
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/version.sh
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/basic.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/custom_data.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/magnetometer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/osc.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/plotter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/pressure.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/raycasting.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/sensors.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/basic.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/pressure.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/gatt_scanner.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/uuids.py
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/watch.py
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/watch_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/vec_pb2.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_input_pb2.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_output_pb2.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.gitignore
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/PKG-INFO
```

### Comparing `touch_sdk-0.6.3/examples/basic.py` & `touch_sdk-0.6.4/examples/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/examples/magnetometer.py` & `touch_sdk-0.6.4/examples/magnetometer.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/examples/plotter.py` & `touch_sdk-0.6.4/examples/plotter.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/examples/raycasting.py` & `touch_sdk-0.6.4/examples/raycasting.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/examples/sensors.py` & `touch_sdk-0.6.4/examples/sensors.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/basic.py` & `touch_sdk-0.6.4/src/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/touch_sdk/gatt_scanner.py` & `touch_sdk-0.6.4/src/touch_sdk/gatt_scanner.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/touch_sdk/utils.py` & `touch_sdk-0.6.4/src/touch_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/touch_sdk/watch.py` & `touch_sdk-0.6.4/src/touch_sdk/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,17 @@
         self._proto_on_touch_events(message.touchEvents)
         self._proto_on_button_events(message.buttonEvents)
         self._proto_on_rotary_events(message.rotaryEvents)
 
         if message.HasField("info"):
             self._proto_on_info(message.info)
 
+        if message.pressure != 0.0:
+            self.on_pressure(message.pressure)
+
     # Sensor events
 
     def _proto_on_sensors(self, frames, timestamp):
         frame = frames[-1]
         sensor_frame = SensorFrame(
             acceleration=_protovec3_to_tuple(frame.acc),
             gravity=_protovec3_to_tuple(frame.grav),
@@ -178,14 +181,17 @@
         delta_y = handedness_scale * (av_y * grav[2] - av_x * grav[1])
 
         self.on_arm_direction_change(delta_x, delta_y)
 
     def on_arm_direction_change(self, delta_x: float, delta_y: float):
         """Gyroscope-based raycasting output. Called after sensor updates."""
 
+    def on_pressure(self, pressure: float):
+        """Called when new pressure value (in hectopascals) is received."""
+
     # Gestures
 
     def _proto_on_gestures(self, gestures):
         if any(g.type == Gesture.GestureType.TAP for g in gestures):
             self.on_tap()
 
     def on_tap(self):
@@ -270,8 +276,8 @@
         loop = asyncio.get_running_loop()
         loop.create_task(
             self._async_write_input_characteristic(PROTOBUF_INPUT, data, client)
         )
 
     async def _async_write_input_characteristic(self, characteristic, data, client):
         if client:
-            await client.write_gatt_char(characteristic, data)
+            await client.write_gatt_char(characteristic, data, True)
```

### Comparing `touch_sdk-0.6.3/src/touch_sdk/watch_connector.py` & `touch_sdk-0.6.4/src/touch_sdk/watch_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,38 +72,41 @@
                 if not client.is_connected
             ]
 
             await asyncio.gather(*disconnect_tasks)
             await asyncio.sleep(2)
 
     async def _on_scan_result(self, device, name):
-        try:
-            client = BleakClient(device)
+        client = BleakClient(device)
+        address = device.address
 
+        try:
             await client.connect()
-            self._clients[device.address] = client
+        except asyncio.exceptions.TimeoutError:
+            await self.disconnect(address)
+            return
+
+        self._clients[address] = client
 
-            await self._send_client_info(client)
+        await self._send_client_info(client)
 
+        try:
             await client.start_notify(
                 PROTOBUF_OUTPUT, partial_async(self._on_protobuf, device, name)
             )
-
-        except (
-            bleak.exc.BleakDBusError,
-            bleak.exc.BleakError,
-            asyncio.TimeoutError,
-        ) as error:
-            # catches:
-            # - ATT Invalid Handle error, coming from _send_client_info
-            # - le-connection-abort-by-local, coming from client.connect
-            # - Characteristic not found, coming from_send_client_info or client.start_notify
-            # - asyncio timeout error, coming from client.connect
-            print(f"Disconnecting {name}. {error}")
-            await self.disconnect(device.address)
+        except bleak.exc.BleakDBusError:
+            # [org.bluez.Error.NotConnected] Not Connected
+            #
+            # Sometimes (~50%) Bleak thinks the client is connected even though
+            # BlueZ thinks it's not. We could try to reconnect, but that messes
+            # up with _monitor_connections. Easier to just give up and try again
+            # through the scanner, even though it adds a delay and a bit of
+            # noise to the console.
+            print('Connecting failed, trying again')
+            await self.disconnect(address)
 
     async def disconnect(self, address):
         """Disconnect the client associated with the argument device if it exists,
         and clean up.
         """
         if (client := self._clients.pop(address, None)) is not None:
             await client.disconnect()
@@ -164,10 +167,23 @@
         client_info = ClientInfo()
         client_info.appName = sys.argv[0]
         client_info.deviceName = platform.node()
         client_info.os = platform.system()
         input_update = InputUpdate()
         input_update.clientInfo.CopyFrom(client_info)
 
-        await client.write_gatt_char(PROTOBUF_INPUT, input_update.SerializeToString())
+        try:
+            await client.write_gatt_char(PROTOBUF_INPUT, input_update.SerializeToString(), True)
+        except bleak.exc.BleakDBusError:
+            # [org.bluez.Error.Failed] Operation failed with ATT error:
+            # 0x01 (Invalid Handle)
+            #
+            # This happens if the client is not already approved by the
+            # watch before this connection (= connection dialog shows up).
+            # However, the client info seems to still end up to the watch,
+            # so we don't need to abort the handshake.
+            pass
+        except bleak.exc.BleakError:
+            # macOS says "Failed to write characteristic" but it succeeds
+            pass
 
         self._informed_addresses.add(client.address)
```

### Comparing `touch_sdk-0.6.3/src/touch_sdk/protobuf/vec_pb2.py` & `touch_sdk-0.6.4/src/touch_sdk/protobuf/vec_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/touch_sdk/protobuf/watch_input_pb2.py` & `touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_input_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/src/touch_sdk/protobuf/watch_output_pb2.py` & `touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_output_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import touch_sdk.protobuf.vec_pb2 as vec__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12watch_output.proto\x1a\tvec.proto\"G\n\x04Info\x12\x18\n\x04hand\x18\x01 \x01(\x0e\x32\n.Info.Hand\"%\n\x04Hand\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05RIGHT\x10\x01\x12\x08\n\x04LEFT\x10\x02\"\x9e\x01\n\x0bSensorFrame\x12\x13\n\x04gyro\x18\x01 \x01(\x0b\x32\x05.Vec3\x12\x12\n\x03\x61\x63\x63\x18\x02 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04grav\x18\x03 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04quat\x18\x04 \x01(\x0b\x32\x05.Quat\x12\x12\n\x03mag\x18\x06 \x01(\x0b\x32\x05.Vec3\x12\x15\n\x06magCal\x18\x07 \x01(\x0b\x32\x05.Vec3\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"n\n\x07Gesture\x12\"\n\x04type\x18\x01 \x01(\x0e\x32\x14.Gesture.GestureType\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0bGestureType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03TAP\x10\x01\x12\n\n\x06\x43LENCH\x10\x02\"\xd4\x01\n\nTouchEvent\x12-\n\teventType\x18\x01 \x01(\x0e\x32\x1a.TouchEvent.TouchEventType\x12\x13\n\x0b\x61\x63tionIndex\x18\x02 \x01(\x05\x12\x12\n\npointerIds\x18\x03 \x03(\x05\x12\x15\n\x06\x63oords\x18\x04 \x03(\x0b\x32\x05.Vec2\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"D\n\x0eTouchEventType\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x42\x45GIN\x10\x01\x12\x07\n\x03\x45ND\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04\".\n\x0bRotaryEvent\x12\x0c\n\x04step\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0b\x42uttonEvent\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\"\xdf\x02\n\x06Update\x12\"\n\x0csensorFrames\x18\x01 \x03(\x0b\x32\x0c.SensorFrame\x12\x1a\n\x08gestures\x18\x02 \x03(\x0b\x32\x08.Gesture\x12 \n\x0btouchEvents\x18\x03 \x03(\x0b\x32\x0b.TouchEvent\x12\"\n\x0c\x62uttonEvents\x18\x04 \x03(\x0b\x32\x0c.ButtonEvent\x12\"\n\x0crotaryEvents\x18\x05 \x03(\x0b\x32\x0c.RotaryEvent\x12\x1f\n\x07signals\x18\x06 \x03(\x0e\x32\x0e.Update.Signal\x12\x11\n\tdeltaTime\x18\x07 \x01(\x05\x12\x10\n\x08unixTime\x18\x08 \x01(\x03\x12\x13\n\x04info\x18\t \x01(\x0b\x32\x05.Info\"P\n\x06Signal\x12\x08\n\x04NONE\x10\x00\x12\x0e\n\nDISCONNECT\x10\x01\x12\x14\n\x10\x43ONNECT_APPROVED\x10\x02\x12\x16\n\x12\x44\x45SCRIPTION_UPDATE\x10\x03\x42\r\xaa\x02\nPsix.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12watch_output.proto\x1a\tvec.proto\"j\n\x04Info\x12\x18\n\x04hand\x18\x01 \x01(\x0e\x32\n.Info.Hand\x12\r\n\x05\x61ppId\x18\x02 \x01(\t\x12\x12\n\nappVersion\x18\x03 \x01(\t\"%\n\x04Hand\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05RIGHT\x10\x01\x12\x08\n\x04LEFT\x10\x02\"\x9e\x01\n\x0bSensorFrame\x12\x13\n\x04gyro\x18\x01 \x01(\x0b\x32\x05.Vec3\x12\x12\n\x03\x61\x63\x63\x18\x02 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04grav\x18\x03 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04quat\x18\x04 \x01(\x0b\x32\x05.Quat\x12\x12\n\x03mag\x18\x06 \x01(\x0b\x32\x05.Vec3\x12\x15\n\x06magCal\x18\x07 \x01(\x0b\x32\x05.Vec3\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"n\n\x07Gesture\x12\"\n\x04type\x18\x01 \x01(\x0e\x32\x14.Gesture.GestureType\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0bGestureType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03TAP\x10\x01\x12\n\n\x06\x43LENCH\x10\x02\"\xd4\x01\n\nTouchEvent\x12-\n\teventType\x18\x01 \x01(\x0e\x32\x1a.TouchEvent.TouchEventType\x12\x13\n\x0b\x61\x63tionIndex\x18\x02 \x01(\x05\x12\x12\n\npointerIds\x18\x03 \x03(\x05\x12\x15\n\x06\x63oords\x18\x04 \x03(\x0b\x32\x05.Vec2\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"D\n\x0eTouchEventType\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x42\x45GIN\x10\x01\x12\x07\n\x03\x45ND\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04\".\n\x0bRotaryEvent\x12\x0c\n\x04step\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0b\x42uttonEvent\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\"\xf1\x02\n\x06Update\x12\"\n\x0csensorFrames\x18\x01 \x03(\x0b\x32\x0c.SensorFrame\x12\x1a\n\x08gestures\x18\x02 \x03(\x0b\x32\x08.Gesture\x12 \n\x0btouchEvents\x18\x03 \x03(\x0b\x32\x0b.TouchEvent\x12\"\n\x0c\x62uttonEvents\x18\x04 \x03(\x0b\x32\x0c.ButtonEvent\x12\"\n\x0crotaryEvents\x18\x05 \x03(\x0b\x32\x0c.RotaryEvent\x12\x1f\n\x07signals\x18\x06 \x03(\x0e\x32\x0e.Update.Signal\x12\x11\n\tdeltaTime\x18\x07 \x01(\x05\x12\x10\n\x08unixTime\x18\x08 \x01(\x03\x12\x13\n\x04info\x18\t \x01(\x0b\x32\x05.Info\x12\x10\n\x08pressure\x18\x10 \x01(\x02\"P\n\x06Signal\x12\x08\n\x04NONE\x10\x00\x12\x0e\n\nDISCONNECT\x10\x01\x12\x14\n\x10\x43ONNECT_APPROVED\x10\x02\x12\x16\n\x12\x44\x45SCRIPTION_UPDATE\x10\x03\x42\r\xaa\x02\nPsix.Protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'watch_output_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\nPsix.Proto'
   _INFO._serialized_start=33
-  _INFO._serialized_end=104
-  _INFO_HAND._serialized_start=67
-  _INFO_HAND._serialized_end=104
-  _SENSORFRAME._serialized_start=107
-  _SENSORFRAME._serialized_end=265
-  _GESTURE._serialized_start=267
-  _GESTURE._serialized_end=377
-  _GESTURE_GESTURETYPE._serialized_start=333
-  _GESTURE_GESTURETYPE._serialized_end=377
-  _TOUCHEVENT._serialized_start=380
-  _TOUCHEVENT._serialized_end=592
-  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_start=524
-  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_end=592
-  _ROTARYEVENT._serialized_start=594
-  _ROTARYEVENT._serialized_end=640
-  _BUTTONEVENT._serialized_start=642
-  _BUTTONEVENT._serialized_end=686
-  _UPDATE._serialized_start=689
-  _UPDATE._serialized_end=1040
-  _UPDATE_SIGNAL._serialized_start=960
-  _UPDATE_SIGNAL._serialized_end=1040
+  _INFO._serialized_end=139
+  _INFO_HAND._serialized_start=102
+  _INFO_HAND._serialized_end=139
+  _SENSORFRAME._serialized_start=142
+  _SENSORFRAME._serialized_end=300
+  _GESTURE._serialized_start=302
+  _GESTURE._serialized_end=412
+  _GESTURE_GESTURETYPE._serialized_start=368
+  _GESTURE_GESTURETYPE._serialized_end=412
+  _TOUCHEVENT._serialized_start=415
+  _TOUCHEVENT._serialized_end=627
+  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_start=559
+  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_end=627
+  _ROTARYEVENT._serialized_start=629
+  _ROTARYEVENT._serialized_end=675
+  _BUTTONEVENT._serialized_start=677
+  _BUTTONEVENT._serialized_end=721
+  _UPDATE._serialized_start=724
+  _UPDATE._serialized_end=1093
+  _UPDATE_SIGNAL._serialized_start=1013
+  _UPDATE_SIGNAL._serialized_end=1093
 # @@protoc_insertion_point(module_scope)
```

### Comparing `touch_sdk-0.6.3/LICENSE` & `touch_sdk-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/README.md` & `touch_sdk-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.3/pyproject.toml` & `touch_sdk-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "touch-sdk"
-version = "0.6.3"
+version = "0.6.4"
 description = "Port 6 Touch SDK"
 license = "ISC"
 authors = [
     { name="Port 6", email="developer@port6.io" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -21,15 +21,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: Android",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
 ]
 dependencies = [
-    "bleak==0.19.5",
+    "bleak==0.20.1",
     "protobuf==3.20.0",
     "asyncio-atexit==1.0.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/port6io/touch-sdk-py#readme"
 "Bug Tracker" = "https://github.com/port6io/touch-sdk-py/issues"
```

### Comparing `touch_sdk-0.6.3/PKG-INFO` & `touch_sdk-0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touch-sdk
-Version: 0.6.3
+Version: 0.6.4
 Summary: Port 6 Touch SDK
 Project-URL: Homepage, https://github.com/port6io/touch-sdk-py#readme
 Project-URL: Bug Tracker, https://github.com/port6io/touch-sdk-py/issues
 Author-email: Port 6 <developer@port6.io>
 License-Expression: ISC
 License-File: LICENSE
 Keywords: bluetooth
@@ -15,15 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.8
 Requires-Dist: asyncio-atexit==1.0.1
-Requires-Dist: bleak==0.19.5
+Requires-Dist: bleak==0.20.1
 Requires-Dist: protobuf==3.20.0
 Description-Content-Type: text/markdown
 
 # Touch SDK py
 
 ![PyPI](https://img.shields.io/pypi/v/touch-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/touch-sdk)
```

