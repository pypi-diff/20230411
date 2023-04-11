# Comparing `tmp/hil_core-0.0.2-cp37-cp37m-win_amd64.whl.zip` & `tmp/hil_core-0.0.3-cp37-cp37m-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 115756 bytes, number of entries: 14
+Zip file size: 136072 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat       27 b- defN 23-Apr-11 08:33 hil/bus/__init__.py
+-rw-rw-rw-  2.0 fat      182 b- defN 23-Apr-11 08:33 hil/bus/utils.py
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Mar-16 08:56 hil/common/__init__.py
 -rw-rw-rw-  2.0 fat     1499 b- defN 23-Mar-15 01:14 hil/common/log.py
--rw-rw-rw-  2.0 fat     4749 b- defN 23-Mar-16 07:43 hil/common/utils.py
--rw-rw-rw-  2.0 fat      458 b- defN 23-Mar-17 07:10 hil/core/__init__.py
--rw-rw-rw-  2.0 fat    65024 b- defN 23-Mar-17 07:04 hil/core/cantp.cp37-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5293 b- defN 23-Apr-11 10:25 hil/common/utils.py
+-rw-rw-rw-  2.0 fat      493 b- defN 23-Apr-11 10:45 hil/core/__init__.py
+-rw-rw-rw-  2.0 fat    65024 b- defN 23-Apr-11 10:12 hil/core/cantp.cp37-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      630 b- defN 23-Mar-17 07:03 hil/core/cantp.pyi
--rw-rw-rw-  2.0 fat    78336 b- defN 23-Mar-16 16:05 hil/core/doip_client.cp37-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    78336 b- defN 23-Apr-11 10:12 hil/core/doip_client.cp37-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      702 b- defN 23-Mar-15 01:14 hil/core/doip_client.pyi
--rw-rw-rw-  2.0 fat   106496 b- defN 23-Mar-16 16:05 hil/core/uds_client.cp37-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   106496 b- defN 23-Apr-11 10:12 hil/core/uds_client.cp37-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      693 b- defN 23-Mar-15 01:14 hil/core/uds_client.pyi
--rw-rw-rw-  2.0 fat      220 b- defN 23-Mar-17 07:10 hil_core-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      101 b- defN 23-Mar-17 07:10 hil_core-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-17 07:10 hil_core-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1123 b- defN 23-Mar-17 07:10 hil_core-0.0.2.dist-info/RECORD
-14 files, 260427 bytes uncompressed, 113900 bytes compressed:  56.3%
+-rw-rw-rw-  2.0 fat    43008 b- defN 23-Apr-11 10:25 hil/core/uds_server.cp37-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      426 b- defN 23-Apr-11 10:39 hil/core/uds_server.pyi
+-rw-rw-rw-  2.0 fat      220 b- defN 23-Apr-11 10:45 hil_core-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-11 10:45 hil_core-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-11 10:45 hil_core-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1444 b- defN 23-Apr-11 10:45 hil_core-0.0.3.dist-info/RECORD
+18 files, 304970 bytes uncompressed, 133720 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: hil/bus/__init__.py
+Comment: 
+
+Filename: hil/bus/utils.py
+Comment: 
+
 Filename: hil/common/__init__.py
 Comment: 
 
 Filename: hil/common/log.py
 Comment: 
 
 Filename: hil/common/utils.py
@@ -24,20 +30,26 @@
 
 Filename: hil/core/uds_client.cp37-win_amd64.pyd
 Comment: 
 
 Filename: hil/core/uds_client.pyi
 Comment: 
 
-Filename: hil_core-0.0.2.dist-info/METADATA
+Filename: hil/core/uds_server.cp37-win_amd64.pyd
+Comment: 
+
+Filename: hil/core/uds_server.pyi
+Comment: 
+
+Filename: hil_core-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: hil_core-0.0.2.dist-info/WHEEL
+Filename: hil_core-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: hil_core-0.0.2.dist-info/top_level.txt
+Filename: hil_core-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hil_core-0.0.2.dist-info/RECORD
+Filename: hil_core-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hil/common/utils.py

