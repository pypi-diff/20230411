# Comparing `tmp/pactsdk-0.6.0.tar.gz` & `tmp/pactsdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pactsdk-0.6.0.tar", max compression
+gzip compressed data, was "pactsdk-0.6.1.tar", max compression
```

## Comparing `pactsdk-0.6.0.tar` & `pactsdk-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.6.0/LICENSE
--rw-r--r--   0        0        0     5482 2023-03-30 10:07:17.918258 pactsdk-0.6.0/README.md
--rw-r--r--   0        0        0      538 2023-03-30 10:07:05.564919 pactsdk-0.6.0/pactsdk/__init__.py
--rw-r--r--   0        0        0     4504 2023-01-03 15:45:49.490178 pactsdk-0.6.0/pactsdk/add_liquidity.py
--rw-r--r--   0        0        0     2174 2022-07-14 08:55:23.297528 pactsdk-0.6.0/pactsdk/api.py
--rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.6.0/pactsdk/asset.py
--rw-r--r--   0        0        0     5263 2023-03-30 10:07:12.264922 pactsdk-0.6.0/pactsdk/client.py
--rw-r--r--   0        0        0     1716 2023-03-30 10:07:05.564919 pactsdk-0.6.0/pactsdk/config.py
--rw-r--r--   0        0        0     2353 2022-07-14 08:55:23.297528 pactsdk-0.6.0/pactsdk/constant_product_calculator.py
--rw-r--r--   0        0        0      852 2023-03-09 15:26:59.934347 pactsdk-0.6.0/pactsdk/encoding.py
--rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.6.0/pactsdk/exceptions.py
--rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.6.0/pactsdk/factories/__init__.py
--rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.6.0/pactsdk/factories/base_factory.py
--rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.6.0/pactsdk/factories/constant_product.py
--rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.6.0/pactsdk/factories/get_pool_factory.py
--rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.6.0/pactsdk/farming/README.md
--rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.6.0/pactsdk/farming/__init__.py
--rw-r--r--   0        0        0     7728 2023-03-30 09:06:45.864508 pactsdk-0.6.0/pactsdk/farming/escrow.py
--rw-r--r--   0        0        0    17146 2023-03-30 09:06:45.871175 pactsdk-0.6.0/pactsdk/farming/farm.py
--rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.6.0/pactsdk/farming/farm_state.py
--rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.6.0/pactsdk/farming/farming_client.py
--rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.6.0/pactsdk/gas_station.py
--rw-r--r--   0        0        0    24155 2023-03-30 10:07:05.564919 pactsdk-0.6.0/pactsdk/pool.py
--rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.6.0/pactsdk/pool_calculator.py
--rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.6.0/pactsdk/pool_state.py
--rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.6.0/pactsdk/stableswap_calculator.py
--rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.6.0/pactsdk/swap.py
--rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.6.0/pactsdk/transaction_group.py
--rw-r--r--   0        0        0     2166 2023-03-30 09:06:45.861175 pactsdk-0.6.0/pactsdk/utils.py
--rw-r--r--   0        0        0     5535 2022-08-18 13:32:35.849222 pactsdk-0.6.0/pactsdk/zap.py
--rw-r--r--   0        0        0     1022 2023-03-30 10:07:05.564919 pactsdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 pactsdk-0.6.0/setup.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 pactsdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5482 2023-03-30 10:07:17.918258 pactsdk-0.6.1/README.md
+-rw-r--r--   0        0        0      538 2023-04-11 09:21:24.923112 pactsdk-0.6.1/pactsdk/__init__.py
+-rw-r--r--   0        0        0     4504 2023-01-03 15:45:49.490178 pactsdk-0.6.1/pactsdk/add_liquidity.py
+-rw-r--r--   0        0        0     2174 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/api.py
+-rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.6.1/pactsdk/asset.py
+-rw-r--r--   0        0        0     5263 2023-03-30 10:07:12.264922 pactsdk-0.6.1/pactsdk/client.py
+-rw-r--r--   0        0        0     1725 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/config.py
+-rw-r--r--   0        0        0     2353 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/constant_product_calculator.py
+-rw-r--r--   0        0        0      852 2023-03-09 15:26:59.934347 pactsdk-0.6.1/pactsdk/encoding.py
+-rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/exceptions.py
+-rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/factories/__init__.py
+-rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/base_factory.py
+-rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/constant_product.py
+-rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/get_pool_factory.py
+-rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.6.1/pactsdk/farming/README.md
+-rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.6.1/pactsdk/farming/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/farming/escrow.py
+-rw-r--r--   0        0        0    16770 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/farming/farm.py
+-rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.6.1/pactsdk/farming/farm_state.py
+-rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.6.1/pactsdk/farming/farming_client.py
+-rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.6.1/pactsdk/gas_station.py
+-rw-r--r--   0        0        0    24155 2023-03-30 10:07:05.564919 pactsdk-0.6.1/pactsdk/pool.py
+-rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/pool_calculator.py
+-rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/pool_state.py
+-rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.6.1/pactsdk/stableswap_calculator.py
+-rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.6.1/pactsdk/swap.py
+-rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.6.1/pactsdk/transaction_group.py
+-rw-r--r--   0        0        0     2166 2023-03-30 09:06:45.861175 pactsdk-0.6.1/pactsdk/utils.py
+-rw-r--r--   0        0        0     5535 2022-08-18 13:32:35.849222 pactsdk-0.6.1/pactsdk/zap.py
+-rw-r--r--   0        0        0     1022 2023-04-11 09:21:14.509777 pactsdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 pactsdk-0.6.1/setup.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 pactsdk-0.6.1/PKG-INFO
```

### Comparing `pactsdk-0.6.0/LICENSE` & `pactsdk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/README.md` & `pactsdk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/__init__.py` & `pactsdk-0.6.1/pactsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 from .add_liquidity import LiquidityAddition  # noqa
 from .asset import Asset, fetch_asset_by_index  # noqa
 from .client import PactClient  # noqa
 from .exceptions import PactSdkError  # noqa
 from .factories import *  # noqa
 from .farming import *  # noqa
