# Comparing `tmp/elementpath-4.1.0.tar.gz` & `tmp/elementpath-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementpath-4.1.0.tar", last modified: Tue Mar 21 14:33:22 2023, max compression
+gzip compressed data, was "elementpath-4.1.1.tar", last modified: Tue Apr 11 07:40:51 2023, max compression
```

## Comparing `elementpath-4.1.0.tar` & `elementpath-4.1.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.835602 elementpath-4.1.0/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.0/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15312 2023-03-21 14:20:17.000000 elementpath-4.1.0/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.0/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.0/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6375 2023-03-21 14:33:22.835602 elementpath-4.1.0/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5034 2023-03-21 14:20:17.000000 elementpath-4.1.0/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.806602 elementpath-4.1.0/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.0/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.0/doc/advanced.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-03-21 14:20:18.000000 elementpath-4.1.0/doc/conf.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.0/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.0/doc/introduction.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.0/doc/make.bat
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.0/doc/pratt_api.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.0/doc/xpath_api.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.811602 elementpath-4.1.0/elementpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.0/elementpath/collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.0/elementpath/compare.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.815602 elementpath-4.1.0/elementpath/datatypes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6774 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.0/elementpath/datatypes/atomic_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/binary.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    39612 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/datetime.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/numeric.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/proxies.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/qname.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/string.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/datatypes/untyped.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.0/elementpath/datatypes/uri.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9264 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.0/elementpath/protocols.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.0/elementpath/py.typed
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.817602 elementpath-4.1.0/elementpath/regex/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.0/elementpath/regex/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.0/elementpath/regex/character_classes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.0/elementpath/regex/codepoints.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4028 2021-11-06 21:19:58.000000 elementpath-4.1.0/elementpath/regex/generate_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/regex/patterns.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.0/elementpath/regex/unicode_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/regex/unicode_subsets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13475 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17093 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35171 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/tdop.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    12708 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/tree_builders.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.818602 elementpath-4.1.0/elementpath/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/validators/analyze-string.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/validators/schema-for-json.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.819602 elementpath-4.1.0/elementpath/xpath1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.0/elementpath/xpath1/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3802 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/xpath1/_xpath1_axes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16812 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/xpath1/_xpath1_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28748 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath1/_xpath1_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath1/xpath1_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.820602 elementpath-4.1.0/elementpath/xpath2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.0/elementpath/xpath2/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19420 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/xpath2/_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    60218 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath2/_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30844 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath2/_xpath2_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24626 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath2/xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.822602 elementpath-4.1.0/elementpath/xpath30/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.0/elementpath/xpath30/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.0/elementpath/xpath30/_translation_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67756 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath30/_xpath30_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8110 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath30/_xpath30_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath30/xpath30_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3706 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath30/xpath30_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.823602 elementpath-4.1.0/elementpath/xpath31/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.0/elementpath/xpath31/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49068 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath31/_xpath31_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8205 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath31/_xpath31_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.0/elementpath/xpath31/xpath31_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20638 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    29981 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath_nodes.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6118 2023-03-01 07:00:44.000000 elementpath-4.1.0/elementpath/xpath_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    73776 2023-03-21 14:20:18.000000 elementpath-4.1.0/elementpath/xpath_tokens.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.813602 elementpath-4.1.0/elementpath.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6375 2023-03-21 14:33:22.000000 elementpath-4.1.0/elementpath.egg-info/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3450 2023-03-21 14:33:22.000000 elementpath-4.1.0/elementpath.egg-info/SOURCES.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-03-21 14:33:22.000000 elementpath-4.1.0/elementpath.egg-info/dependency_links.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-03-21 14:33:22.000000 elementpath-4.1.0/elementpath.egg-info/requires.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-03-21 14:33:22.000000 elementpath-4.1.0/elementpath.egg-info/top_level.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.0/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-02-01 12:54:01.000000 elementpath-4.1.0/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-03-21 14:33:22.835602 elementpath-4.1.0/setup.cfg
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2296 2023-03-21 14:20:18.000000 elementpath-4.1.0/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.832602 elementpath-4.1.0/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.0/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/execute_w3c_tests.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/memory_profiling.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.832602 elementpath-4.1.0/tests/mypy_tests/
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2021-11-06 19:48:44.000000 elementpath-4.1.0/tests/mypy_tests/selectors.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-21 14:33:22.834602 elementpath-4.1.0/tests/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.0/tests/resources/analyze-string.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.0/tests/resources/sample.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/resources/schema-for-json.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/resources/unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/resources/unused_external_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/resources/unused_unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_compare.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_datatypes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.0/tests/test_elementpath.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11984 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.0/tests/test_namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_regex.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_schema_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3790 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8120 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14616 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_tdop_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7098 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_tree_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1887 2023-03-01 06:49:20.000000 elementpath-4.1.0/tests/test_typing.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_validators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    83318 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath1_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66728 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    57332 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath30.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath31.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.0/tests/test_xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16701 2023-02-01 12:54:01.000000 elementpath-4.1.0/tests/test_xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/test_xpath_tokens.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11906 2023-03-21 14:20:19.000000 elementpath-4.1.0/tests/xpath_test_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1421 2023-03-21 14:20:19.000000 elementpath-4.1.0/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.358302 elementpath-4.1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.1/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15546 2023-04-11 07:36:42.000000 elementpath-4.1.1/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.1/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.1/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6235 2023-04-11 07:40:51.357302 elementpath-4.1.1/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:37:27.000000 elementpath-4.1.1/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.325302 elementpath-4.1.1/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.1/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.1/doc/advanced.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-04-11 07:36:42.000000 elementpath-4.1.1/doc/conf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.1/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.1/doc/introduction.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.1/doc/make.bat
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.1/doc/pratt_api.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.1/doc/xpath_api.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.331302 elementpath-4.1.1/elementpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.1/elementpath/collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.1/elementpath/compare.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.337302 elementpath-4.1.1/elementpath/datatypes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/datatypes/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.1/elementpath/datatypes/atomic_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/binary.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/datatypes/datetime.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/numeric.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/proxies.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/qname.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/string.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/untyped.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.1/elementpath/datatypes/uri.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.1/elementpath/protocols.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.1/elementpath/py.typed
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.339302 elementpath-4.1.1/elementpath/regex/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.1/elementpath/regex/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.1/elementpath/regex/character_classes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.1/elementpath/regex/codepoints.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/regex/generate_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/regex/patterns.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.1/elementpath/regex/unicode_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/regex/unicode_subsets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17093 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35171 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/tdop.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12844 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/tree_builders.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.339302 elementpath-4.1.1/elementpath/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/validators/analyze-string.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/validators/schema-for-json.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.340302 elementpath-4.1.1/elementpath/xpath1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.1/elementpath/xpath1/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_axes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28755 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/xpath1/xpath1_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.342302 elementpath-4.1.1/elementpath/xpath2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.1/elementpath/xpath2/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.343302 elementpath-4.1.1/elementpath/xpath30/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.1/elementpath/xpath30/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.1/elementpath/xpath30/_translation_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67763 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/_xpath30_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/_xpath30_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/xpath30/xpath30_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/xpath30_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.344302 elementpath-4.1.1/elementpath/xpath31/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.1/elementpath/xpath31/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath31/_xpath31_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath31/_xpath31_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/xpath31/xpath31_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    29844 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_tokens.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.333302 elementpath-4.1.1/elementpath.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6235 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3450 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/SOURCES.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/dependency_links.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/requires.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/top_level.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.1/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-02-01 12:54:01.000000 elementpath-4.1.1/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-04-11 07:40:51.358302 elementpath-4.1.1/setup.cfg
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2296 2023-04-11 07:36:42.000000 elementpath-4.1.1/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.354302 elementpath-4.1.1/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.1/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/execute_w3c_tests.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/memory_profiling.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.355302 elementpath-4.1.1/tests/mypy_tests/
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2021-11-06 19:48:44.000000 elementpath-4.1.1/tests/mypy_tests/selectors.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.356302 elementpath-4.1.1/tests/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.1/tests/resources/analyze-string.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.1/tests/resources/sample.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/resources/schema-for-json.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unused_external_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unused_unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_compare.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_datatypes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.1/tests/test_elementpath.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_regex.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_schema_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3790 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15390 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14616 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_tdop_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7098 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_tree_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1887 2023-03-01 06:49:20.000000 elementpath-4.1.1/tests/test_typing.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_validators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    83882 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_xpath1_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    57332 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath30.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath31.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/test_xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16701 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath_tokens.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11906 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/xpath_test_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1429 2023-04-11 07:36:42.000000 elementpath-4.1.1/tox.ini
```

### Comparing `elementpath-4.1.0/CHANGELOG.rst` & `elementpath-4.1.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v4.1.1`_ (2023-04-11)
+======================
+* Simplify type annotations for XSD datatypes
+* Full test coverage of sequence type functions with bugfixes
+
 `v4.1.0`_ (2023-03-21)
 ======================
 * Refactor XPath function call (context=None only as keyword argument)
 * Add external function support (issue #60)
 * Some fixes to string representation and source property of tokens
 * Extend documentation and tests
 * Clean XSD datatypes hierarchy
@@ -402,7 +407,8 @@
 .. _v2.5.3: https://github.com/sissaschool/elementpath/compare/v2.5.2...v2.5.3
 .. _v3.0.0: https://github.com/sissaschool/elementpath/compare/v2.5.3...v3.0.0
 .. _v3.0.1: https://github.com/sissaschool/elementpath/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/sissaschool/elementpath/compare/v3.0.1...v3.0.2
 .. _v4.0.0: https://github.com/sissaschool/elementpath/compare/v3.0.2...v4.0.0
 .. _v4.0.1: https://github.com/sissaschool/elementpath/compare/v4.0.0...v4.0.1
 .. _v4.1.0: https://github.com/sissaschool/elementpath/compare/v4.0.1...v4.1.0
+.. _v4.1.1: https://github.com/sissaschool/elementpath/compare/v4.1.0...v4.1.1
```

