# Comparing `tmp/sui_brownie-0.30.2-py3-none-any.whl.zip` & `tmp/sui_brownie-0.31.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27413 bytes, number of entries: 16
+Zip file size: 27329 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
--rw-r--r--  2.0 unx      114 b- defN 22-Dec-02 09:41 sui_brownie/__init__.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-01 10:43 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    85328 b- defN 23-Apr-11 01:45 sui_brownie/sui_brownie.py
--rw-r--r--  2.0 unx    32515 b- defN 23-Apr-01 08:56 sui_brownie/sui_client.py
+-rw-r--r--  2.0 unx    86164 b- defN 23-Apr-11 09:37 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    32439 b- defN 23-Apr-11 02:45 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
--rw-r--r--  2.0 unx      940 b- defN 23-Apr-01 03:46 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1301 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/RECORD
-16 files, 151363 bytes uncompressed, 25271 bytes compressed:  83.3%
+-rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-11 09:38 sui_brownie-0.31.0.dist-info/RECORD
+16 files, 151972 bytes uncompressed, 25187 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.30.2.dist-info/METADATA
+Filename: sui_brownie-0.31.0.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.30.2.dist-info/WHEEL
+Filename: sui_brownie-0.31.0.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.30.2.dist-info/top_level.txt
+Filename: sui_brownie-0.31.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.30.2.dist-info/RECORD
+Filename: sui_brownie-0.31.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/__init__.py

```diff
@@ -1,5 +1 @@
-# @Time    : 2022/11/28 11:07
-# @Author  : WeiDai
-# @FileName: __init__.py
-
 from sui_brownie.sui_brownie import *
```

## sui_brownie/sui_brownie.py

```diff
@@ -836,25 +836,27 @@
             transactions: list,
             gas_price,
             gas_budget
     ):
         batch_commands = []
         batch_call_args = []
         batch_parameters = []
+        batch_call_args_index = {}
         has_actual_params = DefaultDict(False)
         for (package_id, abi, type_args, call_args) in transactions:
             call_args, type_args = cls.check_args(abi, call_args, type_args)
             # format param
             abi = cls.format_abi_param(abi, type_args)
 
             for i in range(len(call_args)):
                 call_arg = call_args[i]
                 assert isinstance(call_arg, Argument), f"Not support:{call_arg}"
                 actual_params_index = call_arg.value.v0
                 if call_arg.key == "Input" and not has_actual_params[actual_params_index]:
+                    batch_call_args_index[len(batch_call_args)] = actual_params_index
                     batch_call_args.append(actual_params[actual_params_index])
                     batch_parameters.append(abi["parameters"][i])
                     has_actual_params[actual_params_index] = True
             # generate commands
             type_arguments = [
                 cls.generate_type_arg(v) for v in type_args
             ]
@@ -869,16 +871,18 @@
             ]
             batch_commands.extend(commands)
 
         # Prepare object
         object_infos = cls.prepare_object_info(batch_call_args, batch_parameters)
         batch_inputs = []
         for i in range(len(batch_call_args)):
-            batch_inputs.append(cls.generate_call_arg(batch_parameters[i], batch_call_args[i], object_infos))
-
+            batch_inputs.append((batch_call_args_index[i],
+                                 cls.generate_call_arg(batch_parameters[i], batch_call_args[i], object_infos)))
+        batch_inputs.sort(key=lambda x: x[0])
+        batch_inputs = [v[1] for v in batch_inputs]
         return cls.build_intent_message(sender, batch_inputs, batch_commands, gas_price, gas_budget)
 
     @classmethod
     def upgrade(
             cls,
             package_id,
             sender,
@@ -944,29 +948,29 @@
     ):
         object_infos = cls.get_objects([governance_info, governance_contracts, proposal])
         inputs = [
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
                                             ObjectID(governance_info),
                                             SequenceNumber(int(object_infos[governance_info]["owner"]["Shared"]
-                                                           ["initial_shared_version"])),
+                                                               ["initial_shared_version"])),
                                             Bool(False)
                                         ))),
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
                                             ObjectID(governance_contracts),
                                             SequenceNumber(int(object_infos[governance_contracts]["owner"]["Shared"]
-                                                           ["initial_shared_version"])),
+                                                               ["initial_shared_version"])),
                                             Bool(True)
                                         ))),
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
                                             ObjectID(proposal),
                                             SequenceNumber(int(object_infos[proposal]["owner"]["Shared"]
-                                                           ["initial_shared_version"])),
+                                                               ["initial_shared_version"])),
                                             Bool(True)
                                         ))),
         ]
         arguments = [Argument("Input", U16(i)) for i in range(len(inputs))]
         commands = [
             Command("MoveCall", ProgrammableMoveCall(
                 ObjectID(proposal_package_id),
@@ -1425,14 +1429,31 @@
         except:
             for k in replace_tomls:
                 replace_tomls[k].restore()
             traceback.print_exc()
             raise
         return result
 
+    def generate_digest(
+            self,
+            replace_address: dict = None,
+    ):
+        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        try:
+            cmd = f"sui move build --dump-package-digest " \
+                  f"--path {self.package_path.absolute()}"
+            with os.popen(cmd) as f:
+                result = f.read()
+            return result
+        except:
+            traceback.print_exc()
+
+        for k in replace_tomls:
+            replace_tomls[k].restore()
+
     def program_dola_upgrade_package(
             self,
             proposal_package_id,
             governance_info: str,
             governance_contracts: str,
             proposal: str,
             replace_address: dict = None,
@@ -1929,15 +1950,15 @@
         )
 
     def unsafe_pay_all_sui(self, input_coins=None, recipient=None, gas_budget=100000000):
         if recipient is None:
             recipient = self.account.account_address
         if input_coins is None:
             input_coins = list(self.get_account_sui().keys())
-        result = self.client.unsafe_payAllSui(self.account.account_address, input_coins, recipient, gas_budget)
+        result = self.client.unsafe_payAllSui(self.account.account_address, input_coins, recipient, str(gas_budget))
 
         # Simulate before execute
         tx_bytes = result["txBytes"]
         self.client.sui_dryRunTransactionBlock(tx_bytes)
 
         # sig
         msg = bytes([IntentScope.TransactionData[1], IntentVersion.V0[1], AppId.Sui[1]]
```