```

### Comparing `pactsdk-0.6.0/pactsdk/add_liquidity.py` & `pactsdk-0.6.1/pactsdk/add_liquidity.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/api.py` & `pactsdk-0.6.1/pactsdk/api.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/asset.py` & `pactsdk-0.6.1/pactsdk/asset.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/client.py` & `pactsdk-0.6.1/pactsdk/client.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/config.py` & `pactsdk-0.6.1/pactsdk/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 from typing import Literal
 
 MAINNET_API_URL = "https://api.pact.fi"
 MAINNET_GAS_STATION_ID = 1027956681
 MAINNET_FACTORY_CONSTANT_PRODUCT_ID = 1072843805
-MAINNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 0
+MAINNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 1076423760
 
 TESTNET_API_URL = "https://api.testnet.pact.fi"
 TESTNET_GAS_STATION_ID = 156575978
 TESTNET_FACTORY_CONSTANT_PRODUCT_ID = 166540424
 TESTNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 166540708
 
 Network = Literal["mainnet", "testnet", "dev"]
```

### Comparing `pactsdk-0.6.0/pactsdk/constant_product_calculator.py` & `pactsdk-0.6.1/pactsdk/constant_product_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/encoding.py` & `pactsdk-0.6.1/pactsdk/encoding.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/factories/base_factory.py` & `pactsdk-0.6.1/pactsdk/factories/base_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/factories/constant_product.py` & `pactsdk-0.6.1/pactsdk/factories/constant_product.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/factories/get_pool_factory.py` & `pactsdk-0.6.1/pactsdk/factories/get_pool_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/farming/README.md` & `pactsdk-0.6.1/pactsdk/farming/README.md`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/farming/__init__.py` & `pactsdk-0.6.1/pactsdk/farming/__init__.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/farming/escrow.py` & `pactsdk-0.6.1/pactsdk/farming/escrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from ..gas_station import get_gas_station
 from ..utils import get_selector, parse_app_state, sp_fee
 
 if TYPE_CHECKING:
     from .farm import Farm
 
+COMPILED_HUSK_APPROVAL = "CCACAAExGEAASYALTWFzdGVyQXBwSUQ2GgEXwDJnsYEGshA2GgIXwDKyGIAEtzVf0bIaIrIBs7GBBLIQMgqyFCKyEjYaAxfAMLIRIrIBsyNCAAEjQw=="
 COMPILED_CLEAR_PROGRAM_B64 = "CIEBQw=="
 
 REKEY_TO_USER_FEE = 2000
 REKEY_TO_CONTRACT_FEE = 1000
 
 CREATE_SIG = get_selector("create(application,application,asset)void")
 UNSTAKE_SIG = get_selector("unstake(asset,uint64,application)void")
@@ -39,18 +40,18 @@
     return base64.b64decode(box["value"])
 
 
 def build_deploy_escrow_txs(
     sender: str,
     farm_app_id: int,
     staked_asset_id: int,
-    approval_program: bytes,
     suggested_params: transaction.SuggestedParams,
 ) -> list[transaction.Transaction]:
 
+    approval_program = base64.b64decode(COMPILED_HUSK_APPROVAL)
     clear_program = base64.b64decode(COMPILED_CLEAR_PROGRAM_B64)
 
     gas_station = get_gas_station()
 
     fund_tx = gas_station.build_fund_tx(
         sender=sender,
         amount=200_000,
@@ -60,15 +61,15 @@
     create_app_tx = transaction.ApplicationCreateTxn(
         sender=sender,
         approval_program=approval_program,
         clear_program=clear_program,
         on_complete=transaction.OnComplete.NoOpOC,
         global_schema=transaction.StateSchema(1, 0),
         local_schema=transaction.StateSchema(0, 0),
-        sp=sp_fee(suggested_params, 4000),
+        sp=sp_fee(suggested_params, 5000),
         foreign_apps=[farm_app_id, gas_station.app_id],
         foreign_assets=[staked_asset_id],
         app_args=[CREATE_SIG, 1, 2, 0],
     )
 
     app_opt_in_tx = transaction.ApplicationOptInTxn(
         sender=sender, sp=suggested_params, index=farm_app_id
```

