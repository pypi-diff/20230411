# Comparing `tmp/unicat-0.1.5.tar.gz` & `tmp/unicat-0.2.0.tar.gz`

## Comparing `unicat-0.1.5.tar` & `unicat-0.2.0.tar`

### file list

```diff
@@ -1,1177 +1,2172 @@
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/Activate.ps1
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/activate
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/activate.csh
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/activate.fish
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/normalizer
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/pip
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/pip3
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/pip3.11
--rwxr-xr-x   0        0        0      294 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/bin/python3.11 -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0    19190 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build/__init__.py
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build/__main__.py
--rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build/py.typed
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build/util.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/METADATA
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/LICENSE
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/METADATA
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/top_level.txt
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0    18601 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    19101 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/legacy.py
--rwxr-xr-x   0        0        0    50565 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so
--rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md.py
--rwxr-xr-x   0        0        0   274060 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0    20069 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/assets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/cli/normalizer.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/METADATA
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/ElementTree.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/__init__.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/cElementTree.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/common.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/expatbuilder.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/expatreader.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/lxml.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/minidom.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/pulldom.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/sax.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/xmlrpc.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0    32518 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/METADATA
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile/__init__.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile/xmlfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/LICENCE.rst
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/METADATA
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/WHEEL
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/_constants.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/__init__.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/_writer.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/cell.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/read_only.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/text.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/_3d.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/__init__.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/_chart.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/area_chart.py
--rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/axis.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/bar_chart.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/bubble_chart.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/chartspace.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/data_source.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/descriptors.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/error_bar.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/label.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/layout.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/legend.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/line_chart.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/marker.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/picture.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/pie_chart.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/pivot.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/plotarea.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/print_settings.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/radar_chart.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/reader.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/reference.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/scatter_chart.py
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/series.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/series_factory.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/shapes.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/stock_chart.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/surface_chart.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/text.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/title.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/trendline.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/updown_bars.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/chartsheet.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/custom.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/properties.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/protection.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/publish.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/relation.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/views.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/author.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/comment_sheet.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/comments.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/shape_writer.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/abc.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/numbers.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/product.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/singleton.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/strings.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/__init__.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/base.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/excel.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/namespace.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/nested.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/sequence.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/serialisable.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/slots.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/__init__.py
--rw-r--r--   0        0        0    15278 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/colors.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/connector.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/drawing.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/effect.py
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/fill.py
--rw-r--r--   0        0        0    17733 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/geometry.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/graphic.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/image.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/line.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/picture.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/properties.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/relation.py
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/spreadsheet_drawing.py
--rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/text.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/xdr.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formatting/__init__.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formatting/formatting.py
--rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formatting/rule.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formula/__init__.py
--rw-r--r--   0        0        0    15104 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formula/tokenizer.py
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formula/translate.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/__init__.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/core.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/extended.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/interface.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/manifest.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/relationship.py
--rw-r--r--   0        0        0     7024 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/workbook.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/__init__.py
--rw-r--r--   0        0        0    30587 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/cache.py
--rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/fields.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/record.py
--rw-r--r--   0        0        0    37786 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/table.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/drawings.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/excel.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/strings.py
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/workbook.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/alignment.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/borders.py
--rw-r--r--   0        0        0    31182 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/builtins.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/cell_style.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/colors.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/differential.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/fills.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/fonts.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/named_styles.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/numbers.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/protection.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/proxy.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/styleable.py
--rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/stylesheet.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/table.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/bound_dictionary.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/cell.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/dataframe.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/datetime.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/escape.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/exceptions.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/formulas.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/indexed_list.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/inference.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/protection.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/units.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/__init__.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/_writer.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/child.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/defined_name.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/external_reference.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/function_group.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/properties.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/protection.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/smart_tags.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/views.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/web.py
--rw-r--r--   0        0        0    13948 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/workbook.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/__init__.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/external.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/__init__.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_read_only.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_reader.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_write_only.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_writer.py
--rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_range.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_watch.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/controls.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/copier.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/custom.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/datavalidation.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/dimensions.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/drawing.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/errors.py
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/filters.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/header_footer.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/hyperlink.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/merge.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/ole.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/page.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/pagebreak.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/picture.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/properties.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/protection.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/related.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/scenario.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/smart_tag.py
--rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/table.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/views.py
--rw-r--r--   0        0        0    27473 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/worksheet.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/writer/__init__.py
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/writer/excel.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/writer/theme.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/__init__.py
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/constants.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/functions.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/INSTALLER
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/LICENCE.rst
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/METADATA
--rw-r--r--   0        0        0    27015 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/top_level.txt
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/METADATA
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    24244 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    16507 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35763 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    97992 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    37414 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45686 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26070 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14298 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/METADATA
--rw-r--r--   0        0        0    77163 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    21287 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33228 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/LICENSE
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/METADATA
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/build_meta.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-32.exe
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-64.exe
--rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-32.exe
--rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-64.exe
--rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/METADATA
--rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/request.py
--rw-r--r--   0        0        0    30761 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34416 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/queue.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/INSTALLER
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt
--rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/METADATA
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/top_level.txt
--rw-r--r--   0        0        0    26601 2020-02-02 00:00:00.000000 unicat-0.1.5/src/lib-unicat-v0.1.5.zip
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 unicat-0.1.5/src/requirements.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/__init__.py
--rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/api.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/asset.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/class_.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/definition.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/error.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/field.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/layout.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/project.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/projectmember.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/query.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/record.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/record_class_field.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/record_field.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/transform.py
--rw-r--r--   0        0        0    18884 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/unicat.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/user.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/utils.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/excel/styles.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/excel/to_excel.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/assets.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/classes.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/definitions.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/fields.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/project.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/queries.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 unicat-0.1.5/src/unicat/mutate/records.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 unicat-0.1.5/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 unicat-0.1.5/LICENSE
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 unicat-0.1.5/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 unicat-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 unicat-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/Activate.ps1
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/activate
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/activate.csh
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/activate.fish
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/docutils
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/keyring
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/markdown-it
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/normalizer
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pip
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pip3
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pip3.11
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pkginfo
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pygmentize
+-rwxr-xr-x   0        0        0      294 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/python3.11 -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
+-rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2html.py
+-rwxr-xr-x   0        0        0      783 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2man.py
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2odt.py
+-rwxr-xr-x   0        0        0     1787 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      737 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/bin/twine
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/AUTHORS
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0    42164 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/Pygments-2.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/callbacks.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/css_sanitizer.py
+-rw-r--r--   0        0        0    22779 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/html5lib_shim.py
+-rw-r--r--   0        0        0    22350 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/linkifier.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/parse_shim.py
+-rw-r--r--   0        0        0    21934 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/sanitizer.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/__init__.py
+-rw-r--r--   0        0        0    39023 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/parse.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/parse.py.SHA256SUM
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/vendor.txt
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/vendor_install.sh
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/__init__.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0        0        0    32300 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0        0        0    77028 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_utils.py
+-rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/constants.py
+-rw-r--r--   0        0        0   117174 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rw-r--r--   0        0        0    15747 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/serializer.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0        0        0    26885 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0        0        0    14754 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    16076 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    29799 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/bleach-6.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0    19190 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build/__init__.py
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build/__main__.py
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build/py.typed
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build/util.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0    18601 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    19101 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    50565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so
+-rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   274060 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0    20069 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/assets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/ElementTree.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/__init__.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/cElementTree.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/common.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/expatbuilder.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/expatreader.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/lxml.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/minidom.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/pulldom.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/sax.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/xmlrpc.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    32518 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/__init__.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/__main__.py
+-rw-r--r--   0        0        0    30945 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/core.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/examples.py
+-rw-r--r--   0        0        0    39697 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/frontend.py
+-rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/io.py
+-rw-r--r--   0        0        0    80986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/nodes.py
+-rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/statemachine.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/af.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/ar.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/ca.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/cs.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/da.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/de.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/en.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/eo.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/es.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/fa.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/fi.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/fr.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/gl.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/he.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/it.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/ja.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/ko.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/lt.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/lv.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/nl.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/pl.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/pt_br.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/ru.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/sk.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/sv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/zh_cn.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/languages/zh_tw.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/null.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/recommonmark_wrapper.py
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/__init__.py
+-rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/roles.py
+-rw-r--r--   0        0        0   132550 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/states.py
+-rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/tableparser.py
+-rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/body.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/html.py
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/images.py
+-rw-r--r--   0        0        0    26770 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/references.py
+-rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/directives/tables.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/README.txt
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/af.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/da.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/de.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/en.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/es.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/he.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/it.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/readers/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/readers/doctree.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/readers/pep.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/readers/standalone.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/components.py
+-rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/frontmatter.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/misc.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/parts.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/peps.py
+-rw-r--r--   0        0        0    36544 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/references.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/universal.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/transforms/writer_aux.py
+-rw-r--r--   0        0        0    28742 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/__init__.py
+-rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/code_analyzer.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/error_reporting.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/punctuation_chars.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/roman.py
+-rw-r--r--   0        0        0    38945 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/smartquotes.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/urischemes.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/__init__.py
+-rw-r--r--   0        0        0    51043 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/latex2mathml.py
+-rw-r--r--   0        0        0    98692 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/math2html.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-r--r--   0        0        0    36734 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/tex2unichar.py
+-rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/utils/math/unichar2tex.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/__init__.py
+-rw-r--r--   0        0        0    70253 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/_html_base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/docutils_xml.py
+-rw-r--r--   0        0        0    36527 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/manpage.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/null.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/pseudoxml.py
+-rw-r--r--   0        0        0    37638 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html4css1/__init__.py
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html4css1/html4css1.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html4css1/template.txt
+-rw-r--r--   0        0        0    18212 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/template.txt
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/html5_polyglot/tuftig.css
+-rw-r--r--   0        0        0   136872 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/default.tex
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/docutils.sty
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/titlepage.tex
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/titlingpage.tex
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/latex2e/xelatex.tex
+-rw-r--r--   0        0        0   132399 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/odf_odt/__init__.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/odf_odt/styles.odt
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/pep_html/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/pep_html/pep.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/pep_html/template.txt
+-rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/README.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/big-black/__base__
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/slides.css
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/default/slides.js
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/small-black/__base__
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils/writers/xetex/__init__.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/COPYING.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/METADATA
+-rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/RECORD
+-rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/SOURCES.html
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/WHEEL
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/dependency_links.html
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/top_level.html
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/docutils-0.19.dist-info/top_level.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile/__init__.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile/xmlfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/LICENCE.rst
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/METADATA
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0    26518 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata-6.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco/classes/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco/classes/ancestry.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco/classes/meta.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco/classes/properties.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/__main__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/_compat.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/_properties_compat.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backend.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backend_complete.zsh
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/cli.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/completion.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/core.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/credentials.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/devpi_client.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/errors.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/py.typed
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/py312compat.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/OS_X.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/SecretService.py
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/Windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/__init__.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/chainer.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/fail.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/kwallet.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/libsecret.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/null.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/macOS/__init__.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/backends/macOS/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/testing/__init__.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/testing/backend.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/testing/util.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/util/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/util/platform_.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring/util/properties.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/METADATA
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/keyring-23.13.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/_punycode.py
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/main.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/parser_block.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/port.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/py.typed
+-rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/renderer.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/ruler.py
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/token.py
+-rw-r--r--   0        0        0    11052 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/tree.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it/rules_inline/text_collapse.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/_decode.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/_encode.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/_format.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/_parse.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/_url.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/__init__.pyi
+-rwxr-xr-x   0        0        0   134968 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/more.py
+-rw-r--r--   0        0        0    20105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/py.typed
+-rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools-9.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools-9.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    32271 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools-9.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools-9.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/more_itertools-9.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/_constants.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/__init__.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/_writer.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/cell.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/read_only.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/text.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/_3d.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/__init__.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/_chart.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/area_chart.py
+-rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/axis.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/bar_chart.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/bubble_chart.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/chartspace.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/data_source.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/descriptors.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/error_bar.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/label.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/layout.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/legend.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/line_chart.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/marker.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/picture.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/pie_chart.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/pivot.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/plotarea.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/print_settings.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/radar_chart.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/reader.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/reference.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/scatter_chart.py
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/series.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/series_factory.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/shapes.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/stock_chart.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/surface_chart.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/text.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/title.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/trendline.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/updown_bars.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/chartsheet.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/custom.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/properties.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/protection.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/publish.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/relation.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/views.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/author.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/comment_sheet.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/comments.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/shape_writer.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/abc.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/numbers.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/product.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/singleton.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/strings.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/__init__.py
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/base.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/excel.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/namespace.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/nested.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/sequence.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/serialisable.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/slots.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/__init__.py
+-rw-r--r--   0        0        0    15278 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/colors.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/connector.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/drawing.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/effect.py
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/fill.py
+-rw-r--r--   0        0        0    17733 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/geometry.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/graphic.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/image.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/line.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/picture.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/properties.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/relation.py
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/spreadsheet_drawing.py
+-rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/text.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/xdr.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formatting/__init__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formatting/formatting.py
+-rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formatting/rule.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formula/__init__.py
+-rw-r--r--   0        0        0    15104 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formula/tokenizer.py
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formula/translate.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/__init__.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/core.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/extended.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/interface.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/manifest.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/relationship.py
+-rw-r--r--   0        0        0     7024 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/workbook.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/__init__.py
+-rw-r--r--   0        0        0    30587 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/cache.py
+-rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/fields.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/record.py
+-rw-r--r--   0        0        0    37786 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/table.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/drawings.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/excel.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/strings.py
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/workbook.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/alignment.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/borders.py
+-rw-r--r--   0        0        0    31182 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/builtins.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/cell_style.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/colors.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/differential.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/fills.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/fonts.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/named_styles.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/numbers.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/protection.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/proxy.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/styleable.py
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/stylesheet.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/table.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/bound_dictionary.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/cell.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/dataframe.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/datetime.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/escape.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/exceptions.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/formulas.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/indexed_list.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/inference.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/protection.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/units.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/__init__.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/_writer.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/child.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/defined_name.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/external_reference.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/function_group.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/properties.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/protection.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/smart_tags.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/views.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/web.py
+-rw-r--r--   0        0        0    13948 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/workbook.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/__init__.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/external.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/__init__.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_read_only.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_reader.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_write_only.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_writer.py
+-rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_range.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_watch.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/controls.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/copier.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/custom.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/datavalidation.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/dimensions.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/drawing.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/errors.py
+-rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/filters.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/header_footer.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/hyperlink.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/merge.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/ole.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/page.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/pagebreak.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/picture.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/properties.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/protection.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/related.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/scenario.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/smart_tag.py
+-rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/table.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/views.py
+-rw-r--r--   0        0        0    27473 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/worksheet.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/writer/__init__.py
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/writer/excel.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/writer/theme.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/__init__.py
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/constants.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/functions.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/LICENCE.rst
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/METADATA
+-rw-r--r--   0        0        0    27015 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/top_level.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    24244 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    16507 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35763 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    97992 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    37414 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45686 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    26070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14298 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0    77163 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/__init__.pyi
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/bdist.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/bdist.pyi
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/commandline.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/commandline.pyi
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/develop.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/develop.pyi
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/distribution.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/distribution.pyi
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/index.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/index.pyi
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/installed.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/installed.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/py.typed
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/sdist.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/sdist.pyi
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/utils.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/utils.pyi
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/wheel.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/wheel.pyi
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_bdist.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_commandline.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_develop.py
+-rw-r--r--   0        0        0    19377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_distribution.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_index.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_installed.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_sdist.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_utils.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo/tests/test_wheel.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/METADATA
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/WHEEL
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/__main__.py
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/filter.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatter.py
+-rw-r--r--   0        0        0    31987 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/modeline.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/scanner.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/util.py
+-rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21914 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11116 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py
+-rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0        0        0   106781 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0        0        0    64980 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0        0        0    26745 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/actionscript.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ada.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/agile.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/algebra.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ambient.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/amdgpu.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ampl.py
+-rw-r--r--   0        0        0    26654 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/apdlexer.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/apl.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/archetype.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/arrow.py
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/arturo.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/asc.py
+-rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/asm.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/automation.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/bare.py
+-rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/basic.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/bdd.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/berry.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/bibtex.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/boa.py
+-rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/business.py
+-rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/c_cpp.py
+-rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/c_like.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/capnproto.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/cddl.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/chapel.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/clean.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/comal.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/compiled.py
+-rw-r--r--   0        0        0    41825 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/configs.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/console.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/cplint.py
+-rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/crystal.py
+-rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/csound.py
+-rw-r--r--   0        0        0    25314 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/css.py
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/d.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/dalvik.py
+-rw-r--r--   0        0        0    26940 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/data.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/devicetree.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/diff.py
+-rw-r--r--   0        0        0    29696 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/dotnet.py
+-rw-r--r--   0        0        0    36774 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/dsls.py
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/dylan.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ecl.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/eiffel.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/elm.py
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/elpi.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/email.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/erlang.py
+-rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/esoteric.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ezhil.py
+-rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/factor.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/fantom.py
+-rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/felix.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/fift.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/floscript.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/forth.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/fortran.py
+-rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/foxpro.py
+-rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/freefem.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/func.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/functional.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/futhark.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/gdscript.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/go.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/graph.py
+-rw-r--r--   0        0        0    38931 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/graphics.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/graphviz.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/gsql.py
+-rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/haskell.py
+-rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/haxe.py
+-rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/hdl.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/hexdump.py
+-rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/html.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/idl.py
+-rw-r--r--   0        0        0    30631 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/igor.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/inferno.py
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/installers.py
+-rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/int_fiction.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/iolang.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/j.py
+-rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/javascript.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/jmespath.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/jslt.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/jsonnet.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/julia.py
+-rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/jvm.py
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/kuin.py
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/lilypond.py
+-rw-r--r--   0        0        0   144039 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/lisp.py
+-rw-r--r--   0        0        0    31914 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/macaulay2.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/make.py
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/markup.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/math.py
+-rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/matlab.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/maxima.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/meson.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/mime.py
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/minecraft.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/mips.py
+-rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ml.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/modeling.py
+-rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/modula2.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/monte.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/mosel.py
+-rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ncl.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/nimrod.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/nit.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/nix.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/oberon.py
+-rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/objective.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ooc.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/other.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/parasail.py
+-rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/parsers.py
+-rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/pascal.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/pawn.py
+-rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/perl.py
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/phix.py
+-rw-r--r--   0        0        0    12505 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/php.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/pointless.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/pony.py
+-rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/praat.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/procfile.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/prolog.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/promql.py
+-rw-r--r--   0        0        0    53524 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/python.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/q.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/qlik.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/qvt.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/r.py
+-rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/rdf.py
+-rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/rebol.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/resource.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ride.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/rita.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/rnc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/roboconf.py
+-rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/robotframework.py
+-rw-r--r--   0        0        0    22775 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ruby.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/rust.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/sas.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/savi.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/scdoc.py
+-rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/scripting.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/sgf.py
+-rw-r--r--   0        0        0    36344 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/shell.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/sieve.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/slash.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/smalltalk.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/smithy.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/smv.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/snobol.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/solidity.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/sophia.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/special.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/spice.py
+-rw-r--r--   0        0        0    34151 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/sql.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/srcinfo.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/stata.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/supercollider.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/tal.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/tcl.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/teal.py
+-rw-r--r--   0        0        0    72695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/templates.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/teraterm.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/testing.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/text.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/textedit.py
+-rw-r--r--   0        0        0    15192 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/textfmts.py
+-rw-r--r--   0        0        0    20157 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/theorem.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/thingsdb.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/tlb.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/tnt.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/trafficscript.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/typoscript.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/ul4.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/unicon.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/urbi.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/usd.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/varnish.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/verification.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/web.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/webassembly.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/webidl.py
+-rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/webmisc.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/whiley.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/wowtoc.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/wren.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/x10.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/xorg.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/yang.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/lexers/zig.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/abap.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/algol.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/algol_nu.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/arduino.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/autumn.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/borland.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/bw.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/colorful.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/default.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/dracula.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/emacs.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/friendly.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/fruity.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/gh_dark.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/gruvbox.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/igor.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/inkpot.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/lilypond.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/lovelace.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/manni.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/material.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/monokai.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/murphy.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/native.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/nord.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/onedark.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/paraiso_light.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/pastie.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/perldoc.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/rrt.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/sas.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/solarized.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/staroffice.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/stata_dark.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/stata_light.py
+-rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/tango.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/trac.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/vim.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/vs.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/xcode.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pygments/styles/zenburn.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/__about__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/__main__.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/clean.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/rst.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer/txt.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/readme_renderer-37.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21287 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33228 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/__init__.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/_compat.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/exceptions.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/sessions.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/streaming_iterator.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/source.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/adapters/x509.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/auth/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/auth/guess.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/auth/handler.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/cookies/forgetful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/threaded/pool.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/threaded/thread.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/utils/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/utils/dump.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/utils/formdata.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt/utils/user_agent.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/METADATA
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/requests_toolbelt-0.10.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/__init__.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/_mixin.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/abnf_regexp.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/api.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/builder.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/compat.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/exceptions.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/iri.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/misc.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/normalizers.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/parseresult.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/uri.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986/validators.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/__init__.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_export_format.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_inspect.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_pick.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_timer.py
+-rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_win32_console.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_windows.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/abc.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/bar.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/columns.py
+-rw-r--r--   0        0        0    99123 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/containers.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/control.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/default_styles.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/diagnose.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/highlighter.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/json.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/jupyter.py
+-rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/live.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/live_render.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/logging.py
+-rw-r--r--   0        0        0    22368 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/markdown.py
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/measure.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/pager.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/panel.py
+-rw-r--r--   0        0        0    35816 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/pretty.py
+-rw-r--r--   0        0        0    59694 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/progress_bar.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/prompt.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/region.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/repr.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/rule.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/scope.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/screen.py
+-rw-r--r--   0        0        0    24211 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/style.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/styled.py
+-rw-r--r--   0        0        0    35045 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/syntax.py
+-rw-r--r--   0        0        0    39648 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45513 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/themes.py
+-rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/traceback.py
+-rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich/tree.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich-13.3.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich-13.3.3.dist-info/LICENSE
+-rw-r--r--   0        0        0    18844 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich-13.3.3.dist-info/METADATA
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich-13.3.3.dist-info/RECORD
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/rich-13.3.3.dist-info/WHEEL
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/METADATA
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/six-1.16.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/__main__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/auth.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/cli.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/exceptions.py
+-rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/py.typed
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/repository.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/settings.py
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/utils.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/wheel.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/wininst.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/commands/__init__.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/commands/check.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/commands/register.py
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine/commands/upload.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/twine-4.0.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/request.py
+-rw-r--r--   0        0        0    30761 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34416 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/METADATA
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/top_level.txt
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/metadata.json
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/webencodings-0.5.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp/py310compat.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/METADATA
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 unicat-0.2.0/py311/lib/python3.11/site-packages/zipp-3.15.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0    26601 2020-02-02 00:00:00.000000 unicat-0.2.0/src/lib-unicat-v0.1.5.zip
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 unicat-0.2.0/src/requirements.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/__init__.py
+-rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/api.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/asset.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/class_.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/definition.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/error.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/field.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/layout.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/project.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/projectmember.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/query.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/record.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/record_class_field.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/record_field.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/transform.py
+-rw-r--r--   0        0        0    19407 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/unicat.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/user.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/utils.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/assets.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/classes.py
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/definitions.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/fields.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/project.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/queries.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 unicat-0.2.0/src/unicat/mutate/records.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 unicat-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 unicat-0.2.0/LICENSE
+-rw-r--r--   0        0        0    23628 2020-02-02 00:00:00.000000 unicat-0.2.0/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 unicat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    25223 2020-02-02 00:00:00.000000 unicat-0.2.0/PKG-INFO
```

