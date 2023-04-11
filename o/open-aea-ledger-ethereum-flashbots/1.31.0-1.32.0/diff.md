# Comparing `tmp/open-aea-ledger-ethereum-flashbots-1.31.0.tar.gz` & `tmp/open-aea-ledger-ethereum-flashbots-1.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.31.0.tar", last modified: Tue Mar 21 11:37:10 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.32.0.tar", last modified: Tue Apr 11 12:20:29 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-flashbots-1.31.0.tar` & `open-aea-ledger-ethereum-flashbots-1.32.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:37:10.875155 open-aea-ledger-ethereum-flashbots-1.31.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-03-21 11:37:10.875155 open-aea-ledger-ethereum-flashbots-1.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:37:10.871155 open-aea-ledger-ethereum-flashbots-1.31.0/aea_ledger_ethereum_flashbots/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/aea_ledger_ethereum_flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9181 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:37:10.875155 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-21 11:37:10.000000 open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-21 11:37:10.875155 open-aea-ledger-ethereum-flashbots-1.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:37:10.875155 open-aea-ledger-ethereum-flashbots-1.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8745 2023-03-21 11:36:24.000000 open-aea-ledger-ethereum-flashbots-1.31.0/tests/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9630 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9419 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/tests/test_ethereum.py
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/LICENSE` & `open-aea-ledger-ethereum-flashbots-1.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.32.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.31.0
+Version: 1.32.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/aea_ledger_ethereum_flashbots/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py` & `open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,22 +32,24 @@
 from hexbytes import HexBytes
 from web3.exceptions import TransactionNotFound
 
 from aea.common import JSONLike
 from aea.helpers.base import try_decorator
 
 
-_default_logger = logging.getLogger(__name__)
+_default_logger = logging.getLogger("aea.ledger_apis.ethereum_flashbots")
 
 _ETHEREUM_FLASHBOTS = "ethereum_flashbots"
 
 _TARGET_BLOCKS = "target_blocks"
 
 _DEFAULT_TARGET_BLOCKS = 25
 
+_RAISE_ON_FAILED_SIMULATION = "raise_on_failed_simulation"
+
 
 class EthereumFlashbotApi(EthereumApi):
     """Class to interact with the Ethereum Web3 APIs."""
 
     identifier = _ETHEREUM_FLASHBOTS
 
     def __init__(self, **kwargs: Any):
@@ -114,33 +116,36 @@
             _default_logger.warning(f"Simulation failed for bundle {bundle}: {e}")
         return False
 
     def send_bundle(
         self,
         bundle: List[Union[FlashbotsBundleTx, FlashbotsBundleRawTx]],
         target_blocks: List[int],
+        raise_on_failed_simulation: bool = False,
     ) -> Optional[List[str]]:
         """
         Send a bundle.
 
         1. Simulate the bundle.
         2. Send the bundle in a try catch block.
         3. Wait for the response. If successful, go to step 4.
          If current block number is less than the maximum target block number, go to step 1.
         4. Return the transaction digests if the transactions went through, or None if something went wrong.
 
         :param bundle: the signed transactions to bundle together and send.
         :param target_blocks: the target blocks for the transactions.
+        :param raise_on_failed_simulation: whether to raise an exception if the simulation fails.
         :return: the transaction digest if the transaction went through, None otherwise.
         """
         for target_block in target_blocks:
             if not self.simulate(bundle, target_block):
