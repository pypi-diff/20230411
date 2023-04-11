# Comparing `tmp/smdb_api-0.9.1.tar.gz` & `tmp/smdb_api-0.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smdb_api-0.9.1.tar", last modified: Tue Feb 14 06:14:48 2023, max compression
+gzip compressed data, was "smdb_api-0.9.12.tar", last modified: Tue Feb 14 16:41:45 2023, max compression
```

## Comparing `smdb_api-0.9.1.tar` & `smdb_api-0.9.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 06:14:48.474165 smdb_api-0.9.1/
--rw-rw-rw-   0        0        0     4010 2023-02-14 06:14:48.474165 smdb_api-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     3435 2023-01-15 15:17:06.000000 smdb_api-0.9.1/README.md
--rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_api-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      662 2023-02-14 06:14:48.475666 smdb_api-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-14 06:14:48.467164 smdb_api-0.9.1/smdb_api/
--rw-rw-rw-   0        0        0    22498 2023-02-14 06:13:27.000000 smdb_api-0.9.1/smdb_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 06:14:48.472664 smdb_api-0.9.1/smdb_api.egg-info/
--rw-rw-rw-   0        0        0     4010 2023-02-14 06:14:48.000000 smdb_api-0.9.1/smdb_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-02-14 06:14:48.000000 smdb_api-0.9.1/smdb_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 06:14:48.000000 smdb_api-0.9.1/smdb_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-14 06:14:48.000000 smdb_api-0.9.1/smdb_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-14 06:14:48.473164 smdb_api-0.9.1/tests/
--rw-rw-rw-   0        0        0     5745 2023-01-24 19:46:18.000000 smdb_api-0.9.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-02-14 16:41:45.309165 smdb_api-0.9.12/
+-rw-rw-rw-   0        0        0     4011 2023-02-14 16:41:45.309665 smdb_api-0.9.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3435 2023-01-15 15:17:06.000000 smdb_api-0.9.12/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_api-0.9.12/pyproject.toml
+-rw-rw-rw-   0        0        0      663 2023-02-14 16:41:45.310666 smdb_api-0.9.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-14 16:41:45.303664 smdb_api-0.9.12/smdb_api/
+-rw-rw-rw-   0        0        0    22498 2023-02-14 16:40:37.000000 smdb_api-0.9.12/smdb_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-14 16:41:45.308165 smdb_api-0.9.12/smdb_api.egg-info/
+-rw-rw-rw-   0        0        0     4011 2023-02-14 16:41:45.000000 smdb_api-0.9.12/smdb_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-02-14 16:41:45.000000 smdb_api-0.9.12/smdb_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-14 16:41:45.000000 smdb_api-0.9.12/smdb_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-02-14 16:41:45.000000 smdb_api-0.9.12/smdb_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-14 16:41:45.308665 smdb_api-0.9.12/tests/
+-rw-rw-rw-   0        0        0     5745 2023-01-24 19:46:18.000000 smdb_api-0.9.12/tests/test.py
```

### Comparing `smdb_api-0.9.1/PKG-INFO` & `smdb_api-0.9.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_api
-Version: 0.9.1
+Version: 0.9.12
 Summary: API package for Server Monitoring Discord Bot
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_api-0.9.1/README.md` & `smdb_api-0.9.12/README.md`

 * *Files identical despite different names*

### Comparing `smdb_api-0.9.1/setup.cfg` & `smdb_api-0.9.12/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6d64 625f 6170 690d 0a76 6572   = smdb_api..ver
-00000020: 7369 6f6e 203d 2030 2e39 2e31 0d0a 6175  sion = 0.9.1..au
-00000030: 7468 6f72 203d 204a 616e 7468 c3b3 2044  thor = Janth.. D
-00000040: c3a1 7669 640d 0a61 7574 686f 725f 656d  ..vid..author_em
-00000050: 6169 6c20 3d20 6461 7669 646a 616e 7468  ail = davidjanth
-00000060: 6f40 676d 6169 6c2e 636f 6d0d 0a64 6573  o@gmail.com..des
-00000070: 6372 6970 7469 6f6e 203d 2041 5049 2070  cription = API p
-00000080: 6163 6b61 6765 2066 6f72 2053 6572 7665  ackage for Serve
-00000090: 7220 4d6f 6e69 746f 7269 6e67 2044 6973  r Monitoring Dis
-000000a0: 636f 7264 2042 6f74 0d0a 6c6f 6e67 5f64  cord Bot..long_d
-000000b0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000c0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000d0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000e0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000f0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000100: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000110: 622e 636f 6d2f 4e69 6768 744b 6579 2f53  b.com/NightKey/S
-00000120: 6572 7665 722d 6d6f 6e69 746f 7269 6e67  erver-monitoring
-00000130: 2d64 6973 636f 7264 2d62 6f74 0d0a 7072  -discord-bot..pr
-00000140: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000150: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-00000160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000170: 2f4e 6967 6874 4b65 792f 5365 7276 6572  /NightKey/Server
-00000180: 2d6d 6f6e 6974 6f72 696e 672d 6469 7363  -monitoring-disc
-00000190: 6f72 642d 626f 742f 6973 7375 6573 0d0a  ord-bot/issues..
-000001a0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001b0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001c0: 7475 7320 3a3a 2034 202d 2042 6574 610d  tus :: 4 - Beta.
-000001d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001f0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-00000200: 3a3a 2046 7265 6577 6172 650d 0a09 4f70  :: Freeware...Op
-00000210: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000220: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000230: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-00000240: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000250: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000260: 203d 203e 3d33 2e37 0d0a 0d0a 5b65 6767   = >=3.7....[egg
-00000270: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000280: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000290: 2030 0d0a 0d0a                            0....
+00000020: 7369 6f6e 203d 2030 2e39 2e31 320d 0a61  sion = 0.9.12..a
+00000030: 7574 686f 7220 3d20 4a61 6e74 68c3 b320  uthor = Janth.. 
+00000040: 44c3 a176 6964 0d0a 6175 7468 6f72 5f65  D..vid..author_e
+00000050: 6d61 696c 203d 2064 6176 6964 6a61 6e74  mail = davidjant
+00000060: 686f 4067 6d61 696c 2e63 6f6d 0d0a 6465  ho@gmail.com..de
+00000070: 7363 7269 7074 696f 6e20 3d20 4150 4920  scription = API 
+00000080: 7061 636b 6167 6520 666f 7220 5365 7276  package for Serv
+00000090: 6572 204d 6f6e 6974 6f72 696e 6720 4469  er Monitoring Di
+000000a0: 7363 6f72 6420 426f 740d 0a6c 6f6e 675f  scord Bot..long_
+000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000c0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+000000e0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+000000f0: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
+00000100: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000110: 7562 2e63 6f6d 2f4e 6967 6874 4b65 792f  ub.com/NightKey/
+00000120: 5365 7276 6572 2d6d 6f6e 6974 6f72 696e  Server-monitorin
+00000130: 672d 6469 7363 6f72 642d 626f 740d 0a70  g-discord-bot..p
+00000140: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000150: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000170: 6d2f 4e69 6768 744b 6579 2f53 6572 7665  m/NightKey/Serve
+00000180: 722d 6d6f 6e69 746f 7269 6e67 2d64 6973  r-monitoring-dis
+00000190: 636f 7264 2d62 6f74 2f69 7373 7565 730d  cord-bot/issues.
+000001a0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000001b0: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+000001c0: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
+000001d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001f0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
+00000200: 203a 3a20 4672 6565 7761 7265 0d0a 094f   :: Freeware...O
+00000210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000220: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000230: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+00000240: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000250: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000260: 7320 3d20 3e3d 332e 370d 0a0d 0a5b 6567  s = >=3.7....[eg
+00000270: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000280: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000290: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `smdb_api-0.9.1/smdb_api/__init__.py` & `smdb_api-0.9.12/smdb_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     def __repr__(self):
         tmp = self.__dict__
         tmp["response"] = self.response.__repr__()
         return tmp
 
     @staticmethod
     def from_message(json: dict) -> "Response":
-        return Response(ResponseCode(json["response"]), json["Data"], json["__bool"] if "__bool" in json.keys() else None)
+        return Response(ResponseCode(json["response"]), json["data"], json["__bool"] if "__bool" in json.keys() else None)
 
 
 class MessageSendingResponse():
 
     def __init__(self, state: ResponseCode, message: Optional[str]) -> None:
         self.state = state
         self.message = message
@@ -323,15 +323,15 @@
                             self.connection_alive = False
                             self.socket.close()
                             self.socket = socket.socket(
                                 socket.AF_INET, socket.SOCK_STREAM)
                             self.socket_list = []
                             if self.sending:
                                 self.buffer.append(
-                                    {"response": ResponseCode.InternalError, "Data": "Connection closed"})
+                                    {"response": ResponseCode.InternalError, "data": "Connection closed"})
                         elif self.sending:
                             self.buffer.append(msg)
                             self.last_message = msg
                         elif not self.sending:
                             message = Message.from_json(msg)
                             if self.last_message is not None and self.last_message == message:
                                 continue
@@ -355,15 +355,15 @@
     def __close_connection(self):
         self.connection_alive = False
         self.socket.close()
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket_list = []
         if self.sending:
             self.buffer.append(
-                {"response": ResponseCode.InternalError, "Data": "Connection closed"})
+                {"response": ResponseCode.InternalError, "data": "Connection closed"})
 
     def __get_copy_function_list(self):
         ret = []
         for item in self.created_function_list:
             ret.append(item)
         return ret
 
@@ -400,15 +400,15 @@
                 if (timeout is not None and timeout > 0 and time() - start > timeout) or not self.running:
                     return False
             self.__send({"Command": self.name, "Value": self.key})
             ansvear = self.__retrive()
             if not isinstance(ansvear, dict):
                 raise ValueError("Bad value retrieved from socket.")
             elif ansvear["response"] == ResponseCode.Denied:
-                raise ValidationError(ansvear["Data"])
+                raise ValidationError(ansvear["data"])
             else:
                 self.valid = True
                 self.socket_list.append(self.socket)
                 if self.created_function_list != []:
                     self.connection_alive = True
                     self.__re_init_commands()
                 if self.initial:
@@ -426,15 +426,15 @@
 
     def is_admin(self, uid: str) -> bool:
         if self.valid:
             self.sending = True
             self.__send({"Command": "Is Admin", "Value": uid})
             tmp = self.__wait_for_response()
             if tmp["response"] == ResponseCode.Success:
-                return tmp["Data"]
+                return tmp["data"]
         else:
             NotValidatedError()
 
     def update(self, _) -> None:
         """Trys to update the API with PIP, and calls the given update function if there is one avaleable.
         """
         system("pip install --user --upgrade smdb_api > pip.txt")
@@ -453,27 +453,27 @@
         else:
             raise NotValidatedError()
 
     def get_username(self, key: str) -> str:
         self.sending = True
         self.__send({"Command": 'Username', "Value": key})
         tmp = self.__wait_for_response()
-        return tmp["Data"] if tmp["response"] == ResponseCode.Success else "unknown"
+        return tmp["data"] if tmp["response"] == ResponseCode.Success else "unknown"
 
     def send_message(self, message: str, interface: Interface, destination: str = None, file_path: str = None) -> bool:
         """Sends a message trough the discord bot.
         """
         msg = Message("API", message, destination, [Attachment(file_path.split(
             "/")[-1], file_path, path.getsize(file_path))] if file_path is not None else [], "API", interface)
         if self.valid:
             self.sending = True
             self.__send({"Command": "Send", 'Value': msg.to_json()})
             tmp = self.__wait_for_response()
             if tmp["response"] == ResponseCode.BadRequest:
-                raise ActionFailed(tmp["Data"])
+                raise ActionFailed(tmp["data"])
             elif tmp["response"] == ResponseCode.InternalError:
                 print(
                     f"[Message sending exception] Internal error: {tmp['Data']}")
                 return False
             return True
         else:
             raise NotValidatedError
@@ -514,15 +514,15 @@
             self.sending = False
             if tmp["response"] == ResponseCode.Success:
                 self.call_list[name] = callback
             elif tmp["response"] == ResponseCode.InternalError:
                 print(
                     f"[_create_function exception] Internal error: {tmp['Data']}")
             else:
-                raise ActionFailed(tmp["Data"])
+                raise ActionFailed(tmp["data"])
         except Exception as ex:
             raise ex
         finally:
             self.sending = False
             self.communicateLock.release()
 
     def __wait_for_response(self) -> Any:
```

### Comparing `smdb_api-0.9.1/smdb_api.egg-info/PKG-INFO` & `smdb_api-0.9.12/smdb_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb-api
-Version: 0.9.1
+Version: 0.9.12
 Summary: API package for Server Monitoring Discord Bot
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_api-0.9.1/tests/test.py` & `smdb_api-0.9.12/tests/test.py`

 * *Files identical despite different names*