### Comparing `unicat-0.1.5/py311/bin/Activate.ps1` & `unicat-0.2.0/py311/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/bin/activate` & `unicat-0.2.0/py311/bin/activate`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/bin/activate.csh` & `unicat-0.2.0/py311/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/bin/activate.fish` & `unicat-0.2.0/py311/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build/__main__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build/__main__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build/env.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build/env.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/build-0.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/cacert.pem` & `unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/certifi/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/certifi-2022.12.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/api.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/cd.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/constant.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/models.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/assets/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer/cli/normalizer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/charset_normalizer-3.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/ElementTree.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/ElementTree.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/cElementTree.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/cElementTree.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/expatbuilder.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/expatbuilder.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/expatreader.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/expatreader.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/lxml.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/lxml.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/minidom.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/minidom.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/pulldom.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/pulldom.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/sax.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/sax.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml/xmlrpc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/defusedxml-0.7.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile/xmlfile.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile/xmlfile.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/LICENCE.rst` & `unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/et_xmlfile-1.1.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/codec.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/idnadata.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/intranges.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna/uts46data.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/LICENSE.md` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/idna-3.4.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/idna-3.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/_writer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/_writer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/cell.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/cell.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/read_only.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/read_only.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/cell/text.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/cell/text.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/_3d.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/_3d.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/area_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/area_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/axis.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/axis.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/bar_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/bar_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/bubble_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/bubble_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/chartspace.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/chartspace.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/data_source.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/data_source.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/descriptors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/descriptors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/error_bar.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/error_bar.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/label.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/label.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/layout.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/layout.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/legend.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/legend.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/line_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/line_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/marker.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/marker.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/picture.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/picture.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/pie_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/pie_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/pivot.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/pivot.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/plotarea.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/plotarea.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/print_settings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/print_settings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/radar_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/radar_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/reader.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/reader.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/reference.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/reference.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/scatter_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/scatter_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/series.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/series.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/series_factory.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/series_factory.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/shapes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/shapes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/stock_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/stock_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/surface_chart.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/surface_chart.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/text.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/text.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/title.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/title.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/trendline.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/trendline.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chart/updown_bars.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chart/updown_bars.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/chartsheet.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/chartsheet.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/custom.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/custom.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/properties.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/properties.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/protection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/protection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/publish.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/publish.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/relation.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/relation.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/chartsheet/views.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/chartsheet/views.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/comment_sheet.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/comment_sheet.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/comments.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/comments.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/comments/shape_writer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/comments/shape_writer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/numbers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/numbers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/singleton.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/singleton.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/compat/strings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/compat/strings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/excel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/excel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/nested.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/nested.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/sequence.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/sequence.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/serialisable.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/serialisable.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/descriptors/slots.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/descriptors/slots.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/colors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/colors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/connector.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/connector.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/drawing.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/drawing.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/effect.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/effect.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/fill.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/fill.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/geometry.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/geometry.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/graphic.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/graphic.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/image.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/image.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/line.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/line.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/picture.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/picture.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/properties.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/properties.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/spreadsheet_drawing.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/spreadsheet_drawing.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/text.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/text.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/drawing/xdr.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/drawing/xdr.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formatting/formatting.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formatting/formatting.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formatting/rule.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formatting/rule.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formula/tokenizer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formula/tokenizer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/formula/translate.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/formula/translate.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/extended.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/extended.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/interface.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/interface.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/manifest.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/manifest.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/relationship.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/relationship.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/packaging/workbook.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/packaging/workbook.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/fields.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/fields.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/record.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/record.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/pivot/table.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/pivot/table.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/drawings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/drawings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/excel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/excel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/strings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/strings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/reader/workbook.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/reader/workbook.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/alignment.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/alignment.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/borders.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/borders.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/builtins.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/builtins.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/cell_style.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/cell_style.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/colors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/colors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/differential.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/differential.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/fills.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/fills.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/fonts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/named_styles.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/named_styles.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/numbers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/numbers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/proxy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/proxy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/styleable.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/styleable.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/stylesheet.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/stylesheet.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/styles/table.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/styles/table.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/bound_dictionary.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/bound_dictionary.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/cell.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/cell.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/dataframe.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/datetime.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/escape.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/escape.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/formulas.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/formulas.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/indexed_list.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/indexed_list.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/inference.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/inference.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/protection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/protection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/utils/units.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/utils/units.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/_writer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/_writer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/child.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/child.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/defined_name.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/defined_name.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/function_group.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/function_group.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/properties.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/properties.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/protection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/protection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/smart_tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/smart_tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/views.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/views.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/web.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/web.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/workbook.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/workbook.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/external.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/workbook/external_link/external.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_read_only.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_read_only.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_reader.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_reader.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_write_only.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_write_only.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/_writer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/_writer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_range.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_range.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_watch.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/cell_watch.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/controls.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/controls.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/copier.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/copier.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/custom.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/custom.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/datavalidation.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/datavalidation.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/dimensions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/dimensions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/errors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/errors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/filters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/filters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/header_footer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/header_footer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/hyperlink.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/hyperlink.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/merge.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/merge.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/ole.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/ole.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/page.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/page.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/pagebreak.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/pagebreak.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/properties.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/properties.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/protection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/protection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/scenario.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/scenario.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/smart_tag.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/smart_tag.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/table.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/table.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/views.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/views.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/worksheet/worksheet.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/worksheet/worksheet.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/writer/excel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/writer/excel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/writer/theme.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/writer/theme.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/constants.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/constants.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl/xml/functions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl/xml/functions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/LICENCE.rst` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/openpyxl-3.0.10.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_elffile.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_manylinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_musllinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_parser.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/_tokenizer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/markers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/requirements.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/specifiers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.APACHE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.BSD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/packaging-23.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/__main__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/__pip-runner__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/build_env.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/configuration.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/index.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/link.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/download.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/session.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/six.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/six.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/LICENSE.txt` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pip-23.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_impl.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/_in_process.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/_internal_utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/adapters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/api.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/auth.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/cookies.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/help.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/hooks.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/models.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/packages.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/sessions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/status_codes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/requests-2.28.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_entry_points.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_imp.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_importlib.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_itertools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_path.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/archive_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/build_meta.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-32.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli-arm64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/cli.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/dep_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/depends.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/discovery.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/dist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/errors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/extension.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/glob.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-32.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui-arm64.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/gui.exe` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/installer.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/launch.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/logging.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/monkey.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/msvc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/namespaces.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/package_index.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/sandbox.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/windows_support.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/alias.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/build_py.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/develop.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/py36compat.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/rotate.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/sdist.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/setopt.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/test.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/expand.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `unicat-0.2.0/py311/lib/python3.11/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/entry_points.txt` & `unicat-0.2.0/py311/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/_collections.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/connection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/connectionpool.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/exceptions.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/fields.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/filepost.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/poolmanager.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/request.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/response.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_appengine_environ.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/appengine.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/ntlmpool.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/securetransport.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/socks.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/bindings.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/low_level.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/six.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/packages/backports/makefile.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/__init__.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/connection.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/proxy.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/request.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/response.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/retry.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssl_.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/ssltransport.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/timeout.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/url.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3/util/wait.py` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/METADATA` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/RECORD` & `unicat-0.2.0/py311/lib/python3.11/site-packages/urllib3-1.26.14.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/lib-unicat-v0.1.5.zip` & `unicat-0.2.0/src/lib-unicat-v0.1.5.zip`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/api.py` & `unicat-0.2.0/src/unicat/api.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/asset.py` & `unicat-0.2.0/src/unicat/asset.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,25 +44,37 @@
         return self._data["info"]
 
     @property
     def transforms(self):
         return self._data["transforms"]
 
     @property