### Comparing `elementpath-4.1.0/LICENSE` & `elementpath-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/PKG-INFO` & `elementpath-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.0
+Version: 4.1.1
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,16 +38,14 @@
 .. image:: https://img.shields.io/pypi/pyversions/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/pypi/implementation/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/badge/License-MIT-blue.svg
    :alt: MIT License
    :target: https://lbesson.mit-license.org/
-.. image:: https://travis-ci.org/sissaschool/elementpath.svg?branch=master
-   :target: https://travis-ci.org/sissaschool/elementpath
 .. image:: https://img.shields.io/pypi/dm/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 
 .. elementpath-introduction
 
 The proposal of this package is to provide XPath 1.0, 2.0, 3.0 and 3.1
 selectors for ElementTree XML data structures, both for the standard
@@ -137,15 +135,15 @@
 
 The XPath parsers are based on an implementation of the Pratt's Top Down Operator Precedence parser.
 The implemented parser includes some lookup-ahead features, helpers for registering tokens and for
 extending language implementations. Also the token class has been generalized using a `MutableSequence`
 as base class. See *tdop.py* for the basic internal classes and *xpath1_parser.py* for extensions
 and for a basic usage of the parser.
 
-If you like you can use the basic parser and tokens provided by the *tdop_parser.py* module to
+If you like you can use the basic parser and tokens provided by the *tdop.py* module to
 implement other types of parsers (I think it could be also a funny exercise!).
 
 
 License
 =======
 
 This software is distributed under the terms of the MIT License.
```

### Comparing `elementpath-4.1.0/README.rst` & `elementpath-4.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 .. image:: https://img.shields.io/pypi/pyversions/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/pypi/implementation/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/badge/License-MIT-blue.svg
    :alt: MIT License
    :target: https://lbesson.mit-license.org/
-.. image:: https://travis-ci.org/sissaschool/elementpath.svg?branch=master
-   :target: https://travis-ci.org/sissaschool/elementpath
 .. image:: https://img.shields.io/pypi/dm/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 
 .. elementpath-introduction
 
 The proposal of this package is to provide XPath 1.0, 2.0, 3.0 and 3.1
 selectors for ElementTree XML data structures, both for the standard
@@ -106,15 +104,15 @@
 
 The XPath parsers are based on an implementation of the Pratt's Top Down Operator Precedence parser.
 The implemented parser includes some lookup-ahead features, helpers for registering tokens and for
 extending language implementations. Also the token class has been generalized using a `MutableSequence`
 as base class. See *tdop.py* for the basic internal classes and *xpath1_parser.py* for extensions
 and for a basic usage of the parser.
 
-If you like you can use the basic parser and tokens provided by the *tdop_parser.py* module to
+If you like you can use the basic parser and tokens provided by the *tdop.py* module to
 implement other types of parsers (I think it could be also a funny exercise!).
 
 
 License
 =======
 
 This software is distributed under the terms of the MIT License.
```

### Comparing `elementpath-4.1.0/doc/Makefile` & `elementpath-4.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/doc/advanced.rst` & `elementpath-4.1.1/doc/advanced.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/doc/conf.py` & `elementpath-4.1.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = 'elementpath'
 copyright = '2018-2023, SISSA (International School for Advanced Studies)'
 author = 'Davide Brunato'
 
 # The short X.Y version
 version = '4.1'
 # The full version, including alpha/beta/rc tags
-release = '4.1.0'
+release = '4.1.1'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `elementpath-4.1.0/doc/make.bat` & `elementpath-4.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/doc/pratt_api.rst` & `elementpath-4.1.1/doc/pratt_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/doc/xpath_api.rst` & `elementpath-4.1.1/doc/xpath_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/__init__.py` & `elementpath-4.1.1/elementpath/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-__version__ = '4.1.0'
+__version__ = '4.1.1'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2018-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 # Imports here are considered as stable API, other internal calls may change.
```

### Comparing `elementpath-4.1.0/elementpath/collations.py` & `elementpath-4.1.1/elementpath/collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/compare.py` & `elementpath-4.1.1/elementpath/compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/__init__.py` & `elementpath-4.1.1/elementpath/datatypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,16 @@
 from .proxies import BooleanProxy, DecimalProxy, DoubleProxy10, DoubleProxy, \
     StringProxy, NumericProxy, ArithmeticProxy
 
 xsd11_atomic_types.update(
     (k, v) for k, v in xsd10_atomic_types.items() if k not in xsd11_atomic_types
 )
 
