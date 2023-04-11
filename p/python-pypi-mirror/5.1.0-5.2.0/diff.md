# Comparing `tmp/python-pypi-mirror-5.1.0.tar.gz` & `tmp/python-pypi-mirror-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-pypi-mirror-5.1.0.tar", last modified: Tue Mar  7 15:32:57 2023, max compression
+gzip compressed data, was "python-pypi-mirror-5.2.0.tar", last modified: Tue Apr 11 13:52:15 2023, max compression
```

## Comparing `python-pypi-mirror-5.1.0.tar` & `python-pypi-mirror-5.2.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     3950 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2543 2020-09-06 16:04:00.000000 python-pypi-mirror-5.1.0/README.rst
--rwxr-xr-x   0 vincent   (1000) vincent   (1000)    26995 2023-03-04 11:41:22.000000 python-pypi-mirror-5.1.0/pypi_mirror.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     3950 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)      257 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/SOURCES.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/dependency_links.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       50 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/entry_points.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       12 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       96 2023-03-07 15:32:57.000000 python-pypi-mirror-5.1.0/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      940 2023-03-07 15:29:50.000000 python-pypi-mirror-5.1.0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 13:52:15.808369 python-pypi-mirror-5.2.0/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1066 2019-11-11 13:15:28.000000 python-pypi-mirror-5.2.0/LICENSE
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3394 2023-04-11 13:52:15.808369 python-pypi-mirror-5.2.0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2632 2023-04-11 13:49:51.000000 python-pypi-mirror-5.2.0/README.rst
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)    27340 2023-04-11 13:49:51.000000 python-pypi-mirror-5.2.0/pypi_mirror.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       57 2023-03-02 09:44:01.000000 python-pypi-mirror-5.2.0/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 13:52:15.808369 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3394 2023-04-11 13:52:15.000000 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      280 2023-04-11 13:52:15.000000 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-11 13:52:15.000000 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       49 2023-04-11 13:52:15.000000 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/entry_points.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       12 2023-04-11 13:52:15.000000 python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-04-11 13:52:15.808369 python-pypi-mirror-5.2.0/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      940 2023-04-11 13:50:11.000000 python-pypi-mirror-5.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-pypi-mirror-5.1.0/PKG-INFO` & `python-pypi-mirror-5.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,112 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: python-pypi-mirror
-Version: 5.1.0
+Version: 5.2.0
 Summary: A script to create a partial PyPI mirror
 Home-page: https://github.com/montag451/pypi-mirror
 Author: montag451
 Author-email: montag451@laposte.net
 Maintainer: montag451
 Maintainer-email: montag451@laposte.net
 License: UNKNOWN
