# Comparing `tmp/glitter_sdk-0.1.2.tar.gz` & `tmp/glitter_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/root/python/glitter-sdk-py/dist/tmp5807n9yy/glitter_sdk-0.1.2.tar", last modified: Mon May  9 14:44:19 2022, max compression
+gzip compressed data, was "glitter_sdk-0.2.0.tar", max compression
```

## Comparing `glitter_sdk-0.1.2.tar` & `glitter_sdk-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,152 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      235 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)      131 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3809 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/tests/test_driver.py
--rw-r--r--   0 root         (0) root         (0)       37 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2563 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/glitter_sdk/
--rw-r--r--   0 root         (0) root         (0)    15995 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/glitter_sdk/driver.py
--rw-r--r--   0 root         (0) root         (0)     2406 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/glitter_sdk/pool.py
--rw-r--r--   0 root         (0) root         (0)     4901 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/glitter_sdk/connection.py
--rw-r--r--   0 root         (0) root         (0)     2144 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/glitter_sdk/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      349 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/glitter_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3435 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/glitter_sdk/utils.py
--rw-r--r--   0 root         (0) root         (0)     3216 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/glitter_sdk/transport.py
--rw-r--r--   0 root         (0) root         (0)     1866 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/README.rst
--rw-r--r--   0 root         (0) root         (0)    10696 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1436 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-09 14:44:18.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-05-09 14:44:18.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      354 2022-05-09 14:44:18.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      575 2022-05-09 14:44:18.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2563 2022-05-09 14:44:18.000000 glitter_sdk-0.1.2/glitter_sdk.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 14:44:19.000000 glitter_sdk-0.1.2/docs/
--rw-r--r--   0 root         (0) root         (0)     3831 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/docs/tutorial.rst
--rw-r--r--   0 root         (0) root         (0)      634 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      361 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/docs/libref.rst
--rw-r--r--   0 root         (0) root         (0)     2245 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     5174 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/docs/quickstart.rst
--rw-r--r--   0 root         (0) root         (0)    18945 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/docs/examples.rst
--rw-r--r--   0 root         (0) root         (0)      800 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      305 2022-04-11 03:28:15.000000 glitter_sdk-0.1.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1508 2022-05-09 14:43:16.000000 glitter_sdk-0.1.2/docs/install.rst
+-rw-r--r--   0        0        0     1073 2023-03-05 15:04:49.729817 glitter_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1912 2023-04-01 03:19:53.336155 glitter_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0       13 2023-03-13 11:08:58.347247 glitter_sdk-0.2.0/glitter_sdk/.gitignore
+-rw-r--r--   0        0        0      163 2023-03-13 11:08:58.347884 glitter_sdk-0.2.0/glitter_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.347981 glitter_sdk-0.2.0/glitter_sdk/client/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-01 03:19:53.341248 glitter_sdk-0.2.0/glitter_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.348980 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      812 2023-03-13 11:08:58.349462 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0     1491 2023-03-26 07:42:53.767656 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     3436 2023-03-13 11:08:58.350610 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     2471 2023-03-13 11:08:58.351174 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     4394 2023-03-13 11:08:58.351558 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     3632 2023-03-13 11:08:58.352180 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10274 2023-03-13 11:08:58.352841 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2023-03-13 11:08:58.353005 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2023-03-13 11:08:58.353409 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2330 2023-03-13 11:08:58.353973 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     3776 2023-03-13 11:08:58.354544 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13196 2023-03-13 11:08:58.355132 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     3065 2023-03-13 11:08:58.355281 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0    14761 2023-04-01 03:49:21.407472 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     5011 2023-03-13 11:08:58.356484 glitter_sdk-0.2.0/glitter_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0      878 2023-03-13 11:08:58.357495 glitter_sdk-0.2.0/glitter_sdk/client/lcd/constants/CLIENT.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.357577 glitter_sdk-0.2.0/glitter_sdk/client/lcd/constants/__init__.py
+-rw-r--r--   0        0        0    13565 2023-04-11 14:04:54.684976 glitter_sdk-0.2.0/glitter_sdk/client/lcd/db.py
+-rw-r--r--   0        0        0    11243 2023-04-01 03:21:04.039552 glitter_sdk-0.2.0/glitter_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     1803 2023-03-13 11:08:58.358639 glitter_sdk-0.2.0/glitter_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.359148 glitter_sdk-0.2.0/glitter_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0      949 2023-03-27 15:23:06.688797 glitter_sdk-0.2.0/glitter_sdk/core/__init__.py
+-rw-r--r--   0        0        0      661 2023-03-26 07:20:19.533891 glitter_sdk-0.2.0/glitter_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      656 2023-03-26 07:19:34.210859 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0     1835 2023-03-26 07:18:28.803583 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2953 2023-03-13 11:08:58.362249 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3965 2023-03-13 11:08:58.362787 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     2731 2023-03-13 11:08:58.363597 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/continuous_vesting_account.py
+-rw-r--r--   0        0        0     2498 2023-03-13 11:08:58.364171 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/delayed_vesting_account.py
+-rw-r--r--   0        0        0     2340 2023-03-26 07:47:19.134258 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/eth_account.py
+-rw-r--r--   0        0        0     4441 2023-03-13 11:08:58.364906 glitter_sdk-0.2.0/glitter_sdk/core/auth/data/periodic_vesting_account.py
+-rw-r--r--   0        0        0      331 2023-03-13 11:08:58.365065 glitter_sdk-0.2.0/glitter_sdk/core/auth/msgs/__init__.py
+-rw-r--r--   0        0        0     2921 2023-03-13 11:08:58.365643 glitter_sdk-0.2.0/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
+-rw-r--r--   0        0        0     2838 2023-03-13 11:08:58.366178 glitter_sdk-0.2.0/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py
+-rw-r--r--   0        0        0     1620 2023-03-13 11:08:58.366670 glitter_sdk-0.2.0/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
+-rw-r--r--   0        0        0      446 2023-03-13 11:08:58.366825 glitter_sdk-0.2.0/glitter_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0     9613 2023-03-13 11:08:58.367344 glitter_sdk-0.2.0/glitter_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6109 2023-03-13 11:08:58.367944 glitter_sdk-0.2.0/glitter_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2023-03-13 11:08:58.368579 glitter_sdk-0.2.0/glitter_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0     7099 2023-03-13 11:08:58.369139 glitter_sdk-0.2.0/glitter_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     5009 2023-03-13 11:08:58.369678 glitter_sdk-0.2.0/glitter_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2023-03-13 11:08:58.369822 glitter_sdk-0.2.0/glitter_sdk/core/block.py
+-rw-r--r--   0        0        0     2724 2023-03-13 11:08:58.370319 glitter_sdk-0.2.0/glitter_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7746 2023-03-13 11:08:58.370786 glitter_sdk-0.2.0/glitter_sdk/core/coin.py
+-rw-r--r--   0        0        0     8360 2023-03-13 11:08:58.371350 glitter_sdk-0.2.0/glitter_sdk/core/coins.py
+-rw-r--r--   0        0        0     2707 2023-03-13 11:08:58.371947 glitter_sdk-0.2.0/glitter_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2023-03-13 11:08:58.372138 glitter_sdk-0.2.0/glitter_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0     2069 2023-03-13 11:08:58.372665 glitter_sdk-0.2.0/glitter_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1085 2023-03-13 11:08:58.373096 glitter_sdk-0.2.0/glitter_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2023-03-13 11:08:58.373255 glitter_sdk-0.2.0/glitter_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0     6940 2023-03-13 11:08:58.373671 glitter_sdk-0.2.0/glitter_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2692 2023-03-13 11:08:58.374225 glitter_sdk-0.2.0/glitter_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2008 2023-03-13 11:08:58.374552 glitter_sdk-0.2.0/glitter_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2023-03-13 11:08:58.374699 glitter_sdk-0.2.0/glitter_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0     9141 2023-03-13 11:08:58.375006 glitter_sdk-0.2.0/glitter_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     3178 2023-03-13 11:08:58.375537 glitter_sdk-0.2.0/glitter_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      412 2023-03-13 11:08:58.376076 glitter_sdk-0.2.0/glitter_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0     6154 2023-03-13 11:08:58.376639 glitter_sdk-0.2.0/glitter_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6516 2023-03-13 11:08:58.377173 glitter_sdk-0.2.0/glitter_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1695 2023-03-13 11:08:58.377677 glitter_sdk-0.2.0/glitter_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0       47 2023-03-13 11:08:58.377816 glitter_sdk-0.2.0/glitter_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      492 2023-03-13 11:08:58.377946 glitter_sdk-0.2.0/glitter_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0     4811 2023-03-13 11:08:58.378397 glitter_sdk-0.2.0/glitter_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5323 2023-03-13 11:08:58.378944 glitter_sdk-0.2.0/glitter_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1407 2023-03-13 11:08:58.379538 glitter_sdk-0.2.0/glitter_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1947 2023-03-13 11:08:58.380124 glitter_sdk-0.2.0/glitter_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2023-03-13 11:08:58.380315 glitter_sdk-0.2.0/glitter_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0    14728 2023-03-13 11:08:58.380848 glitter_sdk-0.2.0/glitter_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5942 2023-03-13 11:08:58.381430 glitter_sdk-0.2.0/glitter_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0     9941 2023-03-13 11:08:58.381746 glitter_sdk-0.2.0/glitter_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       80 2023-03-13 11:08:58.381885 glitter_sdk-0.2.0/glitter_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0     2205 2023-03-13 11:08:58.382371 glitter_sdk-0.2.0/glitter_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2023-03-13 11:08:58.382853 glitter_sdk-0.2.0/glitter_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      703 2023-03-13 11:08:58.383309 glitter_sdk-0.2.0/glitter_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3369 2023-03-13 11:08:58.383789 glitter_sdk-0.2.0/glitter_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0     3334 2023-03-13 11:08:58.384170 glitter_sdk-0.2.0/glitter_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      805 2023-03-13 11:08:58.384582 glitter_sdk-0.2.0/glitter_sdk/core/msg.py
+-rw-r--r--   0        0        0      188 2023-03-13 11:08:58.385068 glitter_sdk-0.2.0/glitter_sdk/core/msgs/__init__.py
+-rw-r--r--   0        0        0     1033 2023-03-13 11:08:58.385519 glitter_sdk-0.2.0/glitter_sdk/core/msgs/argument.py
+-rw-r--r--   0        0        0     3793 2023-03-13 11:08:58.385939 glitter_sdk-0.2.0/glitter_sdk/core/msgs/arguments.py
+-rw-r--r--   0        0        0     2993 2023-03-13 11:08:58.386453 glitter_sdk-0.2.0/glitter_sdk/core/msgs/msgs.py
+-rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.386999 glitter_sdk-0.2.0/glitter_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11366 2023-03-13 11:08:58.387613 glitter_sdk-0.2.0/glitter_sdk/core/numeric.py
+-rw-r--r--   0        0        0      114 2023-03-13 11:08:58.387760 glitter_sdk-0.2.0/glitter_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0     3325 2023-03-13 11:08:58.388287 glitter_sdk-0.2.0/glitter_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    12728 2023-04-01 02:49:01.061356 glitter_sdk-0.2.0/glitter_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2621 2023-03-28 05:25:40.105427 glitter_sdk-0.2.0/glitter_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3550 2023-03-13 11:08:58.389976 glitter_sdk-0.2.0/glitter_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2023-03-13 11:08:58.390162 glitter_sdk-0.2.0/glitter_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0     1103 2023-03-13 11:08:58.390660 glitter_sdk-0.2.0/glitter_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2023-03-13 11:08:58.390909 glitter_sdk-0.2.0/glitter_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      429 2023-03-13 11:08:58.391064 glitter_sdk-0.2.0/glitter_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0    11301 2023-03-13 11:08:58.391674 glitter_sdk-0.2.0/glitter_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     9625 2023-03-13 11:08:58.392264 glitter_sdk-0.2.0/glitter_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11092 2023-03-13 11:08:58.392899 glitter_sdk-0.2.0/glitter_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0    15136 2023-03-28 05:26:03.502060 glitter_sdk-0.2.0/glitter_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2023-03-13 11:08:58.393573 glitter_sdk-0.2.0/glitter_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      149 2023-03-13 11:08:58.393699 glitter_sdk-0.2.0/glitter_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0     3330 2023-03-13 11:08:58.394221 glitter_sdk-0.2.0/glitter_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2191 2023-03-13 11:08:58.394592 glitter_sdk-0.2.0/glitter_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      315 2023-03-13 11:08:58.394733 glitter_sdk-0.2.0/glitter_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0     9320 2023-03-13 11:08:58.395189 glitter_sdk-0.2.0/glitter_sdk/core/wasm/data.py
+-rw-r--r--   0        0        0    11303 2023-03-13 11:08:58.395703 glitter_sdk-0.2.0/glitter_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0    24195 2023-03-13 11:08:58.396188 glitter_sdk-0.2.0/glitter_sdk/core/wasm/proposals.py
+-rw-r--r--   0        0        0      968 2023-04-09 13:57:19.944409 glitter_sdk-0.2.0/glitter_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.396859 glitter_sdk-0.2.0/glitter_sdk/key/__init__.py
+-rw-r--r--   0        0        0     8381 2023-04-02 10:34:15.503189 glitter_sdk-0.2.0/glitter_sdk/key/key.py
+-rw-r--r--   0        0        0     2365 2023-04-05 14:48:32.941589 glitter_sdk-0.2.0/glitter_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1846 2023-04-02 15:21:54.394109 glitter_sdk-0.2.0/glitter_sdk/key/raw.py
+-rw-r--r--   0        0        0     3623 2023-03-26 02:18:44.107996 glitter_sdk-0.2.0/glitter_sdk/key/topub.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.398493 glitter_sdk-0.2.0/glitter_sdk/util/__init__.py
+-rw-r--r--   0        0        0     1678 2023-03-13 11:08:58.398629 glitter_sdk-0.2.0/glitter_sdk/util/base.py
+-rw-r--r--   0        0        0      878 2023-03-13 11:08:58.398824 glitter_sdk-0.2.0/glitter_sdk/util/constants/CLIENT.py
+-rw-r--r--   0        0        0      679 2023-03-13 11:08:58.399255 glitter_sdk-0.2.0/glitter_sdk/util/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2023-03-13 11:08:58.399786 glitter_sdk-0.2.0/glitter_sdk/util/constants/CR.py
+-rw-r--r--   0        0        0    12296 2023-03-13 11:08:58.400320 glitter_sdk-0.2.0/glitter_sdk/util/constants/ER.py
+-rw-r--r--   0        0        0      370 2023-03-13 11:08:58.400832 glitter_sdk-0.2.0/glitter_sdk/util/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2023-03-13 11:08:58.401339 glitter_sdk-0.2.0/glitter_sdk/util/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2023-03-13 11:08:58.401638 glitter_sdk-0.2.0/glitter_sdk/util/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.401707 glitter_sdk-0.2.0/glitter_sdk/util/constants/__init__.py
+-rw-r--r--   0        0        0     3253 2023-03-13 11:08:58.402210 glitter_sdk-0.2.0/glitter_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2023-03-13 11:08:58.402331 glitter_sdk-0.2.0/glitter_sdk/util/converter.py
+-rw-r--r--   0        0        0     1325 2023-04-06 08:22:21.253664 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/__init__.py
+-rw-r--r--   0        0        0     1386 2023-04-06 03:28:40.834754 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/converter/__init__.py
+-rw-r--r--   0        0        0     5017 2023-04-01 02:40:55.205070 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/converter/bech32.py
+-rw-r--r--   0        0        0      230 2023-04-01 02:49:31.013058 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-01 02:49:31.022589 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/ecdsa.py
+-rw-r--r--   0        0        0     6072 2023-04-01 02:40:55.205900 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/ecdsa_base.py
+-rw-r--r--   0        0        0    14377 2023-04-01 02:40:55.206225 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py
+-rw-r--r--   0        0        0    24914 2023-04-01 02:49:31.016470 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/ecdsa_python.py
+-rw-r--r--   0        0        0    17376 2023-04-01 02:40:55.207175 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/openssl.py
+-rw-r--r--   0        0        0     8962 2023-04-01 02:40:55.207492 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/crypto/utils.py
+-rw-r--r--   0        0        0        0 2023-04-01 02:40:55.207660 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/eth/__init__.py
+-rw-r--r--   0        0        0    55432 2023-04-01 02:49:31.019972 glitter_sdk-0.2.0/glitter_sdk/util/encrypt/eth/ethereum.py
+-rw-r--r--   0        0        0      211 2023-03-13 11:08:58.402439 glitter_sdk-0.2.0/glitter_sdk/util/hash.py
+-rw-r--r--   0        0        0     1696 2023-03-13 11:08:58.403849 glitter_sdk-0.2.0/glitter_sdk/util/json.py
+-rw-r--r--   0        0        0     1045 2023-03-13 11:08:58.404376 glitter_sdk-0.2.0/glitter_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2550 2023-03-13 11:08:58.404831 glitter_sdk-0.2.0/glitter_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     3887 2023-03-13 11:08:58.405152 glitter_sdk-0.2.0/glitter_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0      732 2023-03-13 11:08:58.405653 glitter_sdk-0.2.0/glitter_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0    10425 2023-03-13 11:08:58.406211 glitter_sdk-0.2.0/glitter_sdk/util/parse_sql.py
+-rw-r--r--   0        0        0      294 2023-03-13 11:08:58.406577 glitter_sdk-0.2.0/glitter_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      133 2023-03-13 11:08:58.406694 glitter_sdk-0.2.0/glitter_sdk/util/url.py
+-rw-r--r--   0        0        0      727 2023-04-11 14:23:42.634429 glitter_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 glitter_sdk-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