-DatetimeValueType = Union[OrderedDateTime, Date10, Date, DateTime10, DateTime, Time,
-                          GregorianDay, GregorianMonth, GregorianMonthDay, GregorianYear10,
-                          GregorianYear, GregorianYearMonth10, GregorianYearMonth]
-
-AtomicValueType = Union[str, int, float, Decimal, bool, Integer, Float10, NormalizedString,
-                        AnyURI, HexBinary, Base64Binary, QName, AbstractDateTime, Duration,
-                        UntypedAtomic, DatetimeValueType]
+DatetimeValueType = AbstractDateTime  # keep until v5.0 for backward compatibility
+AtomicValueType = Union[str, int, float, Decimal, bool, AnyAtomicType]
 
 
 ATOMIC_VALUES: Dict[Optional[str], AtomicValueType] = {
     f'{{{XSD_NAMESPACE}}}untypedAtomic': UntypedAtomic('1'),
     f'{{{XSD_NAMESPACE}}}anyType': UntypedAtomic('1'),
     f'{{{XSD_NAMESPACE}}}anySimpleType': UntypedAtomic('1'),
     f'{{{XSD_NAMESPACE}}}anyAtomicType': UntypedAtomic('1'),
```

### Comparing `elementpath-4.1.0/elementpath/datatypes/atomic_types.py` & `elementpath-4.1.1/elementpath/datatypes/atomic_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/binary.py` & `elementpath-4.1.1/elementpath/datatypes/binary.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/datetime.py` & `elementpath-4.1.1/elementpath/datatypes/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,39 @@
 
         if self.tzinfo is not None:
             arg_string += ', tzinfo=%r' % self.tzinfo
         return '%s(%s)' % (self.__class__.__name__, arg_string)
 
     @abstractmethod
     def __str__(self) -> str:
-        raise NotImplementedError()
+        raise NotImplementedError
+
+    @abstractmethod
+    def __lt__(self, other: object) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __le__(self, other: object) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __gt__(self, other: object) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __ge__(self, other: object) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __add__(self, other: object) -> Any:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __sub__(self, other: object) -> Any:
+        raise NotImplementedError
 
     @property
     def year(self) -> int:
         return self._year or self._dt.year
 
     @property
     def bce(self) -> bool:
@@ -344,15 +368,15 @@
             return True
 
 
 class OrderedDateTime(AbstractDateTime):
 
     @abstractmethod
     def __str__(self) -> str:
-        raise NotImplementedError()
+        raise NotImplementedError
 
     @classmethod
     def fromdelta(cls, delta: datetime.timedelta, adjust_timezone: bool = False) \
             -> 'OrderedDateTime':
         """
         Creates an XSD dateTime/date instance from a datetime.timedelta related to
         0001-01-01T00:00:00 CE. In case of a date the time part is not counted.
```

### Comparing `elementpath-4.1.0/elementpath/datatypes/numeric.py` & `elementpath-4.1.1/elementpath/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/proxies.py` & `elementpath-4.1.1/elementpath/datatypes/proxies.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/qname.py` & `elementpath-4.1.1/elementpath/datatypes/qname.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/string.py` & `elementpath-4.1.1/elementpath/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/untyped.py` & `elementpath-4.1.1/elementpath/datatypes/untyped.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/datatypes/uri.py` & `elementpath-4.1.1/elementpath/datatypes/uri.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/etree.py` & `elementpath-4.1.1/elementpath/etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/exceptions.py` & `elementpath-4.1.1/elementpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/helpers.py` & `elementpath-4.1.1/elementpath/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,24 +57,14 @@
 def is_idrefs(value: Optional[str]) -> bool:
     return isinstance(value, str) and \
         all(NCNAME_PATTERN.match(x) is not None for x in value.split())
 
 
 node_position = attrgetter('position')
 
-###
-# Sequence type checking
-SEQUENCE_TYPE_PATTERN = re.compile(r'\s?([()?*+,])\s?')
-
-
-def normalize_sequence_type(sequence_type: str) -> str:
-    sequence_type = WHITESPACES_PATTERN.sub(' ', sequence_type).strip()
-    sequence_type = SEQUENCE_TYPE_PATTERN.sub(r'\1', sequence_type)
-    return sequence_type.replace(',', ', ').replace(')as', ') as')
-
 
 ###
 # Date/Time helpers
 MONTH_DAYS = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 MONTH_DAYS_LEAP = [0, 31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
```

### Comparing `elementpath-4.1.0/elementpath/namespaces.py` & `elementpath-4.1.1/elementpath/namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/protocols.py` & `elementpath-4.1.1/elementpath/protocols.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/__init__.py` & `elementpath-4.1.1/elementpath/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/character_classes.py` & `elementpath-4.1.1/elementpath/regex/character_classes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/codepoints.py` & `elementpath-4.1.1/elementpath/regex/codepoints.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/generate_categories.py` & `elementpath-4.1.1/elementpath/regex/generate_categories.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """Codepoints module generator utility."""
 
 CATEGORIES_TEMPLATE = """#
 # Copyright (c), 2018-2020, SISSA (International School for Advanced Studies).
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
```

### Comparing `elementpath-4.1.0/elementpath/regex/patterns.py` & `elementpath-4.1.1/elementpath/regex/patterns.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/unicode_categories.py` & `elementpath-4.1.1/elementpath/regex/unicode_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/regex/unicode_subsets.py` & `elementpath-4.1.1/elementpath/regex/unicode_subsets.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/schema_proxy.py` & `elementpath-4.1.1/elementpath/schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/sequence_types.py` & `elementpath-4.1.1/elementpath/sequence_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
+import re
 from itertools import zip_longest
 from typing import TYPE_CHECKING, cast, Any, Optional
 
 from .exceptions import ElementPathKeyError, xpath_error
-from .helpers import OCCURRENCE_INDICATORS, EQNAME_PATTERN, normalize_sequence_type
+from .helpers import OCCURRENCE_INDICATORS, EQNAME_PATTERN, WHITESPACES_PATTERN
 from .namespaces import XSD_NAMESPACE, XSD_ERROR, XSD_ANY_SIMPLE_TYPE, XSD_NUMERIC, \
     get_expanded_name
 from .datatypes import xsd10_atomic_types, xsd11_atomic_types, AnyAtomicType, \
     QName, NumericProxy
 from .xpath_nodes import XPathNode, DocumentNode, ElementNode, AttributeNode
 from . import xpath_tokens
 
@@ -37,17 +38,29 @@
     'xs:nonPositiveInteger', 'xs:nonNegativeInteger', 'xs:unsignedLong',
     'xs:unsignedInt', 'xs:unsignedShort', 'xs:unsignedByte',
     'xs:untyped', 'xs:untypedAtomic', 'attribute()', 'attribute(*)',
     'element()', 'element(*)', 'text()', 'document-node()', 'comment()',
     'processing-instruction()', 'item()', 'node()', 'numeric'
 }
 
+###
+# Sequence type checking
+SEQUENCE_TYPE_PATTERN = re.compile(r'\s?([()?*+,])\s?')
+
+
+def normalize_sequence_type(sequence_type: str) -> str:
+    sequence_type = WHITESPACES_PATTERN.sub(' ', sequence_type).strip()
+    sequence_type = SEQUENCE_TYPE_PATTERN.sub(r'\1', sequence_type)
+    return sequence_type.replace(',', ', ').replace(')as', ') as')
+
 
 def is_sequence_type_restriction(st1: str, st2: str) -> bool:
     """Returns `True` if st2 is a restriction of st1."""
+    st1, st2 = normalize_sequence_type(st1), normalize_sequence_type(st2)
+
     if st2 in ('empty-sequence()', 'none') and \
             (st1 in ('empty-sequence()', 'none') or st1.endswith(('?', '*'))):
         return True
 
     # check occurrences
     if st1[-1] not in '?+*':
         if st2[-1] in '+*':
@@ -166,15 +179,15 @@
         elif st[-1] in OCCURRENCE_INDICATORS:
             st = st[:-1]
 
         if st in COMMON_SEQUENCE_TYPES:
             return True
 
         elif st.startswith(('map(', 'array(')):
-            if version < '3.1' or not st.endswith(')'):
+            if parser and parser.version < '3.1' or not st.endswith(')'):
                 return False
 
             if st in ('map(*)', 'array(*)'):
                 return True
 
             if st.startswith('map('):
                 key_type, _, value_type = st[4:-1].partition(', ')
@@ -199,64 +212,59 @@
 
         elif st.startswith('document-node(') and st.endswith(')'):
             if not st.startswith('document-node(element('):
                 return False
             return is_st(st[14:-1])
 
         elif st.startswith('function('):
-            if getattr(parser, 'version', '1.0') >= '3.0':
-                if st == 'function(*)':
-                    return True
-                elif ' as ' in st:
-                    pass
-                elif not st.endswith(')'):
-                    return False
-                else:
-                    return is_st(st[9:-1])
-
-            try:
-                st, return_type = st.rsplit(' as ', 1)
-            except ValueError:
+            if parser and parser.version < '3.0':
+                return False
+            elif st == 'function(*)':
+                return True
+            elif ' as ' in st:
+                pass
+            elif not st.endswith(')'):
                 return False
             else:
-                if not is_st(return_type):
-                    return False
-                elif st == 'function()':
-                    return True
+                return is_st(st[9:-1])
 