-Description: ``pypi-mirror`` is a small script to generate a partial PyPI mirror. It
-        relies on ``pip`` to do the most difficult part of the job (downloading
-        a package and its dependencies).
-        
-        Why?
-        ====
-        
-        Because most of the time you don't need a full PyPI mirror but only a
-        mirror that contains the packages you use. If you want a full PyPI
-        mirror you should look at `bandersnatch`_.
-        
-        Installation
-        ============
-        
-        You can install ``pypi-mirror`` using ``pip``:
-        
-        .. code:: sh
-        
-           pip install python-pypi-mirror
-        
-        How to use it?
-        ==============
-        
-        The script provides several commands to manage your mirror. To find out
-        which commands are available, type:
-        
-        .. code:: sh
-        
-           pypi-mirror --help
-        
-        Every command provides its own help message. So for example to get the
-        help message of the ``download`` command, type:
-        
-        .. code:: sh
-        
-           pypi-mirror download --help
-        
-        The commands that you will probably use the most are the ``download``
-        command and the ``create`` command. For example to create a mirror which
-        contains the ``requests`` package and its dependencies, you can type the
-        following:
-        
-        .. code:: sh
-        
-           pypi-mirror download -d downloads requests
-           pypi-mirror create -d downloads -m simple
-        
-        The first command will create a ``downloads`` directory into the current
-        directory and use ``pip`` to download the ``requests`` package and its
-        dependencies into the newly created directory. Then the ``create``
-        command will create a ``simple`` directory into the current directory
-        and will build the mirror inside this newly created directory. You can
-        add new packages by repeating this sequence of commands.
-        
-        To make your mirror available through HTTP, you can point your HTTP
-        server of choice to the ``simple`` directory. For exemple, type the
-        following command into the current directory:
-        
-        .. code:: sh
-        
-           python3 -m http.server
-        
-        It will start a HTTP server that will serve file from the current
-        directory (which should contains the ``downloads`` directory and the
-        ``simple`` directory). You can then install packages using your brand
-        new mirror using the following command:
-        
-        .. code:: sh
-        
-           pip install -i http://127.0.0.1:8000/simple requests
-        
-        About versioning
-        ================
-        
-        This package use `semver`_ to manage version numbering. It means that
-        every times the major number is increased a backward incompatible
-        change has been introduced in the API (the command line is an API). So
-        be careful when upgrading to a new major release as it will surely
-        break your scripts.
-        
-        .. _bandersnatch: https://github.com/pypa/bandersnatch.git
-        .. _semver: https://semver.org/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE
+
+``pypi-mirror`` is a small script to generate a partial PyPI mirror. It
+relies on ``pip`` to do the most difficult part of the job (downloading
+a package and its dependencies).
+
+Why?
+====
+
+Because most of the time you don't need a full PyPI mirror but only a
+mirror that contains the packages you use. If you want a full PyPI
+mirror you should look at `bandersnatch`_.
+
+Installation
+============
+
+You can install ``pypi-mirror`` using ``pip``:
+
+.. code:: sh
+
+   pip install python-pypi-mirror
+
+Or using ``conda``:
+
+.. code:: sh
+
+    conda install -c conda-forge python-pypi-mirror 
+
+How to use it?
+==============
+
+The script provides several commands to manage your mirror. To find out
+which commands are available, type:
+
+.. code:: sh
+
+   pypi-mirror --help
+
+Every command provides its own help message. So for example to get the
+help message of the ``download`` command, type:
+
+.. code:: sh
+
+   pypi-mirror download --help
+
+The commands that you will probably use the most are the ``download``
+command and the ``create`` command. For example to create a mirror which
+contains the ``requests`` package and its dependencies, you can type the
+following:
+
+.. code:: sh
+
+   pypi-mirror download -d downloads requests
+   pypi-mirror create -d downloads -m simple
+
+The first command will create a ``downloads`` directory into the current
+directory and use ``pip`` to download the ``requests`` package and its
+dependencies into the newly created directory. Then the ``create``
+command will create a ``simple`` directory into the current directory
+and will build the mirror inside this newly created directory. You can
+add new packages by repeating this sequence of commands.
+
+To make your mirror available through HTTP, you can point your HTTP
+server of choice to the ``simple`` directory. For exemple, type the
+following command into the current directory:
+
+.. code:: sh
+
+   python3 -m http.server
+
+It will start a HTTP server that will serve file from the current
+directory (which should contains the ``downloads`` directory and the
+``simple`` directory). You can then install packages using your brand
+new mirror using the following command:
+
+.. code:: sh
+
+   pip install -i http://127.0.0.1:8000/simple requests
+
+About versioning
+================
+
+This package use `semver`_ to manage version numbering. It means that
+every times the major number is increased a backward incompatible
+change has been introduced in the API (the command line is an API). So
+be careful when upgrading to a new major release as it will surely
+break your scripts.
+
+.. _bandersnatch: https://github.com/pypa/bandersnatch.git
+.. _semver: https://semver.org/
+
+
```

### Comparing `python-pypi-mirror-5.1.0/README.rst` & `python-pypi-mirror-5.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -24,136 +24,142 @@
 00000170: 0a0a 496e 7374 616c 6c61 7469 6f6e 0a3d  ..Installation.=
 00000180: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a59 6f75  ===========..You
 00000190: 2063 616e 2069 6e73 7461 6c6c 2060 6070   can install ``p
 000001a0: 7970 692d 6d69 7272 6f72 6060 2075 7369  ypi-mirror`` usi
 000001b0: 6e67 2060 6070 6970 6060 3a0a 0a2e 2e20  ng ``pip``:.... 
 000001c0: 636f 6465 3a3a 2073 680a 0a20 2020 7069  code:: sh..   pi
 000001d0: 7020 696e 7374 616c 6c20 7079 7468 6f6e  p install python