```diff
@@ -1,122 +1,133 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 '''
 Author: notmmao@gmail.com
 Date: 2022-06-02 10:11:48
-LastEditors: hufeng.mao@carota.ai
-LastEditTime: 2023-03-16 15:42:12
+LastEditors: notmmao@gmail.com
+LastEditTime: 2023-04-11 18:25:02
 Description: 
 '''
 import os
+import time
 import json
 import datetime
 import argparse
 import hashlib
 from typing import Union, Dict
 
 import can
 
+
 def now():
     n = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     return n
 
-def save_json(tag, data:dict):
+
+def save_json(tag, data: dict):
     n = now()
     fn = f"json/{tag}_{n}.json"
     with open(fn, "w+", encoding="utf-8") as f:
         json.dump(data, f, indent=4, ensure_ascii=False)
         print(f"save {fn} success")
 
+
 def filter_uds(bus: can.BusABC):
     filters = [
         {"can_id": 0x700, "can_mask": 0xf00, "extended": False},
     ]
     bus.set_filters(filters)
 
+
 def filter_sk(bus: can.BusABC):
     filters = [
         {"can_id": 0x700, "can_mask": 0xf00, "extended": False},
         # {"can_id": 0x40B, "can_mask": 0xfff, "extended": False},
         {"can_id": 0x456, "can_mask": 0xfff, "extended": False},
         {"can_id": 0x45c, "can_mask": 0xfff, "extended": False},
         {"can_id": 0x47d, "can_mask": 0xfff, "extended": False},
         {"can_id": 0x47f, "can_mask": 0xfff, "extended": False},
         # {"can_id": 0x2EA, "can_mask": 0xfff, "extended": False},
     ]
     bus.set_filters(filters)
 
-def parser_bus(t:str):
+
+def parser_bus(t: str):
     if t == "vector":
-        bus = can.interface.Bus(bustype='vector', channel=0, app_name="python_can", fd=True)
+        bus = can.interface.Bus(
+            bustype='vector', channel=0, app_name="python_can", fd=True)
     elif t == "vector0":
-        bus = can.interface.Bus(bustype='vector', channel=0, app_name="python_can", fd=True)
+        bus = can.interface.Bus(
+            bustype='vector', channel=0, app_name="python_can", fd=True)
     elif t == "vector1":
-        bus = can.interface.Bus(bustype='vector', channel=1, app_name="python_can", fd=True)
+        bus = can.interface.Bus(
+            bustype='vector', channel=1, app_name="python_can", fd=True)
     elif t.startswith("vcan"):
         bus = can.interface.Bus(bustype='socketcan', channel=t, bitrate=500000)
     elif t.startswith("can"):
         bus = can.interface.Bus(bustype='socketcan', channel=t, bitrate=500000)
     else:
         bus = can.interface.Bus(bustype='virtual')
     return bus
 
+
 def parser_canid(id):
     # print(id)
     try:
         canid = int(id)
     except ValueError:
         canid = int(id, 16)
 
     return canid
 
-def parser_hex(data:str):
+
+def parser_hex(data: str):
     data = data.replace(" ", "")
     data = bytearray.fromhex(data)
     return data
 
 
 def common_parser(description: str = None) -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description=description)
 
     parser.add_argument('-l', '--log', help='log文件')
     parser.add_argument('-t', '--txid', default=0x707, type=parser_canid,
                         help='Tester tx id')
     parser.add_argument('-r', '--rxid', default=0x717, type=parser_canid,
                         help='Tester rx id')
     parser.add_argument('-v', '--vin', default="LVTDB21B6ND167534",
-                            help='VIN')
+                        help='VIN')
     parser.add_argument('-b', '--bus', type=parser_bus, default='vector')
     parser.add_argument('--app-name', default='python_can')
     parser.add_argument('--busses',  type=parser_bus, nargs="+")
     parser.add_argument('-d', '--dbc', default="gp01.dbc")
     parser.add_argument('--data', type=parser_hex)
     parser.add_argument('--mask', type=parser_canid)
 
     parser.add_argument('-a', '--action')
-    parser.add_argument('-p', '--platform', choices=["m1e", "t18p", "m1e_tenpao"], default="m1e")
-    
-    return parser
+    parser.add_argument('-p', '--platform',
+                        choices=["m1e", "t18p", "m1e_tenpao"], default="m1e")
 
+    return parser
 
 
 def get_input(dump=False) -> Union[Dict, None]:
     '''从环境变量获取客户端传来的input参数
 
     :param bool dump: 是否打印输入字符串, defaults to False
     :return None or dict: None或者解析后的dict类型参数
     '''
     input = os.getenv('input')
     if input is not None:
         if dump:
             print(input)
         input.replace('\\', '\\\\')
         input = json.loads(input)
-    
+
     return input
 
 
 # 一个装饰器, 在函数执行前后打印日志
 def run_script(func):
     def wrapper(*args, **kwargs):
         try:
@@ -125,29 +136,50 @@
             print(f"结束")
         except Exception as e:
             print(e)
             exit(-1)
         return result
     return wrapper
 
+
 def md5file(fn):
     '''计算文件的md5值
 
     :param function fn: 要计算md5值的文件
     :return str: MD5摘要值, hex格式
     '''
     md5 = hashlib.md5()
     with open(fn, "rb") as f:
         while True:
             d = f.read(4096)
-            if not d: break
+            if not d:
+                break
             md5.update(d)
         return md5.hexdigest()
 
 
+def debounce(wait):
+    def decorator(fn):
+        last_call_time = 0
+
+        def debounced(*args, **kwargs):
+            nonlocal last_call_time
+
+            elapsed_time = time.time() - last_call_time
+            if elapsed_time < wait:
+                return None
+
+            result = fn(*args, **kwargs)
+            last_call_time = time.time()
+
+            return result
+        return debounced
+    return decorator
+
+
 __version__ = '1.0.0'
 __author__ = 'notmmao@gmail.com'
 
 
 def main():
     parser = common_parser("hello")
     args = parser.parse_args()
```

## hil/core/__init__.py