-                st = st[9:-1]
-                if st.endswith(', ...'):
-                    st = st[:-5]
-
-                if 'function(' not in st:
-                    return all(is_st(x) for x in st.split(', '))
-                elif st.startswith('function(*)') and 'function(' not in st[11:]:
-                    return all(is_st(x) for x in st.split(', '))
-
-                # Cover only if function() spec is the last argument
-                k = st.index('function(')
-                if not is_st(st[k:]):
-                    return False
-                return all(is_st(x) for x in st[:k].split(', ') if x)
+            st, return_type = st.rsplit(' as ', 1)
+            if not is_st(return_type):
+                return False
+            elif st == 'function()':
+                return True
+
+            st = st[9:-1]
+            if st.endswith(', ...'):
+                st = st[:-5]
+
+            if 'function(' not in st:
+                return all(is_st(x) for x in st.split(', '))
+            elif st.startswith('function(*)') and 'function(' not in st[11:]:
+                return all(is_st(x) for x in st.split(', '))
+
+            # Cover only if function() spec is the last argument
+            k = st.index('function(')
+            if not is_st(st[k:]):
+                return False
+            return all(is_st(x) for x in st[:k].split(', ') if x)
 
         elif QName.pattern.match(st) is None:
             return False
 
         if parser is None:
             return False
 
         try:
             is_instance(None, st, parser)
         except (KeyError, ValueError):
             return False
         else:
             return True
 
-    version = '2.0' if parser is None else parser.version
-
     if not isinstance(value, str):
         return False
     return is_st(normalize_sequence_type(value))
 
 
 def match_sequence_type(value: Any,
                         sequence_type: str,
@@ -319,17 +327,15 @@
         elif '(' in st:
             return False
         elif not strict and st == 'xs:anyURI' and isinstance(v, str):
             return True
         else:
             try:
                 return is_instance(v, st, parser)
-            except ValueError:
-                return False
-            except KeyError:
+            except (KeyError, ValueError):
                 raise xpath_error('XPST0051')
 
         if st == 'node()':
             return True
         elif not st.startswith(value_kind) or not st.endswith(')'):
             return False
         elif st == f'{value_kind}()':
@@ -342,40 +348,40 @@
             return any(
                 match_st(e, element_test) for e in document if isinstance(e, ElementNode)
             )
         elif value_kind not in ('element', 'attribute'):
             return False
 
         _, params = st[:-1].split('(')
-        if ',' not in st:
+        if ', ' not in st:
             name = params
         else:
-            name, type_name = params.split(',')
+            name, type_name = params.rsplit(', ', 1)
             if type_name.endswith('?'):
                 type_name = type_name[:-1]
             elif isinstance(v, ElementNode) and v.nilled:
                 return False
 
             if type_name == 'xs:untyped':
                 if isinstance(v, (ElementNode, AttributeNode)) \
                         and v.xsd_type is not None:
                     return False
             else:
                 try:
-                    if not is_instance(v, type_name, parser):
+                    if not is_instance(v.typed_value, type_name, parser):
                         return False
-                except ValueError:
-                    return False
-                except KeyError:
+                except (KeyError, ValueError):
                     raise xpath_error('XPST0051')
 
         if name == '*':
             return True
 
         try:
             exp_name = get_expanded_name(name, parser.namespaces)  # type: ignore[union-attr]
-        except (KeyError, ValueError, AttributeError):
+        except (KeyError, ValueError):
             return False
+        except AttributeError:
+            return True if v.name == name else False
         else:
             return True if v.name == exp_name else False
 
-    return match_st(value, sequence_type)
+    return match_st(value, normalize_sequence_type(sequence_type))
```

### Comparing `elementpath-4.1.0/elementpath/serialization.py` & `elementpath-4.1.1/elementpath/serialization.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/tdop.py` & `elementpath-4.1.1/elementpath/tdop.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/tree_builders.py` & `elementpath-4.1.1/elementpath/tree_builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 #
 from typing import cast, Any, Dict, Iterator, List, MutableMapping, Optional, Union
 
 from .exceptions import ElementPathTypeError
 from .protocols import ElementProtocol, LxmlElementProtocol, \
     DocumentProtocol, XsdElementProtocol
 from .etree import is_etree_document, is_etree_element
-from .xpath_nodes import SchemaElemType, RootArgType, ChildNodeType, \
-    ElementMapType, TextNode, CommentNode, ProcessingInstructionNode, \
+from .xpath_nodes import SchemaElemType, ChildNodeType, ElementMapType, \
+    TextNode, CommentNode, ProcessingInstructionNode, \
     ElementNode, SchemaElementNode, DocumentNode
 
-__all__ = ['get_node_tree', 'build_node_tree', 'build_lxml_node_tree', 'build_schema_node_tree']
+__all__ = ['RootArgType', 'get_node_tree', 'build_node_tree',
+           'build_lxml_node_tree', 'build_schema_node_tree']
+
+RootArgType = Union[DocumentProtocol, ElementProtocol, SchemaElemType,
+                    'DocumentNode', 'ElementNode']
 
 
 def is_schema(obj: Any) -> bool:
     return hasattr(obj, 'xsd_version') and hasattr(obj, 'maps') and not hasattr(obj, 'parent')
 
 
 def get_node_tree(root: RootArgType, namespaces: Optional[Dict[str, str]] = None) \
```

### Comparing `elementpath-4.1.0/elementpath/validators/__init__.py` & `elementpath-4.1.1/elementpath/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/validators/analyze-string.xsd` & `elementpath-4.1.1/elementpath/validators/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/validators/schema-for-json.xsd` & `elementpath-4.1.1/elementpath/validators/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath1/_xpath1_axes.py` & `elementpath-4.1.1/elementpath/xpath1/_xpath1_axes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 1.0 implementation - part 4 (axes)
 """
 from ..xpath_nodes import ElementNode
 from ..xpath_context import XPathSchemaContext
 from ._xpath1_functions import XPath1Parser
```

### Comparing `elementpath-4.1.0/elementpath/xpath1/_xpath1_functions.py` & `elementpath-4.1.1/elementpath/xpath1/_xpath1_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 1.0 implementation - part 3 (functions)
 """
 import sys
 import math
 import decimal
```

### Comparing `elementpath-4.1.0/elementpath/xpath1/_xpath1_operators.py` & `elementpath-4.1.1/elementpath/xpath1/_xpath1_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 1.0 implementation - part 2 (operators and expressions)
 """
 import math
 import decimal
 import operator
 from copy import copy
```

### Comparing `elementpath-4.1.0/elementpath/xpath1/xpath1_parser.py` & `elementpath-4.1.1/elementpath/xpath1/xpath1_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath2/__init__.py` & `elementpath-4.1.1/elementpath/xpath2/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath2/_xpath2_constructors.py` & `elementpath-4.1.1/elementpath/xpath2/_xpath2_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 2.0 implementation - part 4 (XSD constructors)
 """
 from ..exceptions import ElementPathError, ElementPathSyntaxError
 from ..namespaces import XSD_NAMESPACE
 from ..datatypes import xsd10_atomic_types, xsd11_atomic_types, GregorianDay, \
     GregorianMonth, GregorianMonthDay, GregorianYear10, GregorianYear, \
```

### Comparing `elementpath-4.1.0/elementpath/xpath2/_xpath2_functions.py` & `elementpath-4.1.1/elementpath/xpath2/_xpath2_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 2.0 implementation - part 3 (functions)
 """
 import math
 import datetime
 import time
 import re
```

### Comparing `elementpath-4.1.0/elementpath/xpath2/_xpath2_operators.py` & `elementpath-4.1.1/elementpath/xpath2/_xpath2_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 2.0 implementation - part 2 (operators, expressions and multi-role tokens)
 """
 import math
 import operator
 from copy import copy
 from decimal import Decimal, DivisionByZero
```

### Comparing `elementpath-4.1.0/elementpath/xpath2/xpath2_parser.py` & `elementpath-4.1.1/elementpath/xpath2/xpath2_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from abc import ABCMeta
 import locale
 from collections.abc import MutableSequence
 from urllib.parse import urlparse
 from typing import cast, Any, Callable, ClassVar, Dict, List, \
     MutableMapping, Optional, Tuple, Type, Union
 
-from ..helpers import upper_camel_case, is_ncname, normalize_sequence_type, ordinal
+from ..helpers import upper_camel_case, is_ncname, ordinal
 from ..exceptions import ElementPathError, ElementPathTypeError, \
     ElementPathValueError, MissingContextError, xpath_error
 from ..namespaces import NamespacesType, XSD_NAMESPACE, XML_NAMESPACE, \
     XPATH_FUNCTIONS_NAMESPACE, XQT_ERRORS_NAMESPACE, \
     XSD_NOTATION, XSD_ANY_ATOMIC_TYPE, get_prefixed_name
 from ..collations import UNICODE_COLLATION_BASE_URI, UNICODE_CODEPOINT_COLLATION
 from ..datatypes import UntypedAtomic, AtomicValueType, QName
@@ -148,17 +148,15 @@
             raise ElementPathTypeError(msg)
         else:
             schema.bind_parser(self)
 
         if not variable_types:
             self.variable_types = {}
         elif all(is_sequence_type(v, self) for v in variable_types.values()):
-            self.variable_types = {
-                k: normalize_sequence_type(v) for k, v in variable_types.items()
-            }
+            self.variable_types = variable_types.copy()
         else:
             raise ElementPathValueError('invalid sequence type for in-scope variable types')
 
         self.base_uri = None if base_uri is None else urlparse(base_uri).geturl()
 
         if document_types:
             if any(not is_sequence_type(v, self) for v in document_types.values()):
@@ -363,17 +361,14 @@
     def external_function(self,
                           callback: Callable[..., Any],
                           name: Optional[str] = None,
                           prefix: Optional[str] = None,
                           sequence_types: Tuple[str, ...] = (),
                           bp: int = 90) -> Type[XPathFunction]:
         """Registers a token class for an external function."""
-        """
-        Registers a token class for a symbol that represents an XPath function.
-        """
         import inspect
 
         symbol = name or callback.__name__
         if not is_ncname(symbol):
             raise ElementPathValueError(f'{symbol!r} is not a name')
         elif symbol in self.RESERVED_FUNCTION_NAMES:
             raise ElementPathValueError(f'{symbol!r} is a reserved function name')
```

### Comparing `elementpath-4.1.0/elementpath/xpath30/__init__.py` & `elementpath-4.1.1/elementpath/xpath30/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath30/_translation_maps.py` & `elementpath-4.1.1/elementpath/xpath30/_translation_maps.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath30/_xpath30_functions.py` & `elementpath-4.1.1/elementpath/xpath30/_xpath30_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 3.0 implementation - part 3 (functions)
 """
 import decimal
 import os
 import re
 import codecs
```

### Comparing `elementpath-4.1.0/elementpath/xpath30/_xpath30_operators.py` & `elementpath-4.1.1/elementpath/xpath30/_xpath30_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 3.0 implementation - part 2 (symbols, operators and expressions)
 """
 from copy import copy
 
 from ..namespaces import XPATH_FUNCTIONS_NAMESPACE, XSD_NAMESPACE
 from ..xpath_nodes import AttributeNode, ElementNode
```

### Comparing `elementpath-4.1.0/elementpath/xpath30/xpath30_helpers.py` & `elementpath-4.1.1/elementpath/xpath30/xpath30_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath30/xpath30_parser.py` & `elementpath-4.1.1/elementpath/xpath30/xpath30_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,23 @@
         'math': XPATH_MATH_FUNCTIONS_NAMESPACE, **XPath2Parser.DEFAULT_NAMESPACES
     }
     PATH_STEP_SYMBOLS = {
         '(integer)', '(string)', '(float)', '(decimal)', '(name)',
         '*', '@', '..', '.', '(', '{', 'Q{', '$',
     }
 