-000001e0: 2d70 7970 692d 6d69 7272 6f72 0a0a 486f  -pypi-mirror..Ho
-000001f0: 7720 746f 2075 7365 2069 743f 0a3d 3d3d  w to use it?.===
-00000200: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a54 6865  ===========..The
-00000210: 2073 6372 6970 7420 7072 6f76 6964 6573   script provides
-00000220: 2073 6576 6572 616c 2063 6f6d 6d61 6e64   several command
-00000230: 7320 746f 206d 616e 6167 6520 796f 7572  s to manage your
-00000240: 206d 6972 726f 722e 2054 6f20 6669 6e64   mirror. To find
-00000250: 206f 7574 0a77 6869 6368 2063 6f6d 6d61   out.which comma
-00000260: 6e64 7320 6172 6520 6176 6169 6c61 626c  nds are availabl
-00000270: 652c 2074 7970 653a 0a0a 2e2e 2063 6f64  e, type:.... cod
-00000280: 653a 3a20 7368 0a0a 2020 2070 7970 692d  e:: sh..   pypi-
-00000290: 6d69 7272 6f72 202d 2d68 656c 700a 0a45  mirror --help..E
-000002a0: 7665 7279 2063 6f6d 6d61 6e64 2070 726f  very command pro
-000002b0: 7669 6465 7320 6974 7320 6f77 6e20 6865  vides its own he
-000002c0: 6c70 206d 6573 7361 6765 2e20 536f 2066  lp message. So f
-000002d0: 6f72 2065 7861 6d70 6c65 2074 6f20 6765  or example to ge
-000002e0: 7420 7468 650a 6865 6c70 206d 6573 7361  t the.help messa
-000002f0: 6765 206f 6620 7468 6520 6060 646f 776e  ge of the ``down
-00000300: 6c6f 6164 6060 2063 6f6d 6d61 6e64 2c20  load`` command, 
-00000310: 7479 7065 3a0a 0a2e 2e20 636f 6465 3a3a  type:.... code::
-00000320: 2073 680a 0a20 2020 7079 7069 2d6d 6972   sh..   pypi-mir
-00000330: 726f 7220 646f 776e 6c6f 6164 202d 2d68  ror download --h
-00000340: 656c 700a 0a54 6865 2063 6f6d 6d61 6e64  elp..The command
-00000350: 7320 7468 6174 2079 6f75 2077 696c 6c20  s that you will 
-00000360: 7072 6f62 6162 6c79 2075 7365 2074 6865  probably use the
-00000370: 206d 6f73 7420 6172 6520 7468 6520 6060   most are the ``
-00000380: 646f 776e 6c6f 6164 6060 0a63 6f6d 6d61  download``.comma
-00000390: 6e64 2061 6e64 2074 6865 2060 6063 7265  nd and the ``cre
-000003a0: 6174 6560 6020 636f 6d6d 616e 642e 2046  ate`` command. F
-000003b0: 6f72 2065 7861 6d70 6c65 2074 6f20 6372  or example to cr
-000003c0: 6561 7465 2061 206d 6972 726f 7220 7768  eate a mirror wh
-000003d0: 6963 680a 636f 6e74 6169 6e73 2074 6865  ich.contains the
-000003e0: 2060 6072 6571 7565 7374 7360 6020 7061   ``requests`` pa
-000003f0: 636b 6167 6520 616e 6420 6974 7320 6465  ckage and its de
-00000400: 7065 6e64 656e 6369 6573 2c20 796f 7520  pendencies, you 
-00000410: 6361 6e20 7479 7065 2074 6865 0a66 6f6c  can type the.fol
-00000420: 6c6f 7769 6e67 3a0a 0a2e 2e20 636f 6465  lowing:.... code
-00000430: 3a3a 2073 680a 0a20 2020 7079 7069 2d6d  :: sh..   pypi-m
-00000440: 6972 726f 7220 646f 776e 6c6f 6164 202d  irror download -
-00000450: 6420 646f 776e 6c6f 6164 7320 7265 7175  d downloads requ
-00000460: 6573 7473 0a20 2020 7079 7069 2d6d 6972  ests.   pypi-mir
-00000470: 726f 7220 6372 6561 7465 202d 6420 646f  ror create -d do
-00000480: 776e 6c6f 6164 7320 2d6d 2073 696d 706c  wnloads -m simpl
-00000490: 650a 0a54 6865 2066 6972 7374 2063 6f6d  e..The first com
-000004a0: 6d61 6e64 2077 696c 6c20 6372 6561 7465  mand will create
-000004b0: 2061 2060 6064 6f77 6e6c 6f61 6473 6060   a ``downloads``
-000004c0: 2064 6972 6563 746f 7279 2069 6e74 6f20   directory into 
-000004d0: 7468 6520 6375 7272 656e 740a 6469 7265  the current.dire
-000004e0: 6374 6f72 7920 616e 6420 7573 6520 6060  ctory and use ``
-000004f0: 7069 7060 6020 746f 2064 6f77 6e6c 6f61  pip`` to downloa
-00000500: 6420 7468 6520 6060 7265 7175 6573 7473  d the ``requests
-00000510: 6060 2070 6163 6b61 6765 2061 6e64 2069  `` package and i
-00000520: 7473 0a64 6570 656e 6465 6e63 6965 7320  ts.dependencies 
-00000530: 696e 746f 2074 6865 206e 6577 6c79 2063  into the newly c
-00000540: 7265 6174 6564 2064 6972 6563 746f 7279  reated directory
-00000550: 2e20 5468 656e 2074 6865 2060 6063 7265  . Then the ``cre
-00000560: 6174 6560 600a 636f 6d6d 616e 6420 7769  ate``.command wi
-00000570: 6c6c 2063 7265 6174 6520 6120 6060 7369  ll create a ``si
-00000580: 6d70 6c65 6060 2064 6972 6563 746f 7279  mple`` directory
-00000590: 2069 6e74 6f20 7468 6520 6375 7272 656e   into the curren
-000005a0: 7420 6469 7265 6374 6f72 790a 616e 6420  t directory.and 
-000005b0: 7769 6c6c 2062 7569 6c64 2074 6865 206d  will build the m
-000005c0: 6972 726f 7220 696e 7369 6465 2074 6869  irror inside thi
-000005d0: 7320 6e65 776c 7920 6372 6561 7465 6420  s newly created 
-000005e0: 6469 7265 6374 6f72 792e 2059 6f75 2063  directory. You c
-000005f0: 616e 0a61 6464 206e 6577 2070 6163 6b61  an.add new packa
-00000600: 6765 7320 6279 2072 6570 6561 7469 6e67  ges by repeating
-00000610: 2074 6869 7320 7365 7175 656e 6365 206f   this sequence o
-00000620: 6620 636f 6d6d 616e 6473 2e0a 0a54 6f20  f commands...To 
-00000630: 6d61 6b65 2079 6f75 7220 6d69 7272 6f72  make your mirror
-00000640: 2061 7661 696c 6162 6c65 2074 6872 6f75   available throu
-00000650: 6768 2048 5454 502c 2079 6f75 2063 616e  gh HTTP, you can
-00000660: 2070 6f69 6e74 2079 6f75 7220 4854 5450   point your HTTP
-00000670: 0a73 6572 7665 7220 6f66 2063 686f 6963  .server of choic
-00000680: 6520 746f 2074 6865 2060 6073 696d 706c  e to the ``simpl
-00000690: 6560 6020 6469 7265 6374 6f72 792e 2046  e`` directory. F
-000006a0: 6f72 2065 7865 6d70 6c65 2c20 7479 7065  or exemple, type
-000006b0: 2074 6865 0a66 6f6c 6c6f 7769 6e67 2063   the.following c
-000006c0: 6f6d 6d61 6e64 2069 6e74 6f20 7468 6520  ommand into the 
-000006d0: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
-000006e0: 793a 0a0a 2e2e 2063 6f64 653a 3a20 7368  y:.... code:: sh
-000006f0: 0a0a 2020 2070 7974 686f 6e33 202d 6d20  ..   python3 -m 
-00000700: 6874 7470 2e73 6572 7665 720a 0a49 7420  http.server..It 
-00000710: 7769 6c6c 2073 7461 7274 2061 2048 5454  will start a HTT
-00000720: 5020 7365 7276 6572 2074 6861 7420 7769  P server that wi
-00000730: 6c6c 2073 6572 7665 2066 696c 6520 6672  ll serve file fr
-00000740: 6f6d 2074 6865 2063 7572 7265 6e74 0a64  om the current.d
-00000750: 6972 6563 746f 7279 2028 7768 6963 6820  irectory (which 
-00000760: 7368 6f75 6c64 2063 6f6e 7461 696e 7320  should contains 
-00000770: 7468 6520 6060 646f 776e 6c6f 6164 7360  the ``downloads`
-00000780: 6020 6469 7265 6374 6f72 7920 616e 6420  ` directory and 
-00000790: 7468 650a 6060 7369 6d70 6c65 6060 2064  the.``simple`` d
-000007a0: 6972 6563 746f 7279 292e 2059 6f75 2063  irectory). You c
-000007b0: 616e 2074 6865 6e20 696e 7374 616c 6c20  an then install 
-000007c0: 7061 636b 6167 6573 2075 7369 6e67 2079  packages using y
-000007d0: 6f75 7220 6272 616e 640a 6e65 7720 6d69  our brand.new mi
-000007e0: 7272 6f72 2075 7369 6e67 2074 6865 2066  rror using the f
-000007f0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000800: 3a0a 0a2e 2e20 636f 6465 3a3a 2073 680a  :.... code:: sh.
-00000810: 0a20 2020 7069 7020 696e 7374 616c 6c20  .   pip install 
-00000820: 2d69 2068 7474 703a 2f2f 3132 372e 302e  -i http://127.0.
-00000830: 302e 313a 3830 3030 2f73 696d 706c 6520  0.1:8000/simple 
-00000840: 7265 7175 6573 7473 0a0a 4162 6f75 7420  requests..About 
-00000850: 7665 7273 696f 6e69 6e67 0a3d 3d3d 3d3d  versioning.=====
-00000860: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a54 6869  ===========..Thi
-00000870: 7320 7061 636b 6167 6520 7573 6520 6073  s package use `s
-00000880: 656d 7665 7260 5f20 746f 206d 616e 6167  emver`_ to manag
-00000890: 6520 7665 7273 696f 6e20 6e75 6d62 6572  e version number
-000008a0: 696e 672e 2049 7420 6d65 616e 7320 7468  ing. It means th
-000008b0: 6174 0a65 7665 7279 2074 696d 6573 2074  at.every times t
-000008c0: 6865 206d 616a 6f72 206e 756d 6265 7220  he major number 
-000008d0: 6973 2069 6e63 7265 6173 6564 2061 2062  is increased a b
-000008e0: 6163 6b77 6172 6420 696e 636f 6d70 6174  ackward incompat
-000008f0: 6962 6c65 0a63 6861 6e67 6520 6861 7320  ible.change has 
-00000900: 6265 656e 2069 6e74 726f 6475 6365 6420  been introduced 
-00000910: 696e 2074 6865 2041 5049 2028 7468 6520  in the API (the 
-00000920: 636f 6d6d 616e 6420 6c69 6e65 2069 7320  command line is 
-00000930: 616e 2041 5049 292e 2053 6f0a 6265 2063  an API). So.be c
-00000940: 6172 6566 756c 2077 6865 6e20 7570 6772  areful when upgr
-00000950: 6164 696e 6720 746f 2061 206e 6577 206d  ading to a new m
-00000960: 616a 6f72 2072 656c 6561 7365 2061 7320  ajor release as 
-00000970: 6974 2077 696c 6c20 7375 7265 6c79 0a62  it will surely.b
-00000980: 7265 616b 2079 6f75 7220 7363 7269 7074  reak your script
-00000990: 732e 0a0a 2e2e 205f 6261 6e64 6572 736e  s..... _bandersn
-000009a0: 6174 6368 3a20 6874 7470 733a 2f2f 6769  atch: https://gi
-000009b0: 7468 7562 2e63 6f6d 2f70 7970 612f 6261  thub.com/pypa/ba
-000009c0: 6e64 6572 736e 6174 6368 2e67 6974 0a2e  ndersnatch.git..
-000009d0: 2e20 5f73 656d 7665 723a 2068 7474 7073  . _semver: https
-000009e0: 3a2f 2f73 656d 7665 722e 6f72 672f 0a    ://semver.org/.
+000001e0: 2d70 7970 692d 6d69 7272 6f72 0a0a 4f72  -pypi-mirror..Or
+000001f0: 2075 7369 6e67 2060 6063 6f6e 6461 6060   using ``conda``
+00000200: 3a0a 0a2e 2e20 636f 6465 3a3a 2073 680a  :.... code:: sh.
+00000210: 0a20 2020 2063 6f6e 6461 2069 6e73 7461  .    conda insta
+00000220: 6c6c 202d 6320 636f 6e64 612d 666f 7267  ll -c conda-forg
+00000230: 6520 7079 7468 6f6e 2d70 7970 692d 6d69  e python-pypi-mi
+00000240: 7272 6f72 200a 0a48 6f77 2074 6f20 7573  rror ..How to us
+00000250: 6520 6974 3f0a 3d3d 3d3d 3d3d 3d3d 3d3d  e it?.==========
+00000260: 3d3d 3d3d 0a0a 5468 6520 7363 7269 7074  ====..The script
+00000270: 2070 726f 7669 6465 7320 7365 7665 7261   provides severa
+00000280: 6c20 636f 6d6d 616e 6473 2074 6f20 6d61  l commands to ma
+00000290: 6e61 6765 2079 6f75 7220 6d69 7272 6f72  nage your mirror
+000002a0: 2e20 546f 2066 696e 6420 6f75 740a 7768  . To find out.wh
+000002b0: 6963 6820 636f 6d6d 616e 6473 2061 7265  ich commands are
+000002c0: 2061 7661 696c 6162 6c65 2c20 7479 7065   available, type
+000002d0: 3a0a 0a2e 2e20 636f 6465 3a3a 2073 680a  :.... code:: sh.
+000002e0: 0a20 2020 7079 7069 2d6d 6972 726f 7220  .   pypi-mirror 
+000002f0: 2d2d 6865 6c70 0a0a 4576 6572 7920 636f  --help..Every co
+00000300: 6d6d 616e 6420 7072 6f76 6964 6573 2069  mmand provides i
+00000310: 7473 206f 776e 2068 656c 7020 6d65 7373  ts own help mess
+00000320: 6167 652e 2053 6f20 666f 7220 6578 616d  age. So for exam
+00000330: 706c 6520 746f 2067 6574 2074 6865 0a68  ple to get the.h
+00000340: 656c 7020 6d65 7373 6167 6520 6f66 2074  elp message of t
+00000350: 6865 2060 6064 6f77 6e6c 6f61 6460 6020  he ``download`` 
+00000360: 636f 6d6d 616e 642c 2074 7970 653a 0a0a  command, type:..
+00000370: 2e2e 2063 6f64 653a 3a20 7368 0a0a 2020  .. code:: sh..  
+00000380: 2070 7970 692d 6d69 7272 6f72 2064 6f77   pypi-mirror dow
+00000390: 6e6c 6f61 6420 2d2d 6865 6c70 0a0a 5468  nload --help..Th
+000003a0: 6520 636f 6d6d 616e 6473 2074 6861 7420  e commands that 
+000003b0: 796f 7520 7769 6c6c 2070 726f 6261 626c  you will probabl
+000003c0: 7920 7573 6520 7468 6520 6d6f 7374 2061  y use the most a
+000003d0: 7265 2074 6865 2060 6064 6f77 6e6c 6f61  re the ``downloa
+000003e0: 6460 600a 636f 6d6d 616e 6420 616e 6420  d``.command and 
+000003f0: 7468 6520 6060 6372 6561 7465 6060 2063  the ``create`` c
+00000400: 6f6d 6d61 6e64 2e20 466f 7220 6578 616d  ommand. For exam
+00000410: 706c 6520 746f 2063 7265 6174 6520 6120  ple to create a 
+00000420: 6d69 7272 6f72 2077 6869 6368 0a63 6f6e  mirror which.con
+00000430: 7461 696e 7320 7468 6520 6060 7265 7175  tains the ``requ
+00000440: 6573 7473 6060 2070 6163 6b61 6765 2061  ests`` package a
+00000450: 6e64 2069 7473 2064 6570 656e 6465 6e63  nd its dependenc
+00000460: 6965 732c 2079 6f75 2063 616e 2074 7970  ies, you can typ
+00000470: 6520 7468 650a 666f 6c6c 6f77 696e 673a  e the.following:
+00000480: 0a0a 2e2e 2063 6f64 653a 3a20 7368 0a0a  .... code:: sh..
+00000490: 2020 2070 7970 692d 6d69 7272 6f72 2064     pypi-mirror d
+000004a0: 6f77 6e6c 6f61 6420 2d64 2064 6f77 6e6c  ownload -d downl
+000004b0: 6f61 6473 2072 6571 7565 7374 730a 2020  oads requests.  
+000004c0: 2070 7970 692d 6d69 7272 6f72 2063 7265   pypi-mirror cre
+000004d0: 6174 6520 2d64 2064 6f77 6e6c 6f61 6473  ate -d downloads
+000004e0: 202d 6d20 7369 6d70 6c65 0a0a 5468 6520   -m simple..The 
+000004f0: 6669 7273 7420 636f 6d6d 616e 6420 7769  first command wi
+00000500: 6c6c 2063 7265 6174 6520 6120 6060 646f  ll create a ``do
+00000510: 776e 6c6f 6164 7360 6020 6469 7265 6374  wnloads`` direct
+00000520: 6f72 7920 696e 746f 2074 6865 2063 7572  ory into the cur
+00000530: 7265 6e74 0a64 6972 6563 746f 7279 2061  rent.directory a
+00000540: 6e64 2075 7365 2060 6070 6970 6060 2074  nd use ``pip`` t
+00000550: 6f20 646f 776e 6c6f 6164 2074 6865 2060  o download the `
+00000560: 6072 6571 7565 7374 7360 6020 7061 636b  `requests`` pack
+00000570: 6167 6520 616e 6420 6974 730a 6465 7065  age and its.depe
+00000580: 6e64 656e 6369 6573 2069 6e74 6f20 7468  ndencies into th
+00000590: 6520 6e65 776c 7920 6372 6561 7465 6420  e newly created 
+000005a0: 6469 7265 6374 6f72 792e 2054 6865 6e20  directory. Then 
+000005b0: 7468 6520 6060 6372 6561 7465 6060 0a63  the ``create``.c
+000005c0: 6f6d 6d61 6e64 2077 696c 6c20 6372 6561  ommand will crea
+000005d0: 7465 2061 2060 6073 696d 706c 6560 6020  te a ``simple`` 
+000005e0: 6469 7265 6374 6f72 7920 696e 746f 2074  directory into t
+000005f0: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
+00000600: 746f 7279 0a61 6e64 2077 696c 6c20 6275  tory.and will bu
+00000610: 696c 6420 7468 6520 6d69 7272 6f72 2069  ild the mirror i
+00000620: 6e73 6964 6520 7468 6973 206e 6577 6c79  nside this newly
+00000630: 2063 7265 6174 6564 2064 6972 6563 746f   created directo
+00000640: 7279 2e20 596f 7520 6361 6e0a 6164 6420  ry. You can.add 
+00000650: 6e65 7720 7061 636b 6167 6573 2062 7920  new packages by 
+00000660: 7265 7065 6174 696e 6720 7468 6973 2073  repeating this s
+00000670: 6571 7565 6e63 6520 6f66 2063 6f6d 6d61  equence of comma
+00000680: 6e64 732e 0a0a 546f 206d 616b 6520 796f  nds...To make yo
+00000690: 7572 206d 6972 726f 7220 6176 6169 6c61  ur mirror availa
+000006a0: 626c 6520 7468 726f 7567 6820 4854 5450  ble through HTTP
+000006b0: 2c20 796f 7520 6361 6e20 706f 696e 7420  , you can point 
+000006c0: 796f 7572 2048 5454 500a 7365 7276 6572  your HTTP.server
+000006d0: 206f 6620 6368 6f69 6365 2074 6f20 7468   of choice to th
+000006e0: 6520 6060 7369 6d70 6c65 6060 2064 6972  e ``simple`` dir
+000006f0: 6563 746f 7279 2e20 466f 7220 6578 656d  ectory. For exem
+00000700: 706c 652c 2074 7970 6520 7468 650a 666f  ple, type the.fo
+00000710: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+00000720: 696e 746f 2074 6865 2063 7572 7265 6e74  into the current
+00000730: 2064 6972 6563 746f 7279 3a0a 0a2e 2e20   directory:.... 
+00000740: 636f 6465 3a3a 2073 680a 0a20 2020 7079  code:: sh..   py
+00000750: 7468 6f6e 3320 2d6d 2068 7474 702e 7365  thon3 -m http.se
+00000760: 7276 6572 0a0a 4974 2077 696c 6c20 7374  rver..It will st
+00000770: 6172 7420 6120 4854 5450 2073 6572 7665  art a HTTP serve
+00000780: 7220 7468 6174 2077 696c 6c20 7365 7276  r that will serv
+00000790: 6520 6669 6c65 2066 726f 6d20 7468 6520  e file from the 
+000007a0: 6375 7272 656e 740a 6469 7265 6374 6f72  current.director
+000007b0: 7920 2877 6869 6368 2073 686f 756c 6420  y (which should 
+000007c0: 636f 6e74 6169 6e73 2074 6865 2060 6064  contains the ``d
+000007d0: 6f77 6e6c 6f61 6473 6060 2064 6972 6563  ownloads`` direc
+000007e0: 746f 7279 2061 6e64 2074 6865 0a60 6073  tory and the.``s
+000007f0: 696d 706c 6560 6020 6469 7265 6374 6f72  imple`` director
+00000800: 7929 2e20 596f 7520 6361 6e20 7468 656e  y). You can then
+00000810: 2069 6e73 7461 6c6c 2070 6163 6b61 6765   install package
+00000820: 7320 7573 696e 6720 796f 7572 2062 7261  s using your bra
+00000830: 6e64 0a6e 6577 206d 6972 726f 7220 7573  nd.new mirror us
+00000840: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
+00000850: 6720 636f 6d6d 616e 643a 0a0a 2e2e 2063  g command:.... c
+00000860: 6f64 653a 3a20 7368 0a0a 2020 2070 6970  ode:: sh..   pip
+00000870: 2069 6e73 7461 6c6c 202d 6920 6874 7470   install -i http
+00000880: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3030  ://127.0.0.1:800
+00000890: 302f 7369 6d70 6c65 2072 6571 7565 7374  0/simple request
+000008a0: 730a 0a41 626f 7574 2076 6572 7369 6f6e  s..About version
+000008b0: 696e 670a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ing.============
+000008c0: 3d3d 3d3d 0a0a 5468 6973 2070 6163 6b61  ====..This packa
+000008d0: 6765 2075 7365 2060 7365 6d76 6572 605f  ge use `semver`_
+000008e0: 2074 6f20 6d61 6e61 6765 2076 6572 7369   to manage versi
+000008f0: 6f6e 206e 756d 6265 7269 6e67 2e20 4974  on numbering. It
+00000900: 206d 6561 6e73 2074 6861 740a 6576 6572   means that.ever
+00000910: 7920 7469 6d65 7320 7468 6520 6d61 6a6f  y times the majo
+00000920: 7220 6e75 6d62 6572 2069 7320 696e 6372  r number is incr
+00000930: 6561 7365 6420 6120 6261 636b 7761 7264  eased a backward
+00000940: 2069 6e63 6f6d 7061 7469 626c 650a 6368   incompatible.ch
+00000950: 616e 6765 2068 6173 2062 6565 6e20 696e  ange has been in
+00000960: 7472 6f64 7563 6564 2069 6e20 7468 6520  troduced in the 
+00000970: 4150 4920 2874 6865 2063 6f6d 6d61 6e64  API (the command
+00000980: 206c 696e 6520 6973 2061 6e20 4150 4929   line is an API)
+00000990: 2e20 536f 0a62 6520 6361 7265 6675 6c20  . So.be careful 
+000009a0: 7768 656e 2075 7067 7261 6469 6e67 2074  when upgrading t
+000009b0: 6f20 6120 6e65 7720 6d61 6a6f 7220 7265  o a new major re
+000009c0: 6c65 6173 6520 6173 2069 7420 7769 6c6c  lease as it will
+000009d0: 2073 7572 656c 790a 6272 6561 6b20 796f   surely.break yo
+000009e0: 7572 2073 6372 6970 7473 2e0a 0a2e 2e20  ur scripts..... 
+000009f0: 5f62 616e 6465 7273 6e61 7463 683a 2068  _bandersnatch: h
+00000a00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000a10: 6d2f 7079 7061 2f62 616e 6465 7273 6e61  m/pypa/bandersna
+00000a20: 7463 682e 6769 740a 2e2e 205f 7365 6d76  tch.git... _semv
+00000a30: 6572 3a20 6874 7470 733a 2f2f 7365 6d76  er: https://semv
+00000a40: 6572 2e6f 7267 2f0a                      er.org/.
```

### Comparing `python-pypi-mirror-5.1.0/pypi_mirror.py` & `python-pypi-mirror-5.2.0/pypi_mirror.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,20 +451,29 @@
             action="store_true",
             help="list only the name of the packages",
         )
         parser.add_argument(
             "-n", "--name", metavar="NAME", help="list only the versions of %(metavar)s"
         )
         parser.add_argument("-j", "--json", action="store_true", help="JSON output")
