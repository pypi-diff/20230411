# Comparing `tmp/pytorch-calibrated-0.0.0.tar.gz` & `tmp/pytorch-calibrated-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-calibrated-0.0.0.tar", last modified: Tue Apr  4 20:41:38 2023, max compression
+gzip compressed data, was "pytorch-calibrated-0.0.2.tar", last modified: Tue Apr 11 01:27:17 2023, max compression
```

## Comparing `pytorch-calibrated-0.0.0.tar` & `pytorch-calibrated-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/pytorch_calibrated/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/pytorch_calibrated/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/pytorch_calibrated/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-04 20:41:38.000000 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-04 20:41:38.000000 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:41:38.000000 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-04 20:41:38.000000 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 20:41:38.000000 pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:41:38.198217 pytorch-calibrated-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-04 20:41:29.000000 pytorch-calibrated-0.0.0/tests/test_numerical_calibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_numerical_calibrator.py
```

### Comparing `pytorch-calibrated-0.0.0/LICENSE` & `pytorch-calibrated-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/PKG-INFO` & `pytorch-calibrated-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 746f  : 2.1.Name: pyto
 00000020: 7263 682d 6361 6c69 6272 6174 6564 0a56  rch-calibrated.V
-00000030: 6572 7369 6f6e 3a20 302e 302e 300a 5375  ersion: 0.0.0.Su
+00000030: 6572 7369 6f6e 3a20 302e 302e 320a 5375  ersion: 0.0.2.Su
 00000040: 6d6d 6172 793a 2041 2050 7954 6f72 6368  mmary: A PyTorch
 00000050: 204c 6962 7261 7279 2046 6f72 2049 6e74   Library For Int
 00000060: 6572 7072 6574 6162 6c65 204d 6163 6869  erpretable Machi
 00000070: 6e65 204c 6561 726e 696e 670a 4175 7468  ne Learning.Auth
 00000080: 6f72 2d65 6d61 696c 3a20 534f 5441 4920  or-email: SOTAI 
 00000090: 3c73 7570 706f 7274 4073 6f74 6169 2e61  <support@sotai.a
 000000a0: 693e 0a4d 6169 6e74 6169 6e65 722d 656d  i>.Maintainer-em
@@ -57,110 +57,146 @@
 00000380: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
 00000390: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
 000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000003b0: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
 000003c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 000003d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
 000003e0: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-000003f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000410: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