+    def default_transform(self):
+        return self._data["transforms"].get("_main_", None)
+
+    @property
     def title(self):
         return self._data["title"]
 
     @property
     def description(self):
         return self._data["description"]
 
     @property
     def updated_on(self):
         return self._data["updated_on"]
 
+    def publish(self):
+        public_url = self._unicat.publish_asset(self)
+        return public_url
+
+    def publish_transformed(self, transform=None):
+        public_url = self._unicat.publish_transformed_asset(self, transform=transform)
+        return public_url
+
     def download(self, pathname=None):
         pathname = self._unicat.download_asset(
             self, pathname=pathname, updated_on=self.updated_on
         )
         return pathname
 
     def download_transformed(self, transform=None, pathname=None):
```

### Comparing `unicat-0.1.5/src/unicat/class_.py` & `unicat-0.2.0/src/unicat/class_.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     @property
     def fields(self):
         from .field import UnicatField
 
         return [UnicatField(self._unicat, gid) for gid in self._data["fields"]]
 
     @property
+    def fields_as_gids(self):
+        return self._data["fields"]
+
+    @property
     def layout(self):
         from .layout import UnicatLayout
 
         return UnicatLayout(self._unicat, self._data["layout"])
 
     @property
     def is_new(self):
```

### Comparing `unicat-0.1.5/src/unicat/definition.py` & `unicat-0.2.0/src/unicat/definition.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/error.py` & `unicat-0.2.0/src/unicat/error.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/field.py` & `unicat-0.2.0/src/unicat/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,20 @@
         return self._data["initial"]
 
     @property
     def unit(self):
         return self._data["unit"]
 
     @property