+    # https://www.w3.org/TR/xpath-30/#id-reserved-fn-names
+    RESERVED_FUNCTION_NAMES = {
+        'attribute', 'comment', 'document-node', 'element', 'empty-sequence',
+        'function', 'if', 'item', 'namespace-node', 'node', 'processing-instruction',
+        'schema-attribute', 'schema-element', 'switch', 'text', 'typeswitch',
+    }
+
+    function_signatures = XPath2Parser.function_signatures.copy()
+
     decimal_formats: DecimalFormatsType = {
         None: {
             'decimal-separator': '.',
             'grouping-separator': ',',
             'exponent-separator': 'e',
             'infinity': 'Infinity',
             'minus-sign': '-',
@@ -56,39 +65,33 @@
             'percent': '%',
             'per-mille': '‰',
             'zero-digit': '0',
             'digit': '#',
             'pattern-separator': ';',
         }
     }
-
-    # https://www.w3.org/TR/xpath-30/#id-reserved-fn-names
-    RESERVED_FUNCTION_NAMES = {
-        'attribute', 'comment', 'document-node', 'element', 'empty-sequence',
-        'function', 'if', 'item', 'namespace-node', 'node', 'processing-instruction',
-        'schema-attribute', 'schema-element', 'switch', 'text', 'typeswitch',
-    }
-
-    function_signatures = XPath2Parser.function_signatures.copy()
+    defuse_xml: bool = True
 
     def __init__(self, *args: Any, decimal_formats: Optional[DecimalFormatsType] = None,
                  defuse_xml: bool = True, **kwargs: Any) -> None:
         kwargs.pop('strict', None)
         super(XPath30Parser, self).__init__(*args, **kwargs)
-        self.defuse_xml = defuse_xml
+
         if decimal_formats is not None:
             self.decimal_formats = deepcopy(self.decimal_formats)
 
             for k, v in decimal_formats.items():
                 if k is not None:
                     self.decimal_formats[k] = self.decimal_formats[None].copy()
                     self.decimal_formats[k].update(v)
 
             if None in decimal_formats:
                 self.decimal_formats[None].update(decimal_formats[None])
+        if not defuse_xml:
+            self.defuse_xml = defuse_xml
 
     def __repr__(self) -> str:
         args = []
         if self.decimal_formats != self.__class__.decimal_formats:
             args.append(f'decimal_formats={self.decimal_formats!r}')
         if not self.defuse_xml:
             args.append('defuse_xml=False')
```

### Comparing `elementpath-4.1.0/elementpath/xpath31/__init__.py` & `elementpath-4.1.1/elementpath/xpath31/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath31/_xpath31_functions.py` & `elementpath-4.1.1/elementpath/xpath31/_xpath31_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 3.1 implementation - part 3 (functions)
 """
 import json
 import locale
 import math
 import pathlib
```

### Comparing `elementpath-4.1.0/elementpath/xpath31/_xpath31_operators.py` & `elementpath-4.1.1/elementpath/xpath31/_xpath31_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 XPath 3.1 implementation - part 2 (operators and constructors)
 """
 from ..helpers import iter_sequence
 from ..sequence_types import is_sequence_type, match_sequence_type
 from ..xpath_tokens import XPathToken, ProxyToken, XPathFunction, XPathMap, XPathArray
 from .xpath31_parser import XPath31Parser
```

### Comparing `elementpath-4.1.0/elementpath/xpath31/xpath31_parser.py` & `elementpath-4.1.1/elementpath/xpath31/xpath31_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/elementpath/xpath_context.py` & `elementpath-4.1.1/elementpath/xpath_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,27 @@
     Optional, Sequence, Union, Callable, Set
 
 from .exceptions import ElementPathTypeError
 from .namespaces import NamespacesType
 from .datatypes import AnyAtomicType, Timezone, Language
 from .protocols import ElementProtocol, DocumentProtocol
 from .etree import is_etree_element, is_etree_document
-from .xpath_nodes import RootArgType, ChildNodeType, XPathNode, \
-    AttributeNode, NamespaceNode, CommentNode, ProcessingInstructionNode, \
-    ElementNode, DocumentNode
-from .tree_builders import get_node_tree
+from .xpath_nodes import ChildNodeType, XPathNode, AttributeNode, NamespaceNode, \
+    CommentNode, ProcessingInstructionNode, ElementNode, DocumentNode
+from .tree_builders import RootArgType, get_node_tree
 
 if TYPE_CHECKING:
-    from .xpath_tokens import XPathToken, XPathAxis
+    from .xpath_tokens import XPathToken, XPathAxis, XPathFunction
+    ItemType = Union[XPathNode, AnyAtomicType, XPathFunction]
+else:
+    ItemType = Any
 
 __all__ = ['XPathContext', 'XPathSchemaContext']
 
-ItemArgType = Union[RootArgType, XPathNode, AnyAtomicType]
+ItemArgType = Union[RootArgType, ItemType]
 
 
 def is_xpath_node(obj: Any) -> bool:
     return isinstance(obj, XPathNode) or is_etree_element(obj) or is_etree_document(obj)
 
 
 class XPathContext:
@@ -74,15 +76,15 @@
     fn:uri-collection is called with no arguments.
     :param allow_environment: defines if the access to system environment is allowed, \
     for default is `False`. Used by the XPath 3.0+ functions fn:environment-variable \
     and fn:available-environment-variables.
     """
     _etree: Optional[ModuleType] = None
     root: Union[DocumentNode, ElementNode]
-    item: Union[XPathNode, AnyAtomicType, None]
+    item: Optional[ItemType]
     total_nodes: int = 0  # Number of nodes associated to the context
 
     documents: Optional[Dict[str, Union[DocumentNode, ElementNode]]] = None
     collections = None
     default_collection: Optional[List[Union[XPathNode, ElementProtocol, DocumentProtocol]]] = None
 
     def __init__(self,
@@ -193,23 +195,21 @@
             return isinstance(self.item, AttributeNode)
         elif self.axis == 'namespace':
             return isinstance(self.item, NamespaceNode)
         else:
             return isinstance(self.item, ElementNode)
 
     @overload
-    def get_context_item(self, item: ItemArgType) \
-        -> Union[XPathNode, AnyAtomicType]: ...
+    def get_context_item(self, item: ItemArgType) -> ItemType: ...
 
     @overload
-    def get_context_item(self, item: List[ItemArgType]) \
-        -> List[Union[XPathNode, AnyAtomicType]]: ...
+    def get_context_item(self, item: List[ItemArgType]) -> List[ItemType]: ...
 
     def get_context_item(self, item: Union[ItemArgType, List[ItemArgType]]) \
-            -> Union[XPathNode, AnyAtomicType, List[Union[XPathNode, AnyAtomicType]]]:
+            -> Union[ItemType, List[ItemType]]:
         """
         Checks the item and returns an item suitable for XPath processing.
         For XML trees and elements try a match with an existing node in the
         context. If it fails then builds a new node.
         """
         if isinstance(item, XPathNode):
             return item
@@ -237,15 +237,15 @@
 
             if callable(item.tag):  # type: ignore[union-attr]
                 if item.tag.__name__ == 'Comment':  # type: ignore[union-attr]
                     return CommentNode(cast(ElementProtocol, item))
                 else:
                     return ProcessingInstructionNode(cast(ElementProtocol, item))
         else:
-            return cast(AnyAtomicType, item)
+            return cast(Union[AnyAtomicType, 'XPathFunction'], item)
 
         return get_node_tree(
             root=cast(Union[RootArgType], item),
             namespaces=self.namespaces
         )
 
     def inner_focus_select(self, token: Union['XPathToken', 'XPathAxis']) -> Iterator[Any]:
@@ -300,15 +300,15 @@
                     yield tuple(prod)
                 else:
                     k += 1
 
     ##
     # Context item iterators for axis
 
-    def iter_self(self) -> Iterator[Union[XPathNode, AnyAtomicType, None]]:
+    def iter_self(self) -> Iterator[Optional[ItemType]]:
         """Iterator for 'self' axis and '.' shortcut."""
         status = self.axis
         self.axis = 'self'
         yield self.item
         self.axis = status
 
     def iter_attributes(self) -> Iterator[AttributeNode]:
@@ -326,15 +326,15 @@
             self.axis = 'attribute'
 
             for self.item in self.item.attributes:
                 yield self.item
 
             self.item, self.axis = status
 
-    def iter_children_or_self(self) -> Iterator[Union[XPathNode, AnyAtomicType, None]]:
+    def iter_children_or_self(self) -> Iterator[Optional[ItemType]]:
         """Iterator for 'child' forward axis and '/' step."""
         if self.axis is not None:
             yield self.item
         elif isinstance(self.item, (ElementNode, DocumentNode)):
             _status = self.item, self.axis
             self.axis = 'child'
```

### Comparing `elementpath-4.1.0/elementpath/xpath_nodes.py` & `elementpath-4.1.1/elementpath/xpath_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,22 @@
     XSD_ANY_TYPE, XSD_ANY_SIMPLE_TYPE, XSD_ANY_ATOMIC_TYPE, \
     XML_ID, XSD_IDREF, XSD_IDREFS
 from .protocols import ElementProtocol, DocumentProtocol, XsdElementProtocol, \
     XsdAttributeProtocol, XsdTypeProtocol, XsdSchemaProtocol
 from .helpers import match_wildcard
 from .etree import etree_iter_strings
 
-__all__ = ['SchemaElemType', 'RootArgType', 'ChildNodeType', 'ElementMapType',
+__all__ = ['SchemaElemType', 'ChildNodeType', 'ElementMapType',
            'XPathNode', 'AttributeNode', 'NamespaceNode', 'TextNode',
            'CommentNode', 'ProcessingInstructionNode', 'ElementNode',
            'LazyElementNode', 'SchemaElementNode', 'DocumentNode']
 
 _XSD_SPECIAL_TYPES = {XSD_ANY_TYPE, XSD_ANY_SIMPLE_TYPE, XSD_ANY_ATOMIC_TYPE}
 
 SchemaElemType = Union[XsdSchemaProtocol, XsdElementProtocol]
-RootArgType = Union[DocumentProtocol, ElementProtocol, SchemaElemType,
-                    'DocumentNode', 'ElementNode']
 ChildNodeType = Union['TextNode', 'ElementNode', 'CommentNode', 'ProcessingInstructionNode']
 ElementMapType = Dict[Union[ElementProtocol, SchemaElemType], 'ElementNode']
 
 
 ###
 # XQuery and XPath Data Model: https://www.w3.org/TR/xpath-datamodel/
 #
```

### Comparing `elementpath-4.1.0/elementpath/xpath_selectors.py` & `elementpath-4.1.1/elementpath/xpath_selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 from typing import TYPE_CHECKING, Any, Dict, Optional, Iterator, Union, Type
 
 from .namespaces import NamespacesType
-from .xpath_nodes import RootArgType
+from .tree_builders import RootArgType
 from .xpath_context import XPathContext
 from .xpath2 import XPath2Parser
 
 if TYPE_CHECKING:
     from .xpath1 import XPath1Parser
     from .xpath30 import XPath30Parser
```

### Comparing `elementpath-4.1.0/elementpath/xpath_tokens.py` & `elementpath-4.1.1/elementpath/xpath_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 from .namespaces import XSD_NAMESPACE, XPATH_FUNCTIONS_NAMESPACE, \
     XPATH_MATH_FUNCTIONS_NAMESPACE, XSD_SCHEMA, XSD_DECIMAL, \
     XSD_ANY_TYPE, XSD_ANY_SIMPLE_TYPE, XSD_ANY_ATOMIC_TYPE
 from .xpath_nodes import XPathNode, ElementNode, AttributeNode, \
     DocumentNode, NamespaceNode, SchemaElementNode
 from .datatypes import xsd10_atomic_types, AbstractDateTime, AnyURI, \
     UntypedAtomic, Timezone, DateTime10, Date10, DayTimeDuration, Duration, \
-    Integer, DoubleProxy10, DoubleProxy, QName, DatetimeValueType, \
-    AtomicValueType, AnyAtomicType
+    Integer, DoubleProxy10, DoubleProxy, QName, AtomicValueType, AnyAtomicType
 from .protocols import ElementProtocol, DocumentProtocol, XsdAttributeProtocol, \
     XsdElementProtocol, XsdTypeProtocol, XsdSchemaProtocol
 from .sequence_types import is_sequence_type_restriction, match_sequence_type
 from .schema_proxy import AbstractSchemaProxy
 from .tdop import Token, MultiLabel
 from .xpath_context import XPathContext, XPathSchemaContext
 
@@ -271,15 +270,16 @@
         :param default_to_context: if set to `True` then the item of the dynamic context is \
         returned when the argument is missing.
         :param default: the default value returned in case the argument is an empty sequence. \
         If not provided returns `None`.
         :param cls: if a type is provided performs a type checking on item.
         :param promote: a class or a tuple of classes that are promoted to `cls` class.
         """