-00000420: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000430: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000440: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
-00000450: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
-00000460: 6765 6e63 650a 436c 6173 7369 6669 6572  gence.Classifier
-00000470: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
-00000480: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-00000490: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
-000004a0: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
-000004b0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000004c0: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
-000004d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000004e0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
-000004f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000500: 4e53 450a 0a23 2050 7954 6f72 6368 2043  NSE..# PyTorch C
-00000510: 616c 6962 7261 7465 640a 0a41 2050 7954  alibrated..A PyT
-00000520: 6f72 6368 204c 6962 7261 7279 2046 6f72  orch Library For
-00000530: 2049 6e74 6572 7072 6574 6162 6c65 204d   Interpretable M
-00000540: 6163 6869 6e65 204c 6561 726e 696e 672e  achine Learning.
-00000550: 2054 6869 7320 6c69 6272 6172 7920 6973   This library is
-00000560: 2061 2050 7954 6f72 6368 2069 6d70 6c65   a PyTorch imple
-00000570: 6d65 6e74 6174 696f 6e20 6f66 206d 6f64  mentation of mod
-00000580: 656c 696e 6720 7465 6368 6e69 7175 6573  eling techniques
-00000590: 2066 6f75 6e64 2069 6e20 5b4d 6f6e 6f74   found in [Monot
-000005a0: 6f6e 6963 2043 616c 6962 7261 7465 6420  onic Calibrated 
-000005b0: 496e 7465 7270 6f6c 6174 6564 204c 6f6f  Interpolated Loo
-000005c0: 6b2d 5570 2054 6162 6c65 735d 2868 7474  k-Up Tables](htt
-000005d0: 7073 3a2f 2f6a 6d6c 722e 6f72 672f 7061  ps://jmlr.org/pa
-000005e0: 7065 7273 2f76 6f6c 756d 6531 372f 3135  pers/volume17/15
-000005f0: 2d32 3433 2f31 352d 3234 332e 7064 6629  -243/15-243.pdf)
-00000600: 2e0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
-00000610: 696f 6e0a 0a5b 5265 6665 7265 6e63 655d  ion..[Reference]
-00000620: 2872 6566 6572 656e 6365 2f72 6566 6572  (reference/refer
-00000630: 656e 6365 2e6d 6429 2070 726f 7669 6465  ence.md) provide
-00000640: 7320 6120 7465 6368 6e69 6361 6c20 7265  s a technical re
-00000650: 6665 7265 6e63 6520 666f 7220 7468 6520  ference for the 
-00000660: 6c69 6272 6172 792e 0a0a 416c 6c20 646f  library...All do
-00000670: 6375 6d65 6e74 7320 6172 6520 686f 7374  cuments are host
-00000680: 6564 2061 7420 5b68 7474 7073 3a2f 2f64  ed at [https://d
-00000690: 6f63 732e 736f 7461 692e 6169 2f70 7974  ocs.sotai.ai/pyt
-000006a0: 6f72 6368 2d63 616c 6962 7261 7465 645d  orch-calibrated]
-000006b0: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
-000006c0: 7461 692e 6169 2f70 7974 6f72 6368 2d63  tai.ai/pytorch-c
-000006d0: 616c 6962 7261 7465 6429 2e0a 0a23 2320  alibrated)...## 
-000006e0: 436f 6e74 7269 6275 7469 6f6e 2047 7569  Contribution Gui
-000006f0: 6465 6c69 6e65 730a 0a53 6565 2074 6865  delines..See the
-00000700: 2067 7569 6465 206f 6e20 5b63 6f6e 7472   guide on [contr
-00000710: 6962 7574 696e 675d 2843 4f4e 5452 4942  ibuting](CONTRIB
-00000720: 5554 494e 472e 6d64 2920 666f 7220 6675  UTING.md) for fu
-00000730: 6c6c 2064 6574 6169 6c73 206f 6e20 686f  ll details on ho
-00000740: 7720 746f 2063 6f6e 7472 6962 7574 6520  w to contribute 
-00000750: 746f 2074 6865 206c 6962 7261 7279 2e20  to the library. 
-00000760: 466f 7220 616e 7920 6665 6174 7572 6520  For any feature 
-00000770: 616e 642f 6f72 2062 7567 2072 6571 7565  and/or bug reque
-00000780: 7374 732c 2076 6973 6974 206f 7572 205b  sts, visit our [
-00000790: 4973 7375 6573 5d28 6874 7470 733a 2f2f  Issues](https://
-000007a0: 6769 7468 7562 2e63 6f6d 2f53 4f54 4149  github.com/SOTAI
-000007b0: 2d4c 6162 732f 7079 746f 7263 682d 6361  -Labs/pytorch-ca
-000007c0: 6c69 6272 6174 6564 2f69 7373 7565 7329  librated/issues)
-000007d0: 206f 7220 5b50 726f 6a65 6374 5d28 6874   or [Project](ht
-000007e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007f0: 2f6f 7267 732f 534f 5441 492d 4c61 6273  /orgs/SOTAI-Labs
-00000800: 2f70 726f 6a65 6374 732f 3429 2070 6167  /projects/4) pag
-00000810: 652e 0a0a 2323 2041 7274 6966 6963 650a  e...## Artifice.
-00000820: 0a41 7274 6966 6963 6520 6973 2061 2066  .Artifice is a f
-00000830: 756c 6c79 2d68 6f73 7465 6420 706c 6174  ully-hosted plat
-00000840: 666f 726d 2066 6f72 2069 6e74 6572 7072  form for interpr
-00000850: 6574 6162 6c65 206d 6163 6869 6e65 206c  etable machine l
-00000860: 6561 726e 696e 672e 2049 7420 7072 6f76  earning. It prov
-00000870: 6964 6573 2061 6e20 6561 7379 2077 6179  ides an easy way
-00000880: 2074 6f20 636f 6e66 6967 7572 6520 616e   to configure an
-00000890: 6420 7472 6169 6e20 6361 6c69 6272 6174  d train calibrat
-000008a0: 6564 206d 6f64 656c 7320 616e 6420 6973  ed models and is
-000008b0: 2070 6f77 6572 6564 2062 7920 5b50 7954   powered by [PyT
-000008c0: 6f72 6368 2043 616c 6962 7261 7465 645d  orch Calibrated]
-000008d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000008e0: 636f 6d2f 534f 5441 492d 4c61 6273 2f70  com/SOTAI-Labs/p
-000008f0: 7974 6f72 6368 2d63 616c 6962 7261 7465  ytorch-calibrate
-00000900: 6429 2061 6e64 205b 5465 6e73 6f72 466c  d) and [TensorFl
-00000910: 6f77 204c 6174 7469 6365 5d28 6874 7470  ow Lattice](http
-00000920: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000930: 656e 736f 7266 6c6f 772f 6c61 7474 6963  ensorflow/lattic
-00000940: 6529 2e0a 0a53 6565 205b 6874 7470 733a  e)...See [https:
-00000950: 2f2f 646f 6373 2e73 6f74 6169 2e61 692f  //docs.sotai.ai/
-00000960: 6172 7469 6669 6365 5d28 6874 7470 733a  artifice](https:
-00000970: 2f2f 646f 6373 2e73 6f74 6169 2e61 692f  //docs.sotai.ai/
-00000980: 6172 7469 6669 6365 2920 746f 206c 6561  artifice) to lea
-00000990: 726e 206d 6f72 652e 0a0a 2323 2045 7861  rn more...## Exa
-000009a0: 6d70 6c65 730a 0a46 6f72 2064 6574 6169  mples..For detai
-000009b0: 6c65 6420 6578 616d 706c 6573 206f 6e20  led examples on 
-000009c0: 686f 7720 746f 2075 7365 2074 6865 206c  how to use the l
-000009d0: 6962 7261 7279 2c20 7365 6520 5b45 7861  ibrary, see [Exa
-000009e0: 6d70 6c65 735d 2865 7861 6d70 6c65 732f  mples](examples/
-000009f0: 6578 616d 706c 6573 2e6d 6429 2e0a 0a23  examples.md)...#
-00000a00: 2320 4c69 6365 6e73 650a 0a5b 4170 6163  # License..[Apac
-00000a10: 6865 2032 2e30 5d28 6874 7470 733a 2f2f  he 2.0](https://
-00000a20: 6769 7468 7562 2e63 6f6d 2f53 4f54 4149  github.com/SOTAI
-00000a30: 2d4c 6162 732f 7079 746f 7263 682d 6361  -Labs/pytorch-ca
-00000a40: 6c69 6272 6174 6564 2f62 6c6f 622f 6465  librated/blob/de
-00000a50: 762f 4c49 4345 4e53 4529 0a              v/LICENSE).
+000003f0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000400: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000410: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+00000420: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000430: 6365 0a43 6c61 7373 6966 6965 723a 2054  ce.Classifier: T
+00000440: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000450: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000460: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
+00000470: 686f 6e20 4d6f 6475 6c65 730a 5265 7175  hon Modules.Requ
+00000480: 6972 6573 2d50 7974 686f 6e3a 203c 332e  ires-Python: <3.
+00000490: 3131 2c3e 3d33 2e38 0a44 6573 6372 6970  11,>=3.8.Descrip
+000004a0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+000004b0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+000004c0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+000004d0: 4943 454e 5345 0a0a 3c68 3120 616c 6967  ICENSE..<h1 alig
+000004e0: 6e3d 2263 656e 7465 7222 3e50 7954 6f72  n="center">PyTor
+000004f0: 6368 2043 616c 6962 7261 7465 643c 2f68  ch Calibrated</h
+00000500: 313e 0a0a 3c70 2061 6c69 676e 3d27 6365  1>..<p align='ce
+00000510: 6e74 6572 273e 0a3c 6120 6872 6566 3d22  nter'>.<a href="
+00000520: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000530: 2f70 726f 6a65 6374 2f70 7974 6f72 6368  /project/pytorch
+00000540: 2d63 616c 6962 7261 7465 642f 223e 3c69  -calibrated/"><i
+00000550: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000560: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000570: 7970 692f 762f 7079 746f 7263 682d 6361  ypi/v/pytorch-ca
+00000580: 6c69 6272 6174 6564 2220 2f3e 3c2f 613e  librated" /></a>
+00000590: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000005a0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
+000005b0: 4149 2d4c 6162 732f 7079 746f 7263 682d  AI-Labs/pytorch-
+000005c0: 6361 6c69 6272 6174 6564 2f61 6374 696f  calibrated/actio
+000005d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000005e0: 7473 2e79 6d6c 2220 3e3c 696d 6720 7372  ts.yml" ><img sr
+000005f0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000600: 622e 636f 6d2f 534f 5441 492d 4c61 6273  b.com/SOTAI-Labs
+00000610: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+00000620: 7465 642f 6163 7469 6f6e 732f 776f 726b  ted/actions/work
+00000630: 666c 6f77 732f 7465 7374 732e 796d 6c2f  flows/tests.yml/
+00000640: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000650: 3d64 6576 2220 2f3e 3c2f 613e 0a3c 2f70  =dev" /></a>.</p
+00000660: 3e0a 0a41 2050 7954 6f72 6368 204c 6962  >..A PyTorch Lib
+00000670: 7261 7279 2046 6f72 2049 6e74 6572 7072  rary For Interpr
+00000680: 6574 6162 6c65 204d 6163 6869 6e65 204c  etable Machine L
+00000690: 6561 726e 696e 672e 2054 6869 7320 6c69  earning. This li
+000006a0: 6272 6172 7920 6973 2061 2050 7954 6f72  brary is a PyTor
+000006b0: 6368 2069 6d70 6c65 6d65 6e74 6174 696f  ch implementatio
+000006c0: 6e20 6f66 206d 6f64 656c 696e 6720 7465  n of modeling te
+000006d0: 6368 6e69 7175 6573 2066 6f75 6e64 2069  chniques found i
+000006e0: 6e20 5b4d 6f6e 6f74 6f6e 6963 2043 616c  n [Monotonic Cal
+000006f0: 6962 7261 7465 6420 496e 7465 7270 6f6c  ibrated Interpol
+00000700: 6174 6564 204c 6f6f 6b2d 5570 2054 6162  ated Look-Up Tab
+00000710: 6c65 735d 2868 7474 7073 3a2f 2f6a 6d6c  les](https://jml
+00000720: 722e 6f72 672f 7061 7065 7273 2f76 6f6c  r.org/papers/vol
+00000730: 756d 6531 372f 3135 2d32 3433 2f31 352d  ume17/15-243/15-
+00000740: 3234 332e 7064 6629 2e0a 0a49 6e73 7461  243.pdf)...Insta
+00000750: 6c6c 6c69 6e67 2074 6865 2070 6163 6b61  llling the packa
+00000760: 6765 3a0a 0a60 6060 7368 656c 6c0a 7069  ge:..```shell.pi
+00000770: 7020 696e 7374 616c 6c20 7079 746f 7263  p install pytorc
+00000780: 682d 6361 6c69 6272 6174 6564 0a60 6060  h-calibrated.```
+00000790: 0a0a 496d 706f 7274 696e 6720 7468 6520  ..Importing the 
+000007a0: 7061 636b 6167 653a 0a0a 6060 6070 7974  package:..```pyt
+000007b0: 686f 6e0a 696d 706f 7274 2070 7974 6f72  hon.import pytor
+000007c0: 6368 5f63 616c 6962 7261 7465 6420 6173  ch_calibrated as
+000007d0: 2070 7463 6d0a 6060 600a 0a23 2320 446f   ptcm.```..## Do
+000007e0: 6375 6d65 6e74 6174 696f 6e0a 0a5b 5265  cumentation..[Re
+000007f0: 6665 7265 6e63 655d 2868 7474 7073 3a2f  ference](https:/
+00000800: 2f64 6f63 732e 736f 7461 692e 6169 2f70  /docs.sotai.ai/p
+00000810: 7974 6f72 6368 2d63 616c 6962 7261 7465  ytorch-calibrate
+00000820: 642f 7265 6665 7265 6e63 6529 2070 726f  d/reference) pro
+00000830: 7669 6465 7320 6120 7465 6368 6e69 6361  vides a technica
+00000840: 6c20 7265 6665 7265 6e63 6520 666f 7220  l reference for 
+00000850: 7468 6520 6c69 6272 6172 792e 0a0a 416c  the library...Al
+00000860: 6c20 646f 6375 6d65 6e74 7320 6172 6520  l documents are 
+00000870: 686f 7374 6564 2061 7420 5b68 7474 7073  hosted at [https
+00000880: 3a2f 2f64 6f63 732e 736f 7461 692e 6169  ://docs.sotai.ai
+00000890: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+000008a0: 7465 645d 2868 7474 7073 3a2f 2f64 6f63  ted](https://doc
+000008b0: 732e 736f 7461 692e 6169 2f70 7974 6f72  s.sotai.ai/pytor
+000008c0: 6368 2d63 616c 6962 7261 7465 6429 2e0a  ch-calibrated)..
+000008d0: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
+000008e0: 2047 7569 6465 6c69 6e65 730a 0a53 6565   Guidelines..See
+000008f0: 2074 6865 2067 7569 6465 206f 6e20 5b63   the guide on [c
+00000900: 6f6e 7472 6962 7574 696e 675d 2868 7474  ontributing](htt
+00000910: 7073 3a2f 2f64 6f63 732e 736f 7461 692e  ps://docs.sotai.
+00000920: 6169 2f70 7974 6f72 6368 2d63 616c 6962  ai/pytorch-calib
+00000930: 7261 7465 642f 636f 6e74 7269 6275 7469  rated/contributi
+00000940: 6e67 2920 666f 7220 6675 6c6c 2064 6574  ng) for full det
+00000950: 6169 6c73 206f 6e20 686f 7720 746f 2063  ails on how to c
+00000960: 6f6e 7472 6962 7574 6520 746f 2074 6865  ontribute to the
+00000970: 206c 6962 7261 7279 2e20 466f 7220 616e   library. For an
+00000980: 7920 6665 6174 7572 6520 616e 642f 6f72  y feature and/or
+00000990: 2062 7567 2072 6571 7565 7374 732c 2076   bug requests, v
+000009a0: 6973 6974 206f 7572 205b 4973 7375 6573  isit our [Issues
+000009b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000009c0: 2e63 6f6d 2f53 4f54 4149 2d4c 6162 732f  .com/SOTAI-Labs/
+000009d0: 7079 746f 7263 682d 6361 6c69 6272 6174  pytorch-calibrat
+000009e0: 6564 2f69 7373 7565 7329 206f 7220 5b50  ed/issues) or [P
+000009f0: 726f 6a65 6374 5d28 6874 7470 733a 2f2f  roject](https://
+00000a00: 6769 7468 7562 2e63 6f6d 2f6f 7267 732f  github.com/orgs/
+00000a10: 534f 5441 492d 4c61 6273 2f70 726f 6a65  SOTAI-Labs/proje
+00000a20: 6374 732f 3429 2070 6167 652e 0a0a 2323  cts/4) page...##
+00000a30: 2041 7274 6966 6963 650a 0a41 7274 6966   Artifice..Artif
+00000a40: 6963 6520 6973 2061 2066 756c 6c79 2d68  ice is a fully-h
+00000a50: 6f73 7465 6420 706c 6174 666f 726d 2066  osted platform f
+00000a60: 6f72 2069 6e74 6572 7072 6574 6162 6c65  or interpretable
+00000a70: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00000a80: 672e 2049 7420 7072 6f76 6964 6573 2061  g. It provides a
+00000a90: 6e20 6561 7379 2077 6179 2074 6f20 636f  n easy way to co
+00000aa0: 6e66 6967 7572 6520 616e 6420 7472 6169  nfigure and trai
+00000ab0: 6e20 6361 6c69 6272 6174 6564 206d 6f64  n calibrated mod
+00000ac0: 656c 7320 616e 6420 6973 2070 6f77 6572  els and is power
+00000ad0: 6564 2062 7920 5b50 7954 6f72 6368 2043  ed by [PyTorch C
+00000ae0: 616c 6962 7261 7465 645d 2868 7474 7073  alibrated](https
+00000af0: 3a2f 2f67 6974 6875 622e 636f 6d2f 534f  ://github.com/SO
+00000b00: 5441 492d 4c61 6273 2f70 7974 6f72 6368  TAI-Labs/pytorch
+00000b10: 2d63 616c 6962 7261 7465 6429 2061 6e64  -calibrated) and
+00000b20: 205b 5465 6e73 6f72 466c 6f77 204c 6174   [TensorFlow Lat
+00000b30: 7469 6365 5d28 6874 7470 733a 2f2f 6769  tice](https://gi
+00000b40: 7468 7562 2e63 6f6d 2f74 656e 736f 7266  thub.com/tensorf
+00000b50: 6c6f 772f 6c61 7474 6963 6529 2e0a 0a53  low/lattice)...S
+00000b60: 6565 205b 6874 7470 733a 2f2f 646f 6373  ee [https://docs
+00000b70: 2e73 6f74 6169 2e61 692f 6172 7469 6669  .sotai.ai/artifi
+00000b80: 6365 5d28 6874 7470 733a 2f2f 646f 6373  ce](https://docs
+00000b90: 2e73 6f74 6169 2e61 692f 6172 7469 6669  .sotai.ai/artifi
+00000ba0: 6365 2920 746f 206c 6561 726e 206d 6f72  ce) to learn mor
+00000bb0: 652e 0a0a 2323 2045 7861 6d70 6c65 730a  e...## Examples.
+00000bc0: 0a46 6f72 2064 6574 6169 6c65 6420 6578  .For detailed ex
+00000bd0: 616d 706c 6573 206f 6e20 686f 7720 746f  amples on how to
+00000be0: 2075 7365 2074 6865 206c 6962 7261 7279   use the library
+00000bf0: 2c20 7365 6520 5b45 7861 6d70 6c65 735d  , see [Examples]
+00000c00: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
+00000c10: 7461 692e 6169 2f70 7974 6f72 6368 2d63  tai.ai/pytorch-c
+00000c20: 616c 6962 7261 7465 642f 6578 616d 706c  alibrated/exampl
+00000c30: 6573 292e 0a0a 2323 204c 6963 656e 7365  es)...## License
+00000c40: 0a0a 5b41 7061 6368 6520 322e 305d 2868  ..[Apache 2.0](h
+00000c50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c60: 6d2f 534f 5441 492d 4c61 6273 2f70 7974  m/SOTAI-Labs/pyt
+00000c70: 6f72 6368 2d63 616c 6962 7261 7465 642f  orch-calibrated/
+00000c80: 626c 6f62 2f64 6576 2f4c 4943 454e 5345  blob/dev/LICENSE
+00000c90: 290a                                     ).
```

### Comparing `pytorch-calibrated-0.0.0/docs/README.md` & `pytorch-calibrated-0.0.2/docs/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,124 @@
-00000000: 2320 5079 546f 7263 6820 4361 6c69 6272  # PyTorch Calibr
-00000010: 6174 6564 0a0a 4120 5079 546f 7263 6820  ated..A PyTorch 
-00000020: 4c69 6272 6172 7920 466f 7220 496e 7465  Library For Inte
-00000030: 7270 7265 7461 626c 6520 4d61 6368 696e  rpretable Machin
-00000040: 6520 4c65 6172 6e69 6e67 2e20 5468 6973  e Learning. This
-00000050: 206c 6962 7261 7279 2069 7320 6120 5079   library is a Py
-00000060: 546f 7263 6820 696d 706c 656d 656e 7461  Torch implementa
-00000070: 7469 6f6e 206f 6620 6d6f 6465 6c69 6e67  tion of modeling
-00000080: 2074 6563 686e 6971 7565 7320 666f 756e   techniques foun
-00000090: 6420 696e 205b 4d6f 6e6f 746f 6e69 6320  d in [Monotonic 
-000000a0: 4361 6c69 6272 6174 6564 2049 6e74 6572  Calibrated Inter
-000000b0: 706f 6c61 7465 6420 4c6f 6f6b 2d55 7020  polated Look-Up 
-000000c0: 5461 626c 6573 5d28 6874 7470 733a 2f2f  Tables](https://
-000000d0: 6a6d 6c72 2e6f 7267 2f70 6170 6572 732f  jmlr.org/papers/
-000000e0: 766f 6c75 6d65 3137 2f31 352d 3234 332f  volume17/15-243/
-000000f0: 3135 2d32 3433 2e70 6466 292e 0a0a 2323  15-243.pdf)...##
-00000100: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
-00000110: 5b52 6566 6572 656e 6365 5d28 7265 6665  [Reference](refe
-00000120: 7265 6e63 652f 7265 6665 7265 6e63 652e  rence/reference.
-00000130: 6d64 2920 7072 6f76 6964 6573 2061 2074  md) provides a t
-00000140: 6563 686e 6963 616c 2072 6566 6572 656e  echnical referen
-00000150: 6365 2066 6f72 2074 6865 206c 6962 7261  ce for the libra
-00000160: 7279 2e0a 0a41 6c6c 2064 6f63 756d 656e  ry...All documen
-00000170: 7473 2061 7265 2068 6f73 7465 6420 6174  ts are hosted at
-00000180: 205b 6874 7470 733a 2f2f 646f 6373 2e73   [https://docs.s
-00000190: 6f74 6169 2e61 692f 7079 746f 7263 682d  otai.ai/pytorch-
-000001a0: 6361 6c69 6272 6174 6564 5d28 6874 7470  calibrated](http
-000001b0: 733a 2f2f 646f 6373 2e73 6f74 6169 2e61  s://docs.sotai.a
-000001c0: 692f 7079 746f 7263 682d 6361 6c69 6272  i/pytorch-calibr
-000001d0: 6174 6564 292e 0a0a 2323 2043 6f6e 7472  ated)...## Contr
-000001e0: 6962 7574 696f 6e20 4775 6964 656c 696e  ibution Guidelin
-000001f0: 6573 0a0a 5365 6520 7468 6520 6775 6964  es..See the guid
-00000200: 6520 6f6e 205b 636f 6e74 7269 6275 7469  e on [contributi
-00000210: 6e67 5d28 434f 4e54 5249 4255 5449 4e47  ng](CONTRIBUTING
-00000220: 2e6d 6429 2066 6f72 2066 756c 6c20 6465  .md) for full de
-00000230: 7461 696c 7320 6f6e 2068 6f77 2074 6f20  tails on how to 
-00000240: 636f 6e74 7269 6275 7465 2074 6f20 7468  contribute to th
-00000250: 6520 6c69 6272 6172 792e 2046 6f72 2061  e library. For a
-00000260: 6e79 2066 6561 7475 7265 2061 6e64 2f6f  ny feature and/o
-00000270: 7220 6275 6720 7265 7175 6573 7473 2c20  r bug requests, 
-00000280: 7669 7369 7420 6f75 7220 5b49 7373 7565  visit our [Issue
-00000290: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-000002a0: 622e 636f 6d2f 534f 5441 492d 4c61 6273  b.com/SOTAI-Labs
-000002b0: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
-000002c0: 7465 642f 6973 7375 6573 2920 6f72 205b  ted/issues) or [
-000002d0: 5072 6f6a 6563 745d 2868 7474 7073 3a2f  Project](https:/
-000002e0: 2f67 6974 6875 622e 636f 6d2f 6f72 6773  /github.com/orgs
-000002f0: 2f53 4f54 4149 2d4c 6162 732f 7072 6f6a  /SOTAI-Labs/proj
-00000300: 6563 7473 2f34 2920 7061 6765 2e0a 0a23  ects/4) page...#
-00000310: 2320 4172 7469 6669 6365 0a0a 4172 7469  # Artifice..Arti
-00000320: 6669 6365 2069 7320 6120 6675 6c6c 792d  fice is a fully-
-00000330: 686f 7374 6564 2070 6c61 7466 6f72 6d20  hosted platform 
-00000340: 666f 7220 696e 7465 7270 7265 7461 626c  for interpretabl
-00000350: 6520 6d61 6368 696e 6520 6c65 6172 6e69  e machine learni
-00000360: 6e67 2e20 4974 2070 726f 7669 6465 7320  ng. It provides 
-00000370: 616e 2065 6173 7920 7761 7920 746f 2063  an easy way to c
-00000380: 6f6e 6669 6775 7265 2061 6e64 2074 7261  onfigure and tra
-00000390: 696e 2063 616c 6962 7261 7465 6420 6d6f  in calibrated mo
-000003a0: 6465 6c73 2061 6e64 2069 7320 706f 7765  dels and is powe
-000003b0: 7265 6420 6279 205b 5079 546f 7263 6820  red by [PyTorch 
-000003c0: 4361 6c69 6272 6174 6564 5d28 6874 7470  Calibrated](http
-000003d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000003e0: 4f54 4149 2d4c 6162 732f 7079 746f 7263  OTAI-Labs/pytorc
-000003f0: 682d 6361 6c69 6272 6174 6564 2920 616e  h-calibrated) an
-00000400: 6420 5b54 656e 736f 7246 6c6f 7720 4c61  d [TensorFlow La
-00000410: 7474 6963 655d 2868 7474 7073 3a2f 2f67  ttice](https://g
-00000420: 6974 6875 622e 636f 6d2f 7465 6e73 6f72  ithub.com/tensor
-00000430: 666c 6f77 2f6c 6174 7469 6365 292e 0a0a  flow/lattice)...
-00000440: 5365 6520 5b68 7474 7073 3a2f 2f64 6f63  See [https://doc
-00000450: 732e 736f 7461 692e 6169 2f61 7274 6966  s.sotai.ai/artif
-00000460: 6963 655d 2868 7474 7073 3a2f 2f64 6f63  ice](https://doc
-00000470: 732e 736f 7461 692e 6169 2f61 7274 6966  s.sotai.ai/artif
-00000480: 6963 6529 2074 6f20 6c65 6172 6e20 6d6f  ice) to learn mo
-00000490: 7265 2e0a 0a23 2320 4578 616d 706c 6573  re...## Examples
-000004a0: 0a0a 466f 7220 6465 7461 696c 6564 2065  ..For detailed e
-000004b0: 7861 6d70 6c65 7320 6f6e 2068 6f77 2074  xamples on how t
-000004c0: 6f20 7573 6520 7468 6520 6c69 6272 6172  o use the librar
-000004d0: 792c 2073 6565 205b 4578 616d 706c 6573  y, see [Examples
-000004e0: 5d28 6578 616d 706c 6573 2f65 7861 6d70  ](examples/examp
-000004f0: 6c65 732e 6d64 292e 0a0a 2323 204c 6963  les.md)...## Lic
-00000500: 656e 7365 0a0a 5b41 7061 6368 6520 322e  ense..[Apache 2.
-00000510: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
-00000520: 622e 636f 6d2f 534f 5441 492d 4c61 6273  b.com/SOTAI-Labs
-00000530: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
-00000540: 7465 642f 626c 6f62 2f64 6576 2f4c 4943  ted/blob/dev/LIC
-00000550: 454e 5345 290a                           ENSE).
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e50 7954 6f72 6368 2043 616c 6962  r">PyTorch Calib
+00000020: 7261 7465 643c 2f68 313e 0a0a 3c70 2061  rated</h1>..<p a
+00000030: 6c69 676e 3d27 6365 6e74 6572 273e 0a3c  lign='center'>.<
+00000040: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000050: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000060: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+00000070: 7465 642f 223e 3c69 6d67 2073 7263 3d22  ted/"><img src="
+00000080: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000090: 6c64 732e 696f 2f70 7970 692f 762f 7079  lds.io/pypi/v/py
+000000a0: 746f 7263 682d 6361 6c69 6272 6174 6564  torch-calibrated
+000000b0: 2220 2f3e 3c2f 613e 0a3c 6120 6872 6566  " /></a>.<a href
+000000c0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000000d0: 2e63 6f6d 2f53 4f54 4149 2d4c 6162 732f  .com/SOTAI-Labs/
+000000e0: 7079 746f 7263 682d 6361 6c69 6272 6174  pytorch-calibrat
+000000f0: 6564 2f61 6374 696f 6e73 2f77 6f72 6b66  ed/actions/workf
+00000100: 6c6f 7773 2f74 6573 7473 2e79 6d6c 2220  lows/tests.yml" 
+00000110: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 534f  ://github.com/SO
+00000130: 5441 492d 4c61 6273 2f70 7974 6f72 6368  TAI-Labs/pytorch
+00000140: 2d63 616c 6962 7261 7465 642f 6163 7469  -calibrated/acti
+00000150: 6f6e 732f 776f 726b 666c 6f77 732f 7465  ons/workflows/te
+00000160: 7374 732e 796d 6c2f 6261 6467 652e 7376  sts.yml/badge.sv
+00000170: 673f 6272 616e 6368 3d64 6576 2220 2f3e  g?branch=dev" />
+00000180: 3c2f 613e 0a3c 2f70 3e0a 0a41 2050 7954  </a>.</p>..A PyT
+00000190: 6f72 6368 204c 6962 7261 7279 2046 6f72  orch Library For
+000001a0: 2049 6e74 6572 7072 6574 6162 6c65 204d   Interpretable M
+000001b0: 6163 6869 6e65 204c 6561 726e 696e 672e  achine Learning.
+000001c0: 2054 6869 7320 6c69 6272 6172 7920 6973   This library is
+000001d0: 2061 2050 7954 6f72 6368 2069 6d70 6c65   a PyTorch imple
+000001e0: 6d65 6e74 6174 696f 6e20 6f66 206d 6f64  mentation of mod
+000001f0: 656c 696e 6720 7465 6368 6e69 7175 6573  eling techniques
+00000200: 2066 6f75 6e64 2069 6e20 5b4d 6f6e 6f74   found in [Monot
+00000210: 6f6e 6963 2043 616c 6962 7261 7465 6420  onic Calibrated 
+00000220: 496e 7465 7270 6f6c 6174 6564 204c 6f6f  Interpolated Loo
+00000230: 6b2d 5570 2054 6162 6c65 735d 2868 7474  k-Up Tables](htt
+00000240: 7073 3a2f 2f6a 6d6c 722e 6f72 672f 7061  ps://jmlr.org/pa
+00000250: 7065 7273 2f76 6f6c 756d 6531 372f 3135  pers/volume17/15
+00000260: 2d32 3433 2f31 352d 3234 332e 7064 6629  -243/15-243.pdf)
+00000270: 2e0a 0a49 6e73 7461 6c6c 6c69 6e67 2074  ...Installling t
+00000280: 6865 2070 6163 6b61 6765 3a0a 0a60 6060  he package:..```
+00000290: 7368 656c 6c0a 7069 7020 696e 7374 616c  shell.pip instal
+000002a0: 6c20 7079 746f 7263 682d 6361 6c69 6272  l pytorch-calibr
+000002b0: 6174 6564 0a60 6060 0a0a 496d 706f 7274  ated.```..Import
+000002c0: 696e 6720 7468 6520 7061 636b 6167 653a  ing the package:
+000002d0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+000002e0: 7274 2070 7974 6f72 6368 5f63 616c 6962  rt pytorch_calib
+000002f0: 7261 7465 6420 6173 2070 7463 6d0a 6060  rated as ptcm.``
+00000300: 600a 0a23 2320 446f 6375 6d65 6e74 6174  `..## Documentat
+00000310: 696f 6e0a 0a5b 5265 6665 7265 6e63 655d  ion..[Reference]
+00000320: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
+00000330: 7461 692e 6169 2f70 7974 6f72 6368 2d63  tai.ai/pytorch-c
+00000340: 616c 6962 7261 7465 642f 7265 6665 7265  alibrated/refere
+00000350: 6e63 6529 2070 726f 7669 6465 7320 6120  nce) provides a 
+00000360: 7465 6368 6e69 6361 6c20 7265 6665 7265  technical refere
+00000370: 6e63 6520 666f 7220 7468 6520 6c69 6272  nce for the libr
+00000380: 6172 792e 0a0a 416c 6c20 646f 6375 6d65  ary...All docume
+00000390: 6e74 7320 6172 6520 686f 7374 6564 2061  nts are hosted a
+000003a0: 7420 5b68 7474 7073 3a2f 2f64 6f63 732e  t [https://docs.
+000003b0: 736f 7461 692e 6169 2f70 7974 6f72 6368  sotai.ai/pytorch
+000003c0: 2d63 616c 6962 7261 7465 645d 2868 7474  -calibrated](htt
+000003d0: 7073 3a2f 2f64 6f63 732e 736f 7461 692e  ps://docs.sotai.
+000003e0: 6169 2f70 7974 6f72 6368 2d63 616c 6962  ai/pytorch-calib
+000003f0: 7261 7465 6429 2e0a 0a23 2320 436f 6e74  rated)...## Cont
+00000400: 7269 6275 7469 6f6e 2047 7569 6465 6c69  ribution Guideli
+00000410: 6e65 730a 0a53 6565 2074 6865 2067 7569  nes..See the gui
+00000420: 6465 206f 6e20 5b63 6f6e 7472 6962 7574  de on [contribut
+00000430: 696e 675d 2868 7474 7073 3a2f 2f64 6f63  ing](https://doc
+00000440: 732e 736f 7461 692e 6169 2f70 7974 6f72  s.sotai.ai/pytor
+00000450: 6368 2d63 616c 6962 7261 7465 642f 636f  ch-calibrated/co
+00000460: 6e74 7269 6275 7469 6e67 2920 666f 7220  ntributing) for 
+00000470: 6675 6c6c 2064 6574 6169 6c73 206f 6e20  full details on 
+00000480: 686f 7720 746f 2063 6f6e 7472 6962 7574  how to contribut
+00000490: 6520 746f 2074 6865 206c 6962 7261 7279  e to the library
+000004a0: 2e20 466f 7220 616e 7920 6665 6174 7572  . For any featur
+000004b0: 6520 616e 642f 6f72 2062 7567 2072 6571  e and/or bug req
+000004c0: 7565 7374 732c 2076 6973 6974 206f 7572  uests, visit our
+000004d0: 205b 4973 7375 6573 5d28 6874 7470 733a   [Issues](https:
+000004e0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
+000004f0: 4149 2d4c 6162 732f 7079 746f 7263 682d  AI-Labs/pytorch-
+00000500: 6361 6c69 6272 6174 6564 2f69 7373 7565  calibrated/issue
+00000510: 7329 206f 7220 5b50 726f 6a65 6374 5d28  s) or [Project](
+00000520: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000530: 6f6d 2f6f 7267 732f 534f 5441 492d 4c61  om/orgs/SOTAI-La
+00000540: 6273 2f70 726f 6a65 6374 732f 3429 2070  bs/projects/4) p
+00000550: 6167 652e 0a0a 2323 2041 7274 6966 6963  age...## Artific
+00000560: 650a 0a41 7274 6966 6963 6520 6973 2061  e..Artifice is a
+00000570: 2066 756c 6c79 2d68 6f73 7465 6420 706c   fully-hosted pl
+00000580: 6174 666f 726d 2066 6f72 2069 6e74 6572  atform for inter
+00000590: 7072 6574 6162 6c65 206d 6163 6869 6e65  pretable machine
+000005a0: 206c 6561 726e 696e 672e 2049 7420 7072   learning. It pr
+000005b0: 6f76 6964 6573 2061 6e20 6561 7379 2077  ovides an easy w
+000005c0: 6179 2074 6f20 636f 6e66 6967 7572 6520  ay to configure 
+000005d0: 616e 6420 7472 6169 6e20 6361 6c69 6272  and train calibr
+000005e0: 6174 6564 206d 6f64 656c 7320 616e 6420  ated models and 
+000005f0: 6973 2070 6f77 6572 6564 2062 7920 5b50  is powered by [P
+00000600: 7954 6f72 6368 2043 616c 6962 7261 7465  yTorch Calibrate
+00000610: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
+00000620: 622e 636f 6d2f 534f 5441 492d 4c61 6273  b.com/SOTAI-Labs
+00000630: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+00000640: 7465 6429 2061 6e64 205b 5465 6e73 6f72  ted) and [Tensor
+00000650: 466c 6f77 204c 6174 7469 6365 5d28 6874  Flow Lattice](ht
+00000660: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000670: 2f74 656e 736f 7266 6c6f 772f 6c61 7474  /tensorflow/latt
+00000680: 6963 6529 2e0a 0a53 6565 205b 6874 7470  ice)...See [http
+00000690: 733a 2f2f 646f 6373 2e73 6f74 6169 2e61  s://docs.sotai.a
+000006a0: 692f 6172 7469 6669 6365 5d28 6874 7470  i/artifice](http
+000006b0: 733a 2f2f 646f 6373 2e73 6f74 6169 2e61  s://docs.sotai.a
+000006c0: 692f 6172 7469 6669 6365 2920 746f 206c  i/artifice) to l
+000006d0: 6561 726e 206d 6f72 652e 0a0a 2323 2045  earn more...## E
+000006e0: 7861 6d70 6c65 730a 0a46 6f72 2064 6574  xamples..For det
+000006f0: 6169 6c65 6420 6578 616d 706c 6573 206f  ailed examples o
+00000700: 6e20 686f 7720 746f 2075 7365 2074 6865  n how to use the
+00000710: 206c 6962 7261 7279 2c20 7365 6520 5b45   library, see [E
+00000720: 7861 6d70 6c65 735d 2868 7474 7073 3a2f  xamples](https:/
+00000730: 2f64 6f63 732e 736f 7461 692e 6169 2f70  /docs.sotai.ai/p
+00000740: 7974 6f72 6368 2d63 616c 6962 7261 7465  ytorch-calibrate
+00000750: 642f 6578 616d 706c 6573 292e 0a0a 2323  d/examples)...##
+00000760: 204c 6963 656e 7365 0a0a 5b41 7061 6368   License..[Apach
+00000770: 6520 322e 305d 2868 7474 7073 3a2f 2f67  e 2.0](https://g
+00000780: 6974 6875 622e 636f 6d2f 534f 5441 492d  ithub.com/SOTAI-
+00000790: 4c61 6273 2f70 7974 6f72 6368 2d63 616c  Labs/pytorch-cal
+000007a0: 6962 7261 7465 642f 626c 6f62 2f64 6576  ibrated/blob/dev
+000007b0: 2f4c 4943 454e 5345 290a                 /LICENSE).
```

