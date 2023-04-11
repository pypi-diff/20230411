# Comparing `tmp/reedsolo-2.0.9.tar.gz` & `tmp/reedsolo-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reedsolo-2.0.9.tar", last modified: Fri Mar 31 13:38:08 2023, max compression
+gzip compressed data, was "reedsolo-2.1.0b1.tar", last modified: Tue Apr 11 12:36:05 2023, max compression
```

## Comparing `reedsolo-2.0.9.tar` & `reedsolo-2.1.0b1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.392818 reedsolo-2.0.9/
--rw-rw-rw-   0        0        0     2388 2023-01-06 16:38:12.000000 reedsolo-2.0.9/LICENSE
--rw-rw-rw-   0        0        0      174 2023-03-31 10:46:05.000000 reedsolo-2.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0    32045 2023-03-31 13:38:08.390825 reedsolo-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    26536 2023-03-31 11:11:06.000000 reedsolo-2.0.9/README.rst
--rw-rw-rw-   0        0        0    85611 2023-03-31 09:26:17.000000 reedsolo-2.0.9/creedsolo.pyx
--rw-rw-rw-   0        0        0     3863 2023-03-31 13:33:35.000000 reedsolo-2.0.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.369880 reedsolo-2.0.9/reedsolo.egg-info/
--rw-rw-rw-   0        0        0    32045 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    77739 2023-03-30 23:46:59.000000 reedsolo-2.0.9/reedsolo.py
--rw-rw-rw-   0        0        0       42 2023-03-31 13:38:08.392818 reedsolo-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     6011 2023-03-31 13:33:29.000000 reedsolo-2.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.387832 reedsolo-2.0.9/tests/
--rw-rw-rw-   0        0        0     1448 2023-03-30 15:08:31.000000 reedsolo-2.0.9/tests/perf.py
--rw-rw-rw-   0        0        0    38905 2023-03-30 23:16:59.000000 reedsolo-2.0.9/tests/test_creedsolo.py
--rw-rw-rw-   0        0        0    34123 2023-03-30 23:16:59.000000 reedsolo-2.0.9/tests/test_reedsolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43543 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.682986 reedsolo-2.1.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/creedsolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2240244 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/creedsolo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    85611 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/creedsolo.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/reedsolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/reedsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78312 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/reedsolo/reedsolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/reedsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43543 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/tests/test_creedsolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/tests/test_reedsolo.py
```

### Comparing `reedsolo-2.0.9/LICENSE` & `reedsolo-2.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.9/PKG-INFO` & `reedsolo-2.1.0b1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,520 +1,517 @@
-Metadata-Version: 2.1
-Name: reedsolo
-Version: 2.0.9
-Summary: Pure-Python Universal Errors And Erasures Reed-Solomon Encoder and Decoder
-Author: Tomer Filiba
-Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
-Maintainer: Stephen Karl Larroque
-Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
-License: The software is available under your choice of
-        Unlicense (SPDX short identifier: Unlicense) or
-        MIT No Attribution License (SPDX short identifier: MIT-0):
-        
-        -----
-        
-        <<START OF UNLICENSE>>
-        This is free and unencumbered software released into the public domain.
-        
-        Anyone is free to copy, modify, publish, use, compile, sell, or
-        distribute this software, either in source code form or as a compiled
-        binary, for any purpose, commercial or non-commercial, and by any
-        means.
-        
-        In jurisdictions that recognize copyright laws, the author or authors
-        of this software dedicate any and all copyright interest in the
-        software to the public domain. We make this dedication for the benefit
-        of the public at large and to the detriment of our heirs and
-        successors. We intend this dedication to be an overt act of
-        relinquishment in perpetuity of all present and future rights to this
-        software under copyright law.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-        OTHER DEALINGS IN THE SOFTWARE.
-        
-        For more information, please refer to <http://unlicense.org/>
-        <<END OF UNLICENSE>>
-        
-        -----
-        
-        <<START OF MIT-0 LICENSE>>
-        Copyright 2013-2023 Tomer Filiba & Stephen Larroque
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        <<END OF MIT-0 LICENSE>>
-        
-Project-URL: Homepage, https://github.com/tomerfiliba/reedsolomon
-Project-URL: Documentation, https://github.com/tomerfiliba/reedsolomon/blob/master/README.rst
-Project-URL: Source, https://github.com/tomerfiliba/reedsolomon
-Project-URL: Tracker, https://github.com/tomerfiliba/reedsolomon/issues
-Project-URL: Download, https://github.com/tomerfiliba/reedsolomon/releases
-Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
-Project-URL: Gentoo, https://packages.gentoo.org/packages/dev-python/reedsolomon
-Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
-Platform: any
-Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Cython
-Classifier: Topic :: Communications
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Topic :: System :: Recovery Tools
-Requires-Python: >=2.7
-Description-Content-Type: text/x-rst
-Provides-Extra: cythonize
-License-File: LICENSE
-
-Reed Solomon
-============
-
-|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
-
-|Build-Status| |Coverage|
-
-|Conda-Forge-Status| |Conda-Forge-Platforms| |Conda-Forge-Downloads|
-
-A pythonic `universal errors-and-erasures Reed-Solomon Codec <http://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction>`_ to protect your data from errors and bitrot. It includes a pure python implementation and an optional speed-optimized Cython/C extension.
-
-This is a burst-type implementation, so that it supports any Galois field higher than 2^3, but not binary streams. Burst errors are non-random errors that more often happen on data storage mediums such as hard drives, hence this library is better suited for data storage protection, and less for streams noise correction, although it also works for this purpose but with a bit of overhead (since it works with bytes only, instead of bits).
-
-Based on the wonderful tutorial at `Wikiversity <http://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_, written by "Bobmath" and "LRQ3000". If you are just starting with Reed-Solomon error correction codes, the Wikiversity article is a good beginner's introduction.
-
-------------------------------------
-
-.. contents:: Table of contents
-   :backlinks: top
-   :local:
-
-
-Installation
-------------
-
-For the latest stable release, install with:
-
-.. code:: sh
-
-    pip install --upgrade reedsolo
-
-For the latest development release (do not use in production!), use:
-
-.. code:: sh
-
-    pip install --upgrade git+https://github.com/tomerfiliba/reedsolomon
-
-If you have some issues installing through pip, maybe this command may help:
-
-.. code:: sh
-
-    pip install reedsolo --no-binary={reedsolo}
-
-By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0b2) and a C++ compiler, a faster cythonized binary can be optionally built with:
-    
-.. code:: sh
-
-    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose
-    
-or locally with:
-
-.. code:: sh
-
-    python setup.py install --cythonize  # if cython >= 3.0.0b2 is already installed
-    pip install .[cythonize] --install-option="--cythonize" --verbose  # if cython is not installed
-
-or with pep517 ``build`` tool:
-
-.. code:: sh
-
-    pip install build
-    python -sBm build -w --no-isolation -C=--build-option=--cythonize
-    # or
-    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose --use-pip517
-
-The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
-
-As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
-
-.. code:: sh
-
-    conda install -c conda-forge reedsolo
-
-Usage
------
-
-Basic usage with high-level RSCodec class
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    # Initialization
-    >>> from reedsolo import RSCodec, ReedSolomonError
-    >>> rsc = RSCodec(10)  # 10 ecc symbols
-
-    # Encoding
-    # just a list of numbers/symbols:
-    >>> rsc.encode([1,2,3,4])
-    b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M'
-    # bytearrays are accepted and the output will be matched:
-    >>> rsc.encode(bytearray([1,2,3,4]))
-    bytearray(b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M')
-    # encoding a byte string is as easy:
-    >>> rsc.encode(b'hello world')
-    b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa'
-    # Note: strings of any length, even if longer than the Galois field, will be encoded as well using transparent chunking.
-
-    # Decoding (repairing)
-    >>> rsc.decode(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')[0]  # original
-    b'hello world'
-    >>> rsc.decode(b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 3 errors
-    b'hello world'
-    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 5 errors
-    b'hello world'
-    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdXX\xf3\xa8\xaa')[0]        # 6 errors - fail
-    Traceback (most recent call last):
-      ...
-    reedsolo.ReedSolomonError: Too many (or few) errors found by Chien Search for the errata locator polynomial!
-
-**Important upgrade notice for pre-1.0 users:** Note that ``RSCodec.decode()`` returns 3 variables:
-
-    1. the decoded (corrected) message
-    2. the decoded message and error correction code (which is itself also corrected)
-    3. and the list of positions of the errata (errors and erasures)
-
-Here is how to use these outputs:
-
-.. code:: python
-
-    >>> tampered_msg = b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa'
-    >>> decoded_msg, decoded_msgecc, errata_pos = rsc.decode(tampered_msg)
-    >>> print(decoded_msg)  # decoded/corrected message
-    bytearray(b'hello world')
-    >>> print(decoded_msgecc)  # decoded/corrected message and ecc symbols
-    bytearray(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')
-    >>> print(errata_pos)  # errata_pos is returned as a bytearray, hardly intelligible
-    bytearray(b'\x10\t\x02')
-    >>> print(list(errata_pos))  # convert to a list to get the errata positions as integer indices
-    [16, 9, 2]
-
-Since we failed to decode with 6 errors with a codec set with 10 error correction code (ecc) symbols, let's try to use a bigger codec, with 12 ecc symbols.
-
-.. code:: python
-
-    >>> rsc = RSCodec(12)  # using 2 more ecc symbols (to correct max 6 errors or 12 erasures)
-    >>> rsc.encode(b'hello world')
-    b'hello world?Ay\xb2\xbc\xdc\x01q\xb9\xe3\xe2='
-    >>> rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')[0]         # 6 errors - ok, but any more would fail
-    b'hello world'
-    >>> rsc.decode(b'helXXXXXXXXXXy\xb2XX\x01q\xb9\xe3\xe2=', erase_pos=[3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16])[0]  # 12 erasures - OK
-    b'hello world'
-
-This shows that we can decode twice as many erasures (where we provide the location of errors ourselves) than errors (with unknown locations). This is the cost of error correction compared to erasure correction.
-
-To get the maximum number of errors *or* erasures that can be independently corrected (ie, not simultaneously):
-
-.. code:: python
-
-    >>> maxerrors, maxerasures = rsc.maxerrata(verbose=True)
-    This codec can correct up to 6 errors and 12 erasures independently
-    >>> print(maxerrors, maxerasures)
-    6 12
-
-To get the maximum number of errors *and* erasures that can be simultaneously corrected, you need to specify the number of errors or erasures you expect:
-
-.. code:: python
-
-    >>> maxerrors, maxerasures = rsc.maxerrata(erasures=6, verbose=True)  # we know the number of erasures, will calculate how many errors we can afford
-    This codec can correct up to 3 errors and 6 erasures simultaneously
-    >>> print(maxerrors, maxerasures)
-    3 6
-    >>> maxerrors, maxerasures = rsc.maxerrata(errors=5, verbose=True)  # we know the number of errors, will calculate how many erasures we can afford
-    This codec can correct up to 5 errors and 2 erasures simultaneously
-    >>> print(maxerrors, maxerasures)
-    5 2
-
-Note that if a chunk has more errors and erasures than the Singleton Bound as calculated by the ``maxerrata()`` method, the codec will try to raise a ``ReedSolomonError`` exception,
-but may very well not detect any error either (this is a theoretical limitation of error correction codes). In other words, error correction codes are unreliable to detect if a chunk of a message
-is corrupted beyond the Singleton Bound. If you want more reliability in errata detection, use a checksum or hash such as SHA or MD5 on your message, these are much more reliable and have no bounds
-on the number of errata (the only potential issue is with collision but the probability is very very low).
-
-Note: to catch a ``ReedSolomonError`` exception, do not forget to import it first with: ``from reedsolo import ReedSolomonError``
-
-To check if a message is tampered given its error correction symbols, without decoding, use the ``check()`` method:
-
-.. code:: python
-
-    # Checking
-    >> rsc.check(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')  # Tampered message will return False
-    [False]
-    >> rmes, rmesecc, errata_pos = rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')
-    >> rsc.check(rmesecc)  # Corrected or untampered message will return True
-    [True]
-    >> print('Number of detected errors and erasures: %i, their positions: %s' % (len(errata_pos), list(errata_pos)))
-    Number of detected errors and erasures: 6, their positions: [16, 15, 12, 11, 10, 9]
-
-By default, most Reed-Solomon codecs are limited to characters that can be encoded in 256 bits and with a length of maximum 256 characters. But this codec is universal, you can reduce or increase the length and maximum character value by increasing the Galois Field:
-
-.. code:: python
-
-    # To use longer chunks or bigger values than 255 (may be very slow)
-    >> rsc = RSCodec(12, nsize=4095)  # always use a power of 2 minus 1
-    >> rsc = RSCodec(12, c_exp=12)  # alternative way to set nsize=4095
-    >> mes = 'a' * (4095-12)
-    >> mesecc = rsc.encode(mes)
-    >> mesecc[2] = 1
-    >> mesecc[-1] = 1
-    >> rmes, rmesecc, errata_pos = rsc.decode(mesecc)
-    >> rsc.check(mesecc)
-    [False]
-    >> rsc.check(rmesecc)
-    [True]
-
-Note that the ``RSCodec`` class supports transparent chunking, so you don't need to increase the Galois Field to support longer messages, but characters will still be limited to 256 bits (or
-whatever field you set with ``c_exp``).
-
-If you need to use a variable number of error correction symbols (i.e., akin to variable bitrate in videos encoding), this is possible always possible using `RSCodec.decode(nsym=x)` and at encoding by setting `RSCodec(nsym=y, single_gen=False)` and then `RSCodec.encode(nsym=x)`.
-
-Low-level usage via direct access to math functions
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-If you want full control, you can skip the API and directly use the library as-is. Here's how:
-
-First you need to init the precomputed tables:
-
-.. code:: python
-
-    >> import reedsolo as rs
-    >> rs.init_tables(0x11d)
-
-Pro tip: if you get the error: ValueError: byte must be in range(0, 256), please check that your prime polynomial is correct for your field.
-Pro tip2: by default, you can only encode messages of max length and max symbol value = 256. If you want to encode bigger messages,
-please use the following (where c_exp is the exponent of your Galois Field, eg, 12 = max length 2^12 = 4096):
-
-.. code:: python
-
-    >> prim = rs.find_prime_polys(c_exp=12, fast_primes=True, single=True)[0]
-    >> rs.init_tables(c_exp=12, prim=prim)
-    
-Let's define our RS message and ecc size:
-
-.. code:: python
-
-    >> n = 255  # length of total message+ecc
-    >> nsym = 12  # length of ecc
-    >> mes = "a" * (n-nsym)  # generate a sample message
-
-To optimize, you can precompute the generator polynomial:
-
-.. code:: python
-
-    >> gen = rs.rs_generator_poly_all(n)
-
-Then to encode:
-
-.. code:: python
-
-    >> mesecc = rs.rs_encode_msg(mes, nsym, gen=gen[nsym])
-
-Let's tamper our message:
-
-.. code:: python
-
-    >> mesecc[1] = 0
-
-To decode:
-
-.. code:: python
-
-    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym, erase_pos=erase_pos)
-
-Note that both the message and the ecc are corrected (if possible of course).
-Pro tip: if you know a few erasures positions, you can specify them in a list ``erase_pos`` to double the repair power. But you can also just specify an empty list.
-
-You can check how many errors and/or erasures were corrected, which can be useful to design adaptive bitrate algorithms:
-
-.. code:: python
-
-    >> print('A total of %i errata were corrected over all chunks of this message.' % len(errata_pos))
-
-If the decoding fails, it will normally automatically check and raise a ReedSolomonError exception that you can handle.
-However if you want to manually check if the repaired message is correct, you can do so:
-
-.. code:: python
-
-    >> rs.rs_check(rmes + recc, nsym)
-
-Note: if you want to use multiple reedsolomon with different parameters, you need to backup the globals and restore them before calling reedsolo functions:
-
-.. code:: python
-
-    >> rs.init_tables()
-    >> global gf_log, gf_exp, field_charac
-    >> bak_gf_log, bak_gf_exp, bak_field_charac = gf_log, gf_exp, field_charac
-
-
-Then at anytime, you can do:
-
-.. code:: python
-
-    >> global gf_log, gf_exp, field_charac
-    >> gf_log, gf_exp, field_charac = bak_gf_log, bak_gf_exp, bak_field_charac
-    >> mesecc = rs.rs_encode_msg(mes, nsym)
-    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym)
-
-The globals backup is not necessary if you use RSCodec, it will be automatically managed.
-
-Read the sourcecode's comments for more info about how it works, and for the various parameters you can setup if
-you need to interface with other RS codecs.
-
-Extended description
---------------------
-The code of wikiversity is here consolidated into a nice API with exceptions handling.
-The algorithm can correct up to ``2*e+v <= nsym``, where ``e`` is the number of errors,
-``v`` the number of erasures and ``nsym = n-k`` = the number of ECC (error correction code) symbols.
-This means that you can either correct exactly ``floor(nsym/2)`` errors, or ``nsym`` erasures
-(errors where you know the position), and a combination of both errors and erasures.
-This is called the Singleton Bound, and is the maximum/optimal theoretical number
-of erasures and errors any error correction algorithm can correct (although there
-are experimental approaches to go a bit further, named list decoding, not implemented
-here, but feel free to do pull request!).
-
-The code should work on pretty much any reasonable version of python (3.7+),
-but I'm only testing on the latest Python version available on Anaconda at the moment (currently 3.10),
-although there is a unit test on various Python versions to ensure retrocompatibility.
-
-This library is also thoroughly unit tested with branch coverage,
-so that nearly any encoding/decoding case should be covered.
-The unit test includes Cython and PyPy too.
-On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
-thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
-another project using reedsolo for the practical application of on-storage data protection, and which includes
-a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
-
-The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
-as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
-hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
-
-Note however that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
-we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
-Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
-your messages, the quadratically longer it will take to encode/decode!
-
-The algorithm itself can handle messages of a length up to ``(2^c_exp)-1`` symbols per message (or chunk), including the ECC symbols,
-and each symbol can have a value of up to ``(2^c_exp)-1`` (indeed, both the message length and the maximum
-value for one character is constrained by the same mathematical reason). By default, we use the field ``GF(2^8)``,
-which means that you are limited to values between 0 and 255 (perfect to represent a single hexadecimal
-symbol on computers, so you can encode any binary stream) and limited to messages+ecc of maximum
-length 255. However, you can "chunk" longer messages to fit them into the message length limit.
-The ``RSCodec`` class will automatically apply chunking, by splitting longer messages into chunks and
-encode/decode them separately; it shouldn't make a difference from an API perspective (ie, from your POV).
-
-Speed optimizations
--------------------
-
-Thanks to using ``bytearray`` and a functional approach (contrary to unireedsolomon, a sibling implementation), the codec
-has quite reasonable performances despite avoiding hardcoding constants and specific instruction sets optimizations that
-are not mathematically generalizable (and so we avoid them, as we want to try to remain as close to the mathematical formulations as possible).
-
-In particular, good speed performance at encoding can be obtained by using either PyPy JIT Compiler on the pure-python
-implementation (reedsolo.py) or either by compiling the Cython extension creedsolo.pyx (which is much more optimized and hence much faster than PyPy).
-
-From our speed tests, encoding rates of several MB/s can be expected with PyPy JIT,
-and 14.3 MB/s using the Cython extension creedsolo on an Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz
-(benchmarked with `pyFileFixity's ecc_speedtest.py <https://github.com/lrq3000/pyFileFixity/blob/master/pyFileFixity/ecc_speedtest.py>`_).
-
-Decoding remains much slower, and less optimized, but more complicated to do so. However, the rationale to focus optimization efforts primarily on encoding and not decoding
-is that users are more likely to spend most of their processing time encoding data, and much less decoding, as encoding needs to be done indiscriminately apriori to protect data,
-whereas decoding happens only aposteriori on data that the user knows is tampered, so this is a much reduced subset of all the protected data (hopefully).
-
-To use the Cython implementation, it is necessary to ``pip install cython==3.0.0b2`` and to install a C++ compiler (Microsoft Visual C++ 14.x for Windows and Python 3.10+), read the up-to-date instructions in the `official wiki <https://wiki.python.org/moin/WindowsCompilers>`_. Then simply ``cd`` to the root of the folder where creedsolo.pyx is, and type ``python setup.py build_ext --inplace --cythonize``. Alternatively, it is possible to generate just the C++ code by typing ``cython -3 creedsolo.pyx``. When building a distributable egg or installing the module from source, the Cython module can be transpiled and compiled if both Cython and a C compiler are installed and the ``--cythonize`` flag is supplied to the setup.py, otherwise by default only the pure-python implementation and the ``.pyx`` cython source code will be included, but the binary won't be in the wheel.
-
-Then, use ``from creedsolo import RSCodec`` instead of importing from the ``reedsolo`` module, and finally only feed ``bytearray()`` objects to the `RSCodec` object. Exclusively using bytearrays is one of the reasons creedsolo is faster than reedsolo. You can convert any string by specifying the encoding: ``bytearray("Hello World", "UTF-8")``.
-
-Note that there is an inherent limitation of the C implementation which cannot work with higher galois fields than 8 (= characters of max 255 value) because the C implementation only works with bytearrays, and bytearrays only support characters up to 255. If you want to use higher galois fields, you need to use the pure python version, which includes a fake ``_bytearray`` function that overloads the standard bytearray with an ``array.array("i", ...)`` in case galois fields higher than 8 are used to ``init_tables()``, or rewrite the C implementation to use lists instead of bytearrays (which will be MUCH slower so this defeats the purpose and you are better off simply using the pure python version under PyPy - an older version of the C implementation was doing just that, and without bytearrays, all performance gains were lost, hence why the bytearrays were kept despite the limitations).
-
-Edge cases
--------------
-
-Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
-
-* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
-
-* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
-
-Migration from v1.x to v2.x
----------------------------
-
-If you used ``reedsolo`` v1.x, then to upgrade to v2.x, a few changes in the API must be considered.
-
-We will not list everything here, but the biggest breaking change is that now internally, everything is either a ``bytearray``, or a CPython ``array('i', ...)``.
-
-For the pure python implementation ``reedsolo``, this should not change much, it should be retrocompatible with lists (there are a few checks in place to autodetect and convert lists into bytearrays whenever necessary - but only in RSCodec, not in lower level functions if that's what you used!).
-
-However, for the cythonized extension ``creedsolo``, these changes are breaking compatibility with v1.x: if you used ``bytearray`` everywhere whenever supplying a list of values into ``creedsolo`` (both for the ``data`` and ``erasures_pos``), then all is well, you are good to go! On the other hand, if you used ``list`` objects or other types in some places, you are in for some errors.
-
-The good news is that, thanks to these changes, both implementations are much faster, but especially ``creedsolo``, which now encodes at a rate of ``15-20 MB/s`` (yes that's BYTES, not bits!). This however requires Cython >= 3.0.0b2, and is incompatible with Python 2 (the pure python ``reedsolo`` is still compatible, but not the cythonized extension ``creedsolo``).
-
-In practice, there is likely very little you need to change, just add a few ``bytearray()`` calls here and there. For a practical example of what was required to migrate, see `the commits for pyFileFixity migration <https://github.com/lrq3000/pyFileFixity/compare/47407b73dfbcfe34970055524655e21ccf2979aa..23b8f6f6c6f252fb9a641f419a6bfa5a1e6c3343>`_.
-
-Recommended reading
--------------------
-
-* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
-* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
-
-Authors
--------
-
-This module was conceived and developed by Tomer Filiba in 2012.
-
-It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
-
-And several other contributors helped improve and make it more robust:
-
-|Contributors|
-
-For a list of all contributors, please see `the GitHub Contributors graph <https://github.com/tomerfiliba/reedsolomon/graphs/contributors>`_ and the `commits history <https://github.com/tomerfiliba/reedsolomon/commits/master>`_.
-
-License
--------
-
-This software is released under your choice of the Unlicense or the MIT-0 (MIT No Attribution) License. Both licenses are `public-domain-equivalent licenses <https://en.wikipedia.org/wiki/Public-domain-equivalent_license>`_, as intended by the original author Tomer Filiba.
-
-
-.. |PyPI-Status| image:: https://img.shields.io/pypi/v/reedsolo.svg
-   :target: https://pypi.org/project/reedsolo
-.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/reedsolo.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/reedsolo
-.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/reedsolo.svg?label=pypi%20downloads&logo=python&logoColor=white
-   :target: https://pypi.org/project/reedsolo
-.. |Build-Status| image:: https://github.com/tomerfiliba/reedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
-    :target: https://github.com/tomerfiliba/reedsolomon/actions/workflows/ci-build.yml
-.. |Coverage| image:: https://coveralls.io/repos/tomerfiliba/reedsolomon/badge.svg?branch=master&service=github
-  :target: https://coveralls.io/github/tomerfiliba/reedsolomon?branch=master
-.. |Conda-Forge-Status| image:: https://img.shields.io/conda/vn/conda-forge/reedsolo.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Conda-Forge-Platforms| image:: https://anaconda.org/conda-forge/reedsolo/badges/platforms.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Conda-Forge-Downloads| image:: https://anaconda.org/conda-forge/reedsolo/badges/downloads.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Contributors| image:: https://contrib.rocks/image?repo=tomerfiliba/reedsolomon
-   :target: https://github.com/tomerfiliba/reedsolomon/graphs/contributors
+Reed Solomon
+============
+
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
+
+|Build-Status| |Coverage|
+
+|Conda-Forge-Status| |Conda-Forge-Platforms| |Conda-Forge-Downloads|
+
+⏳🛡 Pythonic universal errors-and-erasures `Reed-Solomon encoder/decoder codec <http://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction>`_ to protect your data from errors and bitrot. Includes a future-proof zero-dependencies pure-python implementation 🔮 as well as an optional speed-optimized Cython/C extension 🚀
+
+This is a burst-type implementation, so that it supports any Galois field higher than 2^3, but not binary streams. Burst errors are non-random errors that more often happen on data storage mediums such as hard drives, hence this library is better suited for data storage protection, and less for streams noise correction, although it also works for this purpose but with a bit of overhead (since it works with bytes only, instead of bits).
+
+Based on the wonderful tutorial at `Wikiversity <http://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_, written by "Bobmath" and "LRQ3000". If you are just starting with Reed-Solomon error correction codes, the Wikiversity article is a good beginner's introduction.
+
+------------------------------------
+
+.. contents:: Table of contents
+   :backlinks: top
+   :local:
+
+
+Installation
+------------
+
+For the latest stable release (compatible with Python >= 3.7), install with:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo
+
+For the latest development release, use:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo --pre
+
+For the cutting-edge code (likely unstable, do not use in production!), use:
+
+.. code:: sh
+
+    pip install --upgrade git+https://github.com/tomerfiliba-org/reedsolomon
+
+If you have some issues installing through pip, maybe this command may help:
+
+.. code:: sh
+
+    pip install reedsolo --no-binary={reedsolo}
+
+Note: for Python 2.7 and Python <= 3.6, please use v1.7.0:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo==1.7.0
+
+Through wheels/pip, a pure-python implementation called ``reedsolo`` is installed, and for platforms supported by ``cibuildwheel``, a precompiled speed-optimized ``creedsolo`` module is included. For other platforms or to compile from source (this requires ``cython>=3.0.0b2`` and a C compiler), a build option can be specified:
+
+.. code:: sh
+
+    # To compile from the latest stable release:
+    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --verbose
+    # To compile from the latest development release:
+    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
+    # To compile from the cutting edge code:
+    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
+
+The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension.
+    
+or locally with:
+
+.. code:: sh
+
+    pip install --upgrade . --config-setting="--build-option=--cythonize" --verbose
+
+Note: for development, it's possible to add the ``--editable`` flag to use the local folder without installing in ``site-packages``,
+and use ``.[test]`` instead of ``.`` to install all required packages to test this module locally.
+
+The package for the development or cutting-edge releases can also be built locally with the pep517 compliant ``build`` tool:
+
+.. code:: sh
+
+    pip install build
+    # With cythonization (from *.pyx to *.c to *.pyd)
+    python -sBm build --config-setting="--build-option=--cythonize"
+    # or skip cythonization and only compile from the already transpiled c extension (from *.c to *.pyd)
+    python -sBm build --config-setting="--build-option=--native-compile"
+
+The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
+
+As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
+
+.. code:: sh
+
+    conda install -c conda-forge reedsolo
+
+Various Linux distributions builds are also available, thanks to a network of amazing maintainers:
+
+|dl-gentoo| |dl-debian| |dl-fedora| |dl-archlinux|
+|dl-alpine| |dl-altlinux| |dl-linux-others|
+
+Usage
+-----
+
+Basic usage with high-level RSCodec class
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    # Initialization
+    >>> from reedsolo import RSCodec, ReedSolomonError
+    >>> rsc = RSCodec(10)  # 10 ecc symbols
+
+    # Encoding
+    # just a list of numbers/symbols:
+    >>> rsc.encode([1,2,3,4])
+    b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M'
+    # bytearrays are accepted and the output will be matched:
+    >>> rsc.encode(bytearray([1,2,3,4]))
+    bytearray(b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M')
+    # encoding a byte string is as easy:
+    >>> rsc.encode(b'hello world')
+    b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa'
+
+Note: strings of any length, even if longer than the Galois field, will be encoded as well using transparent chunking.
+
+Note2: it is strongly recommended to always use bytearrays. Using encoded strings is accepted by the RSCodec API, as
+a convenient facility for neophytes, but encodings such as ``UTF-8`` have variable lengths, so internally the module has
+to convert to a bytearray. If you just want to protect a string, you do not need to use a ``bytearray``, but if you need
+to store or send the protected data in a fixed size field, such as in a binary file or a data stream, use a ``bytearray``.
+
+    # Decoding (repairing)
+    >>> rsc.decode(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')[0]  # original
+    b'hello world'
+    >>> rsc.decode(b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 3 errors
+    b'hello world'
+    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 5 errors
+    b'hello world'
+    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdXX\xf3\xa8\xaa')[0]        # 6 errors - fail
+    Traceback (most recent call last):
+    ...
+    reedsolo.ReedSolomonError: Too many (or few) errors found by Chien Search for the errata locator polynomial!
+
+**Important upgrade notice for pre-1.0 users:** Note that ``RSCodec.decode()`` returns 3 variables:
+
+    1. the decoded (corrected) message
+    2. the decoded message and error correction code (which is itself also corrected)
+    3. and the list of positions of the errata (errors and erasures)
+
+Here is how to use these outputs:
+
+    >>> tampered_msg = b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa'
+    >>> decoded_msg, decoded_msgecc, errata_pos = rsc.decode(tampered_msg)
+    >>> print(decoded_msg)  # decoded/corrected message
+    bytearray(b'hello world')
+    >>> print(decoded_msgecc)  # decoded/corrected message and ecc symbols
+    bytearray(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')
+    >>> print(errata_pos)  # errata_pos is returned as a bytearray, hardly intelligible
+    bytearray(b'\x10\t\x02')
+    >>> print(list(errata_pos))  # convert to a list to get the errata positions as integer indices
+    [16, 9, 2]
+
+Since we failed to decode with 6 errors with a codec set with 10 error correction code (ecc) symbols, let's try to use a bigger codec, with 12 ecc symbols.
+
+    >>> rsc = RSCodec(12)  # using 2 more ecc symbols (to correct max 6 errors or 12 erasures)
+    >>> rsc.encode(b'hello world')
+    b'hello world?Ay\xb2\xbc\xdc\x01q\xb9\xe3\xe2='
+    >>> rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')[0]         # 6 errors - ok, but any more would fail
+    b'hello world'
+    >>> rsc.decode(b'helXXXXXXXXXXy\xb2XX\x01q\xb9\xe3\xe2=', erase_pos=[3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16])[0]  # 12 erasures - OK
+    b'hello world'
+
+This shows that we can decode twice as many erasures (where we provide the location of errors ourselves) than errors (with unknown locations). This is the cost of error correction compared to erasure correction.
+
+To get the maximum number of errors *or* erasures that can be independently corrected (ie, not simultaneously):
+
+    >>> maxerrors, maxerasures = rsc.maxerrata(verbose=True)
+    This codec can correct up to 6 errors and 12 erasures independently
+    >>> print(maxerrors, maxerasures)
+    6 12
+
+To get the maximum number of errors *and* erasures that can be simultaneously corrected, you need to specify the number of errors or erasures you expect:
+
+    >>> maxerrors, maxerasures = rsc.maxerrata(erasures=6, verbose=True)  # we know the number of erasures, will calculate how many errors we can afford
+    This codec can correct up to 3 errors and 6 erasures simultaneously
+    >>> print(maxerrors, maxerasures)
+    3 6
+    >>> maxerrors, maxerasures = rsc.maxerrata(errors=5, verbose=True)  # we know the number of errors, will calculate how many erasures we can afford
+    This codec can correct up to 5 errors and 2 erasures simultaneously
+    >>> print(maxerrors, maxerasures)
+    5 2
+
+Note that if a chunk has more errors and erasures than the Singleton Bound as calculated by the ``maxerrata()`` method, the codec will try to raise a ``ReedSolomonError`` exception,
+but may very well not detect any error either (this is a theoretical limitation of error correction codes). In other words, error correction codes are unreliable to detect if a chunk of a message
+is corrupted beyond the Singleton Bound. If you want more reliability in errata detection, use a checksum or hash such as SHA or MD5 on your message, these are much more reliable and have no bounds
+on the number of errata (the only potential issue is with collision but the probability is very very low).
+
+Note: to catch a ``ReedSolomonError`` exception, do not forget to import it first with: ``from reedsolo import ReedSolomonError``
+
+To check if a message is tampered given its error correction symbols, without decoding, use the ``check()`` method:
+
+    # Checking
+    >> rsc.check(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')  # Tampered message will return False
+    [False]
+    >> rmes, rmesecc, errata_pos = rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')
+    >> rsc.check(rmesecc)  # Corrected or untampered message will return True
+    [True]
+    >> print('Number of detected errors and erasures: %i, their positions: %s' % (len(errata_pos), list(errata_pos)))
+    Number of detected errors and erasures: 6, their positions: [16, 15, 12, 11, 10, 9]
+
+By default, most Reed-Solomon codecs are limited to characters that can be encoded in 256 bits and with a length of maximum 256 characters. But this codec is universal, you can reduce or increase the length and maximum character value by increasing the Galois Field:
+
+    # To use longer chunks or bigger values than 255 (may be very slow)
+    >> rsc = RSCodec(12, nsize=4095)  # always use a power of 2 minus 1
+    >> rsc = RSCodec(12, c_exp=12)  # alternative way to set nsize=4095
+    >> mes = 'a' * (4095-12)
+    >> mesecc = rsc.encode(mes)
+    >> mesecc[2] = 1
+    >> mesecc[-1] = 1
+    >> rmes, rmesecc, errata_pos = rsc.decode(mesecc)
+    >> rsc.check(mesecc)
+    [False]
+    >> rsc.check(rmesecc)
+    [True]
+
+Note that the ``RSCodec`` class supports transparent chunking, so you don't need to increase the Galois Field to support longer messages, but characters will still be limited to 256 bits (or
+whatever field you set with ``c_exp``).
+
+If you need to use a variable number of error correction symbols (i.e., akin to variable bitrate in videos encoding), this is possible always possible using `RSCodec.decode(nsym=x)` and at encoding by setting `RSCodec(nsym=y, single_gen=False)` and then `RSCodec.encode(nsym=x)`.
+
+Low-level usage via direct access to math functions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you want full control, you can skip the API and directly use the library as-is. Here's how:
+
+First you need to init the precomputed tables:
+
+    >> import reedsolo as rs
+    >> rs.init_tables(0x11d)
+
+Pro tip: if you get the error: ValueError: byte must be in range(0, 256), please check that your prime polynomial is correct for your field.
+Pro tip2: by default, you can only encode messages of max length and max symbol value = 256. If you want to encode bigger messages,
+please use the following (where c_exp is the exponent of your Galois Field, eg, 12 = max length 2^12 = 4096):
+
+    >> prim = rs.find_prime_polys(c_exp=12, fast_primes=True, single=True)[0]
+    >> rs.init_tables(c_exp=12, prim=prim)
+    
+Let's define our RS message and ecc size:
+
+    >> n = 255  # length of total message+ecc
+    >> nsym = 12  # length of ecc
+    >> mes = "a" * (n-nsym)  # generate a sample message
+
+To optimize, you can precompute the generator polynomial:
+
+    >> gen = rs.rs_generator_poly_all(n)
+
+Note: this generates the generator polynomial for all possible `nsym`,
+so this can easily be used for variable encoding rate.
+
+Then to encode:
+
+    >> mesecc = rs.rs_encode_msg(mes, nsym, gen=gen[nsym])
+
+Let's tamper our message:
+
+    >> mesecc[1] = 0
+
+To decode:
+
+    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym, erase_pos=erase_pos)
+
+Note that both the message and the ecc are corrected (if possible of course).
+Pro tip: if you know a few erasures positions, you can specify them in a list ``erase_pos`` to double the repair power. But you can also just specify an empty list.
+
+You can check how many errors and/or erasures were corrected, which can be useful to design adaptive bitrate algorithms:
+
+    >> print('A total of %i errata were corrected over all chunks of this message.' % len(errata_pos))
+
+If the decoding fails, it will normally automatically check and raise a ReedSolomonError exception that you can handle.
+However if you want to manually check if the repaired message is correct, you can do so:
+
+    >> rs.rs_check(rmes + recc, nsym)
+
+Note: if you want to use multiple reedsolomon with different parameters, you need to backup the globals and restore them before calling reedsolo functions:
+
+    >> rs.init_tables()
+    >> global gf_log, gf_exp, field_charac
+    >> bak_gf_log, bak_gf_exp, bak_field_charac = gf_log, gf_exp, field_charac
+
+
+Then at anytime, you can do:
+
+    >> global gf_log, gf_exp, field_charac
+    >> gf_log, gf_exp, field_charac = bak_gf_log, bak_gf_exp, bak_field_charac
+    >> mesecc = rs.rs_encode_msg(mes, nsym)
+    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym)
+
+The globals backup is not necessary if you use RSCodec, it will be automatically managed.
+
+The speed-optimized C extension ``creedsolo`` can be used similarly once compiled or cythonized:
+
+    >> import creedsolo as crs
+    >> codec = crs.RSCodec(10)
+
+If you want to ``cimport`` the module, you will need to directly access the full package path:
+
+    >> import cython
+    >> cimport cython
+    >> cimport creedsolo.creedsolo as crs
+
+Low-level functions allow to construct new APIs on top of this codec, such as
+`an automatic Reed-Solomon decoder <https://github.com/lrq3000/pyFileFixity/blob/0b18728608f2bceac9eafe5356e0abc573af2768/pyFileFixity/lib/eccman.py#L63>`_
+that can search for any viable set of codec parameters if they are apriori unknown.
+
+If you want to learn more about which internal functions to use and for what purposes,
+read the sourcecode's comments (we follow literate programming principles)
+for more info about how it works and the various parameters
+you can setup if you need to interface with other RS codecs.
+
+Extended description
+--------------------
+The code of wikiversity is here consolidated into a nice API with exceptions handling.
+The algorithm can correct up to ``2*e+v <= nsym``, where ``e`` is the number of errors,
+``v`` the number of erasures and ``nsym = n-k`` = the number of ECC (error correction code) symbols.
+This means that you can either correct exactly ``floor(nsym/2)`` errors, or ``nsym`` erasures
+(errors where you know the position), and a combination of both errors and erasures.
+This is called the Singleton Bound, and is the maximum/optimal theoretical number
+of erasures and errors any error correction algorithm can correct (although there
+are experimental approaches to go a bit further, named list decoding, not implemented
+here, but feel free to do pull request!).
+
+The code should work on pretty much any reasonable version of python (3.7+),
+but I'm only testing on the latest Python version available on Anaconda at the moment (currently 3.10),
+although there is a unit test on various Python versions to ensure retrocompatibility.
+
+This library is also thoroughly unit tested with branch coverage,
+so that nearly any encoding/decoding case should be covered.
+The unit test includes Cython and PyPy too.
+On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
+thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
+another project using reedsolo for the practical application of on-storage data protection, and which includes
+a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
+
+The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
+as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
+hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
+
+The work on this module is motivated by the aim to offer a solution for long-term archival of data, although this can and is also
+used for communication streams. For this purpose, this module is an ideal choice: Reed-Solomon is an optimal (non-quantic) algorithm,
+it corrects up to the Singleton Bound which is the absolute limit of how much erratas an error-correction algorithm can correct, RS
+is hence future-proof. The universality of this implementation further ensures that other future implementations of Reed-Solomon
+should be able to decode data encoded with this universal codec.
+
+Note that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
+we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
+Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
+your messages, the quadratically longer it will take to encode/decode!
+
+The algorithm itself can handle messages of a length up to ``(2^c_exp)-1`` symbols per message (or chunk), including the ECC symbols,
+and each symbol can have a value of up to ``(2^c_exp)-1`` (indeed, both the message length and the maximum
+value for one character is constrained by the same mathematical reason). By default, we use the field ``GF(2^8)``,
+which means that you are limited to values between 0 and 255 (perfect to represent a single hexadecimal
+symbol on computers, so you can encode any binary stream) and limited to messages+ecc of maximum
+length 255. However, you can "chunk" longer messages to fit them into the message length limit.
+The ``RSCodec`` class will automatically apply chunking, by splitting longer messages into chunks and
+encode/decode them separately; it shouldn't make a difference from an API perspective (ie, from your POV).
+
+Speed optimizations
+-------------------
+
+Thanks to using ``bytearray`` and a functional approach (contrary to unireedsolomon, a sibling implementation), the codec
+has quite reasonable performances despite avoiding hardcoding constants and specific instruction sets optimizations that
+are not mathematically generalizable (and so we avoid them, as we want to try to remain as close to the mathematical formulations as possible).
+
+In particular, good speed performance at encoding can be obtained by using either PyPy JIT Compiler on the pure-python
+implementation (reedsolo.py) or either by compiling the Cython extension creedsolo.pyx (which is much more optimized and hence much faster than PyPy).
+
+From our speed tests, encoding rates of several MB/s can be expected with PyPy JIT,
+and 14.3 MB/s using the Cython extension creedsolo on an Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz
+(benchmarked with `pyFileFixity's ecc_speedtest.py <https://github.com/lrq3000/pyFileFixity/blob/master/pyFileFixity/ecc_speedtest.py>`_).
+
+Decoding remains much slower, and less optimized, but more complicated to do so. However, the rationale to focus optimization efforts primarily on encoding and not decoding
+is that users are more likely to spend most of their processing time encoding data, and much less decoding, as encoding needs to be done indiscriminately apriori to protect data,
+whereas decoding happens only aposteriori on data that the user knows is tampered, so this is a much reduced subset of all the protected data (hopefully).
+
+To use the Cython implementation, it is necessary to ``pip install cython==3.0.0b2`` and to install a C++ compiler (Microsoft Visual C++ 14.x for Windows and Python 3.10+), read the up-to-date instructions in the `official wiki <https://wiki.python.org/moin/WindowsCompilers>`_. Then simply ``cd`` to the root of the folder where creedsolo.pyx is, and type ``python setup.py build_ext --inplace --cythonize``. Alternatively, it is possible to generate just the C++ code by typing ``cython -3 creedsolo.pyx``. When building a distributable egg or installing the module from source, the Cython module can be transpiled and compiled if both Cython and a C compiler are installed and the ``--cythonize`` flag is supplied to the setup.py, otherwise by default only the pure-python implementation and the ``.pyx`` cython source code will be included, but the binary won't be in the wheel.
+
+Then, use ``from creedsolo import RSCodec`` instead of importing from the ``reedsolo`` module, and finally only feed ``bytearray()`` objects to the `RSCodec` object. Exclusively using bytearrays is one of the reasons creedsolo is faster than reedsolo. You can convert any string by specifying the encoding: ``bytearray("Hello World", "UTF-8")``.
+
+Note that there is an inherent limitation of the C implementation which cannot work with higher galois fields than 8 (= characters of max 255 value) because the C implementation only works with bytearrays, and bytearrays only support characters up to 255. If you want to use higher galois fields, you need to use the pure python version, which includes a fake ``_bytearray`` function that overloads the standard bytearray with an ``array.array("i", ...)`` in case galois fields higher than 8 are used to ``init_tables()``, or rewrite the C implementation to use lists instead of bytearrays (which will be MUCH slower so this defeats the purpose and you are better off simply using the pure python version under PyPy - an older version of the C implementation was doing just that, and without bytearrays, all performance gains were lost, hence why the bytearrays were kept despite the limitations).
+
+Edge cases
+-------------
+
+Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
+
+* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
+
+* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
+
+Migration from v1.x to v2.x
+---------------------------
+
+If you used ``reedsolo`` v1.x, then to upgrade to v2.x, a few changes in the build requirements, the build system and API must be considered.
+
+One major change is that Cython>=v3.0.0b2 is required to cythonize ``creedsolo.pyx``. To ease migration for operating systems where python packages pre-releases are not available, the intermediary `creedsolo.c` is also shipped in the standard distribution (the `tar.gz` file) to allow compilation with any C compiler, without requiring Cython.
+
+Furthermore, the packaging system was overhauled to be PEP 517 standard compliant, so that it now supports build isolation by default, and it uses a src-layout.
+
+While we tried to keep the import API the same (you can still do ``import reedsolo as rs; codec = rs.RSCodec(10)`` and similarly ``import creedsolo as crs``. However, if you used to ``cimport creedsolo as crs`` using the fast c-import system provided by Cython, now you will need to ``cimport creedsolo.creedsolo as crs``.
+
+Indeed, for Linux distributions package maintainers, it's important to note the module is now using a `"src-layout" <https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure>`_, instead of the `"single-module-layout" <https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#single-module-distribution>`_ before, so this may require some adjustments in packages building processes.
+
+Furthermore, wheels with a precompiled ``creedsolo.pyd`` extension are now built for multiple platforms and Python releases and uploaded to PyPi, thanks to ``cibuildwheel``, and the process is automated with a GitHub Action. In future releases, we will try to improve on build reproducibility, such as by implementing a lockfile (but not there yet, there is no standard for that) and moving away from ``setuptools`` (potentially to ``meson``).
+
+Support for Python 2.7 and Python <= 3.6 was dropped as advised elsewhere, as only the pure python implementation remained retrocompatible, but not the cython extension, so that it is better for older Py2.7 users to simply stick to the fully functional reedsolo v1.7.0. For Python 3.6, support was dropped because these environments are not supported officially anymore by GitHub Actions, so it is harder to unit test and hence no guarantee of correctedness can be provided anymore in an automated fashion, so it's better to also use reedsolo v1.7.0 for these older Py3 versions.
+
+About API changes, a few bugfixes were implemented in the pure python implementation, but breaking changes were limited as much as possible (if there is any, it is unintended). For the `creedsolo` extension, there are LOTS of changes, hence why the major version change (we try to follow SemVer). We will not list everything here, but the biggest breaking change is that now internally, everything is either a ``bytearray``, or a CPython ``array('i', ...)``. So this means that when interacting with `creedsolo`, you want to **always** supply a `bytearray` object, you can't just provide a list or a string anymore. For `reedsolo`, this is still supported, since it transparently converts to a bytearray internally, for ease of use.
+
+For the pure python implementation ``reedsolo``, this should not change much, it should be retrocompatible with lists (there are a few checks in place to autodetect and convert lists into bytearrays whenever necessary - but only in RSCodec, not in lower level functions if that's what you used!).
+
+However, for the cythonized extension ``creedsolo``, these changes are breaking compatibility with v1.x: if you used ``bytearray`` everywhere whenever supplying a list of values into ``creedsolo`` (both for the ``data`` and ``erasures_pos``), then all is well, you are good to go! On the other hand, if you used ``list`` objects or other types in some places, you are in for some errors.
+
+The good news is that, thanks to these changes, both implementations are much faster, but especially ``creedsolo``, which now encodes at a rate of ``15-20 MB/s`` (yes that's BYTES, not bits!). This however requires Cython >= 3.0.0b2, and is incompatible with Python 2 (the pure python ``reedsolo`` is still compatible, but not the cythonized extension ``creedsolo``).
+
+In practice, there is likely very little you need to change, just add a few ``bytearray()`` calls here and there. For a practical example of what was required to migrate, see `the commits for pyFileFixity migration <https://github.com/lrq3000/pyFileFixity/compare/47407b73dfbcfe34970055524655e21ccf2979aa..23b8f6f6c6f252fb9a641f419a6bfa5a1e6c3343>`_.
+
+Projects using reedsolo
+-----------------------
+
+Reedsolo is a critical component of numerous solutions, such as:
+
+* `Matter (ex-Project CHIP) <https://github.com/project-chip/connectedhomeip>`_ - The new standard for the Internet of Things (IoT): Matter (formerly Project CHIP) creates more connections between more objects, simplifying development for manufacturers and increasing compatibility for consumers, guided by the Connectivity Standards Alliance.
+* `esp-idf <https://github.com/espressif/esp-idf>`_ - Espressif IoT Development Framework. Official development framework for Espressif SoCs, such as ESP32, which are very widespread reprogrammable electronic cheaps for scientific, prototype and DIY projects, especially with Arduino and MicroPython.
+* `esptool <https://github.com/espressif/esptool>`_ - A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+* `pyFileFixity <https://github.com/lrq3000/pyFileFixity>`_  - A suite of tools for long term archival of files.
+* `amodem <https://github.com/romanz/amodem>`_ - Audio MODEM Communication Library in Python, allowing true air-gapped communication (via a speaker and a microphone), or an audio cable (for higher transmission speed).
+* `SteganoGAN <https://github.com/DAI-Lab/SteganoGAN>`_ - SteganoGAN is a tool for creating steganographic images using adversarial training.
+* `galacteek <https://github.com/pinnaculum/galacteek>`_ - Multi-platform browser for the distributed web.
+* `ofrak <https://github.com/redballoonsecurity/ofrak>`_ - OFRAK (Open Firmware Reverse Analysis Konsole) is a binary analysis and modification platform.
+* `HoloCubic AIO <https://github.com/ClimbSnail/HoloCubic_AIO>`_ - All-in-One open-source firmware for the HoloCubic device with a wide features set.
+* `MicroPython-Stubber <https://github.com/Josverl/micropython-stubber>`_ - Boost MicroPython productivity in VSCode: Generate and use stubs for different micropython firmwares to use with vscode and pylance or pylint.
+* `qr-backup <https://github.com/za3k/qr-backup>`_ - Paper backup of files using QR codes.
+* `Jade <https://github.com/Blockstream/Jade>`_ - Jade Hardware Wallet.
+* `pied-piper <https://github.com/rraval/pied-piper>`_ - Defunct popular module for data transfer over sound waves.
+* `qreader <https://github.com/ewino/qreader>`_ - A defunct pure python QR code reader.
+* `sonicky <https://github.com/egglang/sonicky>`_ - Proof-of-concept Python and Android modules for connectionless ultrasonic message transfer.
+* `neighborhood-connectivity <https://github.com/shayyzhakov/neighborhood-connectivity>`_ - An example app that implements a noisy communication between clique of thread group with very high error correction handling ability and O(1) rounds of messages sending.
+* `audiotagger <https://github.com/NERVEUML/audiotagger>`_ - Clever use of error correction codes to wirelessly synchronize multiple concurrent video feeds of amateur video filmmakers by injecting AFSK packets with timestamp and location metadata in the audio channel communicated via radios.
+* Several research papers used reedsolo, see a list `here <https://scholar.google.com/scholar?q=%22reedsolo%22>`_.
+
+And many, many `more <https://github.com/tomerfiliba-org/reedsolomon/network/dependents>`_!
+
+Recommended reading
+-------------------
+
+* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
+* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
+* If you want a more mathematically transparent but less optimized implementation, read the sibling open-source project `unireedsolomon <https://github.com/lrq3000/unireedsolomon>`_, also co-authored by the maintainer of reedsolo, so that the codebase is very similar (although reedsolo is more mature and has more bugfixes - unireedsolomon should only be used for learning purposes!).
+
+Authors
+-------
+
+This module was conceived and developed by Tomer Filiba in 2012.
+
+It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
+
+And several other contributors helped improve and make it more robust, thanks a lot to them!
+
+|Contributors|
+
+For a list of all contributors, please see `the GitHub Contributors graph <https://github.com/tomerfiliba-org/reedsolomon/graphs/contributors>`_ and the `commits history <https://github.com/tomerfiliba-org/reedsolomon/commits/master>`_.
+
+License
+-------
+
+This software is released under your choice of the Unlicense or the MIT-0 (MIT No Attribution) License. Both licenses are `public-domain-equivalent licenses <https://en.wikipedia.org/wiki/Public-domain-equivalent_license>`_, as intended by the original author Tomer Filiba.
+
+
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/reedsolo.svg
+   :target: https://pypi.org/project/reedsolo
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/reedsolo.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/reedsolo
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/reedsolo.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/reedsolo
+.. |Build-Status| image:: https://github.com/tomerfiliba-org/reedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
+    :target: https://github.com/tomerfiliba-org/reedsolomon/actions/workflows/ci-build.yml
+.. |Coverage| image:: https://coveralls.io/repos/tomerfiliba-org/reedsolomon/badge.svg?branch=master&service=github
+  :target: https://coveralls.io/github/tomerfiliba-org/reedsolomon?branch=master
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/vn/conda-forge/reedsolo.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Conda-Forge-Platforms| image:: https://anaconda.org/conda-forge/reedsolo/badges/platforms.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Conda-Forge-Downloads| image:: https://anaconda.org/conda-forge/reedsolo/badges/downloads.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Contributors| image:: https://contrib.rocks/image?repo=tomerfiliba-org/reedsolomon
+   :target: https://github.com/tomerfiliba-org/reedsolomon/graphs/contributors
+
+.. |dl-gentoo| image:: https://img.shields.io/badge/Gentoo-54487A?logo=gentoo&logoColor=white
+   :target: https://packages.gentoo.org/packages/dev-python/reedsolomon
+   :alt: Package for Gentoo Linux, thanks to maintainer Michał Górny!
+.. |dl-debian| image:: https://img.shields.io/badge/Debian-D70A53?logo=debian&logoColor=white
+   :target: https://salsa.debian.org/python-team/packages/python-reedsolo/tree/debian/latest
+   :alt: Package for Debian Linux, thanks to maintainer Faidon Liambotis!
+.. |dl-archlinux| image:: https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff
+   :target: https://archlinux.org/packages/community/x86_64/python-reedsolo/
+   :alt: Package for Arch Linux, thanks to maintainer Jelle van der Waa!
+.. |dl-fedora| image:: https://img.shields.io/badge/Fedora-294172?logo=fedora&logoColor=white
+   :target: https://packages.fedoraproject.org/pkgs/python-reedsolo/python3-reedsolo/
+   :alt: Package for Fedora Linux, thanks to maintainer belegdol!
+.. |dl-alpine| image:: https://img.shields.io/badge/Alpine_Linux-%230D597F.svg?logo=alpine-linux&logoColor=white
+   :target: https://pkgs.alpinelinux.org/package/edge/community/x86/py3-reedsolo
+   :alt: Package for Alpine Linux, thanks to maintainer Michał Polański!
+.. |dl-altlinux| image:: https://img.shields.io/badge/Altlinux-yellow.svg
+   :target: https://packages.altlinux.org/en/sisyphus/srpms/python3-module-reedsolo/2902045385933595548
+   :alt: Package for ALT Linux, thanks to maintainer Sergey Bolshakov!
+.. |dl-linux-others| image:: https://img.shields.io/badge/Others-000000?logo=linux&logoColor=white
+   :target: https://pkgs.org/search/?q=reedsolo
+   :alt: List of packages for other Linux distributions
```

### Comparing `reedsolo-2.0.9/creedsolo.pyx` & `reedsolo-2.1.0b1/src/creedsolo/creedsolo.pyx`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.9/reedsolo.egg-info/PKG-INFO` & `reedsolo-2.1.0b1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,520 +1,608 @@
-Metadata-Version: 2.1
-Name: reedsolo
-Version: 2.0.9
-Summary: Pure-Python Universal Errors And Erasures Reed-Solomon Encoder and Decoder
-Author: Tomer Filiba
-Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
-Maintainer: Stephen Karl Larroque
-Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
-License: The software is available under your choice of
-        Unlicense (SPDX short identifier: Unlicense) or
-        MIT No Attribution License (SPDX short identifier: MIT-0):
-        
-        -----
-        
-        <<START OF UNLICENSE>>
-        This is free and unencumbered software released into the public domain.
-        
-        Anyone is free to copy, modify, publish, use, compile, sell, or
-        distribute this software, either in source code form or as a compiled
-        binary, for any purpose, commercial or non-commercial, and by any
-        means.
-        
-        In jurisdictions that recognize copyright laws, the author or authors
-        of this software dedicate any and all copyright interest in the
-        software to the public domain. We make this dedication for the benefit
-        of the public at large and to the detriment of our heirs and
-        successors. We intend this dedication to be an overt act of
-        relinquishment in perpetuity of all present and future rights to this
-        software under copyright law.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-        OTHER DEALINGS IN THE SOFTWARE.
-        
-        For more information, please refer to <http://unlicense.org/>
-        <<END OF UNLICENSE>>
-        
-        -----
-        
-        <<START OF MIT-0 LICENSE>>
-        Copyright 2013-2023 Tomer Filiba & Stephen Larroque
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        <<END OF MIT-0 LICENSE>>
-        
-Project-URL: Homepage, https://github.com/tomerfiliba/reedsolomon
-Project-URL: Documentation, https://github.com/tomerfiliba/reedsolomon/blob/master/README.rst
-Project-URL: Source, https://github.com/tomerfiliba/reedsolomon
-Project-URL: Tracker, https://github.com/tomerfiliba/reedsolomon/issues
-Project-URL: Download, https://github.com/tomerfiliba/reedsolomon/releases
-Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
-Project-URL: Gentoo, https://packages.gentoo.org/packages/dev-python/reedsolomon
-Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
-Platform: any
-Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Cython
-Classifier: Topic :: Communications
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Topic :: System :: Recovery Tools
-Requires-Python: >=2.7
-Description-Content-Type: text/x-rst
-Provides-Extra: cythonize
-License-File: LICENSE
-
-Reed Solomon
-============
-
-|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
-
-|Build-Status| |Coverage|
-
-|Conda-Forge-Status| |Conda-Forge-Platforms| |Conda-Forge-Downloads|
-
-A pythonic `universal errors-and-erasures Reed-Solomon Codec <http://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction>`_ to protect your data from errors and bitrot. It includes a pure python implementation and an optional speed-optimized Cython/C extension.
-
-This is a burst-type implementation, so that it supports any Galois field higher than 2^3, but not binary streams. Burst errors are non-random errors that more often happen on data storage mediums such as hard drives, hence this library is better suited for data storage protection, and less for streams noise correction, although it also works for this purpose but with a bit of overhead (since it works with bytes only, instead of bits).
-
-Based on the wonderful tutorial at `Wikiversity <http://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_, written by "Bobmath" and "LRQ3000". If you are just starting with Reed-Solomon error correction codes, the Wikiversity article is a good beginner's introduction.
-
-------------------------------------
-
-.. contents:: Table of contents
-   :backlinks: top
-   :local:
-
-
-Installation
-------------
-
-For the latest stable release, install with:
-
-.. code:: sh
-
-    pip install --upgrade reedsolo
-
-For the latest development release (do not use in production!), use:
-
-.. code:: sh
-
-    pip install --upgrade git+https://github.com/tomerfiliba/reedsolomon
-
-If you have some issues installing through pip, maybe this command may help:
-
-.. code:: sh
-
-    pip install reedsolo --no-binary={reedsolo}
-
-By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0b2) and a C++ compiler, a faster cythonized binary can be optionally built with:
-    
-.. code:: sh
-
-    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose
-    
-or locally with:
-
-.. code:: sh
-
-    python setup.py install --cythonize  # if cython >= 3.0.0b2 is already installed
-    pip install .[cythonize] --install-option="--cythonize" --verbose  # if cython is not installed
-
-or with pep517 ``build`` tool:
-
-.. code:: sh
-
-    pip install build
-    python -sBm build -w --no-isolation -C=--build-option=--cythonize
-    # or
-    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose --use-pip517
-
-The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
-
-As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
-
-.. code:: sh
-
-    conda install -c conda-forge reedsolo
-
-Usage
------
-
-Basic usage with high-level RSCodec class
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    # Initialization
-    >>> from reedsolo import RSCodec, ReedSolomonError
-    >>> rsc = RSCodec(10)  # 10 ecc symbols
-
-    # Encoding
-    # just a list of numbers/symbols:
-    >>> rsc.encode([1,2,3,4])
-    b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M'
-    # bytearrays are accepted and the output will be matched:
-    >>> rsc.encode(bytearray([1,2,3,4]))
-    bytearray(b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M')
-    # encoding a byte string is as easy:
-    >>> rsc.encode(b'hello world')
-    b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa'
-    # Note: strings of any length, even if longer than the Galois field, will be encoded as well using transparent chunking.
-
-    # Decoding (repairing)
-    >>> rsc.decode(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')[0]  # original
-    b'hello world'
-    >>> rsc.decode(b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 3 errors
-    b'hello world'
-    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 5 errors
-    b'hello world'
-    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdXX\xf3\xa8\xaa')[0]        # 6 errors - fail
-    Traceback (most recent call last):
-      ...
-    reedsolo.ReedSolomonError: Too many (or few) errors found by Chien Search for the errata locator polynomial!
-
-**Important upgrade notice for pre-1.0 users:** Note that ``RSCodec.decode()`` returns 3 variables:
-
-    1. the decoded (corrected) message
-    2. the decoded message and error correction code (which is itself also corrected)
-    3. and the list of positions of the errata (errors and erasures)
-
-Here is how to use these outputs:
-
-.. code:: python
-
-    >>> tampered_msg = b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa'
-    >>> decoded_msg, decoded_msgecc, errata_pos = rsc.decode(tampered_msg)
-    >>> print(decoded_msg)  # decoded/corrected message
-    bytearray(b'hello world')
-    >>> print(decoded_msgecc)  # decoded/corrected message and ecc symbols
-    bytearray(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')
-    >>> print(errata_pos)  # errata_pos is returned as a bytearray, hardly intelligible
-    bytearray(b'\x10\t\x02')
-    >>> print(list(errata_pos))  # convert to a list to get the errata positions as integer indices
-    [16, 9, 2]
-
-Since we failed to decode with 6 errors with a codec set with 10 error correction code (ecc) symbols, let's try to use a bigger codec, with 12 ecc symbols.
-
-.. code:: python
-
-    >>> rsc = RSCodec(12)  # using 2 more ecc symbols (to correct max 6 errors or 12 erasures)
-    >>> rsc.encode(b'hello world')
-    b'hello world?Ay\xb2\xbc\xdc\x01q\xb9\xe3\xe2='
-    >>> rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')[0]         # 6 errors - ok, but any more would fail
-    b'hello world'
-    >>> rsc.decode(b'helXXXXXXXXXXy\xb2XX\x01q\xb9\xe3\xe2=', erase_pos=[3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16])[0]  # 12 erasures - OK
-    b'hello world'
-
-This shows that we can decode twice as many erasures (where we provide the location of errors ourselves) than errors (with unknown locations). This is the cost of error correction compared to erasure correction.
-
-To get the maximum number of errors *or* erasures that can be independently corrected (ie, not simultaneously):
-
-.. code:: python
-
-    >>> maxerrors, maxerasures = rsc.maxerrata(verbose=True)
-    This codec can correct up to 6 errors and 12 erasures independently
-    >>> print(maxerrors, maxerasures)
-    6 12
-
-To get the maximum number of errors *and* erasures that can be simultaneously corrected, you need to specify the number of errors or erasures you expect:
-
-.. code:: python
-
-    >>> maxerrors, maxerasures = rsc.maxerrata(erasures=6, verbose=True)  # we know the number of erasures, will calculate how many errors we can afford
-    This codec can correct up to 3 errors and 6 erasures simultaneously
-    >>> print(maxerrors, maxerasures)
-    3 6
-    >>> maxerrors, maxerasures = rsc.maxerrata(errors=5, verbose=True)  # we know the number of errors, will calculate how many erasures we can afford
-    This codec can correct up to 5 errors and 2 erasures simultaneously
-    >>> print(maxerrors, maxerasures)
-    5 2
-
-Note that if a chunk has more errors and erasures than the Singleton Bound as calculated by the ``maxerrata()`` method, the codec will try to raise a ``ReedSolomonError`` exception,
-but may very well not detect any error either (this is a theoretical limitation of error correction codes). In other words, error correction codes are unreliable to detect if a chunk of a message
-is corrupted beyond the Singleton Bound. If you want more reliability in errata detection, use a checksum or hash such as SHA or MD5 on your message, these are much more reliable and have no bounds
-on the number of errata (the only potential issue is with collision but the probability is very very low).
-
-Note: to catch a ``ReedSolomonError`` exception, do not forget to import it first with: ``from reedsolo import ReedSolomonError``
-
-To check if a message is tampered given its error correction symbols, without decoding, use the ``check()`` method:
-
-.. code:: python
-
-    # Checking
-    >> rsc.check(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')  # Tampered message will return False
-    [False]
-    >> rmes, rmesecc, errata_pos = rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')
-    >> rsc.check(rmesecc)  # Corrected or untampered message will return True
-    [True]
-    >> print('Number of detected errors and erasures: %i, their positions: %s' % (len(errata_pos), list(errata_pos)))
-    Number of detected errors and erasures: 6, their positions: [16, 15, 12, 11, 10, 9]
-
-By default, most Reed-Solomon codecs are limited to characters that can be encoded in 256 bits and with a length of maximum 256 characters. But this codec is universal, you can reduce or increase the length and maximum character value by increasing the Galois Field:
-
-.. code:: python
-
-    # To use longer chunks or bigger values than 255 (may be very slow)
-    >> rsc = RSCodec(12, nsize=4095)  # always use a power of 2 minus 1
-    >> rsc = RSCodec(12, c_exp=12)  # alternative way to set nsize=4095
-    >> mes = 'a' * (4095-12)
-    >> mesecc = rsc.encode(mes)
-    >> mesecc[2] = 1
-    >> mesecc[-1] = 1
-    >> rmes, rmesecc, errata_pos = rsc.decode(mesecc)
-    >> rsc.check(mesecc)
-    [False]
-    >> rsc.check(rmesecc)
-    [True]
-
-Note that the ``RSCodec`` class supports transparent chunking, so you don't need to increase the Galois Field to support longer messages, but characters will still be limited to 256 bits (or
-whatever field you set with ``c_exp``).
-
-If you need to use a variable number of error correction symbols (i.e., akin to variable bitrate in videos encoding), this is possible always possible using `RSCodec.decode(nsym=x)` and at encoding by setting `RSCodec(nsym=y, single_gen=False)` and then `RSCodec.encode(nsym=x)`.
-
-Low-level usage via direct access to math functions
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-If you want full control, you can skip the API and directly use the library as-is. Here's how:
-
-First you need to init the precomputed tables:
-
-.. code:: python
-
-    >> import reedsolo as rs
-    >> rs.init_tables(0x11d)
-
-Pro tip: if you get the error: ValueError: byte must be in range(0, 256), please check that your prime polynomial is correct for your field.
-Pro tip2: by default, you can only encode messages of max length and max symbol value = 256. If you want to encode bigger messages,
-please use the following (where c_exp is the exponent of your Galois Field, eg, 12 = max length 2^12 = 4096):
-
-.. code:: python
-
-    >> prim = rs.find_prime_polys(c_exp=12, fast_primes=True, single=True)[0]
-    >> rs.init_tables(c_exp=12, prim=prim)
-    
-Let's define our RS message and ecc size:
-
-.. code:: python
-
-    >> n = 255  # length of total message+ecc
-    >> nsym = 12  # length of ecc
-    >> mes = "a" * (n-nsym)  # generate a sample message
-
-To optimize, you can precompute the generator polynomial:
-
-.. code:: python
-
-    >> gen = rs.rs_generator_poly_all(n)
-
-Then to encode:
-
-.. code:: python
-
-    >> mesecc = rs.rs_encode_msg(mes, nsym, gen=gen[nsym])
-
-Let's tamper our message:
-
-.. code:: python
-
-    >> mesecc[1] = 0
-
-To decode:
-
-.. code:: python
-
-    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym, erase_pos=erase_pos)
-
-Note that both the message and the ecc are corrected (if possible of course).
-Pro tip: if you know a few erasures positions, you can specify them in a list ``erase_pos`` to double the repair power. But you can also just specify an empty list.
-
-You can check how many errors and/or erasures were corrected, which can be useful to design adaptive bitrate algorithms:
-
-.. code:: python
-
-    >> print('A total of %i errata were corrected over all chunks of this message.' % len(errata_pos))
-
-If the decoding fails, it will normally automatically check and raise a ReedSolomonError exception that you can handle.
-However if you want to manually check if the repaired message is correct, you can do so:
-
-.. code:: python
-
-    >> rs.rs_check(rmes + recc, nsym)
-
-Note: if you want to use multiple reedsolomon with different parameters, you need to backup the globals and restore them before calling reedsolo functions:
-
-.. code:: python
-
-    >> rs.init_tables()
-    >> global gf_log, gf_exp, field_charac
-    >> bak_gf_log, bak_gf_exp, bak_field_charac = gf_log, gf_exp, field_charac
-
-
-Then at anytime, you can do:
-
-.. code:: python
-
-    >> global gf_log, gf_exp, field_charac
-    >> gf_log, gf_exp, field_charac = bak_gf_log, bak_gf_exp, bak_field_charac
-    >> mesecc = rs.rs_encode_msg(mes, nsym)
-    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym)
-
-The globals backup is not necessary if you use RSCodec, it will be automatically managed.
-
-Read the sourcecode's comments for more info about how it works, and for the various parameters you can setup if
-you need to interface with other RS codecs.
-
-Extended description
---------------------
-The code of wikiversity is here consolidated into a nice API with exceptions handling.
-The algorithm can correct up to ``2*e+v <= nsym``, where ``e`` is the number of errors,
-``v`` the number of erasures and ``nsym = n-k`` = the number of ECC (error correction code) symbols.
-This means that you can either correct exactly ``floor(nsym/2)`` errors, or ``nsym`` erasures
-(errors where you know the position), and a combination of both errors and erasures.
-This is called the Singleton Bound, and is the maximum/optimal theoretical number
-of erasures and errors any error correction algorithm can correct (although there
-are experimental approaches to go a bit further, named list decoding, not implemented
-here, but feel free to do pull request!).
-
-The code should work on pretty much any reasonable version of python (3.7+),
-but I'm only testing on the latest Python version available on Anaconda at the moment (currently 3.10),
-although there is a unit test on various Python versions to ensure retrocompatibility.
-
-This library is also thoroughly unit tested with branch coverage,
-so that nearly any encoding/decoding case should be covered.
-The unit test includes Cython and PyPy too.
-On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
-thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
-another project using reedsolo for the practical application of on-storage data protection, and which includes
-a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
-
-The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
-as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
-hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
-
-Note however that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
-we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
-Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
-your messages, the quadratically longer it will take to encode/decode!
-
-The algorithm itself can handle messages of a length up to ``(2^c_exp)-1`` symbols per message (or chunk), including the ECC symbols,
-and each symbol can have a value of up to ``(2^c_exp)-1`` (indeed, both the message length and the maximum
-value for one character is constrained by the same mathematical reason). By default, we use the field ``GF(2^8)``,
-which means that you are limited to values between 0 and 255 (perfect to represent a single hexadecimal
-symbol on computers, so you can encode any binary stream) and limited to messages+ecc of maximum
-length 255. However, you can "chunk" longer messages to fit them into the message length limit.
-The ``RSCodec`` class will automatically apply chunking, by splitting longer messages into chunks and
-encode/decode them separately; it shouldn't make a difference from an API perspective (ie, from your POV).
-
-Speed optimizations
--------------------
-
-Thanks to using ``bytearray`` and a functional approach (contrary to unireedsolomon, a sibling implementation), the codec
-has quite reasonable performances despite avoiding hardcoding constants and specific instruction sets optimizations that
-are not mathematically generalizable (and so we avoid them, as we want to try to remain as close to the mathematical formulations as possible).
-
-In particular, good speed performance at encoding can be obtained by using either PyPy JIT Compiler on the pure-python
-implementation (reedsolo.py) or either by compiling the Cython extension creedsolo.pyx (which is much more optimized and hence much faster than PyPy).
-
-From our speed tests, encoding rates of several MB/s can be expected with PyPy JIT,
-and 14.3 MB/s using the Cython extension creedsolo on an Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz
-(benchmarked with `pyFileFixity's ecc_speedtest.py <https://github.com/lrq3000/pyFileFixity/blob/master/pyFileFixity/ecc_speedtest.py>`_).
-
-Decoding remains much slower, and less optimized, but more complicated to do so. However, the rationale to focus optimization efforts primarily on encoding and not decoding
-is that users are more likely to spend most of their processing time encoding data, and much less decoding, as encoding needs to be done indiscriminately apriori to protect data,
-whereas decoding happens only aposteriori on data that the user knows is tampered, so this is a much reduced subset of all the protected data (hopefully).
-
-To use the Cython implementation, it is necessary to ``pip install cython==3.0.0b2`` and to install a C++ compiler (Microsoft Visual C++ 14.x for Windows and Python 3.10+), read the up-to-date instructions in the `official wiki <https://wiki.python.org/moin/WindowsCompilers>`_. Then simply ``cd`` to the root of the folder where creedsolo.pyx is, and type ``python setup.py build_ext --inplace --cythonize``. Alternatively, it is possible to generate just the C++ code by typing ``cython -3 creedsolo.pyx``. When building a distributable egg or installing the module from source, the Cython module can be transpiled and compiled if both Cython and a C compiler are installed and the ``--cythonize`` flag is supplied to the setup.py, otherwise by default only the pure-python implementation and the ``.pyx`` cython source code will be included, but the binary won't be in the wheel.
-
-Then, use ``from creedsolo import RSCodec`` instead of importing from the ``reedsolo`` module, and finally only feed ``bytearray()`` objects to the `RSCodec` object. Exclusively using bytearrays is one of the reasons creedsolo is faster than reedsolo. You can convert any string by specifying the encoding: ``bytearray("Hello World", "UTF-8")``.
-
-Note that there is an inherent limitation of the C implementation which cannot work with higher galois fields than 8 (= characters of max 255 value) because the C implementation only works with bytearrays, and bytearrays only support characters up to 255. If you want to use higher galois fields, you need to use the pure python version, which includes a fake ``_bytearray`` function that overloads the standard bytearray with an ``array.array("i", ...)`` in case galois fields higher than 8 are used to ``init_tables()``, or rewrite the C implementation to use lists instead of bytearrays (which will be MUCH slower so this defeats the purpose and you are better off simply using the pure python version under PyPy - an older version of the C implementation was doing just that, and without bytearrays, all performance gains were lost, hence why the bytearrays were kept despite the limitations).
-
-Edge cases
--------------
-
-Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
-
-* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
-
-* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
-
-Migration from v1.x to v2.x
----------------------------
-
-If you used ``reedsolo`` v1.x, then to upgrade to v2.x, a few changes in the API must be considered.
-
-We will not list everything here, but the biggest breaking change is that now internally, everything is either a ``bytearray``, or a CPython ``array('i', ...)``.
-
-For the pure python implementation ``reedsolo``, this should not change much, it should be retrocompatible with lists (there are a few checks in place to autodetect and convert lists into bytearrays whenever necessary - but only in RSCodec, not in lower level functions if that's what you used!).
-
-However, for the cythonized extension ``creedsolo``, these changes are breaking compatibility with v1.x: if you used ``bytearray`` everywhere whenever supplying a list of values into ``creedsolo`` (both for the ``data`` and ``erasures_pos``), then all is well, you are good to go! On the other hand, if you used ``list`` objects or other types in some places, you are in for some errors.
-
-The good news is that, thanks to these changes, both implementations are much faster, but especially ``creedsolo``, which now encodes at a rate of ``15-20 MB/s`` (yes that's BYTES, not bits!). This however requires Cython >= 3.0.0b2, and is incompatible with Python 2 (the pure python ``reedsolo`` is still compatible, but not the cythonized extension ``creedsolo``).
-
-In practice, there is likely very little you need to change, just add a few ``bytearray()`` calls here and there. For a practical example of what was required to migrate, see `the commits for pyFileFixity migration <https://github.com/lrq3000/pyFileFixity/compare/47407b73dfbcfe34970055524655e21ccf2979aa..23b8f6f6c6f252fb9a641f419a6bfa5a1e6c3343>`_.
-
-Recommended reading
--------------------
-
-* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
-* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
-
-Authors
--------
-
-This module was conceived and developed by Tomer Filiba in 2012.
-
-It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
-
-And several other contributors helped improve and make it more robust:
-
-|Contributors|
-
-For a list of all contributors, please see `the GitHub Contributors graph <https://github.com/tomerfiliba/reedsolomon/graphs/contributors>`_ and the `commits history <https://github.com/tomerfiliba/reedsolomon/commits/master>`_.
-
-License
--------
-
-This software is released under your choice of the Unlicense or the MIT-0 (MIT No Attribution) License. Both licenses are `public-domain-equivalent licenses <https://en.wikipedia.org/wiki/Public-domain-equivalent_license>`_, as intended by the original author Tomer Filiba.
-
-
-.. |PyPI-Status| image:: https://img.shields.io/pypi/v/reedsolo.svg
-   :target: https://pypi.org/project/reedsolo
-.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/reedsolo.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/reedsolo
-.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/reedsolo.svg?label=pypi%20downloads&logo=python&logoColor=white
-   :target: https://pypi.org/project/reedsolo
-.. |Build-Status| image:: https://github.com/tomerfiliba/reedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
-    :target: https://github.com/tomerfiliba/reedsolomon/actions/workflows/ci-build.yml
-.. |Coverage| image:: https://coveralls.io/repos/tomerfiliba/reedsolomon/badge.svg?branch=master&service=github
-  :target: https://coveralls.io/github/tomerfiliba/reedsolomon?branch=master
-.. |Conda-Forge-Status| image:: https://img.shields.io/conda/vn/conda-forge/reedsolo.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Conda-Forge-Platforms| image:: https://anaconda.org/conda-forge/reedsolo/badges/platforms.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Conda-Forge-Downloads| image:: https://anaconda.org/conda-forge/reedsolo/badges/downloads.svg
-   :target: https://anaconda.org/conda-forge/reedsolo
-.. |Contributors| image:: https://contrib.rocks/image?repo=tomerfiliba/reedsolomon
-   :target: https://github.com/tomerfiliba/reedsolomon/graphs/contributors
+Metadata-Version: 2.1
+Name: reedsolo
+Version: 2.1.0b1
+Summary: Pythonic universal errors-and-erasures Reed-Solomon codec to protect your data from errors and bitrot, with a future-proof zero-dependencies pure-python implementation and an optional speed-optimized Cython/C extension.
+Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: The software is available under your choice of
+        Unlicense (SPDX short identifier: Unlicense) or
+        MIT No Attribution License (SPDX short identifier: MIT-0):
+        
+        -----
+        
+        <<START OF UNLICENSE>>
+        This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <http://unlicense.org/>
+        <<END OF UNLICENSE>>
+        
+        -----
+        
+        <<START OF MIT-0 LICENSE>>
+        Copyright 2013-2023 Tomer Filiba & Stephen Larroque
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        <<END OF MIT-0 LICENSE>>
+        
+Project-URL: Homepage, https://github.com/tomerfiliba-org/reedsolomon
+Project-URL: Documentation, https://github.com/tomerfiliba-org/reedsolomon/blob/master/README.rst
+Project-URL: Source, https://github.com/tomerfiliba-org/reedsolomon
+Project-URL: Tracker, https://github.com/tomerfiliba-org/reedsolomon/issues
+Project-URL: Download, https://github.com/tomerfiliba-org/reedsolomon/releases
+Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
+Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Cython
+Classifier: Topic :: Communications
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: System :: Recovery Tools
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: testmeta
+Provides-Extra: testoptional
+License-File: LICENSE
+
+Reed Solomon
+============
+
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
+
+|Build-Status| |Coverage|
+
+|Conda-Forge-Status| |Conda-Forge-Platforms| |Conda-Forge-Downloads|
+
+⏳🛡 Pythonic universal errors-and-erasures `Reed-Solomon encoder/decoder codec <http://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction>`_ to protect your data from errors and bitrot. Includes a future-proof zero-dependencies pure-python implementation 🔮 as well as an optional speed-optimized Cython/C extension 🚀
+
+This is a burst-type implementation, so that it supports any Galois field higher than 2^3, but not binary streams. Burst errors are non-random errors that more often happen on data storage mediums such as hard drives, hence this library is better suited for data storage protection, and less for streams noise correction, although it also works for this purpose but with a bit of overhead (since it works with bytes only, instead of bits).
+
+Based on the wonderful tutorial at `Wikiversity <http://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_, written by "Bobmath" and "LRQ3000". If you are just starting with Reed-Solomon error correction codes, the Wikiversity article is a good beginner's introduction.
+
+------------------------------------
+
+.. contents:: Table of contents
+   :backlinks: top
+   :local:
+
+
+Installation
+------------
+
+For the latest stable release (compatible with Python >= 3.7), install with:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo
+
+For the latest development release, use:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo --pre
+
+For the cutting-edge code (likely unstable, do not use in production!), use:
+
+.. code:: sh
+
+    pip install --upgrade git+https://github.com/tomerfiliba-org/reedsolomon
+
+If you have some issues installing through pip, maybe this command may help:
+
+.. code:: sh
+
+    pip install reedsolo --no-binary={reedsolo}
+
+Note: for Python 2.7 and Python <= 3.6, please use v1.7.0:
+
+.. code:: sh
+
+    pip install --upgrade reedsolo==1.7.0
+
+Through wheels/pip, a pure-python implementation called ``reedsolo`` is installed, and for platforms supported by ``cibuildwheel``, a precompiled speed-optimized ``creedsolo`` module is included. For other platforms or to compile from source (this requires ``cython>=3.0.0b2`` and a C compiler), a build option can be specified:
+
+.. code:: sh
+
+    # To compile from the latest stable release:
+    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --verbose
+    # To compile from the latest development release:
+    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
+    # To compile from the cutting edge code:
+    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
+
+The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension.
+    
+or locally with:
+
+.. code:: sh
+
+    pip install --upgrade . --config-setting="--build-option=--cythonize" --verbose
+
+Note: for development, it's possible to add the ``--editable`` flag to use the local folder without installing in ``site-packages``,
+and use ``.[test]`` instead of ``.`` to install all required packages to test this module locally.
+
+The package for the development or cutting-edge releases can also be built locally with the pep517 compliant ``build`` tool:
+
+.. code:: sh
+
+    pip install build
+    # With cythonization (from *.pyx to *.c to *.pyd)
+    python -sBm build --config-setting="--build-option=--cythonize"
+    # or skip cythonization and only compile from the already transpiled c extension (from *.c to *.pyd)
+    python -sBm build --config-setting="--build-option=--native-compile"
+
+The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
+
+As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
+
+.. code:: sh
+
+    conda install -c conda-forge reedsolo
+
+Various Linux distributions builds are also available, thanks to a network of amazing maintainers:
+
+|dl-gentoo| |dl-debian| |dl-fedora| |dl-archlinux|
+|dl-alpine| |dl-altlinux| |dl-linux-others|
+
+Usage
+-----
+
+Basic usage with high-level RSCodec class
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    # Initialization
+    >>> from reedsolo import RSCodec, ReedSolomonError
+    >>> rsc = RSCodec(10)  # 10 ecc symbols
+
+    # Encoding
+    # just a list of numbers/symbols:
+    >>> rsc.encode([1,2,3,4])
+    b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M'
+    # bytearrays are accepted and the output will be matched:
+    >>> rsc.encode(bytearray([1,2,3,4]))
+    bytearray(b'\x01\x02\x03\x04,\x9d\x1c+=\xf8h\xfa\x98M')
+    # encoding a byte string is as easy:
+    >>> rsc.encode(b'hello world')
+    b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa'
+
+Note: strings of any length, even if longer than the Galois field, will be encoded as well using transparent chunking.
+
+Note2: it is strongly recommended to always use bytearrays. Using encoded strings is accepted by the RSCodec API, as
+a convenient facility for neophytes, but encodings such as ``UTF-8`` have variable lengths, so internally the module has
+to convert to a bytearray. If you just want to protect a string, you do not need to use a ``bytearray``, but if you need
+to store or send the protected data in a fixed size field, such as in a binary file or a data stream, use a ``bytearray``.
+
+    # Decoding (repairing)
+    >>> rsc.decode(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')[0]  # original
+    b'hello world'
+    >>> rsc.decode(b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 3 errors
+    b'hello world'
+    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa')[0]     # 5 errors
+    b'hello world'
+    >>> rsc.decode(b'hXXXo worXd\xed%T\xc4\xfdXX\xf3\xa8\xaa')[0]        # 6 errors - fail
+    Traceback (most recent call last):
+    ...
+    reedsolo.ReedSolomonError: Too many (or few) errors found by Chien Search for the errata locator polynomial!
+
+**Important upgrade notice for pre-1.0 users:** Note that ``RSCodec.decode()`` returns 3 variables:
+
+    1. the decoded (corrected) message
+    2. the decoded message and error correction code (which is itself also corrected)
+    3. and the list of positions of the errata (errors and erasures)
+
+Here is how to use these outputs:
+
+    >>> tampered_msg = b'heXlo worXd\xed%T\xc4\xfdX\x89\xf3\xa8\xaa'
+    >>> decoded_msg, decoded_msgecc, errata_pos = rsc.decode(tampered_msg)
+    >>> print(decoded_msg)  # decoded/corrected message
+    bytearray(b'hello world')
+    >>> print(decoded_msgecc)  # decoded/corrected message and ecc symbols
+    bytearray(b'hello world\xed%T\xc4\xfd\xfd\x89\xf3\xa8\xaa')
+    >>> print(errata_pos)  # errata_pos is returned as a bytearray, hardly intelligible
+    bytearray(b'\x10\t\x02')
+    >>> print(list(errata_pos))  # convert to a list to get the errata positions as integer indices
+    [16, 9, 2]
+
+Since we failed to decode with 6 errors with a codec set with 10 error correction code (ecc) symbols, let's try to use a bigger codec, with 12 ecc symbols.
+
+    >>> rsc = RSCodec(12)  # using 2 more ecc symbols (to correct max 6 errors or 12 erasures)
+    >>> rsc.encode(b'hello world')
+    b'hello world?Ay\xb2\xbc\xdc\x01q\xb9\xe3\xe2='
+    >>> rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')[0]         # 6 errors - ok, but any more would fail
+    b'hello world'
+    >>> rsc.decode(b'helXXXXXXXXXXy\xb2XX\x01q\xb9\xe3\xe2=', erase_pos=[3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 15, 16])[0]  # 12 erasures - OK
+    b'hello world'
+
+This shows that we can decode twice as many erasures (where we provide the location of errors ourselves) than errors (with unknown locations). This is the cost of error correction compared to erasure correction.
+
+To get the maximum number of errors *or* erasures that can be independently corrected (ie, not simultaneously):
+
+    >>> maxerrors, maxerasures = rsc.maxerrata(verbose=True)
+    This codec can correct up to 6 errors and 12 erasures independently
+    >>> print(maxerrors, maxerasures)
+    6 12
+
+To get the maximum number of errors *and* erasures that can be simultaneously corrected, you need to specify the number of errors or erasures you expect:
+
+    >>> maxerrors, maxerasures = rsc.maxerrata(erasures=6, verbose=True)  # we know the number of erasures, will calculate how many errors we can afford
+    This codec can correct up to 3 errors and 6 erasures simultaneously
+    >>> print(maxerrors, maxerasures)
+    3 6
+    >>> maxerrors, maxerasures = rsc.maxerrata(errors=5, verbose=True)  # we know the number of errors, will calculate how many erasures we can afford
+    This codec can correct up to 5 errors and 2 erasures simultaneously
+    >>> print(maxerrors, maxerasures)
+    5 2
+
+Note that if a chunk has more errors and erasures than the Singleton Bound as calculated by the ``maxerrata()`` method, the codec will try to raise a ``ReedSolomonError`` exception,
+but may very well not detect any error either (this is a theoretical limitation of error correction codes). In other words, error correction codes are unreliable to detect if a chunk of a message
+is corrupted beyond the Singleton Bound. If you want more reliability in errata detection, use a checksum or hash such as SHA or MD5 on your message, these are much more reliable and have no bounds
+on the number of errata (the only potential issue is with collision but the probability is very very low).
+
+Note: to catch a ``ReedSolomonError`` exception, do not forget to import it first with: ``from reedsolo import ReedSolomonError``
+
+To check if a message is tampered given its error correction symbols, without decoding, use the ``check()`` method:
+
+    # Checking
+    >> rsc.check(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')  # Tampered message will return False
+    [False]
+    >> rmes, rmesecc, errata_pos = rsc.decode(b'hello worXXXXy\xb2XX\x01q\xb9\xe3\xe2=')
+    >> rsc.check(rmesecc)  # Corrected or untampered message will return True
+    [True]
+    >> print('Number of detected errors and erasures: %i, their positions: %s' % (len(errata_pos), list(errata_pos)))
+    Number of detected errors and erasures: 6, their positions: [16, 15, 12, 11, 10, 9]
+
+By default, most Reed-Solomon codecs are limited to characters that can be encoded in 256 bits and with a length of maximum 256 characters. But this codec is universal, you can reduce or increase the length and maximum character value by increasing the Galois Field:
+
+    # To use longer chunks or bigger values than 255 (may be very slow)
+    >> rsc = RSCodec(12, nsize=4095)  # always use a power of 2 minus 1
+    >> rsc = RSCodec(12, c_exp=12)  # alternative way to set nsize=4095
+    >> mes = 'a' * (4095-12)
+    >> mesecc = rsc.encode(mes)
+    >> mesecc[2] = 1
+    >> mesecc[-1] = 1
+    >> rmes, rmesecc, errata_pos = rsc.decode(mesecc)
+    >> rsc.check(mesecc)
+    [False]
+    >> rsc.check(rmesecc)
+    [True]
+
+Note that the ``RSCodec`` class supports transparent chunking, so you don't need to increase the Galois Field to support longer messages, but characters will still be limited to 256 bits (or
+whatever field you set with ``c_exp``).
+
+If you need to use a variable number of error correction symbols (i.e., akin to variable bitrate in videos encoding), this is possible always possible using `RSCodec.decode(nsym=x)` and at encoding by setting `RSCodec(nsym=y, single_gen=False)` and then `RSCodec.encode(nsym=x)`.
+
+Low-level usage via direct access to math functions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you want full control, you can skip the API and directly use the library as-is. Here's how:
+
+First you need to init the precomputed tables:
+
+    >> import reedsolo as rs
+    >> rs.init_tables(0x11d)
+
+Pro tip: if you get the error: ValueError: byte must be in range(0, 256), please check that your prime polynomial is correct for your field.
+Pro tip2: by default, you can only encode messages of max length and max symbol value = 256. If you want to encode bigger messages,
+please use the following (where c_exp is the exponent of your Galois Field, eg, 12 = max length 2^12 = 4096):
+
+    >> prim = rs.find_prime_polys(c_exp=12, fast_primes=True, single=True)[0]
+    >> rs.init_tables(c_exp=12, prim=prim)
+    
+Let's define our RS message and ecc size:
+
+    >> n = 255  # length of total message+ecc
+    >> nsym = 12  # length of ecc
+    >> mes = "a" * (n-nsym)  # generate a sample message
+
+To optimize, you can precompute the generator polynomial:
+
+    >> gen = rs.rs_generator_poly_all(n)
+
+Note: this generates the generator polynomial for all possible `nsym`,
+so this can easily be used for variable encoding rate.
+
+Then to encode:
+
+    >> mesecc = rs.rs_encode_msg(mes, nsym, gen=gen[nsym])
+
+Let's tamper our message:
+
+    >> mesecc[1] = 0
+
+To decode:
+
+    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym, erase_pos=erase_pos)
+
+Note that both the message and the ecc are corrected (if possible of course).
+Pro tip: if you know a few erasures positions, you can specify them in a list ``erase_pos`` to double the repair power. But you can also just specify an empty list.
+
+You can check how many errors and/or erasures were corrected, which can be useful to design adaptive bitrate algorithms:
+
+    >> print('A total of %i errata were corrected over all chunks of this message.' % len(errata_pos))
+
+If the decoding fails, it will normally automatically check and raise a ReedSolomonError exception that you can handle.
+However if you want to manually check if the repaired message is correct, you can do so:
+
+    >> rs.rs_check(rmes + recc, nsym)
+
+Note: if you want to use multiple reedsolomon with different parameters, you need to backup the globals and restore them before calling reedsolo functions:
+
+    >> rs.init_tables()
+    >> global gf_log, gf_exp, field_charac
+    >> bak_gf_log, bak_gf_exp, bak_field_charac = gf_log, gf_exp, field_charac
+
+
+Then at anytime, you can do:
+
+    >> global gf_log, gf_exp, field_charac
+    >> gf_log, gf_exp, field_charac = bak_gf_log, bak_gf_exp, bak_field_charac
+    >> mesecc = rs.rs_encode_msg(mes, nsym)
+    >> rmes, recc, errata_pos = rs.rs_correct_msg(mesecc, nsym)
+
+The globals backup is not necessary if you use RSCodec, it will be automatically managed.
+
+The speed-optimized C extension ``creedsolo`` can be used similarly once compiled or cythonized:
+
+    >> import creedsolo as crs
+    >> codec = crs.RSCodec(10)
+
+If you want to ``cimport`` the module, you will need to directly access the full package path:
+
+    >> import cython
+    >> cimport cython
+    >> cimport creedsolo.creedsolo as crs
+
+Low-level functions allow to construct new APIs on top of this codec, such as
+`an automatic Reed-Solomon decoder <https://github.com/lrq3000/pyFileFixity/blob/0b18728608f2bceac9eafe5356e0abc573af2768/pyFileFixity/lib/eccman.py#L63>`_
+that can search for any viable set of codec parameters if they are apriori unknown.
+
+If you want to learn more about which internal functions to use and for what purposes,
+read the sourcecode's comments (we follow literate programming principles)
+for more info about how it works and the various parameters
+you can setup if you need to interface with other RS codecs.
+
+Extended description
+--------------------
+The code of wikiversity is here consolidated into a nice API with exceptions handling.
+The algorithm can correct up to ``2*e+v <= nsym``, where ``e`` is the number of errors,
+``v`` the number of erasures and ``nsym = n-k`` = the number of ECC (error correction code) symbols.
+This means that you can either correct exactly ``floor(nsym/2)`` errors, or ``nsym`` erasures
+(errors where you know the position), and a combination of both errors and erasures.
+This is called the Singleton Bound, and is the maximum/optimal theoretical number
+of erasures and errors any error correction algorithm can correct (although there
+are experimental approaches to go a bit further, named list decoding, not implemented
+here, but feel free to do pull request!).
+
+The code should work on pretty much any reasonable version of python (3.7+),
+but I'm only testing on the latest Python version available on Anaconda at the moment (currently 3.10),
+although there is a unit test on various Python versions to ensure retrocompatibility.
+
+This library is also thoroughly unit tested with branch coverage,
+so that nearly any encoding/decoding case should be covered.
+The unit test includes Cython and PyPy too.
+On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
+thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
+another project using reedsolo for the practical application of on-storage data protection, and which includes
+a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
+
+The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
+as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
+hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
+
+The work on this module is motivated by the aim to offer a solution for long-term archival of data, although this can and is also
+used for communication streams. For this purpose, this module is an ideal choice: Reed-Solomon is an optimal (non-quantic) algorithm,
+it corrects up to the Singleton Bound which is the absolute limit of how much erratas an error-correction algorithm can correct, RS
+is hence future-proof. The universality of this implementation further ensures that other future implementations of Reed-Solomon
+should be able to decode data encoded with this universal codec.
+
+Note that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
+we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
+Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
+your messages, the quadratically longer it will take to encode/decode!
+
+The algorithm itself can handle messages of a length up to ``(2^c_exp)-1`` symbols per message (or chunk), including the ECC symbols,
+and each symbol can have a value of up to ``(2^c_exp)-1`` (indeed, both the message length and the maximum
+value for one character is constrained by the same mathematical reason). By default, we use the field ``GF(2^8)``,
+which means that you are limited to values between 0 and 255 (perfect to represent a single hexadecimal
+symbol on computers, so you can encode any binary stream) and limited to messages+ecc of maximum
+length 255. However, you can "chunk" longer messages to fit them into the message length limit.
+The ``RSCodec`` class will automatically apply chunking, by splitting longer messages into chunks and
+encode/decode them separately; it shouldn't make a difference from an API perspective (ie, from your POV).
+
+Speed optimizations
+-------------------
+
+Thanks to using ``bytearray`` and a functional approach (contrary to unireedsolomon, a sibling implementation), the codec
+has quite reasonable performances despite avoiding hardcoding constants and specific instruction sets optimizations that
+are not mathematically generalizable (and so we avoid them, as we want to try to remain as close to the mathematical formulations as possible).
+
+In particular, good speed performance at encoding can be obtained by using either PyPy JIT Compiler on the pure-python
+implementation (reedsolo.py) or either by compiling the Cython extension creedsolo.pyx (which is much more optimized and hence much faster than PyPy).
+
+From our speed tests, encoding rates of several MB/s can be expected with PyPy JIT,
+and 14.3 MB/s using the Cython extension creedsolo on an Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz
+(benchmarked with `pyFileFixity's ecc_speedtest.py <https://github.com/lrq3000/pyFileFixity/blob/master/pyFileFixity/ecc_speedtest.py>`_).
+
+Decoding remains much slower, and less optimized, but more complicated to do so. However, the rationale to focus optimization efforts primarily on encoding and not decoding
+is that users are more likely to spend most of their processing time encoding data, and much less decoding, as encoding needs to be done indiscriminately apriori to protect data,
+whereas decoding happens only aposteriori on data that the user knows is tampered, so this is a much reduced subset of all the protected data (hopefully).
+
+To use the Cython implementation, it is necessary to ``pip install cython==3.0.0b2`` and to install a C++ compiler (Microsoft Visual C++ 14.x for Windows and Python 3.10+), read the up-to-date instructions in the `official wiki <https://wiki.python.org/moin/WindowsCompilers>`_. Then simply ``cd`` to the root of the folder where creedsolo.pyx is, and type ``python setup.py build_ext --inplace --cythonize``. Alternatively, it is possible to generate just the C++ code by typing ``cython -3 creedsolo.pyx``. When building a distributable egg or installing the module from source, the Cython module can be transpiled and compiled if both Cython and a C compiler are installed and the ``--cythonize`` flag is supplied to the setup.py, otherwise by default only the pure-python implementation and the ``.pyx`` cython source code will be included, but the binary won't be in the wheel.
+
+Then, use ``from creedsolo import RSCodec`` instead of importing from the ``reedsolo`` module, and finally only feed ``bytearray()`` objects to the `RSCodec` object. Exclusively using bytearrays is one of the reasons creedsolo is faster than reedsolo. You can convert any string by specifying the encoding: ``bytearray("Hello World", "UTF-8")``.
+
+Note that there is an inherent limitation of the C implementation which cannot work with higher galois fields than 8 (= characters of max 255 value) because the C implementation only works with bytearrays, and bytearrays only support characters up to 255. If you want to use higher galois fields, you need to use the pure python version, which includes a fake ``_bytearray`` function that overloads the standard bytearray with an ``array.array("i", ...)`` in case galois fields higher than 8 are used to ``init_tables()``, or rewrite the C implementation to use lists instead of bytearrays (which will be MUCH slower so this defeats the purpose and you are better off simply using the pure python version under PyPy - an older version of the C implementation was doing just that, and without bytearrays, all performance gains were lost, hence why the bytearrays were kept despite the limitations).
+
+Edge cases
+-------------
+
+Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
+
+* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
+
+* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
+
+Migration from v1.x to v2.x
+---------------------------
+
+If you used ``reedsolo`` v1.x, then to upgrade to v2.x, a few changes in the build requirements, the build system and API must be considered.
+
+One major change is that Cython>=v3.0.0b2 is required to cythonize ``creedsolo.pyx``. To ease migration for operating systems where python packages pre-releases are not available, the intermediary `creedsolo.c` is also shipped in the standard distribution (the `tar.gz` file) to allow compilation with any C compiler, without requiring Cython.
+
+Furthermore, the packaging system was overhauled to be PEP 517 standard compliant, so that it now supports build isolation by default, and it uses a src-layout.
+
+While we tried to keep the import API the same (you can still do ``import reedsolo as rs; codec = rs.RSCodec(10)`` and similarly ``import creedsolo as crs``. However, if you used to ``cimport creedsolo as crs`` using the fast c-import system provided by Cython, now you will need to ``cimport creedsolo.creedsolo as crs``.
+
+Indeed, for Linux distributions package maintainers, it's important to note the module is now using a `"src-layout" <https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure>`_, instead of the `"single-module-layout" <https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#single-module-distribution>`_ before, so this may require some adjustments in packages building processes.
+
+Furthermore, wheels with a precompiled ``creedsolo.pyd`` extension are now built for multiple platforms and Python releases and uploaded to PyPi, thanks to ``cibuildwheel``, and the process is automated with a GitHub Action. In future releases, we will try to improve on build reproducibility, such as by implementing a lockfile (but not there yet, there is no standard for that) and moving away from ``setuptools`` (potentially to ``meson``).
+
+Support for Python 2.7 and Python <= 3.6 was dropped as advised elsewhere, as only the pure python implementation remained retrocompatible, but not the cython extension, so that it is better for older Py2.7 users to simply stick to the fully functional reedsolo v1.7.0. For Python 3.6, support was dropped because these environments are not supported officially anymore by GitHub Actions, so it is harder to unit test and hence no guarantee of correctedness can be provided anymore in an automated fashion, so it's better to also use reedsolo v1.7.0 for these older Py3 versions.
+
+About API changes, a few bugfixes were implemented in the pure python implementation, but breaking changes were limited as much as possible (if there is any, it is unintended). For the `creedsolo` extension, there are LOTS of changes, hence why the major version change (we try to follow SemVer). We will not list everything here, but the biggest breaking change is that now internally, everything is either a ``bytearray``, or a CPython ``array('i', ...)``. So this means that when interacting with `creedsolo`, you want to **always** supply a `bytearray` object, you can't just provide a list or a string anymore. For `reedsolo`, this is still supported, since it transparently converts to a bytearray internally, for ease of use.
+
+For the pure python implementation ``reedsolo``, this should not change much, it should be retrocompatible with lists (there are a few checks in place to autodetect and convert lists into bytearrays whenever necessary - but only in RSCodec, not in lower level functions if that's what you used!).
+
+However, for the cythonized extension ``creedsolo``, these changes are breaking compatibility with v1.x: if you used ``bytearray`` everywhere whenever supplying a list of values into ``creedsolo`` (both for the ``data`` and ``erasures_pos``), then all is well, you are good to go! On the other hand, if you used ``list`` objects or other types in some places, you are in for some errors.
+
+The good news is that, thanks to these changes, both implementations are much faster, but especially ``creedsolo``, which now encodes at a rate of ``15-20 MB/s`` (yes that's BYTES, not bits!). This however requires Cython >= 3.0.0b2, and is incompatible with Python 2 (the pure python ``reedsolo`` is still compatible, but not the cythonized extension ``creedsolo``).
+
+In practice, there is likely very little you need to change, just add a few ``bytearray()`` calls here and there. For a practical example of what was required to migrate, see `the commits for pyFileFixity migration <https://github.com/lrq3000/pyFileFixity/compare/47407b73dfbcfe34970055524655e21ccf2979aa..23b8f6f6c6f252fb9a641f419a6bfa5a1e6c3343>`_.
+
+Projects using reedsolo
+-----------------------
+
+Reedsolo is a critical component of numerous solutions, such as:
+
+* `Matter (ex-Project CHIP) <https://github.com/project-chip/connectedhomeip>`_ - The new standard for the Internet of Things (IoT): Matter (formerly Project CHIP) creates more connections between more objects, simplifying development for manufacturers and increasing compatibility for consumers, guided by the Connectivity Standards Alliance.
+* `esp-idf <https://github.com/espressif/esp-idf>`_ - Espressif IoT Development Framework. Official development framework for Espressif SoCs, such as ESP32, which are very widespread reprogrammable electronic cheaps for scientific, prototype and DIY projects, especially with Arduino and MicroPython.
+* `esptool <https://github.com/espressif/esptool>`_ - A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+* `pyFileFixity <https://github.com/lrq3000/pyFileFixity>`_  - A suite of tools for long term archival of files.
+* `amodem <https://github.com/romanz/amodem>`_ - Audio MODEM Communication Library in Python, allowing true air-gapped communication (via a speaker and a microphone), or an audio cable (for higher transmission speed).
+* `SteganoGAN <https://github.com/DAI-Lab/SteganoGAN>`_ - SteganoGAN is a tool for creating steganographic images using adversarial training.
+* `galacteek <https://github.com/pinnaculum/galacteek>`_ - Multi-platform browser for the distributed web.
+* `ofrak <https://github.com/redballoonsecurity/ofrak>`_ - OFRAK (Open Firmware Reverse Analysis Konsole) is a binary analysis and modification platform.
+* `HoloCubic AIO <https://github.com/ClimbSnail/HoloCubic_AIO>`_ - All-in-One open-source firmware for the HoloCubic device with a wide features set.
+* `MicroPython-Stubber <https://github.com/Josverl/micropython-stubber>`_ - Boost MicroPython productivity in VSCode: Generate and use stubs for different micropython firmwares to use with vscode and pylance or pylint.
+* `qr-backup <https://github.com/za3k/qr-backup>`_ - Paper backup of files using QR codes.
+* `Jade <https://github.com/Blockstream/Jade>`_ - Jade Hardware Wallet.
+* `pied-piper <https://github.com/rraval/pied-piper>`_ - Defunct popular module for data transfer over sound waves.
+* `qreader <https://github.com/ewino/qreader>`_ - A defunct pure python QR code reader.
+* `sonicky <https://github.com/egglang/sonicky>`_ - Proof-of-concept Python and Android modules for connectionless ultrasonic message transfer.
+* `neighborhood-connectivity <https://github.com/shayyzhakov/neighborhood-connectivity>`_ - An example app that implements a noisy communication between clique of thread group with very high error correction handling ability and O(1) rounds of messages sending.
+* `audiotagger <https://github.com/NERVEUML/audiotagger>`_ - Clever use of error correction codes to wirelessly synchronize multiple concurrent video feeds of amateur video filmmakers by injecting AFSK packets with timestamp and location metadata in the audio channel communicated via radios.
+* Several research papers used reedsolo, see a list `here <https://scholar.google.com/scholar?q=%22reedsolo%22>`_.
+
+And many, many `more <https://github.com/tomerfiliba-org/reedsolomon/network/dependents>`_!
+
+Recommended reading
+-------------------
+
+* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
+* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
+* If you want a more mathematically transparent but less optimized implementation, read the sibling open-source project `unireedsolomon <https://github.com/lrq3000/unireedsolomon>`_, also co-authored by the maintainer of reedsolo, so that the codebase is very similar (although reedsolo is more mature and has more bugfixes - unireedsolomon should only be used for learning purposes!).
+
+Authors
+-------
+
+This module was conceived and developed by Tomer Filiba in 2012.
+
+It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
+
+And several other contributors helped improve and make it more robust, thanks a lot to them!
+
+|Contributors|
+
+For a list of all contributors, please see `the GitHub Contributors graph <https://github.com/tomerfiliba-org/reedsolomon/graphs/contributors>`_ and the `commits history <https://github.com/tomerfiliba-org/reedsolomon/commits/master>`_.
+
+License
+-------
+
+This software is released under your choice of the Unlicense or the MIT-0 (MIT No Attribution) License. Both licenses are `public-domain-equivalent licenses <https://en.wikipedia.org/wiki/Public-domain-equivalent_license>`_, as intended by the original author Tomer Filiba.
+
+
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/reedsolo.svg
+   :target: https://pypi.org/project/reedsolo
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/reedsolo.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/reedsolo
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/reedsolo.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/reedsolo
+.. |Build-Status| image:: https://github.com/tomerfiliba-org/reedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
+    :target: https://github.com/tomerfiliba-org/reedsolomon/actions/workflows/ci-build.yml
+.. |Coverage| image:: https://coveralls.io/repos/tomerfiliba-org/reedsolomon/badge.svg?branch=master&service=github
+  :target: https://coveralls.io/github/tomerfiliba-org/reedsolomon?branch=master
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/vn/conda-forge/reedsolo.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Conda-Forge-Platforms| image:: https://anaconda.org/conda-forge/reedsolo/badges/platforms.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Conda-Forge-Downloads| image:: https://anaconda.org/conda-forge/reedsolo/badges/downloads.svg
+   :target: https://anaconda.org/conda-forge/reedsolo
+.. |Contributors| image:: https://contrib.rocks/image?repo=tomerfiliba-org/reedsolomon
+   :target: https://github.com/tomerfiliba-org/reedsolomon/graphs/contributors
+
+.. |dl-gentoo| image:: https://img.shields.io/badge/Gentoo-54487A?logo=gentoo&logoColor=white
+   :target: https://packages.gentoo.org/packages/dev-python/reedsolomon
+   :alt: Package for Gentoo Linux, thanks to maintainer Michał Górny!
+.. |dl-debian| image:: https://img.shields.io/badge/Debian-D70A53?logo=debian&logoColor=white
+   :target: https://salsa.debian.org/python-team/packages/python-reedsolo/tree/debian/latest
+   :alt: Package for Debian Linux, thanks to maintainer Faidon Liambotis!
+.. |dl-archlinux| image:: https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff
+   :target: https://archlinux.org/packages/community/x86_64/python-reedsolo/
+   :alt: Package for Arch Linux, thanks to maintainer Jelle van der Waa!
+.. |dl-fedora| image:: https://img.shields.io/badge/Fedora-294172?logo=fedora&logoColor=white
+   :target: https://packages.fedoraproject.org/pkgs/python-reedsolo/python3-reedsolo/
+   :alt: Package for Fedora Linux, thanks to maintainer belegdol!
+.. |dl-alpine| image:: https://img.shields.io/badge/Alpine_Linux-%230D597F.svg?logo=alpine-linux&logoColor=white
+   :target: https://pkgs.alpinelinux.org/package/edge/community/x86/py3-reedsolo
+   :alt: Package for Alpine Linux, thanks to maintainer Michał Polański!
+.. |dl-altlinux| image:: https://img.shields.io/badge/Altlinux-yellow.svg
+   :target: https://packages.altlinux.org/en/sisyphus/srpms/python3-module-reedsolo/2902045385933595548
+   :alt: Package for ALT Linux, thanks to maintainer Sergey Bolshakov!
+.. |dl-linux-others| image:: https://img.shields.io/badge/Others-000000?logo=linux&logoColor=white
+   :target: https://pkgs.org/search/?q=reedsolo
+   :alt: List of packages for other Linux distributions
```

### Comparing `reedsolo-2.0.9/reedsolo.py` & `reedsolo-2.1.0b1/src/reedsolo/reedsolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Copyright (c) 2012-2015 Tomer Filiba <tomerfiliba@gmail.com>
 # Copyright (c) 2015 rotorgit
 # Copyright (c) 2015-2023 Stephen Larroque <LRQ3000@gmail.com>
 
 '''
@@ -658,15 +657,15 @@
 
         # Compute the discrepancy Delta
         # Here is the close-to-the-books operation to compute the discrepancy Delta: it's a simple polynomial multiplication of error locator with the syndromes, and then we get the Kth element.
         #delta = gf_poly_mul(err_loc[::-1], synd)[K] # theoretically it should be gf_poly_add(synd[::-1], [1])[::-1] instead of just synd, but it seems it's not absolutely necessary to correctly decode.
         # But this can be optimized: since we only need the Kth element, we don't need to compute the polynomial multiplication for any other element but the Kth. Thus to optimize, we compute the polymul only at the item we need, skipping the rest (avoiding a nested loop, thus we are linear time instead of quadratic).
         # This optimization is actually described in several figures of the book "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press.
         delta = synd[K]
-        for j in xrange(1, len(err_loc)):
+        for j in xrange(1, len(err_loc)):  # range 1:256 is important: if you use range 0:255, if the last byte of the ecc symbols is corrupted, it won't be correctable! You need to use the range 1,256 to include this last byte.
             delta ^= gf_mul(err_loc[-(j+1)], synd[K - j]) # delta is also called discrepancy. Here we do a partial polynomial multiplication (ie, we compute the polynomial multiplication only for the term of degree K). Should be equivalent to brownanrs.polynomial.mul_at().
         #print "delta", K, delta, list(gf_poly_mul(err_loc[::-1], synd)) # debugline
 
         # Shift polynomials to compute the next degree
         old_loc = old_loc + _bytearray([0])
 
         # Iteratively estimate the errata locator and evaluator polynomials
@@ -684,16 +683,16 @@
             err_loc = gf_poly_add(err_loc, gf_poly_scale(old_loc, delta))
 
     # Check if the result is correct, that there's not too many errors to correct
     for i, x in enumerate(err_loc):  #drop leading 0s, else errs will not be of the correct size. This does not use functional closures (ie, lambdas), which Cython and JIT compilers cannot optimize, such as `err_loc = list(itertools.dropwhile(lambda x: x == 0, err_loc))`
         if x != 0:
             err_loc = err_loc[i:]
             break
-    errs = len(err_loc) - 1
-    if (errs-erase_count) * 2 + erase_count > nsym:
+    errs = len(err_loc) - 1  # -1 because range is 1:256, it's offset by 1, it's not 0:255, hence the length would be overestimated without -1
+    if (errs-erase_count) * 2 + erase_count > nsym:  # failure if we have too many erratas for the Singleton Bound.
         raise ReedSolomonError("Too many errors to correct")
 
     # Return result
     return err_loc
 
 def rs_find_errata_locator(e_pos, generator=2):
     '''Compute the erasures/errors/errata locator polynomial from the erasures/errors/errata positions (the positions must be relative to the x coefficient, eg: "hello worldxxxxxxxxx" is tampered to "h_ll_ worldxxxxxxxxx" with xxxxxxxxx being the ecc of length n-k=9, here the string positions are [1, 4], but the coefficients are reversed since the ecc characters are placed as the first coefficients of the polynomial, thus the coefficients of the erased characters are n-1 - [1, 4] = [18, 15] = erasures_loc to be specified as an argument.'''
@@ -712,22 +711,22 @@
     # Faster way that is equivalent
     remainder = gf_poly_mul(synd, err_loc) # first multiply the syndromes with the errata locator polynomial
     remainder = remainder[len(remainder)-(nsym+1):] # then divide by a polynomial of the length we want, which is equivalent to slicing the list (which represents the polynomial)
 
     return remainder
 
 def rs_find_errors(err_loc, nmess, generator=2):
-    '''Find the roots (ie, where evaluation = zero) of error polynomial by bruteforce trial, this is a sort of Chien's search (but less efficient, Chien's search is a way to evaluate the polynomial such that each evaluation only takes constant time).'''
+    '''Find the roots (ie, where evaluation = zero) of error polynomial by smart bruteforce trial. This is a faster form of chien search, processing only useful coefficients (the ones in the messages) instead of the whole 2^8 range. Besides the speed boost, this also allows to fix a number of issue: correctly decoding when the last ecc byte is corrupted, and accepting messages of length n > 2^8.'''
     # nmess = length of whole codeword (message + ecc symbols)
-    errs = len(err_loc) - 1
     err_pos = []
     for i in xrange(nmess): # normally we should try all 2^8 possible values, but here we optimize to just check the interesting symbols
         if gf_poly_eval(err_loc, gf_pow(generator, i)) == 0: # It's a 0? Bingo, it's a root of the error locator polynomial, in other terms this is the location of an error
             err_pos.append(nmess - 1 - i)
     # Sanity check: the number of errors/errata positions found should be exactly the same as the length of the errata locator polynomial
+    errs = len(err_loc) - 1  # compute the exact number of errors/errata that this error locator should find
     if len(err_pos) != errs:
         # TODO: to decode messages+ecc with length n > 255, we may try to use a bruteforce approach: the correct positions ARE in the final array j, but the problem is because we are above the Galois Field's range, there is a wraparound so that for example if j should be [0, 1, 2, 3], we will also get [255, 256, 257, 258] (because 258 % 255 == 3, same for the other values), so we can't discriminate. The issue is that fixing any errs_nb errors among those will always give a correct output message (in the sense that the syndrome will be all 0), so we may not even be able to check if that's correct or not, so I'm not sure the bruteforce approach may even be possible.
         raise ReedSolomonError("Too many (or few) errors found by Chien Search for the errata locator polynomial!")
     return _bytearray(err_pos)
 
 def rs_forney_syndromes(synd, pos, nmess, generator=2):
     # Compute Forney syndromes, which computes a modified syndromes to compute only errors (erasures are trimmed out). Do not confuse this with Forney algorithm, which allows to correct the message based on the location of errors.
```

### Comparing `reedsolo-2.0.9/tests/test_creedsolo.py` & `reedsolo-2.1.0b1/tests/test_creedsolo.py`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.9/tests/test_reedsolo.py` & `reedsolo-2.1.0b1/tests/test_reedsolo.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,15 @@
     def test_gf_poly_neg(self):
         a = [1, 12, 14, 9]
         self.assertEqual(gf_poly_neg(a), a)
 
     def test_rs_simple_encode_msg(self):
         a = bytearray("hello world", "latin1")
         nsym = 10
+        init_tables(prim=0x11d, generator=2, c_exp=8)  # otherwise rs_simple_encode_msg() will fail randomly when using pytest-xdist)
         self.assertEqual(rs_simple_encode_msg(a, nsym), rs_encode_msg(a, nsym))
 
 class TestRSCodecUniversalCrossValidation(unittest.TestCase):
     '''Ultimate set of tests of a full set of different parameters for encoding and decoding. If this passes, the codec is universal and can correctly interface with any other RS codec!'''
 
     def test_main(self):
         def cartesian_product_dict_items(dicts):
```