### Comparing `pactsdk-0.6.0/pactsdk/farming/farm.py` & `pactsdk-0.6.1/pactsdk/farming/farm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,15 @@
 from algosdk.v2client.algod import AlgodClient
 
 from pactsdk.asset import Asset, fetch_asset_by_index
 
 from ..encoding import deserialize_uint64
 from ..gas_station import get_gas_station
 from ..utils import get_selector, parse_app_state, sp_fee
-from .escrow import (
-    Escrow,
-    build_deploy_escrow_txs,
-    fetch_escrow_approval_program,
-    fetch_escrow_by_id,
-)
+from .escrow import Escrow, build_deploy_escrow_txs, fetch_escrow_by_id
 from .farm_state import (
     FarmingRewards,
     FarmInternalState,
     FarmState,
     FarmUserState,
     format_rewards,
     format_rpt,
@@ -339,26 +334,19 @@
     ) -> FarmingRewards[int]:
         return {
             asset: amount + rewards_b.get(asset, 0)
             for asset, amount in rewards_a.items()
         }
 
     def prepare_deploy_escrow_txs(self, sender: str) -> list[transaction.Transaction]:
-        approval_program = fetch_escrow_approval_program(self.algod, self.app_id)
-        return self.build_deploy_escrow_txs(sender, approval_program)
-
-    def build_deploy_escrow_txs(
-        self, sender: str, approval_program: bytes
-    ) -> list[transaction.Transaction]:
         return build_deploy_escrow_txs(
             sender=sender,
             farm_app_id=self.app_id,
             staked_asset_id=self.staked_asset.index,
             suggested_params=self.suggested_params,
-            approval_program=approval_program,
         )
 
     def build_update_increase_opcode_quota_tx(
         self, sender: str
     ) -> Optional[transaction.Transaction]:
         seconds_passed = (datetime.datetime.now() - self.state.updated_at).seconds
         opcodes_cost = 671 if seconds_passed > self.state.duration > 0 else 513