+        parser.add_argument(
+            "--use-norm-name",
+            action="store_true",
+            help="use the normalized name instead of the regular name",
+        )
 
     def run(self, args: argparse.Namespace) -> None:
         super().run(args)
         pkg_by_names = list_pkg_by_names(args.download_dir)
         all_pkgs = []
         for pkg_name, pkgs in pkg_by_names:
+            if args.use_norm_name:
+                pkg = next(pkgs)
+                pkg_name = pkg.metadata.norm_name
+                pkgs = itertools.chain([pkg], pkgs)
             if args.name is not None and pkg_name != args.name:
                 continue
             versions = sort_versions({p.metadata.version for p in pkgs})
             all_pkgs.append({"name": pkg_name, "versions": versions})
         if args.json:
             json.dump(all_pkgs, sys.stdout)
             print()
```

### Comparing `python-pypi-mirror-5.1.0/python_pypi_mirror.egg-info/PKG-INFO` & `python-pypi-mirror-5.2.0/python_pypi_mirror.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,112 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: python-pypi-mirror
-Version: 5.1.0
+Version: 5.2.0
 Summary: A script to create a partial PyPI mirror
 Home-page: https://github.com/montag451/pypi-mirror
 Author: montag451
 Author-email: montag451@laposte.net
 Maintainer: montag451
 Maintainer-email: montag451@laposte.net
 License: UNKNOWN