+    def title(self):
+        return {
+            language: f"{label} [{self.unit}]" for language, label in self.label.items()
+        }
+
+    @property
     def is_new(self):
         return self._data["is_new"]
 
     @property
     def is_working_copy(self):
         return self._data["is_working_copy"]
```

### Comparing `unicat-0.1.5/src/unicat/layout.py` & `unicat-0.2.0/src/unicat/layout.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/project.py` & `unicat-0.2.0/src/unicat/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,49 +18,66 @@
         return UnicatUser(self._unicat, self._data["owner"])
 
     @property
     def status(self):
         return self._data["status"]
 
     @property
-    def channels(self):
-        return self._data["options"]["channels"]
+    def languages(self):
+        return self._data["options"]["languages"]
 
-    def channel_key_by_name(self, name):
-        return list(self.channels.keys())[list(self.channels.values()).index(name)]
+    @property
+    def default_language(self):
+        return self._data["options"]["languages"][0]
 
     @property
-    def ordered_channels(self):
-        return self._data["options"]["orderedchannels"]
+    def channels(self):
+        return {
+            self._data["options"]["channels"][key]: key
+            for key in self._data["options"]["orderedchannels"]
+        }
 
     @property
-    def languages(self):
-        return self._data["options"]["languages"]
+    def default_channel(self):
+        return (
+            self._data["options"]["orderedchannels"][1]
+            if len(self._data["options"]["orderedchannels"]) > 1
+            else None
+        )
+
+    def channel_name(self, key):
+        return self._data["options"]["channels"][key]
 
     @property
     def orderings(self):