```

### Comparing `pactsdk-0.6.0/pactsdk/farming/farm_state.py` & `pactsdk-0.6.1/pactsdk/farming/farm_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/farming/farming_client.py` & `pactsdk-0.6.1/pactsdk/farming/farming_client.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/gas_station.py` & `pactsdk-0.6.1/pactsdk/gas_station.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/pool.py` & `pactsdk-0.6.1/pactsdk/pool.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/pool_calculator.py` & `pactsdk-0.6.1/pactsdk/pool_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/pool_state.py` & `pactsdk-0.6.1/pactsdk/pool_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/stableswap_calculator.py` & `pactsdk-0.6.1/pactsdk/stableswap_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/swap.py` & `pactsdk-0.6.1/pactsdk/swap.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/transaction_group.py` & `pactsdk-0.6.1/pactsdk/transaction_group.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/utils.py` & `pactsdk-0.6.1/pactsdk/utils.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pactsdk/zap.py` & `pactsdk-0.6.1/pactsdk/zap.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.0/pyproject.toml` & `pactsdk-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pactsdk"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python SDK for Pact smart contracts"
 authors = ["Mateusz Tomczyk <mateusz.tomczyk@ulam.io>"]
 homepage = "https://github.com/pactfi/pact-py-sdk"
 repository = "https://github.com/pactfi/pact-py-sdk"
 readme = "README.md"
 license = "MIT"