-                _default_logger.warning(
-                    f"Simulation failed for bundle {bundle} targeting block {target_block}."
-                )
+                msg = f"Simulation failed for bundle {bundle} targeting block {target_block}."
+                if raise_on_failed_simulation:
+                    raise ValueError(msg)
+                _default_logger.warning(msg)
                 continue
 
             replacement_uuid = str(uuid4())
             _default_logger.debug(
                 f"Sending bundle {bundle} with replacement_uuid {replacement_uuid} targeting block {target_block}"
             )
             response = self.flashbots.send_bundle(
@@ -149,31 +154,31 @@
             _default_logger.debug(
                 f"Response from bundle with replacement uuid {replacement_uuid}: {response}"
             )
             response.wait()
             try:
                 receipts = response.receipts()
                 tx_hashes = [tx["hash"].hex() for tx in response.bundle]
-                logging.debug(
+                _default_logger.debug(
                     f"Bundle with replacement uuid {replacement_uuid} was mined in block {receipts[0]['blockNumber']}"
                     f"Tx hashes: {tx_hashes}"
                 )
                 return tx_hashes
             except TransactionNotFound:
                 # get & log the bundle stats in case it was not included in the block
                 stats = self.flashbots.get_bundle_stats_v2(
                     self.api.toHex(response.bundle_hash()), target_block
                 )
-                logging.debug(
+                _default_logger.info(
                     f"Bundle with replacement uuid {replacement_uuid} not found in block {target_block}. "
                     f"bundle stats: {stats}"
                 )
                 # essentially a no-op but it shows that the function works
                 cancel_res = self.flashbots.cancel_bundles(replacement_uuid)
-                logging.debug(
+                _default_logger.debug(
                     f"Response from canceling bundle with replacement uuid {replacement_uuid}: {cancel_res}"
                 )
         return None
 
     def _get_next_blocks(self, num_blocks: int = _DEFAULT_TARGET_BLOCKS) -> List[int]:
         """
         Get the next blocks.
@@ -195,15 +200,16 @@
         :param _kwargs: the keyword arguments. Possible kwargs are:
             `raise_on_try`: bool flag specifying whether the method will raise or log on error (used by `try_decorator`)
             `target_blocks`: the target blocks for the transactions.
         :return: the transaction digest if the transactions went through, None otherwise.
         """
         bundle = self.bundle_transactions(signed_transactions)
         target_blocks = _kwargs.get(_TARGET_BLOCKS, self._get_next_blocks())
-        tx_hashes = self.send_bundle(bundle, target_blocks)
+        raise_on_failed_simulation = _kwargs.get(_RAISE_ON_FAILED_SIMULATION, False)
+        tx_hashes = self.send_bundle(bundle, target_blocks, raise_on_failed_simulation)
         return tx_hashes
 
     def send_signed_transactions(
         self,
         signed_transactions: List[JSONLike],
         raise_on_try: bool = False,
         **kwargs: Any,
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.31.0
+Version: 1.32.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/setup.py` & `open-aea-ledger-ethereum-flashbots-1.32.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_flashbots" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-flashbots",
-    version="1.31.0",
+    version="1.32.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.",
     long_description=(
         "Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."
     ),
     long_description_content_type="text/markdown",
@@ -37,15 +37,15 @@
     package_data={
         "aea_ledger_ethereum_flashbots": [
             "py.typed",
         ]
     },
     python_requires=">=3.9,<4.0",
     install_requires=[
-        "open-aea-ledger-ethereum~=1.31.0",
+        "open-aea-ledger-ethereum~=1.32.0",
         "flashbots==1.1.1",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": [
             "ethereum_flashbots = aea_ledger_ethereum_flashbots:EthereumFlashbotCrypto"
         ],
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/tests/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.32.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.31.0/tests/test_ethereum.py` & `open-aea-ledger-ethereum-flashbots-1.32.0/tests/test_ethereum.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,13 +216,32 @@
     """Test send bundle with failed simulation."""
     # mock
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.bundle_hash = MagicMock()
     response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
     ethereum_flashbot_api.simulate = MagicMock(return_value=False)
+    target_blocks = [0]
 
     # run
-    tx_hashes = ethereum_flashbot_api.send_bundle(MagicMock(), MagicMock())
+    tx_hashes = ethereum_flashbot_api.send_bundle(MagicMock(), target_blocks)
 
     # check
     assert tx_hashes is None
+
+
+def test_send_bundle_with_failed_simulation_and_raise(ethereum_flashbot_api) -> None:
+    """Test send bundle with failed simulation and should raise."""
+    # mock
+    response_mock = MagicMock()
+    response_mock.wait = MagicMock()
+    response_mock.bundle_hash = MagicMock()
+    response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
+    ethereum_flashbot_api.simulate = MagicMock(return_value=False)
+    raise_on_failed_simulation = True
+    target_blocks = [0]
+
+    # run
+    with pytest.raises(ValueError):
+        ethereum_flashbot_api.send_bundle(
+            MagicMock(), target_blocks, raise_on_failed_simulation
+        )
```