-        item: Union[None, ElementProtocol, DocumentProtocol, XPathNode, AnyAtomicType]
+        item: Union[None, ElementProtocol, DocumentProtocol,
+                    XPathNode, AnyAtomicType, XPathFunction]
 
         try:
             token = self._items[index]
         except IndexError:
             if default_to_context:
                 if context is None:
                     raise self.missing_context() from None
@@ -729,27 +729,27 @@
             raise self.wrong_syntax(msg, code='XPST0017')
         elif self.namespace and namespace != self.namespace:
             msg = "unmatched namespace"
             raise self.wrong_syntax(msg, code='XPST0017')
 
         self.namespace = namespace
 
-    def adjust_datetime(self, context: XPathContext, cls: Type[DatetimeValueType]) \
-            -> Union[List[Any], DatetimeValueType, DayTimeDuration]:
+    def adjust_datetime(self, context: XPathContext, cls: Type[AbstractDateTime]) \
+            -> Union[List[Any], AbstractDateTime, DayTimeDuration]:
         """
         XSD datetime adjust function helper.
 
         :param context: the XPath dynamic context.
         :param cls: the XSD datetime subclass to use.
         :return: an empty list if there is only one argument that is the empty sequence \
         or the adjusted XSD datetime instance.
         """
         timezone: Optional[Any]
-        item: Optional[DatetimeValueType]
-        _item: Union[DatetimeValueType, DayTimeDuration]
+        item: Optional[AbstractDateTime]
+        _item: Union[AbstractDateTime, DayTimeDuration]
 
         if len(self) == 1:
             item = self.get_argument(context, cls=cls)
             if item is None:
                 return []
             timezone = getattr(context, 'timezone', None)
         else:
@@ -1659,15 +1659,15 @@
                  context: Optional[XPathContext] = None) -> Any:
         if len(args) == 1 and isinstance(args[0], list) and len(args[0]) == 1:
             args = args[0][0],
         if len(args) != 1 or not isinstance(args[0], AnyAtomicType):
             raise self.error('XPST0003', 'exactly one atomic argument is expected')
 
         map_dict: Dict[Any, Any]
-        key = cast(AnyAtomicType, args[0])
+        key = args[0]
         if self._map is not None:
             map_dict = self._map
         else:
             map_dict = self._evaluate(context)
 
         try:
             if isinstance(key, float) and math.isnan(key):
```

### Comparing `elementpath-4.1.0/elementpath.egg-info/PKG-INFO` & `elementpath-4.1.1/elementpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.0
+Version: 4.1.1
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,16 +38,14 @@
 .. image:: https://img.shields.io/pypi/pyversions/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/pypi/implementation/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 .. image:: https://img.shields.io/badge/License-MIT-blue.svg
    :alt: MIT License
    :target: https://lbesson.mit-license.org/
-.. image:: https://travis-ci.org/sissaschool/elementpath.svg?branch=master
-   :target: https://travis-ci.org/sissaschool/elementpath
 .. image:: https://img.shields.io/pypi/dm/elementpath.svg
    :target: https://pypi.python.org/pypi/elementpath/
 
 .. elementpath-introduction
 
 The proposal of this package is to provide XPath 1.0, 2.0, 3.0 and 3.1
 selectors for ElementTree XML data structures, both for the standard
@@ -137,15 +135,15 @@
 
 The XPath parsers are based on an implementation of the Pratt's Top Down Operator Precedence parser.
 The implemented parser includes some lookup-ahead features, helpers for registering tokens and for
 extending language implementations. Also the token class has been generalized using a `MutableSequence`
 as base class. See *tdop.py* for the basic internal classes and *xpath1_parser.py* for extensions
 and for a basic usage of the parser.
 
-If you like you can use the basic parser and tokens provided by the *tdop_parser.py* module to
+If you like you can use the basic parser and tokens provided by the *tdop.py* module to
 implement other types of parsers (I think it could be also a funny exercise!).
 
 
 License
 =======
 
 This software is distributed under the terms of the MIT License.