```

### Comparing `pactsdk-0.6.0/setup.py` & `pactsdk-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['py-algorand-sdk>=2.0.0,<3.0.0', 'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'pactsdk',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Python SDK for Pact smart contracts',
     'long_description': '# Pact Python SDK\n\n**pactsdk** is a software development kit for interfacing to [Pact](https://pact.fi), a decentralized automated market maker on the Algorand protocol.\n\nThe full documentation for this module can be found here:\n\n[https://pactfi.github.io/pact-py-sdk/latest/](https://pactfi.github.io/pact-py-sdk/latest/)\n\nThe Python SDK provides a set of modules on top of the Algorand Python SDK for interacting with liquidity pools and making swaps.\nClients can use the Python SDK to enhance their trading experience with Pact.\n\nWhat is covered by the library:\n\n- Creating pools\n- Managing liquidity\n- Making swaps\n- Farming\n\nSigning and sending transactions is not covered by the library. The provided examples use algosdk directly to send the transactions.\n\n# Installation\n\n`pip install pactsdk`\n\n# Basic usage\n\n**CAUTION** - The library uses integers for asset amounts e.g. microalgos instead of algos so if you want to send 1 algo, you need to specify it as 1_000_000.\n\nCreate a Pact client.\n\n```py\nfrom algosdk.v2client.algod import AlgodClient\nimport pactsdk\n\nalgod = AlgodClient(token, url)\npact = pactsdk.PactClient(algod)\n```\n\nBy default, the client is configured to work with mainnet. You can easily change it by providing `network` argument. The `network` argument changes the default values in `pact.config` object. It contains things like API URL or global contract ids.\n\n```py\npact = pactsdk.PactClient(algod, network="testnet")\n```\n\nFetching pools by assets pair. It uses Pact API to retrieve the pool. Can return multiple pools with differing fee_bps.\n\n```py\nalgo = pact.fetch_asset(0)\nother_coin = pact.fetch_asset(8949213)\n\npools = pact.fetch_pools_by_assets(algo, other_coin) # The pool will be fetched regardless of assets order.\n```\n\nYou can fetch a pool by providing assets ids instead of Asset objects.\n\n```py\npools = pact.fetch_pools_by_assets(0, 8949213)\n```\n\nYou can also fetch a pool by providing app id. This way the pool is retrieved directly from the chain.\n\n```py\npool = pact.fetch_pool_by_id(456321)\n```\n\nBefore making the transactions you need to opt-in for the assets. There\'s no need to opt-in for algo.\n\n```py\nimport algosdk\n\nprivate_key = algosdk.mnemonic.to_private_key(\'<mnemonic>\')\naddress = algosdk.account.address_from_private_key(private_key)\n\ndef opt_in(asset):\n    is_opted_in = asset.is_opted_in(address)\n    if not is_opted_in:\n        opt_in_tx = asset.prepare_opt_in_tx(address)\n        signed_tx = opt_in_tx.sign(private_key)\n        algod.send_transaction(signed_tx)\n\nopt_in(pool.primary_asset)\nopt_in(pool.secondary_asset)\nopt_in(pool.liquidity_asset) # Needed if you want to manage the liquidity.\n```\n\nCheck the current pool state.\n\n```py\nprint(pool.state)\n# PoolState(\n#   total_liquidity=900000,\n#   total_primary=956659,\n#   total_secondary=849972,\n#   primary_asset_price=0.8884795940873393,\n#   secondary_asset_price=1.1255182523659604,\n# )\n```\n\nExplicit pool state update is necessary periodically and after each pool operation.\n\n```py\npool.update_state()\npool.state  # Now holds fresh values.\n```\n\nManaging the liquidity.\n\n```py\n# Add liquidity.\nliquidity_addition = pool.prepare_add_liquidity(\n  primary_asset_amount=100_000,\n  secondary_asset_amount=50_000,\n);\nadd_liq_tx_group = liquidity_addition.prepare_tx_group(address)\nsigned_add_liq_tx_group = add_liq_tx_group.sign(private_key)\nalgod.send_transactions(signed_add_liq_tx_group)\n\n# Remove liquidity.\nremove_liq_tx_group = pool.prepare_remove_liquidity_tx_group(\n  address=address,\n  amount=100_000,\n)\nsigned_remove_liq_tx_group = remove_liq_tx_group.sign(private_key)\nalgod.send_transactions(signed_remove_liq_tx_group)\n```\n\nMaking a swap.\n\n```py\nswap = pool.prepare_swap(\n  asset=algo,\n  amount=200_000,\n  slippage_pct=2,\n)\n\n# You can inspect swap effect before submitting the transaction.\nprint(swap.effect)\n# SwapEffect(\n#     amount_deposited=200000,\n#     amount_received=146529,\n#     minimum_amount_received=143598,\n#     fee=441,\n#     price=0.73485,\n#     primary_asset_price_after_swap=0.6081680080300244,\n#     secondary_asset_price_after_swap=1.6442824791774173,\n#     primary_asset_price_change_pct=-31.549580645715963,\n#     secondary_asset_price_change_pct=46.091142966447585,\n# )\n\n# Let\'s submit the swap.\nswap_tx_group = swap.prepare_tx_group(address)\nsigned_tx_group = swap_tx_group.sign_txn(private_key)\nalgod.send_transactions(signed_tx_group)\n```\n\n## Composability of transactions.\n\nThe SDK has two sets of methods for creating transactions:\n\n1. `prepare_..._tx_group` e.g. `pool.prepare_swap_tx_group`\n\n   Those methods are convenience methods which ask algod for suggested transaction parameters, build transactions and create a transaction group. You can\'t add you own transactions to the group using those methods.\n\n2. `build_..._txs` e.g. `pool.build_swap_txs`\n\n   Those methods return a list of transactions. You can extend that list with your own transactions and create a `TransactionGroup` manually from this list.\n\n# Development\n\n- `poetry install`\n\nDevelopment requires [Pact contracts V1](https://github.com/pactfi/algorand-testbed) to be checked out.\n\n- `git clone git@github.com:pactfi/algorand-testbed.git`\n- `cd algorand-testbed`\n- `poetry install`\n- `docker compose up -d`\n- `cd ..`\n\n## Building\n\n- `poetry build`\n\nYou can install the package locally with\n`pip install dist/pactsdk-<version>.whl`\n\nValidate the installation `python -c "import pactsdk; print(pactsdk.__version__)"`\n\n## Running tests\n\n- `poetry run pytest`\n',
     'author': 'Mateusz Tomczyk',
     'author_email': 'mateusz.tomczyk@ulam.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pactfi/pact-py-sdk',
```

### Comparing `pactsdk-0.6.0/PKG-INFO` & `pactsdk-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pactsdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python SDK for Pact smart contracts
 Home-page: https://github.com/pactfi/pact-py-sdk
 License: MIT
 Author: Mateusz Tomczyk
 Author-email: mateusz.tomczyk@ulam.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

