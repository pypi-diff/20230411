# Comparing `tmp/sui_brownie-0.30.1-py3-none-any.whl.zip` & `tmp/sui_brownie-0.30.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27407 bytes, number of entries: 16
+Zip file size: 27413 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx      114 b- defN 22-Dec-02 09:41 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-01 10:43 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    85323 b- defN 23-Apr-11 01:42 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    85328 b- defN 23-Apr-11 01:45 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32515 b- defN 23-Apr-01 08:56 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      940 b- defN 23-Apr-01 03:46 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-11 01:43 sui_brownie-0.30.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 01:43 sui_brownie-0.30.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 01:43 sui_brownie-0.30.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1301 b- defN 23-Apr-11 01:43 sui_brownie-0.30.1.dist-info/RECORD
-16 files, 151358 bytes uncompressed, 25265 bytes compressed:  83.3%
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1301 b- defN 23-Apr-11 01:46 sui_brownie-0.30.2.dist-info/RECORD
+16 files, 151363 bytes uncompressed, 25271 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.30.1.dist-info/METADATA
+Filename: sui_brownie-0.30.2.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.30.1.dist-info/WHEEL
+Filename: sui_brownie-0.30.2.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.30.1.dist-info/top_level.txt
+Filename: sui_brownie-0.30.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.30.1.dist-info/RECORD
+Filename: sui_brownie-0.30.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -593,15 +593,15 @@
                 if gas_amount >= gas_budget:
                     break
                 payment = [ObjectRef(
                     ObjectID(gas["coinObjectId"]),
                     SequenceNumber(int(gas["version"])),
                     ObjectDigest(gas["digest"])
                 )]
-                gas_amount += gas["balance"]
+                gas_amount += int(gas["balance"])
 
         owner = SuiAddress(sender)
         price = U64(gas_price)
         budget = U64(gas_budget)
         expiration = TransactionExpiration("NONE", NONE())
         transaction_data_v1 = TransactionDataV1(TransactionKind("ProgrammableTransaction", programmable_transaction),
                                                 SuiAddress(sender),
```

## Comparing `sui_brownie-0.30.1.dist-info/METADATA` & `sui_brownie-0.30.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.30.1
+Version: 0.30.2
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-0.30.1.dist-info/RECORD` & `sui_brownie-0.30.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=2136vfOmqj4xBFk70Z3Ct1-ohClWm4Cz9EUFbS_FgTU,114
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=oeXPDrrnuI5ZnW2C9hyvDtwjwMczLUMfF73iVgGThuQ,85323
+sui_brownie/sui_brownie.py,sha256=zHKa_3TBt2VbzXa_ZJn6ZpalECSeLOoC5XHMDr5R-aM,85328
 sui_brownie/sui_client.py,sha256=kuca5LZkYrAaHRJRf6pUyfl22U_ArUxCoG73fiGcK3A,32515
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=vJj0Uhu9B86y4XDptvvNDcH5-PwS8XEjIgpSqpj8EVU,940
-sui_brownie-0.30.1.dist-info/METADATA,sha256=uDiR2d-2lX_2TaiG8kum2PtWNuINRfUFH2dvt5MQY-U,983
-sui_brownie-0.30.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-0.30.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-0.30.1.dist-info/RECORD,,
+sui_brownie-0.30.2.dist-info/METADATA,sha256=VlsF1VylSiS05S3qJHcP7hNj7MbFmPlwWfpZF0JvHxY,983
+sui_brownie-0.30.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-0.30.2.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-0.30.2.dist-info/RECORD,,
```