-Description: ``pypi-mirror`` is a small script to generate a partial PyPI mirror. It
-        relies on ``pip`` to do the most difficult part of the job (downloading
-        a package and its dependencies).
-        
-        Why?
-        ====
-        
-        Because most of the time you don't need a full PyPI mirror but only a
-        mirror that contains the packages you use. If you want a full PyPI
-        mirror you should look at `bandersnatch`_.
-        
-        Installation
-        ============
-        
-        You can install ``pypi-mirror`` using ``pip``:
-        
-        .. code:: sh
-        
-           pip install python-pypi-mirror
-        
-        How to use it?
-        ==============
-        
-        The script provides several commands to manage your mirror. To find out
-        which commands are available, type:
-        
-        .. code:: sh
-        
-           pypi-mirror --help
-        
-        Every command provides its own help message. So for example to get the
-        help message of the ``download`` command, type:
-        
-        .. code:: sh
-        
-           pypi-mirror download --help
-        
-        The commands that you will probably use the most are the ``download``
-        command and the ``create`` command. For example to create a mirror which
-        contains the ``requests`` package and its dependencies, you can type the
-        following:
-        
-        .. code:: sh
-        
-           pypi-mirror download -d downloads requests
-           pypi-mirror create -d downloads -m simple
-        
-        The first command will create a ``downloads`` directory into the current
-        directory and use ``pip`` to download the ``requests`` package and its
-        dependencies into the newly created directory. Then the ``create``
-        command will create a ``simple`` directory into the current directory
-        and will build the mirror inside this newly created directory. You can
-        add new packages by repeating this sequence of commands.
-        
-        To make your mirror available through HTTP, you can point your HTTP
-        server of choice to the ``simple`` directory. For exemple, type the
-        following command into the current directory:
-        
-        .. code:: sh
-        
-           python3 -m http.server
-        
-        It will start a HTTP server that will serve file from the current
-        directory (which should contains the ``downloads`` directory and the
-        ``simple`` directory). You can then install packages using your brand
-        new mirror using the following command:
-        
-        .. code:: sh
-        
-           pip install -i http://127.0.0.1:8000/simple requests
-        
-        About versioning
-        ================
-        
-        This package use `semver`_ to manage version numbering. It means that
-        every times the major number is increased a backward incompatible
-        change has been introduced in the API (the command line is an API). So
-        be careful when upgrading to a new major release as it will surely
-        break your scripts.
-        
-        .. _bandersnatch: https://github.com/pypa/bandersnatch.git
-        .. _semver: https://semver.org/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE
+
+``pypi-mirror`` is a small script to generate a partial PyPI mirror. It
+relies on ``pip`` to do the most difficult part of the job (downloading
+a package and its dependencies).
+
+Why?
+====
+
+Because most of the time you don't need a full PyPI mirror but only a
+mirror that contains the packages you use. If you want a full PyPI
+mirror you should look at `bandersnatch`_.
+
+Installation
+============
+
+You can install ``pypi-mirror`` using ``pip``:
+
+.. code:: sh
+
+   pip install python-pypi-mirror
+
+Or using ``conda``:
+
+.. code:: sh
+
+    conda install -c conda-forge python-pypi-mirror 
+
+How to use it?
+==============
+
+The script provides several commands to manage your mirror. To find out
+which commands are available, type:
+
+.. code:: sh
+
+   pypi-mirror --help
+
+Every command provides its own help message. So for example to get the
+help message of the ``download`` command, type:
+
+.. code:: sh
+
+   pypi-mirror download --help
+
+The commands that you will probably use the most are the ``download``
+command and the ``create`` command. For example to create a mirror which
+contains the ``requests`` package and its dependencies, you can type the
+following:
+
+.. code:: sh
+
+   pypi-mirror download -d downloads requests
+   pypi-mirror create -d downloads -m simple
+
+The first command will create a ``downloads`` directory into the current
+directory and use ``pip`` to download the ``requests`` package and its
+dependencies into the newly created directory. Then the ``create``
+command will create a ``simple`` directory into the current directory
+and will build the mirror inside this newly created directory. You can
+add new packages by repeating this sequence of commands.
+
+To make your mirror available through HTTP, you can point your HTTP
+server of choice to the ``simple`` directory. For exemple, type the
+following command into the current directory:
+
+.. code:: sh
+
+   python3 -m http.server
+
+It will start a HTTP server that will serve file from the current
+directory (which should contains the ``downloads`` directory and the
+``simple`` directory). You can then install packages using your brand
+new mirror using the following command:
+
+.. code:: sh
+
+   pip install -i http://127.0.0.1:8000/simple requests
+
+About versioning
+================
+
+This package use `semver`_ to manage version numbering. It means that
+every times the major number is increased a backward incompatible
+change has been introduced in the API (the command line is an API). So
+be careful when upgrading to a new major release as it will surely
+break your scripts.
+
+.. _bandersnatch: https://github.com/pypa/bandersnatch.git
+.. _semver: https://semver.org/
+
+
```

### Comparing `python-pypi-mirror-5.1.0/setup.py` & `python-pypi-mirror-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="python-pypi-mirror",
-    version="5.1.0",
+    version="5.2.0",
     author="montag451",
     author_email="montag451@laposte.net",
     maintainer="montag451",
     maintainer_email="montag451@laposte.net",
     url="https://github.com/montag451/pypi-mirror",
     description="A script to create a partial PyPI mirror",
     long_description=open("README.rst").read(),
```