```

### Comparing `elementpath-4.1.0/elementpath.egg-info/SOURCES.txt` & `elementpath-4.1.1/elementpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/setup.py` & `elementpath-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='elementpath',
-    version='4.1.0',
+    version='4.1.1',
     packages=find_packages(include=['elementpath', 'elementpath.*']),
     package_data={
         'elementpath': ['py.typed'],
         'elementpath.validators': ['analyze-string.xsd', 'schema-for-json.xsd'],
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
```

### Comparing `elementpath-4.1.0/tests/execute_w3c_tests.py` & `elementpath-4.1.1/tests/execute_w3c_tests.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/memory_profiling.py` & `elementpath-4.1.1/tests/memory_profiling.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/resources/analyze-string.xsd` & `elementpath-4.1.1/tests/resources/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/resources/schema-for-json.xsd` & `elementpath-4.1.1/tests/resources/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_collations.py` & `elementpath-4.1.1/tests/test_collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_compare.py` & `elementpath-4.1.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_datatypes.py` & `elementpath-4.1.1/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_elementpath.py` & `elementpath-4.1.1/tests/test_elementpath.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_etree.py` & `elementpath-4.1.1/tests/test_etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_exceptions.py` & `elementpath-4.1.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_helpers.py` & `elementpath-4.1.1/tests/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import unittest
 import math
 from xml.etree import ElementTree
 from elementpath.helpers import days_from_common_era, months2days, \
-    round_number, is_idrefs, collapse_white_spaces, normalize_sequence_type, \
-    escape_json_string, get_double, numeric_equal, numeric_not_equal, equal, \
-    not_equal, match_wildcard, unescape_json_string, iter_sequence, \
-    split_function_test
+    round_number, is_idrefs, collapse_white_spaces, escape_json_string, \
+    get_double, numeric_equal, numeric_not_equal, equal, not_equal, \
+    match_wildcard, unescape_json_string, iter_sequence, split_function_test
 
 
 class HelperFunctionsTest(unittest.TestCase):
 
     def test_node_is_idref_function(self):
         self.assertTrue(is_idrefs(ElementTree.XML('<A>xyz</A>').text))
         self.assertTrue(is_idrefs(ElementTree.XML('<A>xyz abc</A>').text))
@@ -135,25 +134,14 @@
         self.assertEqual(round_number(-10.1), -10)
         self.assertEqual(round_number(-9.5), -9)
 
     def test_collapse_white_spaces_function(self):
         self.assertEqual(collapse_white_spaces('  ab  c  '), 'ab c')
         self.assertEqual(collapse_white_spaces('  ab\t\nc  '), 'ab c')
 
-    def test_normalize_sequence_type_function(self):
-        self.assertEqual(normalize_sequence_type(' xs:integer + '), 'xs:integer+')
-        self.assertEqual(normalize_sequence_type(' xs :integer + '), 'xs :integer+')  # Invalid
-        self.assertEqual(normalize_sequence_type(' element( * ) '), 'element(*)')
-        self.assertEqual(normalize_sequence_type(' element( *,xs:int ) '), 'element(*, xs:int)')
-        self.assertEqual(normalize_sequence_type(' \nfunction  ( * )\t '), 'function(*)')
-        self.assertEqual(
-            normalize_sequence_type(' \nfunction  ( item( ) * ) as  xs:integer\t '),
-            'function(item()*) as xs:integer'
-        )
-
     def test_get_double_function(self):
         self.assertEqual(get_double(1), 1.0)
         self.assertEqual(get_double(1.0), 1.0)
 
         self.assertIs(get_double('NaN'), math.nan)
         self.assertIs(get_double(float('nan')), math.nan)
         self.assertTrue(math.isinf(get_double('INF')))
```

### Comparing `elementpath-4.1.0/tests/test_namespaces.py` & `elementpath-4.1.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_package.py` & `elementpath-4.1.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_regex.py` & `elementpath-4.1.1/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_schema_context.py` & `elementpath-4.1.1/tests/test_schema_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_schema_proxy.py` & `elementpath-4.1.1/tests/test_schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_selectors.py` & `elementpath-4.1.1/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_tdop_parser.py` & `elementpath-4.1.1/tests/test_tdop_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_tree_builders.py` & `elementpath-4.1.1/tests/test_tree_builders.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_typing.py` & `elementpath-4.1.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_validators.py` & `elementpath-4.1.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath1_parser.py` & `elementpath-4.1.1/tests/test_xpath1_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,14 @@
 from xml.etree import ElementTree
 
 try:
     import lxml.etree as lxml_etree
 except ImportError:
     lxml_etree = None
 
-try:
-    import xmlschema
-except ImportError:
-    xmlschema = None
-
 from elementpath import datatypes, XPath1Parser, XPathContext, MissingContextError, \
     AttributeNode, NamespaceNode, TextNode, CommentNode, ProcessingInstructionNode, \
     ElementNode, select, XPathFunction
 from elementpath.namespaces import XSD_NAMESPACE, XPATH_FUNCTIONS_NAMESPACE, \
     XPATH_MATH_FUNCTIONS_NAMESPACE
 from elementpath.sequence_types import is_sequence_type
 
@@ -381,17 +376,15 @@
             # Do not test with XPath 1.0 on lxml.
             self.check_selector(
                 "./{http://www.w3.org/2001/04/xmlenc#}EncryptedData", root, [], strict=False)
             self.check_selector("./{http://xpath.test/ns}B1", root, [root[0]], strict=False)
             self.check_selector("./{http://xpath.test/ns}*", root, root[:], strict=False)
 
     def test_node_types(self):
-        document = self.etree.parse(io.StringIO(u'<A/>'))
         element = self.etree.Element('schema')
-
         context = XPathContext(element)
         attribute = AttributeNode('id', '0212349350')
         namespace = NamespaceNode('xs', 'http://www.w3.org/2001/XMLSchema')
         comment = CommentNode(self.etree.Comment('nothing important'))
         pi = ProcessingInstructionNode(self.etree.ProcessingInstruction('action'))
         text = TextNode('aldebaran')
 
@@ -1408,23 +1401,35 @@
         root = self.etree.XML('<A xmlns:tst="http://xpath.test/ns">10<tst:B1/></A>')
         namespaces = list(self.parser.DEFAULT_NAMESPACES.items()) \
             + [('tst', 'http://xpath.test/ns')]
 
         if self.parser.version == '1.0':
             self.check_selector('/A/namespace::*', root, expected=set(namespaces),
                                 namespaces=namespaces[-1:])
+            self.check_selector('/A/namespace::tst', root,
+                                expected=[('tst', 'http://xpath.test/ns')],
+                                namespaces=namespaces[-1:])
         else:
             self.check_selector('/A/namespace::*', root,
                                 expected={'http://www.w3.org/XML/1998/namespace',
                                           'http://xpath.test/ns'},
                                 namespaces=namespaces[-1:])
+            self.check_selector('/A/namespace::tst', root,
+                                expected=['http://xpath.test/ns'],
+                                namespaces=namespaces[-1:])
 
         self.check_value('namespace::*', MissingContextError)
         self.check_value('./text()/namespace::*', [], context=XPathContext(root))
 
+        if self.parser.version >= '3.0':
+            self.check_selector('/A/namespace::namespace-node()', root,
+                                expected={'http://www.w3.org/XML/1998/namespace',
+                                          'http://xpath.test/ns'},
+                                namespaces=namespaces[-1:])
+
     def test_parent_shortcut_and_axis(self):
         root = self.etree.XML(
             '<A><B1><C1/></B1><B2/><B3><C1/><C2/></B3><B4><C3><D1/></C3></B4></A>')
         self.check_selector('/A/*/C2/..', root, [root[2]])
         self.check_selector('/A/*/*/..', root, [root[0], root[2], root[3]])
         self.check_selector('//C2/..', root, [root[2]])
         self.check_selector('/A/*/C2/parent::node()', root, [root[2]])
@@ -1618,15 +1623,15 @@
                 self.assertIn(key[0].namespace, XPATH_FUNCTIONS_NAMESPACE)
             elif self.parser.version == '3.0':
                 self.assertIn(key[0].namespace, {XPATH_FUNCTIONS_NAMESPACE,
                                                  XPATH_MATH_FUNCTIONS_NAMESPACE})
 
             self.assertIsInstance(value, str)
             self.assertTrue(value.startswith('function('))
-            self.assertTrue(is_sequence_type(value, self.parser), msg=value)
+            self.assertTrue(is_sequence_type(value), msg=value)
 
     def test_descendant_predicate__issue_51(self):
         root = self.etree.XML(dedent("""<doc>
           <target>
             <name>V1</name>
             <value>3</value>
             <more>foo</more>
```

### Comparing `elementpath-4.1.0/tests/test_xpath2_constructors.py` & `elementpath-4.1.1/tests/test_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath2_functions.py` & `elementpath-4.1.1/tests/test_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath2_parser.py` & `elementpath-4.1.1/tests/test_xpath2_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 try:
     import xmlschema
 except ImportError:
     xmlschema = None
 else:
     xmlschema.XMLSchema.meta_schema.build()
 
-from elementpath import XPath2Parser, XPathContext, MissingContextError, \
-    ElementNode, select, iter_select
+from elementpath import XPath2Parser, XPathContext, XPathSchemaContext, \
+    MissingContextError, ElementNode, select, iter_select
 from elementpath.datatypes import xsd10_atomic_types, xsd11_atomic_types, DateTime, \
     Date, Time, Timezone, DayTimeDuration, YearMonthDuration, UntypedAtomic, QName
 from elementpath.namespaces import XPATH_FUNCTIONS_NAMESPACE
 from elementpath.collations import get_locale_category
 from elementpath.sequence_types import is_instance
 from elementpath.xpath_tokens import ProxyToken, XPathFunction
 
@@ -566,14 +566,27 @@
         self.check_selector("a = (1 to 30)", root, True)
         self.check_selector("a = (2)", root, False)
         self.check_selector("a[1] = (1 to 10, 30)", root, True)
         self.check_selector("a[2] = (1 to 10, 30)", root, True)
         self.check_selector("a[3] = (1 to 10, 30)", root, True)
         self.check_selector("a[4] = (1 to 10, 30)", root, False)
 
+    @unittest.skipIf(xmlschema is None, "xmlschema library is not installed!")
+    def test_namespace_axis_on_schema_context(self):
+        schema = xmlschema.XMLSchema(dedent("""\n
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+                <xs:simpleType name="floatType">
+                    <xs:restriction base="xs:double"/>
+                </xs:simpleType>
+            </xs:schema>"""))
+
+        context = XPathSchemaContext(schema)
+        token = self.parser.parse('/namespace::*')
+        self.assertListEqual(token.evaluate(context), [])
+
     def test_unknown_axis(self):
         self.wrong_syntax('unknown::node()', 'XPST0003')
         self.wrong_syntax('A/unknown::node()', 'XPST0003')
 
         self.parser.compatibility_mode = True
         self.wrong_name('unknown::node()', 'XPST0010')
         self.wrong_name('A/unknown::node()', 'XPST0010')
```

### Comparing `elementpath-4.1.0/tests/test_xpath30.py` & `elementpath-4.1.1/tests/test_xpath30.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath31.py` & `elementpath-4.1.1/tests/test_xpath31.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath_context.py` & `elementpath-4.1.1/tests/test_xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath_nodes.py` & `elementpath-4.1.1/tests/test_xpath_nodes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/test_xpath_tokens.py` & `elementpath-4.1.1/tests/test_xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tests/xpath_test_class.py` & `elementpath-4.1.1/tests/xpath_test_class.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.0/tox.ini` & `elementpath-4.1.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
 envlist =
     py{37,38,39,310,311}, pypy3, xmlschema{20},
-    docs, flake8, mypy-py{38,39,310,311}, pytest, coverage
+    docs, flake8, mypy-py{38,39,310,311,py3}, pytest, coverage
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/elementpath
 
 [testenv]
 deps =
     lxml
     xmlschema>=2.0.0
@@ -33,17 +33,17 @@
 [testenv:flake8]
 deps =
     flake8
 commands =
     flake8 elementpath
     flake8 tests
 
-[testenv:mypy-py{38,39,310,311}]
+[testenv:mypy-py{38,39,310,311,py3}]
 deps =
-    mypy==1.1.1
+    mypy==1.2.0
     xmlschema
     lxml-stubs
 commands =
     mypy --strict elementpath
     python tests/test_typing.py
 
 [testenv:coverage]
```