```diff
@@ -1,17 +1,18 @@
 '''
 Copyright (c) 2023 by HIL Group
 Author: hufeng.mao@carota.ai
 Date: 2023-03-16 16:13:35
 LastEditors: notmmao@gmail.com
-LastEditTime: 2023-03-17 15:10:01
+LastEditTime: 2023-04-11 18:45:10
 Description: 
 
 ==========  =============  ================
 When        Who            What and why
 ==========  =============  ================
 
 ==========  =============  ================
 '''
 from .uds_client import UdsClient
 from .doip_client import DoipClient
-from .cantp import Cantp
+from .cantp import Cantp
+from .uds_server import UdsServer
```

## Comparing `hil_core-0.0.2.dist-info/RECORD` & `hil_core-0.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+hil/bus/__init__.py,sha256=opjDDG0kGS6ft1bZoa_e70-mmCg85pwUypCADVZUJsQ,27
+hil/bus/utils.py,sha256=v08_DXPkDBE7zED0IvJcZA3w7Nz61Kd87h2bsUDa7wM,182
 hil/common/__init__.py,sha256=bOInhQJDhv9_UuTvVJpwb8MZ3EUNZ6SMTGAyQOxBHF4,392
 hil/common/log.py,sha256=_FE0j-t1rruoszxkbHY0ZbqOhMnPof8vNrOBV4zp1GI,1499
-hil/common/utils.py,sha256=SV1IC4n6zq0yWaCySz1lBm6obrgwHMTxfMXcLiMwLUU,4749
-hil/core/__init__.py,sha256=vovERq2KFCIihO8mka-UabZR-aDV3GZztcKUaZaQ9m8,458
-hil/core/cantp.cp37-win_amd64.pyd,sha256=4fO989p7rUL0-GEKTpFBrzhrMr15TMkPhXO1AhlFj20,65024
+hil/common/utils.py,sha256=Zy-uCCbEH15gwQWyKwXrjY_ifaesqExuKn9TKilLkE0,5293
+hil/core/__init__.py,sha256=6Irtb7633Y1TUENcLQtLuQJN6txcWzeoEJyyjuunvtc,493
+hil/core/cantp.cp37-win_amd64.pyd,sha256=2HFHhh777Laa4MFmqCW5FwSCDn1OE03M-WVbFtdJFbg,65024
 hil/core/cantp.pyi,sha256=CenHISiYlxihBrl7wgKF58-VJM6LnWS_woRPwAgrjxU,630
-hil/core/doip_client.cp37-win_amd64.pyd,sha256=31FHdLJa6OPZb5KGkvfHw2pEwCqoDtnT5CTUbJdoaw4,78336
+hil/core/doip_client.cp37-win_amd64.pyd,sha256=XRSZvF97LSKU64zapJBnriPni0nDHA5E54Nx_acoOws,78336
 hil/core/doip_client.pyi,sha256=AVt3ygh16BN-LEXQ97hLBUdsfBPivvCrhH7V5-tJxHA,702
-hil/core/uds_client.cp37-win_amd64.pyd,sha256=0FI9DZPqyFReKLH089utU5lHZdGvoRdOQT30N0xNrBY,106496
+hil/core/uds_client.cp37-win_amd64.pyd,sha256=1lDZs1ts2F4wJ5BkH12WDDxDNaQqK-7VhQ9uIGHvsQE,106496
 hil/core/uds_client.pyi,sha256=BzG4tDeU2uj888EBHLngnUjBYeX7XGIuitGDCQ7OkW8,693
-hil_core-0.0.2.dist-info/METADATA,sha256=vA3bbdMPoXKYZr3E4E9_VflPcmH5ym2RXGhz4g6XzI0,220
-hil_core-0.0.2.dist-info/WHEEL,sha256=zMRqF9ZfHGxBPfvcWwE-LxcVkdB1hhr8hy4cOfZGPZU,101
-hil_core-0.0.2.dist-info/top_level.txt,sha256=NkmE0ej9RUq1cTbNBwJxAlTf324GfzDyFlCh3vbdJ44,4
-hil_core-0.0.2.dist-info/RECORD,,
+hil/core/uds_server.cp37-win_amd64.pyd,sha256=ip9gCuWANqS1wsxWhDojA5Oj1hgxHSthpwFrkImQV1c,43008
+hil/core/uds_server.pyi,sha256=waVmcIzm4XCkQTkY0TGbhehoT44q8SjlxKk49LJuDjE,426
+hil_core-0.0.3.dist-info/METADATA,sha256=P-2H50IKaDxk3DZ6cEhCaLcThh2Mqv9WgckyPGEfBDA,220
+hil_core-0.0.3.dist-info/WHEEL,sha256=zMRqF9ZfHGxBPfvcWwE-LxcVkdB1hhr8hy4cOfZGPZU,101
+hil_core-0.0.3.dist-info/top_level.txt,sha256=NkmE0ej9RUq1cTbNBwJxAlTf324GfzDyFlCh3vbdJ44,4
+hil_core-0.0.3.dist-info/RECORD,,
```