-        return self._data["options"]["orderings"]
-
-    def ordering_key_by_name(self, name):
-        return list(self.orderings.keys())[list(self.orderings.values()).index(name)]
+        return {
+            self._data["options"]["orderings"][key]: key
+            for key in self._data["options"]["orderedorderings"]
+        }
 
     @property
-    def ordered_orderings(self):
-        return self._data["options"]["orderedorderings"]
+    def default_ordering(self):
+        return self._data["options"]["orderedorderings"][0]
+
+    def ordering_name(self, key):
+        return self._data["options"]["orderings"][key]
 
     @property
     def fieldlists(self):
-        return self._data["options"]["fieldlists"]
-
-    def fieldlist_key_by_name(self, name):
-        return list(self.fieldlists.keys())[list(self.fieldlists.values()).index(name)]
+        return {
+            self._data["options"]["fieldlists"][key]: key
+            for key in self._data["options"]["orderedfieldlists"]
+        }
 
     @property
-    def ordered_fieldlists(self):
-        return self._data["options"]["orderedfieldlists"]
+    def default_fieldlist(self):
+        return self._data["options"]["orderedfieldlists"][0]
+
+    def fieldlist_name(self, key):
+        return self._data["options"]["fieldlists"][key]
 
     @property
     def members(self):
         from .projectmember import UnicatProjectMember
 
         return [
             UnicatProjectMember(self._unicat, project_member)
```

### Comparing `unicat-0.1.5/src/unicat/projectmember.py` & `unicat-0.2.0/src/unicat/projectmember.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/record.py` & `unicat-0.2.0/src/unicat/record.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/record_class_field.py` & `unicat-0.2.0/src/unicat/record_class_field.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/transform.py` & `unicat-0.2.0/src/unicat/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,17 @@
             "padding": self.setPadding,
             "quality": self.setQuality,
             "background": self.setBackground,
             "dpr": self.setDevicePixelRatio,
         }
         for name, value in kwargs.items():
             if name in setters:
-                setters[name](value)
+                setters[name](
+                    *value if type(value) is list or type(value) is tuple else value
+                )
 
     def setName(self, name):
         self.name = str(name)
         return self
 
     def setKey(self, key):
         self.key = str(key)
```

### Comparing `unicat-0.1.5/src/unicat/unicat.py` & `unicat-0.2.0/src/unicat/unicat.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,14 +311,27 @@
 
     def get_schema_query_by_name(self, name):
         return self._get_query_by_type_name("schema", name)
 
     def get_schema_queries_by_name(self, names):
         return self._get_queries_by_type_name("schema", names)
 
+    def publish_asset(self, asset):
+        success, result = self.api.publish(asset._data)
+        if not success:
+            raise UnicatError("publish_asset", result)
+        return result["public_url"]
+
+    def publish_transformed_asset(self, asset, transform=None):
+        options = transformAsOptions(transform)
+        success, result = self.api.transform(asset._data, options=options)
+        if not success:
+            raise UnicatError("publish_transformed_asset", result)
+        return result["public_url"]
+
     def download_asset(self, asset, pathname=None, updated_on=None):
         pathname = self.api.download(
             asset._data, pathname=pathname, updated_on=updated_on
         )
         return pathname
 
     def download_transformed_asset(
```

### Comparing `unicat-0.1.5/src/unicat/utils.py` & `unicat-0.2.0/src/unicat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,14 @@
     try:
         possible_uuid = UUID(possible_gid, version=4)
     except ValueError:
         return False
     return str(possible_uuid) == possible_gid
 
 
-class make_object:
-    def __init__(self, **kwargs):
-        self.__dict__ = kwargs
-
-
-def field_title(field, language):
-    title = field.label[language]
-    if field.unit:
-        title += f" [{field.unit}]"
-    return title
-
-
 def test_false(data):
     return str(data).lower().strip() in (
         "",
         "0",
         "no",
         "n",
         "off",
@@ -45,14 +33,33 @@
     )
 
 
 def test_true(data):
     return not test_false(data)
 
 
+class DuckObject:
+    """Uses keyword arguments to construct any duck-like object with those attributes.
+
+    ```
+    duckquery = DuckObject(
+        q="",
+        filter=["value", "is", [base_artnr_field.gid, article.base_artnr]]
+    )
+    print(duckquery.q, duckquery.filter)
+
+    duckrecord = DuckObject(gid="<anything gid-like>")
+    print(duckrecord.gid)
+    ```
+    """
+
+    def __init__(self, **kwargs):
+        self.__dict__ = kwargs
+
+
 class FieldColumns:
     """FieldColumns are needed for class fields, that have nested subfields.
 
     With FieldColumns, we can flatten a list of fields to a list of columns,
     associated with those fields.
 
     Each column has a fieldstack, that is a list of the field and nested subfields.
@@ -87,15 +94,15 @@
     data structure:
 
     ```
     recordfields_data = {}
     for column in columns:
         fieldvalue = row[column.index].value
         column.update_fields_data(recordfields_data, fieldvalue)
-    unicat.update_record(gid, language, recordfields_data)
+    unicat.mutate.update_record(record, {language: recordfields_data})
     ```
     """
 
     def __init__(self, fields, prefix_column_count=0):
         self._columns = []
         index = prefix_column_count
         for fieldstack in self._flatten_fields(fields, []):
```

### Comparing `unicat-0.1.5/src/unicat/mutate/__init__.py` & `unicat-0.2.0/src/unicat/mutate/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,38 +21,57 @@
         self.delete_fieldlist = self._wrap(delete_fieldlist)
 
         self.create_definition = self._wrap(create_definition)
         self.modify_definition = self._wrap(modify_definition)
         self.modify_definition_modify_layout = self._wrap(
             modify_definition_modify_layout
         )
+        self.modify_definition_add_class = self._wrap(modify_definition_add_class)
+        self.modify_definition_remove_class = self._wrap(modify_definition_remove_class)
+        self.modify_definition_add_field = self._wrap(modify_definition_add_field)
+        self.modify_definition_remove_field = self._wrap(modify_definition_remove_field)
+        self.modify_definition_fieldlist_add_field = self._wrap(
+            modify_definition_fieldlist_add_field
+        )
+        self.modify_definition_fieldlist_remove_field = self._wrap(
+            modify_definition_fieldlist_remove_field
+        )
         self.modify_definition_add_childdefinition = self._wrap(
             modify_definition_add_childdefinition
         )
         self.modify_definition_remove_childdefinition = self._wrap(
             modify_definition_remove_childdefinition
         )
         self.commit_definition = self._wrap(commit_definition)
+        self.save_as_new_definition = self._wrap(save_as_new_definition)
         self.delete_definition = self._wrap(delete_definition)
 
         self.create_class = self._wrap(create_class)
         self.modify_class = self._wrap(modify_class)
         self.modify_class_modify_layout = self._wrap(modify_class_modify_layout)
+        self.modify_class_add_field = self._wrap(modify_class_add_field)
+        self.modify_class_remove_field = self._wrap(modify_class_remove_field)
         self.commit_class = self._wrap(commit_class)
+        self.save_as_new_class = self._wrap(save_as_new_class)
         self.delete_class = self._wrap(delete_class)
 
         self.create_field = self._wrap(create_field)
         self.modify_field = self._wrap(modify_field)
         self.commit_field = self._wrap(commit_field)
+        self.save_as_new_field = self._wrap(save_as_new_field)
         self.delete_field = self._wrap(delete_field)
 
         self.create_record = self._wrap(create_record)
         self.set_record_definition = self._wrap(set_record_definition)
-        self.add_record_definition_class = self._wrap(add_record_definition_class)
-        self.add_record_definition_field = self._wrap(add_record_definition_field)
+        self.extend_record_definition_add_class = self._wrap(
+            extend_record_definition_add_class
+        )
+        self.extend_record_definition_add_field = self._wrap(
+            extend_record_definition_add_field
+        )
         self.update_record = self._wrap(update_record)
         self.set_record_channels = self._wrap(set_record_channels)
         self.set_record_orderings = self._wrap(set_record_orderings)
         self.link_record = self._wrap(link_record)
         self.delete_record = self._wrap(delete_record)
         self.undelete_record = self._wrap(undelete_record)
         self.permanent_delete_record = self._wrap(permanent_delete_record)
```

### Comparing `unicat-0.1.5/src/unicat/mutate/assets.py` & `unicat-0.2.0/src/unicat/mutate/assets.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/mutate/classes.py` & `unicat-0.2.0/src/unicat/mutate/fields.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from ..class_ import UnicatClass
+from ..field import UnicatField
 from ..error import UnicatError
 
 
-def create_class(unicat, properties):
-    success, result = unicat.api.call("/classes/create", properties)
+def create_field(unicat, properties):
+    success, result = unicat.api.call("/fields/create", properties)
     if not success:
-        raise UnicatError("create_class", result)
-    return UnicatClass(unicat, result["class"])
+        raise UnicatError("create_field", result)
+    return UnicatField(unicat, result["field"])
 
 
-def modify_class(unicat, class_, properties):
+def modify_field(unicat, field, properties):
     success, result = unicat.api.call(
-        "/classes/modify",
-        {**properties, "class": class_.gid},
+        "/fields/modify",
+        {**properties, "field": field.gid},
     )
     if not success:
-        raise UnicatError("modify_class", result)
-    return UnicatClass(unicat, result["class"])
+        raise UnicatError("modify_field", result)
+    return UnicatField(unicat, result["field"])
 
 
-def modify_class_modify_layout(unicat, class_, layout_properties):
+def commit_field(unicat, new_or_working_copy):
     success, result = unicat.api.call(
-        "/classes/layouts/modify",
-        {**layout_properties, "class": class_.gid},
+        "/fields/commit", {"field": new_or_working_copy.gid}
     )
     if not success:
-        raise UnicatError("modify_class_modify_layout", result)
-    return UnicatClass(unicat, result["class"])
+        raise UnicatError("commit_field", result)
+    if (
+        result["field"] != new_or_working_copy.gid
+        and new_or_working_copy.gid in unicat.api.data["fields"]
+    ):
+        del unicat.api.data["fields"][new_or_working_copy.gid]
+    return UnicatField(unicat, result["field"])
 
 
-def commit_class(unicat, new_or_working_copy):
+def save_as_new_field(unicat, working_copy):
     success, result = unicat.api.call(
-        "/classes/commit", {"class": new_or_working_copy.gid}
+        "/fields/save_as_new", {"field": working_copy.gid}
     )
     if not success:
-        raise UnicatError("commit_class", result)
-    if (
-        result["class"] != new_or_working_copy.gid
-        and new_or_working_copy.gid in unicat.api.data["classes"]
-    ):
-        del unicat.api.data["classes"][new_or_working_copy.gid]
-    return UnicatClass(unicat, result["class"])
+        raise UnicatError("save_as_new_field", result)
+    return UnicatField(unicat, result["field"])
 
 
-def delete_class(unicat, class_):
-    success, result = unicat.api.call("/classes/delete", {"class": class_.gid})
+def delete_field(unicat, field):
+    success, result = unicat.api.call("/fields/delete", {"field": field.gid})
     if not success:
-        raise UnicatError("delete_class", result)
-    if class_.gid in unicat.api.data["classes"]:
-        del unicat.api.data["classes"][class_.gid]
+        raise UnicatError("delete_field", result)
+    if field.gid in unicat.api.data["fields"]:
+        del unicat.api.data["fields"][field.gid]
     return True
```

### Comparing `unicat-0.1.5/src/unicat/mutate/fields.py` & `unicat-0.2.0/src/unicat/mutate/queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-from ..field import UnicatField
+from ..query import UnicatQuery
 from ..error import UnicatError
 
 
-def create_field(unicat, properties):
-    success, result = unicat.api.call("/fields/create", properties)
+def create_query(unicat, properties):
+    success, result = unicat.api.call("/queries/create", properties)
     if not success:
-        raise UnicatError("create_field", result)
-    return UnicatField(unicat, result["field"])
+        raise UnicatError("create_query", result)
+    return UnicatQuery(unicat, result["query"])
 
 
-def modify_field(unicat, field, properties):
+def update_query(unicat, query, properties):
     success, result = unicat.api.call(
-        "/fields/modify",
-        {**properties, "field": field.gid},
+        "/queries/update",
+        {**properties, "query": query.gid},
     )
     if not success:
-        raise UnicatError("modify_field", result)
-    return UnicatField(unicat, result["field"])
+        raise UnicatError("update_query", result)
+    return UnicatQuery(unicat, result["query"])
 
 
-def commit_field(unicat, new_or_working_copy):
-    success, result = unicat.api.call(
-        "/fields/commit", {"field": new_or_working_copy.gid}
-    )
-    if not success:
-        raise UnicatError("commit_field", result)
-    if (
-        result["field"] != new_or_working_copy.gid
-        and new_or_working_copy.gid in unicat.api.data["fields"]
-    ):
-        del unicat.api.data["fields"][new_or_working_copy.gid]
-    return UnicatField(unicat, result["field"])
-
-
-def delete_field(unicat, field):
-    success, result = unicat.api.call("/fields/delete", {"field": field.gid})
+def delete_query(unicat, query):
+    success, result = unicat.api.call("/queries/delete", {"query": query.gid})
     if not success:
-        raise UnicatError("delete_field", result)
-    if field.gid in unicat.api.data["fields"]:
-        del unicat.api.data["fields"][field.gid]
+        raise UnicatError("delete_query", result)
+    if query.gid in unicat.api.data["queries"]:
+        del unicat.api.data["queries"][query.gid]
     return True
```

### Comparing `unicat-0.1.5/src/unicat/mutate/project.py` & `unicat-0.2.0/src/unicat/mutate/project.py`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/src/unicat/mutate/records.py` & `unicat-0.2.0/src/unicat/mutate/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
         {"record": record.gid, "definition": definition.gid},
     )
     if not success:
         raise UnicatError("set_record_definition", result)
     return UnicatRecord(unicat, result["record"])
 
 
-def add_record_definition_class(unicat, record, class_):
+def extend_record_definition_add_class(unicat, record, class_):
     success, result = unicat.api.call(
         "/records/definition/classes/add",
         {"record": record.gid, "class": class_.gid},
     )
     if not success:
-        raise UnicatError("add_record_definition_class", result)
+        raise UnicatError("extend_record_definition_add_class", result)
     return UnicatRecord(unicat, result["record"])
 
 
-def add_record_definition_field(unicat, record, field):
+def extend_record_definition_add_field(unicat, record, field):
     success, result = unicat.api.call(
         "/records/definition/fields/add",
         {"record": record.gid, "field": field.gid},
     )
     if not success:
-        raise UnicatError("add_record_definition_field", result)
+        raise UnicatError("extend_record_definition_add_field", result)
     return UnicatRecord(unicat, result["record"])
 
 
 def update_record(unicat, record, localizedfielddata):
     success, result = unicat.api.call(
         "/records/update", {"record": record.gid, "fields": localizedfielddata}
     )
```

### Comparing `unicat-0.1.5/.gitignore` & `unicat-0.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -111,7 +111,9 @@
 /unicat-connect/modules/dev/dist
 .env
 /unicat-connect/modules/migrate-from-catalogger/.env.sandbox
 /unicat-connect/modules/migrate-from-catalogger/upload-partner-safety-test.sh
 /unicat-connect/modules/stentor-connect/build
 /unicat-connect/modules/stentor-connect/dist
 /docs/res/unicat-connect
+/unicat-connect/pypi-unicat/py311
+/unicat-connect/pypi-unicat/dist
```

### Comparing `unicat-0.1.5/LICENSE` & `unicat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicat-0.1.5/pyproject.toml` & `unicat-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "unicat"
-version = "0.1.5"
-description = "Unicat client library"
+version = "0.2.0"
+description = "Unicat client library - Unicat is a Product Information Management SaaS."
 readme = "README.md"
 authors = [
   { name="Marc Boeren", email="m.boeren@guidance.nl" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.11"
 dependencies = [
-    "requests >= 2.28",
-    "openpyxl >= 3.0",
-    "defusedxml >= 0.7",
+    "requests >= 2.28"
 ]
```