## sui_brownie/sui_client.py

```diff
@@ -1,10 +1,7 @@
-# @Time    : 2023/3/28 20:03
-# @Author  : WeiDai
-# @FileName: sui_client.py
 from retrying import retry
 import httpx
 
 
 class ApiError(Exception):
     """Error thrown when the API returns >= 400"""
```

## sui_brownie/utils.py

```diff
@@ -1,12 +1,7 @@
-# @Time    : 2022/11/24 13:50
-# @Author  : WeiDai
-# @FileName: utils.py
-
-
 def get_bytes(string: str) -> bytes:
     if isinstance(string, bytes):
         byte = string
     elif isinstance(string, str):
         if string[:2] == "0x":
             string = string[2:]
         byte = bytes.fromhex(string)
```

## Comparing `sui_brownie-0.30.2.dist-info/METADATA` & `sui_brownie-0.31.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.30.2
+Version: 0.31.0
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-0.30.2.dist-info/RECORD` & `sui_brownie-0.31.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
-sui_brownie/__init__.py,sha256=2136vfOmqj4xBFk70Z3Ct1-ohClWm4Cz9EUFbS_FgTU,114
+sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=zHKa_3TBt2VbzXa_ZJn6ZpalECSeLOoC5XHMDr5R-aM,85328
-sui_brownie/sui_client.py,sha256=kuca5LZkYrAaHRJRf6pUyfl22U_ArUxCoG73fiGcK3A,32515
+sui_brownie/sui_brownie.py,sha256=iHrr4e51D6pRPxvu5GcClo1bo5ia0QeP99KDU7bcEh8,86164
+sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
-sui_brownie/utils.py,sha256=vJj0Uhu9B86y4XDptvvNDcH5-PwS8XEjIgpSqpj8EVU,940
-sui_brownie-0.30.2.dist-info/METADATA,sha256=VlsF1VylSiS05S3qJHcP7hNj7MbFmPlwWfpZF0JvHxY,983
-sui_brownie-0.30.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-0.30.2.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-0.30.2.dist-info/RECORD,,
+sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
+sui_brownie-0.31.0.dist-info/METADATA,sha256=fOdHX9q7z3rJt0g1XT78D03ZJbOA4Nxd7rWnFqwdHRk,983
+sui_brownie-0.31.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-0.31.0.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-0.31.0.dist-info/RECORD,,
```