### Comparing `pytorch-calibrated-0.0.0/pyproject.toml` & `pytorch-calibrated-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "pytorch-calibrated"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release.
 #
 # NOTE: as part of the release flow, update this version immediately after release.
-version = "0.0.0"
+version = "0.0.2"
 description = "A PyTorch Library For Interpretable Machine Learning"
 readme = "docs/README.md"
 license = {text = "Apache-2.0"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
@@ -25,23 +25,22 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.8,<3.11"
 dependencies = [
     "absl-py>=1.4.0",
     "graphlib-backport>=1.0.3",
-    "numpy>=1.24.2",
+    "numpy>=1.23.5",
     "pandas>=1.5.3",
     "torch>=1.13.1,<=2.0.0",
 ]
 
 [project.urls]
 "Source" = "https://github.com/SOTAI-Labs/pytorch-calibrated"
 "Documentation" = "https://github.com/SOTAI-Labs/pytorch-calibrated/tree/dev/docs"
```

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/__init__.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # limitations under the License.
 """PyTorch implementation of calibrated modeling."""
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release.
 #
 # NOTE: as part of the release flow, update this version immediately after release.
-__version__ = "0.0.0"
+__version__ = "0.0.2"
 
 from pytorch_calibrated import configs, data, enums, layers, models
 
 __all__ = ["configs", "data", "enums", "layers", "models"]
```

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/configs.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/configs.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/data.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/data.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/enums.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/enums.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/layers/__init__.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/layers/categorical_calibrator.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/layers/linear.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/layers/numerical_calibrator.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated/models.py` & `pytorch-calibrated-0.0.2/pytorch_calibrated/models.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/PKG-INFO` & `pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 746f  : 2.1.Name: pyto
 00000020: 7263 682d 6361 6c69 6272 6174 6564 0a56  rch-calibrated.V
-00000030: 6572 7369 6f6e 3a20 302e 302e 300a 5375  ersion: 0.0.0.Su
+00000030: 6572 7369 6f6e 3a20 302e 302e 320a 5375  ersion: 0.0.2.Su
 00000040: 6d6d 6172 793a 2041 2050 7954 6f72 6368  mmary: A PyTorch
 00000050: 204c 6962 7261 7279 2046 6f72 2049 6e74   Library For Int
 00000060: 6572 7072 6574 6162 6c65 204d 6163 6869  erpretable Machi
 00000070: 6e65 204c 6561 726e 696e 670a 4175 7468  ne Learning.Auth
 00000080: 6f72 2d65 6d61 696c 3a20 534f 5441 4920  or-email: SOTAI 
 00000090: 3c73 7570 706f 7274 4073 6f74 6169 2e61  <support@sotai.a
 000000a0: 693e 0a4d 6169 6e74 6169 6e65 722d 656d  i>.Maintainer-em
@@ -57,110 +57,146 @@
 00000380: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
 00000390: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
 000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000003b0: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
 000003c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 000003d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
 000003e0: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-000003f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000410: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
-00000420: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000430: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000440: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
-00000450: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
-00000460: 6765 6e63 650a 436c 6173 7369 6669 6572  gence.Classifier
-00000470: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
-00000480: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-00000490: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
-000004a0: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
-000004b0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000004c0: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
-000004d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000004e0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
-000004f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000500: 4e53 450a 0a23 2050 7954 6f72 6368 2043  NSE..# PyTorch C
-00000510: 616c 6962 7261 7465 640a 0a41 2050 7954  alibrated..A PyT
-00000520: 6f72 6368 204c 6962 7261 7279 2046 6f72  orch Library For
-00000530: 2049 6e74 6572 7072 6574 6162 6c65 204d   Interpretable M
-00000540: 6163 6869 6e65 204c 6561 726e 696e 672e  achine Learning.
-00000550: 2054 6869 7320 6c69 6272 6172 7920 6973   This library is
-00000560: 2061 2050 7954 6f72 6368 2069 6d70 6c65   a PyTorch imple
-00000570: 6d65 6e74 6174 696f 6e20 6f66 206d 6f64  mentation of mod
-00000580: 656c 696e 6720 7465 6368 6e69 7175 6573  eling techniques
-00000590: 2066 6f75 6e64 2069 6e20 5b4d 6f6e 6f74   found in [Monot
-000005a0: 6f6e 6963 2043 616c 6962 7261 7465 6420  onic Calibrated 
-000005b0: 496e 7465 7270 6f6c 6174 6564 204c 6f6f  Interpolated Loo
-000005c0: 6b2d 5570 2054 6162 6c65 735d 2868 7474  k-Up Tables](htt
-000005d0: 7073 3a2f 2f6a 6d6c 722e 6f72 672f 7061  ps://jmlr.org/pa
-000005e0: 7065 7273 2f76 6f6c 756d 6531 372f 3135  pers/volume17/15
-000005f0: 2d32 3433 2f31 352d 3234 332e 7064 6629  -243/15-243.pdf)
-00000600: 2e0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
-00000610: 696f 6e0a 0a5b 5265 6665 7265 6e63 655d  ion..[Reference]
-00000620: 2872 6566 6572 656e 6365 2f72 6566 6572  (reference/refer
-00000630: 656e 6365 2e6d 6429 2070 726f 7669 6465  ence.md) provide
-00000640: 7320 6120 7465 6368 6e69 6361 6c20 7265  s a technical re
-00000650: 6665 7265 6e63 6520 666f 7220 7468 6520  ference for the 
-00000660: 6c69 6272 6172 792e 0a0a 416c 6c20 646f  library...All do
-00000670: 6375 6d65 6e74 7320 6172 6520 686f 7374  cuments are host
-00000680: 6564 2061 7420 5b68 7474 7073 3a2f 2f64  ed at [https://d
-00000690: 6f63 732e 736f 7461 692e 6169 2f70 7974  ocs.sotai.ai/pyt
-000006a0: 6f72 6368 2d63 616c 6962 7261 7465 645d  orch-calibrated]
-000006b0: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
-000006c0: 7461 692e 6169 2f70 7974 6f72 6368 2d63  tai.ai/pytorch-c
-000006d0: 616c 6962 7261 7465 6429 2e0a 0a23 2320  alibrated)...## 
-000006e0: 436f 6e74 7269 6275 7469 6f6e 2047 7569  Contribution Gui
-000006f0: 6465 6c69 6e65 730a 0a53 6565 2074 6865  delines..See the
-00000700: 2067 7569 6465 206f 6e20 5b63 6f6e 7472   guide on [contr
-00000710: 6962 7574 696e 675d 2843 4f4e 5452 4942  ibuting](CONTRIB
-00000720: 5554 494e 472e 6d64 2920 666f 7220 6675  UTING.md) for fu
-00000730: 6c6c 2064 6574 6169 6c73 206f 6e20 686f  ll details on ho
-00000740: 7720 746f 2063 6f6e 7472 6962 7574 6520  w to contribute 
-00000750: 746f 2074 6865 206c 6962 7261 7279 2e20  to the library. 
-00000760: 466f 7220 616e 7920 6665 6174 7572 6520  For any feature 
-00000770: 616e 642f 6f72 2062 7567 2072 6571 7565  and/or bug reque
-00000780: 7374 732c 2076 6973 6974 206f 7572 205b  sts, visit our [
-00000790: 4973 7375 6573 5d28 6874 7470 733a 2f2f  Issues](https://
-000007a0: 6769 7468 7562 2e63 6f6d 2f53 4f54 4149  github.com/SOTAI
-000007b0: 2d4c 6162 732f 7079 746f 7263 682d 6361  -Labs/pytorch-ca
-000007c0: 6c69 6272 6174 6564 2f69 7373 7565 7329  librated/issues)
-000007d0: 206f 7220 5b50 726f 6a65 6374 5d28 6874   or [Project](ht
-000007e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007f0: 2f6f 7267 732f 534f 5441 492d 4c61 6273  /orgs/SOTAI-Labs
-00000800: 2f70 726f 6a65 6374 732f 3429 2070 6167  /projects/4) pag
-00000810: 652e 0a0a 2323 2041 7274 6966 6963 650a  e...## Artifice.
-00000820: 0a41 7274 6966 6963 6520 6973 2061 2066  .Artifice is a f
-00000830: 756c 6c79 2d68 6f73 7465 6420 706c 6174  ully-hosted plat
-00000840: 666f 726d 2066 6f72 2069 6e74 6572 7072  form for interpr
-00000850: 6574 6162 6c65 206d 6163 6869 6e65 206c  etable machine l
-00000860: 6561 726e 696e 672e 2049 7420 7072 6f76  earning. It prov
-00000870: 6964 6573 2061 6e20 6561 7379 2077 6179  ides an easy way
-00000880: 2074 6f20 636f 6e66 6967 7572 6520 616e   to configure an
-00000890: 6420 7472 6169 6e20 6361 6c69 6272 6174  d train calibrat
-000008a0: 6564 206d 6f64 656c 7320 616e 6420 6973  ed models and is
-000008b0: 2070 6f77 6572 6564 2062 7920 5b50 7954   powered by [PyT
-000008c0: 6f72 6368 2043 616c 6962 7261 7465 645d  orch Calibrated]
-000008d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000008e0: 636f 6d2f 534f 5441 492d 4c61 6273 2f70  com/SOTAI-Labs/p
-000008f0: 7974 6f72 6368 2d63 616c 6962 7261 7465  ytorch-calibrate
-00000900: 6429 2061 6e64 205b 5465 6e73 6f72 466c  d) and [TensorFl
-00000910: 6f77 204c 6174 7469 6365 5d28 6874 7470  ow Lattice](http
-00000920: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000930: 656e 736f 7266 6c6f 772f 6c61 7474 6963  ensorflow/lattic
-00000940: 6529 2e0a 0a53 6565 205b 6874 7470 733a  e)...See [https:
-00000950: 2f2f 646f 6373 2e73 6f74 6169 2e61 692f  //docs.sotai.ai/
-00000960: 6172 7469 6669 6365 5d28 6874 7470 733a  artifice](https:
-00000970: 2f2f 646f 6373 2e73 6f74 6169 2e61 692f  //docs.sotai.ai/
-00000980: 6172 7469 6669 6365 2920 746f 206c 6561  artifice) to lea
-00000990: 726e 206d 6f72 652e 0a0a 2323 2045 7861  rn more...## Exa
-000009a0: 6d70 6c65 730a 0a46 6f72 2064 6574 6169  mples..For detai
-000009b0: 6c65 6420 6578 616d 706c 6573 206f 6e20  led examples on 
-000009c0: 686f 7720 746f 2075 7365 2074 6865 206c  how to use the l
-000009d0: 6962 7261 7279 2c20 7365 6520 5b45 7861  ibrary, see [Exa
-000009e0: 6d70 6c65 735d 2865 7861 6d70 6c65 732f  mples](examples/
-000009f0: 6578 616d 706c 6573 2e6d 6429 2e0a 0a23  examples.md)...#
-00000a00: 2320 4c69 6365 6e73 650a 0a5b 4170 6163  # License..[Apac
-00000a10: 6865 2032 2e30 5d28 6874 7470 733a 2f2f  he 2.0](https://
-00000a20: 6769 7468 7562 2e63 6f6d 2f53 4f54 4149  github.com/SOTAI
-00000a30: 2d4c 6162 732f 7079 746f 7263 682d 6361  -Labs/pytorch-ca
-00000a40: 6c69 6272 6174 6564 2f62 6c6f 622f 6465  librated/blob/de
-00000a50: 762f 4c49 4345 4e53 4529 0a              v/LICENSE).
+000003f0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000400: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000410: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+00000420: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000430: 6365 0a43 6c61 7373 6966 6965 723a 2054  ce.Classifier: T
+00000440: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000450: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000460: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
+00000470: 686f 6e20 4d6f 6475 6c65 730a 5265 7175  hon Modules.Requ
+00000480: 6972 6573 2d50 7974 686f 6e3a 203c 332e  ires-Python: <3.
+00000490: 3131 2c3e 3d33 2e38 0a44 6573 6372 6970  11,>=3.8.Descrip
+000004a0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+000004b0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+000004c0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+000004d0: 4943 454e 5345 0a0a 3c68 3120 616c 6967  ICENSE..<h1 alig
+000004e0: 6e3d 2263 656e 7465 7222 3e50 7954 6f72  n="center">PyTor
+000004f0: 6368 2043 616c 6962 7261 7465 643c 2f68  ch Calibrated</h
+00000500: 313e 0a0a 3c70 2061 6c69 676e 3d27 6365  1>..<p align='ce
+00000510: 6e74 6572 273e 0a3c 6120 6872 6566 3d22  nter'>.<a href="
+00000520: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000530: 2f70 726f 6a65 6374 2f70 7974 6f72 6368  /project/pytorch
+00000540: 2d63 616c 6962 7261 7465 642f 223e 3c69  -calibrated/"><i
+00000550: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000560: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000570: 7970 692f 762f 7079 746f 7263 682d 6361  ypi/v/pytorch-ca
+00000580: 6c69 6272 6174 6564 2220 2f3e 3c2f 613e  librated" /></a>
+00000590: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000005a0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
+000005b0: 4149 2d4c 6162 732f 7079 746f 7263 682d  AI-Labs/pytorch-
+000005c0: 6361 6c69 6272 6174 6564 2f61 6374 696f  calibrated/actio
+000005d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000005e0: 7473 2e79 6d6c 2220 3e3c 696d 6720 7372  ts.yml" ><img sr
+000005f0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000600: 622e 636f 6d2f 534f 5441 492d 4c61 6273  b.com/SOTAI-Labs
+00000610: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+00000620: 7465 642f 6163 7469 6f6e 732f 776f 726b  ted/actions/work
+00000630: 666c 6f77 732f 7465 7374 732e 796d 6c2f  flows/tests.yml/
+00000640: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000650: 3d64 6576 2220 2f3e 3c2f 613e 0a3c 2f70  =dev" /></a>.</p
+00000660: 3e0a 0a41 2050 7954 6f72 6368 204c 6962  >..A PyTorch Lib
+00000670: 7261 7279 2046 6f72 2049 6e74 6572 7072  rary For Interpr
+00000680: 6574 6162 6c65 204d 6163 6869 6e65 204c  etable Machine L
+00000690: 6561 726e 696e 672e 2054 6869 7320 6c69  earning. This li
+000006a0: 6272 6172 7920 6973 2061 2050 7954 6f72  brary is a PyTor
+000006b0: 6368 2069 6d70 6c65 6d65 6e74 6174 696f  ch implementatio
+000006c0: 6e20 6f66 206d 6f64 656c 696e 6720 7465  n of modeling te
+000006d0: 6368 6e69 7175 6573 2066 6f75 6e64 2069  chniques found i
+000006e0: 6e20 5b4d 6f6e 6f74 6f6e 6963 2043 616c  n [Monotonic Cal
+000006f0: 6962 7261 7465 6420 496e 7465 7270 6f6c  ibrated Interpol
+00000700: 6174 6564 204c 6f6f 6b2d 5570 2054 6162  ated Look-Up Tab
+00000710: 6c65 735d 2868 7474 7073 3a2f 2f6a 6d6c  les](https://jml
+00000720: 722e 6f72 672f 7061 7065 7273 2f76 6f6c  r.org/papers/vol
+00000730: 756d 6531 372f 3135 2d32 3433 2f31 352d  ume17/15-243/15-
+00000740: 3234 332e 7064 6629 2e0a 0a49 6e73 7461  243.pdf)...Insta
+00000750: 6c6c 6c69 6e67 2074 6865 2070 6163 6b61  llling the packa
+00000760: 6765 3a0a 0a60 6060 7368 656c 6c0a 7069  ge:..```shell.pi
+00000770: 7020 696e 7374 616c 6c20 7079 746f 7263  p install pytorc
+00000780: 682d 6361 6c69 6272 6174 6564 0a60 6060  h-calibrated.```
+00000790: 0a0a 496d 706f 7274 696e 6720 7468 6520  ..Importing the 
+000007a0: 7061 636b 6167 653a 0a0a 6060 6070 7974  package:..```pyt
+000007b0: 686f 6e0a 696d 706f 7274 2070 7974 6f72  hon.import pytor
+000007c0: 6368 5f63 616c 6962 7261 7465 6420 6173  ch_calibrated as
+000007d0: 2070 7463 6d0a 6060 600a 0a23 2320 446f   ptcm.```..## Do
+000007e0: 6375 6d65 6e74 6174 696f 6e0a 0a5b 5265  cumentation..[Re
+000007f0: 6665 7265 6e63 655d 2868 7474 7073 3a2f  ference](https:/
+00000800: 2f64 6f63 732e 736f 7461 692e 6169 2f70  /docs.sotai.ai/p
+00000810: 7974 6f72 6368 2d63 616c 6962 7261 7465  ytorch-calibrate
+00000820: 642f 7265 6665 7265 6e63 6529 2070 726f  d/reference) pro
+00000830: 7669 6465 7320 6120 7465 6368 6e69 6361  vides a technica
+00000840: 6c20 7265 6665 7265 6e63 6520 666f 7220  l reference for 
+00000850: 7468 6520 6c69 6272 6172 792e 0a0a 416c  the library...Al
+00000860: 6c20 646f 6375 6d65 6e74 7320 6172 6520  l documents are 
+00000870: 686f 7374 6564 2061 7420 5b68 7474 7073  hosted at [https
+00000880: 3a2f 2f64 6f63 732e 736f 7461 692e 6169  ://docs.sotai.ai
+00000890: 2f70 7974 6f72 6368 2d63 616c 6962 7261  /pytorch-calibra
+000008a0: 7465 645d 2868 7474 7073 3a2f 2f64 6f63  ted](https://doc
+000008b0: 732e 736f 7461 692e 6169 2f70 7974 6f72  s.sotai.ai/pytor
+000008c0: 6368 2d63 616c 6962 7261 7465 6429 2e0a  ch-calibrated)..
+000008d0: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
+000008e0: 2047 7569 6465 6c69 6e65 730a 0a53 6565   Guidelines..See
+000008f0: 2074 6865 2067 7569 6465 206f 6e20 5b63   the guide on [c
+00000900: 6f6e 7472 6962 7574 696e 675d 2868 7474  ontributing](htt
+00000910: 7073 3a2f 2f64 6f63 732e 736f 7461 692e  ps://docs.sotai.
+00000920: 6169 2f70 7974 6f72 6368 2d63 616c 6962  ai/pytorch-calib
+00000930: 7261 7465 642f 636f 6e74 7269 6275 7469  rated/contributi
+00000940: 6e67 2920 666f 7220 6675 6c6c 2064 6574  ng) for full det
+00000950: 6169 6c73 206f 6e20 686f 7720 746f 2063  ails on how to c
+00000960: 6f6e 7472 6962 7574 6520 746f 2074 6865  ontribute to the
+00000970: 206c 6962 7261 7279 2e20 466f 7220 616e   library. For an
+00000980: 7920 6665 6174 7572 6520 616e 642f 6f72  y feature and/or
+00000990: 2062 7567 2072 6571 7565 7374 732c 2076   bug requests, v
+000009a0: 6973 6974 206f 7572 205b 4973 7375 6573  isit our [Issues
+000009b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000009c0: 2e63 6f6d 2f53 4f54 4149 2d4c 6162 732f  .com/SOTAI-Labs/
+000009d0: 7079 746f 7263 682d 6361 6c69 6272 6174  pytorch-calibrat
+000009e0: 6564 2f69 7373 7565 7329 206f 7220 5b50  ed/issues) or [P
+000009f0: 726f 6a65 6374 5d28 6874 7470 733a 2f2f  roject](https://
+00000a00: 6769 7468 7562 2e63 6f6d 2f6f 7267 732f  github.com/orgs/
+00000a10: 534f 5441 492d 4c61 6273 2f70 726f 6a65  SOTAI-Labs/proje
+00000a20: 6374 732f 3429 2070 6167 652e 0a0a 2323  cts/4) page...##
+00000a30: 2041 7274 6966 6963 650a 0a41 7274 6966   Artifice..Artif
+00000a40: 6963 6520 6973 2061 2066 756c 6c79 2d68  ice is a fully-h
+00000a50: 6f73 7465 6420 706c 6174 666f 726d 2066  osted platform f
+00000a60: 6f72 2069 6e74 6572 7072 6574 6162 6c65  or interpretable
+00000a70: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00000a80: 672e 2049 7420 7072 6f76 6964 6573 2061  g. It provides a
+00000a90: 6e20 6561 7379 2077 6179 2074 6f20 636f  n easy way to co
+00000aa0: 6e66 6967 7572 6520 616e 6420 7472 6169  nfigure and trai
+00000ab0: 6e20 6361 6c69 6272 6174 6564 206d 6f64  n calibrated mod
+00000ac0: 656c 7320 616e 6420 6973 2070 6f77 6572  els and is power
+00000ad0: 6564 2062 7920 5b50 7954 6f72 6368 2043  ed by [PyTorch C
+00000ae0: 616c 6962 7261 7465 645d 2868 7474 7073  alibrated](https
+00000af0: 3a2f 2f67 6974 6875 622e 636f 6d2f 534f  ://github.com/SO
+00000b00: 5441 492d 4c61 6273 2f70 7974 6f72 6368  TAI-Labs/pytorch
+00000b10: 2d63 616c 6962 7261 7465 6429 2061 6e64  -calibrated) and
+00000b20: 205b 5465 6e73 6f72 466c 6f77 204c 6174   [TensorFlow Lat
+00000b30: 7469 6365 5d28 6874 7470 733a 2f2f 6769  tice](https://gi
+00000b40: 7468 7562 2e63 6f6d 2f74 656e 736f 7266  thub.com/tensorf
+00000b50: 6c6f 772f 6c61 7474 6963 6529 2e0a 0a53  low/lattice)...S
+00000b60: 6565 205b 6874 7470 733a 2f2f 646f 6373  ee [https://docs
+00000b70: 2e73 6f74 6169 2e61 692f 6172 7469 6669  .sotai.ai/artifi
+00000b80: 6365 5d28 6874 7470 733a 2f2f 646f 6373  ce](https://docs
+00000b90: 2e73 6f74 6169 2e61 692f 6172 7469 6669  .sotai.ai/artifi
+00000ba0: 6365 2920 746f 206c 6561 726e 206d 6f72  ce) to learn mor
+00000bb0: 652e 0a0a 2323 2045 7861 6d70 6c65 730a  e...## Examples.
+00000bc0: 0a46 6f72 2064 6574 6169 6c65 6420 6578  .For detailed ex
+00000bd0: 616d 706c 6573 206f 6e20 686f 7720 746f  amples on how to
+00000be0: 2075 7365 2074 6865 206c 6962 7261 7279   use the library
+00000bf0: 2c20 7365 6520 5b45 7861 6d70 6c65 735d  , see [Examples]
+00000c00: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
+00000c10: 7461 692e 6169 2f70 7974 6f72 6368 2d63  tai.ai/pytorch-c
+00000c20: 616c 6962 7261 7465 642f 6578 616d 706c  alibrated/exampl
+00000c30: 6573 292e 0a0a 2323 204c 6963 656e 7365  es)...## License
+00000c40: 0a0a 5b41 7061 6368 6520 322e 305d 2868  ..[Apache 2.0](h
+00000c50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c60: 6d2f 534f 5441 492d 4c61 6273 2f70 7974  m/SOTAI-Labs/pyt
+00000c70: 6f72 6368 2d63 616c 6962 7261 7465 642f  orch-calibrated/
+00000c80: 626c 6f62 2f64 6576 2f4c 4943 454e 5345  blob/dev/LICENSE
+00000c90: 290a                                     ).
```

### Comparing `pytorch-calibrated-0.0.0/pytorch_calibrated.egg-info/SOURCES.txt` & `pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_categorical_calibrator.py` & `pytorch-calibrated-0.0.2/tests/test_categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_configs.py` & `pytorch-calibrated-0.0.2/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_data.py` & `pytorch-calibrated-0.0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_linear.py` & `pytorch-calibrated-0.0.2/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_models.py` & `pytorch-calibrated-0.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.0/tests/test_numerical_calibrator.py` & `pytorch-calibrated-0.0.2/tests/test_numerical_calibrator.py`

 * *Files identical despite different names*

