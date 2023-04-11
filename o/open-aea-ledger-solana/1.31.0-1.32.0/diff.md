# Comparing `tmp/open-aea-ledger-solana-1.31.0.tar.gz` & `tmp/open-aea-ledger-solana-1.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-solana-1.31.0.tar", last modified: Wed Mar 22 07:08:42 2023, max compression
+gzip compressed data, was "open-aea-ledger-solana-1.32.0.tar", last modified: Tue Apr 11 12:20:30 2023, max compression
```

## Comparing `open-aea-ledger-solana-1.31.0.tar` & `open-aea-ledger-solana-1.32.0.tar`

### file list

```diff
@@ -1,44 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.893292 open-aea-ledger-solana-1.31.0/aea_ledger_solana/
--rw-r--r--   0 runner    (1001) docker     (122)      986 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/aea_ledger_solana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39964 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/aea_ledger_solana/solana.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.897292 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-22 07:08:42.000000 open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.897292 open-aea-ledger-solana-1.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.897292 open-aea-ledger-solana-1.31.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.889292 open-aea-ledger-solana-1.31.0/tests/data/dummy_contract/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.897292 open-aea-ledger-solana-1.31.0/tests/data/dummy_contract/build/
--rw-r--r--   0 runner    (1001) docker     (122)    84952 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/dummy_contract/build/idl.json
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/solana_private_key0.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/solana_private_key1.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/solana_private_key2.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/solana_private_key_program.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.889292 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.889292 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.897292 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/deploy/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet-keypair.json
--rwxr-xr-x   0 runner    (1001) docker     (122)   175592 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/idl/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.893292 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.893292 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/deploy/
--rwxr-xr-x   0 runner    (1001) docker     (122)   208064 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-22 07:08:42.901291 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/idl/
--rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json
--rw-r--r--   0 runner    (1001) docker     (122)    19518 2023-03-22 07:07:58.000000 open-aea-ledger-solana-1.31.0/tests/test_solana.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/aea_ledger_solana/
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7016 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/faucet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10538 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23938 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/solana_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/transaction_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/aea_ledger_solana/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-11 12:20:30.000000 open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/tests/data/dummy_contract/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/dummy_contract/build/
+-rw-r--r--   0 runner    (1001) docker     (122)    84952 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/dummy_contract/build/idl.json
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/solana_private_key0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/solana_private_key1.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/solana_private_key2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/solana_private_key_program.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/deploy/
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet-keypair.json
+-rwxr-xr-x   0 runner    (1001) docker     (122)   175592 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/idl/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.072806 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/deploy/
+-rwxr-xr-x   0 runner    (1001) docker     (122)   208064 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:30.076806 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/idl/
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20438 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_solana_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-04-11 12:19:43.000000 open-aea-ledger-solana-1.32.0/tests/test_underlying_lib.py
```

### Comparing `open-aea-ledger-solana-1.31.0/LICENSE` & `open-aea-ledger-solana-1.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/PKG-INFO` & `open-aea-ledger-solana-1.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-solana
-Version: 1.31.0
+Version: 1.32.0
 Summary: Python package wrapping the public and private key cryptography and ledger api of solana.
 Author: dassy23
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-solana-1.31.0/aea_ledger_solana/__init__.py` & `open-aea-ledger-solana-1.32.0/aea_ledger_solana/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,12 +12,19 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
+"""Constants for the solana ledger."""
+_VERSION = "1.24.17"
+_SOLANA = "solana"
+TESTNET_NAME = "n/a"
+DEFAULT_ADDRESS = "https://api.devnet.solana.com"
+DEFAULT_CHAIN_ID = 101
+DEFAULT_CURRENCY_DENOM = "lamports"
+RENT_EXEMPT_AMOUNT = 1000000
 
-"""Python package wrapping the public and private key cryptography and ledger api of Solana."""
-
-from .solana import *  # noqa isort:skip
-from .solana import _IDL, _BYTECODE, _SOLANA  # noqa isort:skip
+LAMPORTS_PER_SOL = 1000000000
+_IDL = "idl"
+_BYTECODE = "bytecode"
```

### Comparing `open-aea-ledger-solana-1.31.0/aea_ledger_solana/solana.py` & `open-aea-ledger-solana-1.32.0/aea_ledger_solana/solana.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,564 +13,139 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 """Solana module wrapping the public and private key cryptography and ledger api."""
-import base64
-import hashlib
 import json
 import logging
 import time
-import zlib
-from pathlib import Path
-from typing import Any, Dict, List, NewType, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple
 
-import base58
+from aea_ledger_solana.constants import (
+    DEFAULT_ADDRESS,
+    DEFAULT_CHAIN_ID,
+    _SOLANA,
+    _VERSION,
+)
+from aea_ledger_solana.crypto import SolanaCrypto
+from aea_ledger_solana.faucet import SolanaFaucetApi  # noqa: F401
+from aea_ledger_solana.helper import SolanaHelper
+from aea_ledger_solana.solana_api import SolanaApiClient
+from aea_ledger_solana.transaction import SolanaTransaction
+from aea_ledger_solana.transaction_instruction import TransactionInstruction
 from anchorpy import Context, Idl, Program  # type: ignore
-from anchorpy.coder.accounts import ACCOUNT_DISCRIMINATOR_SIZE  # type: ignore
-from anchorpy.idl import _decode_idl_account  # type: ignore
-from cryptography.fernet import Fernet  # type: ignore
-from solana.blockhash import BlockhashCache  # type: ignore
-from solana.keypair import Keypair  # type: ignore
-from solana.publickey import PublicKey  # type: ignore
-from solana.rpc.api import Client  # type: ignore
-from solana.system_program import (  # type: ignore
+from solana.blockhash import BlockhashCache
+from solana.transaction import Transaction  # type: ignore
+from solders import system_program as ssp  # type: ignore
+from solders.instruction import Instruction
+from solders.pubkey import Pubkey as PublicKey  # type: ignore
+from solders.signature import Signature  # type: ignore
+from solders.system_program import (  # type: ignore; SYS_PROGRAM_ID,
     CreateAccountParams,
     CreateAccountWithSeedParams,
-    SYS_PROGRAM_ID,
+)
+from solders.system_program import ID as SYS_PROGRAM_ID  # type: ignore
+from solders.system_program import (  # type: ignore; SYS_PROGRAM_ID,
     TransferParams,
     create_account,
     transfer,
 )
-from solana.transaction import Transaction, TransactionInstruction  # type: ignore
-from solders import system_program as ssp  # type: ignore
-from solders.signature import Signature  # type: ignore
-from solders.transaction import Transaction as sTransaction  # type: ignore
 
 from aea.common import Address, JSONLike
-from aea.crypto.base import Crypto, FaucetApi, Helper, LedgerApi
-from aea.crypto.helpers import DecryptError, KeyIsIncorrect
+from aea.crypto.base import LedgerApi
 from aea.helpers.base import try_decorator
-from aea.helpers.io import open_file
-
-
-_default_logger = logging.getLogger(__name__)
-
-_VERSION = "1.24.17"
-_SOLANA = "solana"
-TESTNET_NAME = "n/a"
-DEFAULT_ADDRESS = "https://api.devnet.solana.com"
-DEFAULT_CHAIN_ID = 101
-DEFAULT_CURRENCY_DENOM = "lamports"
-RENT_EXEMPT_AMOUNT = 1000000
-
-LAMPORTS_PER_SOL = 1000000000
-_IDL = "idl"
-_BYTECODE = "bytecode"
-
-
-def _pako_inflate(data):
-    # https://stackoverflow.com/questions/46351275/using-pako-deflate-with-python
-    decompress = zlib.decompressobj(15)
-    decompressed_data = decompress.decompress(data)
-    decompressed_data += decompress.flush()
-    return decompressed_data
-
-
-class SolanaCrypto(Crypto[Keypair]):
-    """Class wrapping the Account Generation from Solana ledger."""
-
-    identifier = _SOLANA
-
-    def __init__(
-        self,
-        private_key_path: Optional[str] = None,
-        password: Optional[str] = None,
-        extra_entropy: Union[str, bytes, int] = "",
-    ) -> None:
-        """
-        Instantiate an solana crypto object.
-
-        :param private_key_path: the private key path of the agent
-        :param password: the password to encrypt/decrypt the private key.
-        :param extra_entropy: add extra randomness to whatever randomness your OS can provide
-        """
-        super().__init__(
-            private_key_path=private_key_path,
-            password=password,
-            extra_entropy=extra_entropy,
-        )
-
-    @property
-    def private_key(self) -> str:
-        """
-        Return a private key.
-
-        64 random hex characters (i.e. 32 bytes) prefix.
-
-        :return: a private key string in hex format
-        """
-
-        return base58.b58encode(self.entity.secret_key).decode()
-
-    @property
-    def public_key(self) -> str:
-        """
-        Return a public key in hex format.
-
-        :return: a public key string in hex format
-        """
-        return self.entity.public_key
-
-    @property
-    def address(self) -> str:
-        """
-        Return the address for the key pair.
-
-        :return: an address string in hex format
-        """
-        return self.entity.public_key.to_base58().decode()
-
-    @classmethod
-    def load_private_key_from_path(
-        cls, file_name: str, password: Optional[str] = None
-    ) -> Keypair:
-        """
-        Load a private key in base58 or bytes format from a file.
-
-        :param file_name: the path to the hex file.
-        :param password: the password to encrypt/decrypt the private key.
-        :return: the Entity.
-        """
-        key_path = Path(file_name)
-        private_key = cls.load(file_name, password)
-        try:
-            key = Keypair.from_secret_key(base58.b58decode(private_key))
-        except Exception as e:
-
-            raise KeyIsIncorrect(
-                f"Error on key `{key_path}` load! : Error: {repr(e)}.{'try password?' if password is None else ''}"
-            ) from e
-
-        return key
-
-    def sign_message(self, message: bytes, is_deprecated_mode: bool = False) -> str:
-        """
-        Sign a message in bytes string form.
-
-        :param message: the message to be signed
-        :param is_deprecated_mode: if the deprecated signing is used
-        :return: signature of the message in string form
-        """
-        if is_deprecated_mode:
-            raise ValueError("is_deprecated_mode is not supported at the moment")
-        keypair = Keypair.from_secret_key(base58.b58decode(self.private_key))
-        signed_msg = keypair.sign(message)
-
-        return signed_msg
-
-    def sign_transaction(
-        self, transaction: JSONLike, signers: Optional[list] = None
-    ) -> JSONLike:
-        """
-        Sign a transaction in bytes string form.
-
-        :param transaction: the transaction to be signed
-        :param signers: list of signers
-        :return: signed transaction
-        """
-        signers = signers or []
-        jsonTx = json.dumps(transaction)
-        stxn = sTransaction.from_json(jsonTx)
-        txn = Transaction.from_solders(stxn)
-
-        keypair = Keypair.from_secret_key(base58.b58decode(self.private_key))
-        signers = [
-            Keypair.from_secret_key(base58.b58decode(signer.private_key))
-            for signer in signers
-        ]
-        signers.append(keypair)
-
-        try:
-            txn.sign(*signers)
-        except Exception as e:
-            raise Exception(e)
-
-        tx = txn._solders.to_json()  # pylint: disable=protected-access
-        return json.loads(tx)
-
-    @classmethod
-    def generate_private_key(
-        cls, extra_entropy: Union[str, bytes, int] = ""
-    ) -> Keypair:
-        """
-        Generate a key pair for Solana network.
-
-        :param extra_entropy: add extra randomness to whatever randomness your OS can provide
-        :return: keypair object
-        """
-        if extra_entropy:
-            raise ValueError("extra_entropy is not supported at the moment")
-        account = Keypair.generate()  # pylint: disable=no-value-for-parameter
-        return account
-
-    def encrypt(self, password: str) -> str:
-        """
-        Encrypt the private key and return in json.
-
-        :param password: the password to decrypt.
-        :return: json string containing encrypted private key.
-        """
-        try:
-            pw = str.encode(password)
-            hash_object = hashlib.sha256(pw)
-            hex_dig = hash_object.digest()
-            base64_bytes = base64.b64encode(hex_dig)
-            fernet = Fernet(base64_bytes)
-            enc_mac = fernet.encrypt(self.private_key.encode())
-        except Exception as e:
-            raise Exception("Encryption failed") from e
-
-        return json.dumps(enc_mac.decode())
-
-    @classmethod
-    def decrypt(cls, keyfile_json: str, password: str) -> str:
-        """
-        Decrypt the private key and return in raw form.
-
-        :param keyfile_json: json str containing encrypted private key.
-        :param password: the password to decrypt.
-        :return: the raw private key.
-        """
-        try:
-            keyfile = json.loads(keyfile_json)
-            keyfile_bytes = keyfile.encode()
-            pw = str.encode(password)
-            hash_object = hashlib.sha256(pw)
-            hex_dig = hash_object.digest()
-            base64_bytes = base64.b64encode(hex_dig)
-            fernet = Fernet(base64_bytes)
-
-            dec_mac = fernet.decrypt(keyfile_bytes).decode()
-        except ValueError as e:
-            raise DecryptError() from e
-        return dec_mac
-
-
-class SolanaHelper(Helper):
-    """Helper class usable as Mixin for SolanaApi or as standalone class."""
-
-    BlockhashCache: BlockhashCache  # defined in SolanaAPi.__init__
-    _api: Client  # defined in SolanaAPi.__init__
-
-    @classmethod
-    def load_contract_interface(
-        cls,
-        idl_file_path: Optional[Path] = None,
-        program_keypair: Optional[Crypto] = None,
-        program_address: Optional[str] = None,
-        rpc_api: Optional[str] = None,
-        bytecode_path: Optional[Path] = None,
-    ) -> Dict[str, Any]:  # type: ignore
-        """
-        Load contract interface.
-
-        :param idl_file_path: the file path to the IDL
-        :param program_keypair: the program keypair
-        :param program_address: the program address
-        :param rpc_api: the rpc api
-        :param bytecode_path: the file path to the bytecode
-
-        :return: the interface
-        """
-        if bytecode_path is not None:
-            in_file = open(bytecode_path, "rb")
-            bytecode = in_file.read()
-        else:
-            bytecode = None
-
-        if (
-            program_keypair is not None or program_address is not None
-        ) and rpc_api is not None:
-            try:
-                pid = program_address or program_keypair.address  # type: ignore # mypy doesnt recognize `if` condition above
-
-                base = PublicKey.find_program_address([], PublicKey(pid))[0]
-                idl_address = PublicKey.create_with_seed(
-                    base, "anchor:idl", PublicKey(pid)
-                )
-                client = Client(endpoint=rpc_api)
-                account_info = client.get_account_info(idl_address)
-
-                account_info_val = account_info.value
-                idl_account = _decode_idl_account(
-                    bytes(account_info_val.data)[ACCOUNT_DISCRIMINATOR_SIZE:]
-                )
-                inflated_idl = _pako_inflate(bytes(idl_account["data"])).decode()
-                json_idl = json.loads(inflated_idl)
-                return {
-                    "idl": json_idl,
-                    "bytecode": bytecode,
-                    "program_address": program_address,
-                    "program_keypair": program_keypair,
-                }
-            except Exception as e:
-                raise Exception("Could not locate IDL") from e
-
-        elif idl_file_path is not None:
-            with open_file(idl_file_path, "r") as interface_file_solana:
-                json_idl = json.load(interface_file_solana)
-
-            return {
-                "idl": json_idl,
-                "bytecode": bytecode,
-                "program_address": program_address,
-                "program_keypair": program_keypair,
-            }
-        else:
-            raise Exception("Could not locate IDL")
-
-    @staticmethod
-    def is_transaction_valid(
-        tx: JSONLike,
-        seller: Address,
-        client: Address,
-        tx_nonce: str,
-        amount: int,
-    ) -> bool:
-        """
-        Check whether a transaction is valid or not.
-
-        :param tx: the transaction.
-        :param seller: the address of the seller.
-        :param client: the address of the client.
-        :param tx_nonce: the transaction nonce.
-        :param amount: the amount we expect to get from the transaction.
-
-        # noqa: DAR202
-
-        :return: True if the random_message is equals to tx['input']
-        """
-        raise NotImplementedError
-
-    @staticmethod
-    def is_transaction_settled(tx_receipt: JSONLike) -> bool:
-        """
-        Check whether a transaction is settled or not.
-
-        :param tx_receipt: the receipt associated to the transaction.
-        :return: True if the transaction has been settled, False o/w.
-        """
-        is_successful = False
-        if tx_receipt is not None:
-            is_successful = tx_receipt["meta"]["status"] == {"Ok": None}  # type: ignore
-        return is_successful
-
-    @staticmethod
-    def get_hash(message: bytes) -> str:
-        """
-        Get the hash of a message.
-
-        :param message: the message to be hashed.
-        :return: the hash of the message as a hex string.
-        """
-        sha = hashlib.sha256()
-        sha.update(message)
-        return sha.hexdigest()
-
-    @classmethod
-    def recover_message(
-        cls, message: bytes, signature: str, is_deprecated_mode: bool = False
-    ) -> Tuple[Address, ...]:
-        """
-        Recover the addresses from the hash.
-
-        **TOBEIMPLEMENTED**
-
-        :param message: the message we expect
-        :param signature: the transaction signature
-        :param is_deprecated_mode: if the deprecated signing was used
-
-        # noqa: DAR202
-
-        :return: the recovered addresses
-        """
-        raise NotImplementedError
-
-    @classmethod
-    def recover_public_keys_from_message(
-        cls, message: bytes, signature: str, is_deprecated_mode: bool = False
-    ) -> Tuple[str, ...]:
-        """
-        Get the public key used to produce the `signature` of the `message`
-
-        **TOBEIMPLEMENTED**
-
-        :param message: raw bytes used to produce signature
-        :param signature: signature of the message
-        :param is_deprecated_mode: if the deprecated signing was used
-
-        # noqa: DAR202
-
-        :return: the recovered public keys
-        """
-
-        raise NotImplementedError
-
-    @try_decorator("Unable to get nonce: {}", logger_method="warning")
-    def _generate_tx_nonce(self) -> str:
-        """
-        Fetch a latest blockhash to distinguish transactions with the same terms.
-
-        :return: return the blockhash as a nonce.
-        """
-
-        try:
-            blockhash = self.BlockhashCache.get()
-            return blockhash
-        except Exception:  # pylint: disable=broad-except
-            result = self._api.get_latest_blockhash()
-            blockhash_json = result.value.to_json()
-            blockhash = json.loads(blockhash_json)
-            self.BlockhashCache.set(
-                blockhash=blockhash["blockhash"], slot=result.context.slot
-            )
-            return blockhash["blockhash"]
-
-    @staticmethod
-    def generate_tx_nonce(seller: Address, client: Address) -> str:
-        """
-        Generate a unique hash to distinguish transactions with the same terms.
-
-        :param seller: the address of the seller.
-        :param client: the address of the client.
-        :return: return the hash in hex.
-        """
-        time_stamp = int(time.time())
-        aggregate_hash = hashlib.sha256(
-            b"".join([seller.encode(), client.encode(), time_stamp.to_bytes(32, "big")])
-        )
-        return aggregate_hash.hexdigest()
-
-    def add_nonce(self, tx: dict) -> JSONLike:
-        """
-        Check whether a transaction is valid or not.
-
-        :param tx: the transaction.
-        :return: True if the random_message is equals to tx['input']
-        """
-        jsonTx = json.dumps(tx)
-        stxn = sTransaction.from_json(jsonTx)
-        txObj = Transaction.from_solders(stxn)
-        # blockash in string format
-        nonce = self._generate_tx_nonce()
-        txObj.recent_blockhash = nonce
-        return json.loads(txObj._solders.to_json())  # pylint: disable=protected-access
-
-    @staticmethod
-    def to_transaction_format(tx: dict) -> Any:
-        """
-        Check whether a transaction is valid or not.
-
-        :param tx: the transaction.
-        :return: True if the random_message is equals to tx['input']
-        """
-        jsonTx = json.dumps(tx)
-        stxn = sTransaction.from_json(jsonTx)
-        return Transaction.from_solders(stxn)
-
-    @staticmethod
-    def to_dict_format(tx) -> JSONLike:
-        """
-        Check whether a transaction is valid or not.
-
-        :param tx: the transaction.
-        :return: True if the random_message is equals to tx['input']
-        """
-
-        return json.loads(tx._solders.to_json())  # pylint: disable=protected-access
-
-    @staticmethod
-    def get_contract_address(tx_receipt: JSONLike) -> Optional[str]:
-        """
-        Retrieve the `contract_addresses` from a transaction receipt.
-
-        **Solana can have many contract addresses in one tx**
-
-        :param tx_receipt: the receipt of the transaction.
-        :return: the contract address, if present
-        """
-        contract_addresses = []
-        keys = tx_receipt["transaction"]["message"]["accountKeys"]  # type: ignore
-        for ix in tx_receipt["transaction"]["message"]["instructions"]:  # type: ignore
-            program_index = ix["programIdIndex"]  # type: ignore
-            contract_addresses.append(cast(str, keys[program_index]))  # type: ignore
-        return contract_addresses[0] if contract_addresses else None
-
-    @classmethod
-    def get_address_from_public_key(cls, public_key: PublicKey) -> str:
-        """
-        Get the address from the public key.
-
-        :param public_key: the public key
-        :return: str
-        """
-
-        return public_key.to_base58().decode()
-
-    @classmethod
-    def is_valid_address(cls, address: str) -> bool:
-        """
-        Check if the address is valid.
-
-        :param address: the address to validate
-        :return: whether the address is valid
-        """
-        try:
-            PublicKey(address)
-            return True
-        except Exception:  # pylint: disable=broad-except
-            return False
 
 
 class SolanaApi(LedgerApi, SolanaHelper):
     """Class to interact with the Solana Web3 APIs."""
 
     identifier = _SOLANA
 
     def __init__(self, **kwargs: Any):
         """
         Initialize the Solana ledger APIs.
 
         :param kwargs: keyword arguments
         """
 
-        Commitment = NewType("Commitment", str)
         """Type for commitment."""
 
-        Confirmed = Commitment("confirmed")
-
-        self._api = Client(
-            endpoint=kwargs.pop("address", DEFAULT_ADDRESS), commitment=Confirmed
+        self._api = SolanaApiClient(
+            endpoint=kwargs.pop("address", DEFAULT_ADDRESS),
         )
 
+        self._chain_id = kwargs.pop("chain_id", DEFAULT_CHAIN_ID)
+        self._version = _VERSION
         self.BlockhashCache = BlockhashCache(ttl=10)
+        self._get_latest_hash()
+
+    def _get_latest_hash(self):
+        """Get the latest block hash."""
         result = self._api.get_latest_blockhash()
         blockhash_json = result.value.to_json()
         blockhash = json.loads(blockhash_json)
-        hash_ = blockhash["blockhash"]
-        self.BlockhashCache.set(blockhash=hash_, slot=result.context.slot)
+        self._hash = blockhash["blockhash"]
+        self.BlockhashCache.set(blockhash=self._hash, slot=result.context.slot)
 
-        self._chain_id = kwargs.pop("chain_id", DEFAULT_CHAIN_ID)
-        self._version = _VERSION
+    @property
+    def latest_hash(self):
+        """Get the latest hash."""
+        self._get_latest_hash()
+        return self._hash
+
+    def wait_get_receipt(
+        self, transaction_digest: str
+    ) -> Tuple[Optional[JSONLike], bool]:
+        """Wait for the transaction to be settled and return the receipt."""
+        transaction_receipt = None
+        not_settled = True
+        elapsed_time = 0
+        time_to_wait = 40
+        sleep_time = 0.25
+        while not_settled and elapsed_time < time_to_wait:
+            elapsed_time += sleep_time
+            time.sleep(sleep_time)
+            transaction_receipt = self.get_transaction_receipt(transaction_digest)
+            if transaction_receipt is None:
+                continue
+            is_settled = self.is_transaction_settled(transaction_receipt)
+            not_settled = not is_settled
+
+        return transaction_receipt, not not_settled
+
+    def construct_and_settle_tx(
+        self,
+        account1: SolanaCrypto,
+        account2: SolanaCrypto,
+        tx_params: dict,
+    ) -> Tuple[str, JSONLike, bool]:
+        """Construct and settle a transaction."""
+        transfer_transaction = self.get_transfer_transaction(
+            **tx_params, tx_fee=0, tx_nonce=""
+        )
+        # add nonce
+        transfer_transaction = self.add_nonce(transfer_transaction)
+
+        signed_transaction = account1.sign_transaction(transfer_transaction)
+
+        transaction_digest = self.send_signed_transaction(signed_transaction)
+        if transaction_digest is None:
+            raise Exception("Failed to submit transfer transaction!")
+
+        transaction_receipt, is_settled = self.wait_get_receipt(transaction_digest)
+
+        if transaction_receipt is None:
+            raise Exception("Failed to settle transfer transaction!")
+
+        return transaction_digest, transaction_receipt, is_settled
 
     @property
-    def api(self) -> Client:
+    def api(self) -> SolanaApiClient:
         """Get the underlying API object."""
         return self._api
 
     def update_with_gas_estimate(self, transaction: JSONLike) -> JSONLike:
         """
         Attempts to update the transaction with a gas estimate
 
@@ -588,15 +163,15 @@
         """Get the balance of a given account."""
         return self._try_get_balance(address, raise_on_try=raise_on_try)
 
     @try_decorator("Unable to retrieve balance: {}", logger_method="warning")
     def _try_get_balance(self, address: Address, **_kwargs: Any) -> Optional[int]:
         """Get the balance of a given account."""
         response = self._api.get_balance(
-            PublicKey(address), commitment="processed"
+            PublicKey.from_string(address), commitment="processed"
         )  # pylint: disable=no-member
         return response.value
 
     def get_state(
         self, callable_name: str, *args: Any, raise_on_try: bool = False, **kwargs: Any
     ) -> Optional[JSONLike]:
         """
@@ -622,17 +197,15 @@
 
         if "raise_on_try" in kwargs:
             logging.info(
                 f"popping `raise_on_try` from {self.__class__.__name__}.get_state kwargs"  # pylint: disable=protected-access
             )
             kwargs.pop("raise_on_try")
 
-        account_object = self._api.get_account_info_json_parsed(PublicKey(address))
-        account_info_val = account_object.value
-        return account_info_val
+        return self._api.get_account_state(address)
 
     def get_transfer_transaction(  # pylint: disable=arguments-differ
         self,
         sender_address: Address,
         destination_address: Address,
         amount: int,
         tx_fee: int,
@@ -650,64 +223,54 @@
         :param kwargs: the keyword arguments.
         :return: the transfer transaction
         """
         chain_id = kwargs.get("kwargs", None)
         chain_id = chain_id if chain_id is not None else self._chain_id
 
         state = self.get_state(destination_address)
+        # this is if there is no account yet at the destination address
+
         if state is None:
-            seed = "seed"
-            acc = PublicKey.create_with_seed(
-                PublicKey(sender_address),
-                seed,
-                PublicKey("11111111111111111111111111111111"),
-            )
-            params = CreateAccountWithSeedParams(
-                PublicKey(sender_address),
-                acc,
-                PublicKey(sender_address),
-                seed,
-                amount,
-                0,
-                PublicKey("11111111111111111111111111111111"),
-            )
-            ix_create_pda = TransactionInstruction.from_solders(
-                ssp.create_account_with_seed(params.to_solders())
-            )
+            # we need to create the account we first get the tx
+            # to create the account
+            # then we get the tx to transfer the funds
+            # then we combine the two txs
+            # then we sign the combined tx
+            # then we return the combined tx
 
-            params = ssp.TransferWithSeedParams(
-                from_pubkey=acc.to_solders(),
-                from_base=PublicKey(sender_address).to_solders(),
-                from_seed=seed,
-                from_owner=PublicKey("11111111111111111111111111111111").to_solders(),
-                to_pubkey=PublicKey(destination_address).to_solders(),
-                lamports=amount,
+            create_account_ixn = self._api.get_create_account_instructions(
+                sender_address, destination_address
             )
-            ix_transfer = TransactionInstruction.from_solders(
-                ssp.transfer_with_seed(params)
+
+            transfer_ixn = self._api.get_transfer_tx(
+                sender_address, destination_address, amount
             )
 
-            txn = (
-                Transaction(fee_payer=PublicKey(sender_address))
-                .add(ix_create_pda)
-                .add(ix_transfer)
+            txn = Transaction(
+                fee_payer=PublicKey.from_string(sender_address),
             )
+
+            ixn_1 = Instruction.from_json(json.dumps(create_account_ixn))
+            ixn_2 = Instruction.from_json(transfer_ixn.to_json())
+
+            # in solana we first create the account then we transfer the funds
+            txn.add(ixn_1).add(ixn_2)
+
         else:
-            txn = Transaction(fee_payer=sender_address).add(
+            txn = Transaction(fee_payer=PublicKey.from_string(sender_address)).add(
                 transfer(
                     TransferParams(
-                        from_pubkey=PublicKey(sender_address),
-                        to_pubkey=PublicKey(destination_address),
+                        from_pubkey=PublicKey.from_string(sender_address),
+                        to_pubkey=PublicKey.from_string(destination_address),
                         lamports=amount,
                     )
                 )
             )
 
-        tx = txn._solders.to_json()  # pylint: disable=protected-access
-
+        tx = txn.to_solders().to_json()  # pylint: disable=protected-access
         return json.loads(tx)
 
     def send_signed_transaction(
         self, tx_signed: JSONLike, raise_on_try: bool = False
     ) -> Optional[str]:
         """
         Send a signed transaction and wait for confirmation.
@@ -729,19 +292,25 @@
 
         :param tx_signed: the signed transaction
         :param _kwargs: the keyword arguments. Possible kwargs are:
             `raise_on_try`: bool flag specifying whether the method will raise or log on error (used by `try_decorator`)
         :return: tx_digest, if present
         """
 
-        jsonTx = json.dumps(tx_signed)
-        stxn = sTransaction.from_json(jsonTx)
-        txn = Transaction.from_solders(stxn)
-
-        txn_resp = self._api.send_raw_transaction(txn.serialize())
+        stxn = SolanaTransaction.from_json(tx_signed)
+        txn_resp = self._api.send_raw_transaction(bytes(stxn.serialize()))
+        retries = 2
+        while True and retries > 0:
+            try:
+                tx_digest = str(txn_resp.value)
+                self.get_transaction_receipt(tx_digest)
+                break
+            except ValueError:
+                time.sleep(1)
+            retries -= 1
 
         return txn_resp.to_json()
 
     def send_signed_transactions(
         self,
         signed_transactions: List[JSONLike],
         raise_on_try: bool = False,
@@ -902,15 +471,15 @@
         Get the instance of a contract.
 
         :param contract_interface: the contract interface.
         :param contract_address: the contract address.
         :return: the contract instance
         """
         bytecode_path = None  # bytecode is not provided for the moment
-        program_id = PublicKey(contract_address)
+        program_id = PublicKey.from_string(contract_address)
         idl = Idl.from_json(json.dumps(contract_interface["idl"]))
         pg = Program(idl, program_id)
 
         pg.provider.connection = self.api
 
         if bytecode_path is not None:
             # opening for [r]eading as [b]inary
@@ -1031,16 +600,15 @@
         data = method_args["data"]
         accounts = method_args["accounts"]
         remaining_accounts = method_args["remaining_accounts"]
 
         txn = contract_instance.transaction[method_name](
             *data, ctx=Context(accounts=accounts, remaining_accounts=remaining_accounts)
         )
-        tx = txn._solders.to_json()  # pylint: disable=protected-access
-        return json.loads(tx)
+        return json.loads(txn.to_solders().to_json())
 
     def get_transaction_transfer_logs(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         contract_instance: Any,
         tx_hash: str,
         target_address: Optional[str] = None,
     ) -> Optional[JSONLike]:
@@ -1086,69 +654,7 @@
                 "postBalances": [
                     {"address": keys[idx], "balance": balance}
                     for idx, balance in enumerate(tx_receipt["meta"]["postBalances"])  # type: ignore
                 ],
             }
 
         return transfers  # type: ignore  # actually ok
-
-
-class SolanaFaucetApi(FaucetApi):
-    """Solana testnet faucet API."""
-
-    identifier = _SOLANA
-    testnet_name = TESTNET_NAME
-    DEFAULT_AMOUNT = 1000000000
-
-    def get_wealth(self, address: Address, url: Optional[str] = None) -> None:
-        """
-        Get wealth from the faucet for the provided address.
-
-        :param address: the address.
-        :param url: the url
-
-        """
-        amount = self.DEFAULT_AMOUNT
-        self._try_get_wealth(address, amount, url)
-
-    @staticmethod
-    @try_decorator(
-        "An error occured while attempting to generate wealth:\n{}",
-        logger_method="error",
-    )
-    def _try_get_wealth(
-        address: Address, amount: Optional[int] = None, url: Optional[str] = None
-    ) -> Optional[str]:
-        """
-        Get wealth from the faucet for the provided address.
-
-        :param address: the address.
-        :param amount: optional int
-        :param url: the url
-
-        :return: optional string
-        """
-        if url is None:
-            url = DEFAULT_ADDRESS
-
-        if amount is None:
-            amount = int(LAMPORTS_PER_SOL * 0.5)
-        else:
-            amount = LAMPORTS_PER_SOL * amount
-
-        solana_client = Client(url, commitment="confirmed")
-        resp = solana_client.request_airdrop(PublicKey(address), amount)
-
-        response = json.loads(resp.to_json())
-        if "message" in response:
-            _default_logger.error("Response: {}".format(response["message"]))
-            raise Exception(response.get("message"))
-        if response["result"] is None:
-            _default_logger.error("Response: {}".format("airdrop failed"))
-        elif "error" in response:  # pragma: no cover
-            _default_logger.error("Response: {}".format("airdrop failed"))
-        elif "result" in response:  # pragma: nocover
-            _default_logger.warning(
-                "Response: {}\nMessage: {}".format("success", response["result"])
-            )
-            return response["result"]
-        raise Exception("airdrop failed")
```

### Comparing `open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/PKG-INFO` & `open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-solana
-Version: 1.31.0
+Version: 1.32.0
 Summary: Python package wrapping the public and private key cryptography and ledger api of solana.
 Author: dassy23
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-solana-1.31.0/open_aea_ledger_solana.egg-info/SOURCES.txt` & `open-aea-ledger-solana-1.32.0/open_aea_ledger_solana.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 aea_ledger_solana/__init__.py
+aea_ledger_solana/account.py
+aea_ledger_solana/constants.py
+aea_ledger_solana/crypto.py
+aea_ledger_solana/faucet.py
+aea_ledger_solana/helper.py
 aea_ledger_solana/solana.py
+aea_ledger_solana/solana_api.py
+aea_ledger_solana/transaction.py
+aea_ledger_solana/transaction_instruction.py
+aea_ledger_solana/utils.py
 open_aea_ledger_solana.egg-info/PKG-INFO
 open_aea_ledger_solana.egg-info/SOURCES.txt
 open_aea_ledger_solana.egg-info/dependency_links.txt
 open_aea_ledger_solana.egg-info/entry_points.txt
 open_aea_ledger_solana.egg-info/requires.txt
 open_aea_ledger_solana.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_contracts.py
+tests/test_crypto.py
+tests/test_faucet.py
 tests/test_solana.py
+tests/test_solana_transaction.py
+tests/test_underlying_lib.py
 tests/data/Dockerfile
 tests/data/solana_private_key0.txt
 tests/data/solana_private_key1.txt
 tests/data/solana_private_key2.txt
 tests/data/solana_private_key_program.txt
 tests/data/dummy_contract/build/idl.json
 tests/data/spl-token-faucet/target/deploy/spl_token_faucet-keypair.json
```

### Comparing `open-aea-ledger-solana-1.31.0/setup.py` & `open-aea-ledger-solana-1.32.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,29 @@
 """Setup script for "aea_ledger_solana" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-solana",
-    version="1.31.0",
+    version="1.32.0",
     author="dassy23",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and ledger api of solana.",
     long_description="Python package wrapping the public and private key cryptography and ledger api of solana.",
     long_description_content_type="text/markdown",
     packages=find_packages(include=["aea_ledger_solana*"]),
     package_data={},
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
-        "ipfshttpclient==0.8.0a2",
+        "cryptography",
+        "PyNaCl==1.5.0",
         "solana==0.28.1",
         "solders==0.10.0",
         "anchorpy==0.14.0",
-        "base58==2.1.1",
-        "cryptography",
-        "PyNaCl==1.5.0",
-        "pythclient==0.1.2",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": ["solana = aea_ledger_solana:SolanaCrypto"],
         "aea.ledger_apis": ["solana = aea_ledger_solana:SolanaApi"],
         "aea.faucet_apis": ["solana = aea_ledger_solana:SolanaFaucetApi"],
     },
```

### Comparing `open-aea-ledger-solana-1.31.0/tests/__init__.py` & `open-aea-ledger-solana-1.32.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/conftest.py` & `open-aea-ledger-solana-1.32.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 SOLANA_DEFAULT_CHAIN_ID = 420
 SOLANA_DEFAULT_CURRENCY_DENOM = "lamports"
 SOLANA_TESTNET_CONFIG = {"address": SOLANA_DEFAULT_ADDRESS}
 
 
 logger = logging.getLogger(__name__)
 
+PROGRAM_KEYPAIR_PATH = Path(ROOT_DIR, "tests", "data", "solana_private_key_program.txt")
+PAYER_KEYPAIR_PATH = Path(ROOT_DIR, "tests", "data", "solana_private_key1.txt")
+PLAYER1_KEYPAIR_PATH = Path(ROOT_DIR, "tests", "data", "solana_private_key1.txt")
+PLAYER2_KEYPAIR_PATH = Path(ROOT_DIR, "tests", "data", "solana_private_key2.txt")
+
 
 def action_for_platform(platform_name: str, skip: bool = True) -> Callable:
     """
     Decorate a pytest class or method to skip on certain platform.
 
     :param platform_name: check `platform.system()` for available platforms.
     :param skip: if True, the test will be skipped; if False, the test will be run ONLY on the chosen platform.
```

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/Dockerfile` & `open-aea-ledger-solana-1.32.0/tests/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/dummy_contract/build/idl.json` & `open-aea-ledger-solana-1.32.0/tests/data/dummy_contract/build/idl.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so` & `open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json` & `open-aea-ledger-solana-1.32.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so` & `open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json` & `open-aea-ledger-solana-1.32.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-solana-1.31.0/tests/test_solana.py` & `open-aea-ledger-solana-1.32.0/tests/test_solana.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,37 @@
 import logging
 import platform
 import time
 from pathlib import Path
 from typing import Optional, Tuple, Union
 
 import pytest
+from solders.signature import Signature
 
 
 if platform.system() != "Linux":
     pytest.skip("Runs only on linux", allow_module_level=True)
 
-from aea_ledger_solana import (
-    LAMPORTS_PER_SOL,
-    PublicKey,
-    SolanaApi,
-    SolanaCrypto,
-    SolanaFaucetApi,
-)
+from aea_ledger_solana import LAMPORTS_PER_SOL, SolanaApi, SolanaCrypto, SolanaFaucetApi
 from nacl.signing import VerifyKey
+from solders.system_program import ID as SYS_PROGRAM_ID
 
 from aea.common import JSONLike
 
 from tests.conftest import AIRDROP_AMOUNT, MAX_FLAKY_RERUNS, ROOT_DIR
 
 
 # testing keys #
 program_keypair_path = Path(ROOT_DIR, "tests", "data", "solana_private_key_program.txt")
 payer_keypair_path = Path(ROOT_DIR, "tests", "data", "solana_private_key1.txt")
 player1_keypair_path = Path(ROOT_DIR, "tests", "data", "solana_private_key1.txt")
 player2_keypair_path = Path(ROOT_DIR, "tests", "data", "solana_private_key2.txt")
 
 # helper functions #
+EXAMPLE_PUBLIC_ADDRESS = "A8eco8kzjUk5CdefzuM1nZMUDmuZ7Eg4UfAstfCqFNTi"
 
 
 def retry_airdrop_if_result_none(faucet, address, amount=None):
     """Fund address with faucet."""
     cnt = 0
     tx = None
     while tx is None and cnt < 10:
@@ -63,26 +60,25 @@
         time.sleep(2)
     return tx
 
 
 def _generate_wealth_if_needed(
     api, address, amount=None, min_amount=None
 ) -> Union[str, None]:
-
     balance = api.get_balance(address)
 
     min_balance = min_amount if min_amount is not None else 1000000000
     if balance >= min_balance:
         return "not required"
     else:
         faucet = SolanaFaucetApi()
         cnt = 0
         transaction_digest = None
         while transaction_digest is None and cnt < 10:
-            transaction_digest = faucet._try_get_wealth(address)
+            transaction_digest = faucet.try_get_wealth(address)
             cnt += 1
             time.sleep(10)
 
         if transaction_digest is None:
             return "failed"
         else:
             _, is_settled = _wait_get_receipt(api, transaction_digest)
@@ -195,34 +191,32 @@
 
 def test_sign_message():
     """Test message sign functionality."""
     wallet = SolanaCrypto()
     wallet2 = SolanaCrypto()
     msg = bytes("hello", "utf8")
     msg2 = bytes("hellooo", "utf8")
-
     sig = wallet.sign_message(msg)
 
+    signature = Signature.from_string(sig)
+
     try:
-        result = VerifyKey(bytes(wallet.public_key)).verify(
-            smessage=msg2, signature=bytes(sig.to_bytes_array())
-        )
+        verification_key = VerifyKey(bytes(wallet.entity.pubkey()))
+        verification_key.verify(smessage=msg2, signature=bytes(signature))
     except Exception as e:
         assert e.args[0] == "Signature was forged or corrupt"
 
     try:
-        result = VerifyKey(bytes(wallet2.public_key)).verify(
-            smessage=msg, signature=bytes(sig.to_bytes_array())
-        )
+        verification_key = VerifyKey(bytes(wallet2.entity.pubkey()))
+        verification_key.verify(smessage=msg, signature=bytes(signature))
     except Exception as e:
         assert e.args[0] == "Signature was forged or corrupt"
 
-    result = VerifyKey(bytes(wallet.public_key)).verify(
-        smessage=msg, signature=bytes(sig.to_bytes_array())
-    )
+    verification_key = VerifyKey(bytes(wallet.entity.pubkey()))
+    result = verification_key.verify(smessage=msg, signature=bytes(signature))
 
     assert result == msg, "Failed to sign message"
 
 
 @pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS)
 @pytest.mark.integration
 @pytest.mark.ledger
@@ -275,55 +269,55 @@
     assert tx["blockTime"] == transaction_receipt["blockTime"], "Should be same"
 
     balance3 = solana_api.get_balance(account2.address)
 
     assert AMOUNT == balance3, "Should be the same balance"
 
 
-@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS)
+@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS, reruns_delay=5)
 @pytest.mark.integration
 @pytest.mark.ledger
 def test_funded_transfer_transaction(solana_private_key_file):
     """Test the construction, signing and submitting of a transfer transaction."""
     account1 = SolanaCrypto(payer_keypair_path)
     account2 = SolanaCrypto(player2_keypair_path)
 
     solana_api = SolanaApi()
     solana_faucet_api = SolanaFaucetApi()
     solana_faucet_api.get_wealth(account1.address)
     solana_faucet_api.get_wealth(account2.address)
 
-    balance1 = solana_api.get_balance(account1.public_key)
-    balance2 = solana_api.get_balance(account2.public_key)
+    balance1 = solana_api.get_balance(account1.address)
+    balance2 = solana_api.get_balance(account2.address)
     assert balance1 >= solana_faucet_api.DEFAULT_AMOUNT
     assert balance2 >= solana_faucet_api.DEFAULT_AMOUNT
 
     AMOUNT = 2222
 
     tx_params = {
-        "sender_address": account1.public_key,
-        "destination_address": account2.public_key,
+        "sender_address": account1.address,
+        "destination_address": account2.address,
         "amount": AMOUNT,
     }
 
     transaction_digest, transaction_receipt, is_settled = _construct_and_settle_tx(
         solana_api,
         account1,
         account2,
         tx_params,
     )
     assert is_settled, "Failed to verify tx!"
 
     tx = solana_api.get_transaction(transaction_digest)
 
     assert tx["blockTime"] == transaction_receipt["blockTime"], "Should be same"
-    assert balance2 + AMOUNT == solana_api.get_balance(account2.public_key)
+    assert balance2 + AMOUNT == solana_api.get_balance(account2.address)
 
 
-@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS)
+@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS, reruns_delay=5)
 @pytest.mark.integration
 @pytest.mark.ledger
 def test_get_sol_balance(caplog, solana_private_key_file):
     """Test the balance is zero for a new account."""
     with caplog.at_level(logging.DEBUG, logger="aea.crypto.solana._default_logger"):
         sc = SolanaCrypto(payer_keypair_path)
         sa = SolanaApi()
@@ -340,18 +334,16 @@
     with caplog.at_level(logging.DEBUG, logger="aea.crypto.solana._default_logger"):
         solana_faucet_api = SolanaFaucetApi()
         sc = SolanaCrypto(private_key_path=solana_private_key_file)
         solana_api = SolanaApi()
 
         retries = 0
         tx_signature = None
-        while retries < MAX_FLAKY_RERUNS:
-            tx_signature = solana_faucet_api._try_get_wealth(
-                sc.public_key, AIRDROP_AMOUNT
-            )
+        while retries <= MAX_FLAKY_RERUNS:
+            tx_signature = solana_faucet_api.try_get_wealth(sc.address, AIRDROP_AMOUNT)
             if tx_signature is None:
                 retries += 1
                 time.sleep(2)
             else:
                 break
 
         assert tx_signature is not None
@@ -412,34 +404,37 @@
     instance = SolanaApi.get_contract_instance(
         SolanaApi, contract_interface=result, contract_address=pid
     )
 
     assert hasattr(instance["program"], "coder")
 
 
+@pytest.mark.integration
+@pytest.mark.ledger
+@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS, reruns_delay=15)
 def test_get_transaction_transfer_logs(solana_private_key_file):
     """Test SolanaApi.get_transaction_transfer_logs."""
     solana_api = SolanaApi()
 
     account1 = SolanaCrypto(payer_keypair_path)
 
     resp = _generate_wealth_if_needed(solana_api, account1.address)
     assert resp != "failed", "Failed to generate wealth"
 
     account2 = SolanaCrypto()
 
-    balance1 = solana_api.get_balance(account1.public_key)
-    balance2 = solana_api.get_balance(account2.public_key)
+    balance1 = solana_api.get_balance(account1.address)
+    balance2 = solana_api.get_balance(account2.address)
     assert balance1 > 0
     assert balance2 >= 0
 
     AMOUNT = 1232323
     tx_params = {
-        "sender_address": account1.public_key,
-        "destination_address": account2.public_key,
+        "sender_address": account1.address,
+        "destination_address": account2.address,
         "amount": AMOUNT,
         "unfunded_account": True,
     }
 
     transaction_digest, transaction_receipt, is_settled = _construct_and_settle_tx(
         solana_api,
         account1,
@@ -501,15 +496,15 @@
         assert balance >= 2 * LAMPORTS_PER_SOL
         print("Payer Balance: " + str(balance / LAMPORTS_PER_SOL) + " SOL")
 
     result = sa.get_deploy_transaction(interface, payer)
     assert result is not None, "Should not be none"
 
 
-@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS)
+@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS, reruns_delay=5)
 @pytest.mark.integration
 @pytest.mark.ledger
 def test_contract_method_call():
     """Test the deploy contract method."""
 
     idl_path = Path(
         ROOT_DIR, "tests", "data", "tic-tac-toe", "target", "idl", "tic_tac_toe.json"
@@ -530,89 +525,106 @@
         idl_file_path=idl_path, bytecode_path=bytecode_path, program_keypair=program_kp
     )
 
     instance = sa.get_contract_instance(
         contract_interface=interface, contract_address=program_kp.address
     )
 
-    player1 = payer
     player2 = SolanaCrypto("./tests/data/solana_private_key2.txt")
+
     game = SolanaCrypto()
 
     resp = _generate_wealth_if_needed(sa, payer.address)
     assert resp != "failed", "Failed to generate wealth"
 
     resp = _generate_wealth_if_needed(sa, player2.address)
     assert resp != "failed", "Failed to generate wealth"
 
     # setup game
     program = instance["program"]
     program.provider.wallet = payer.entity
 
     accounts = {
-        "game": game.public_key,
-        "player_one": payer.public_key,
-        "system_program": PublicKey("11111111111111111111111111111111"),
+        "game": game.entity.pubkey(),
+        "player_one": payer.entity.pubkey(),
+        "system_program": SYS_PROGRAM_ID,
     }
 
     tx = sa.build_transaction(
         program,
         "setup_game",
         method_args={
-            "data": (player2.public_key,),
+            "data": (player2.entity.pubkey(),),
             "accounts": accounts,
         },
         tx_args=None,
     )
 
     tx = sa.add_nonce(tx)
 
     signed_transaction = game.sign_transaction(tx, [payer])
 
     transaction_digest = sa.send_signed_transaction(signed_transaction)
     assert transaction_digest is not None
 
     _, is_settled = _wait_get_receipt(sa, transaction_digest)
     assert is_settled is True
-    state = sa.get_state(game.public_key)
+    state = sa.get_state(game.address)
     decoded_state = program.coder.accounts.decode(state.data)
-
     player1 = payer
     player2 = player2
     column = 0
 
     # game loop
     while decoded_state.state.index == 0:
-
         active_player = player2 if decoded_state.turn % 2 == 0 else player1
         row = 0 if decoded_state.turn % 2 == 0 else 1
-        accounts = {"game": game.public_key, "player": active_player.public_key}
+        accounts = {
+            "game": game.entity.pubkey(),
+            "player": active_player.entity.pubkey(),
+        }
 
         tile = program.type["Tile"](row=row, column=column)
 
         tx1 = sa.build_transaction(
             program,
             "play",
             method_args={
                 "data": (tile,),
                 "accounts": accounts,
             },
             tx_args=None,
         )
 
+        tx1["message"]["header"]["numReadonlySignedAccounts"] = 0
         tx1 = sa.add_nonce(tx1)
 
         signed_transaction = active_player.sign_transaction(
             tx1,
         )
 
         transaction_digest = sa.send_signed_transaction(signed_transaction)
         assert transaction_digest is not None
         _, is_settled = _wait_get_receipt(sa, transaction_digest)
         assert is_settled is True
-        state = sa.get_state(game.public_key)
+        state = sa.get_state(game.address)
         decoded_state = program.coder.accounts.decode(state.data)
 
         if row == 0:
             column += 1
 
-    assert decoded_state.state.winner == player1.public_key
+    assert str(decoded_state.state.winner) == player1.address
+
+
+@pytest.mark.flaky(reruns=MAX_FLAKY_RERUNS)
+@pytest.mark.integration
+def test_get_create_account_tx():
+    """Test whether the create account function necessary for the sending of a transaction to new account works."""
+    solana_api = SolanaApi()
+    account_1 = SolanaCrypto()
+    account_2 = SolanaCrypto()
+    tx = solana_api._api.get_create_account_instructions(
+        sender_address=account_1.address,
+        destination_address=account_2.address,
+        lamports=1,
+    )
+    assert tx is not None, "Create account transaction is None"
```

