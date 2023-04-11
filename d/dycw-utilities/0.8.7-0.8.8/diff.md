# Comparing `tmp/dycw_utilities-0.8.7.tar.gz` & `tmp/dycw_utilities-0.8.8.tar.gz`

## Comparing `dycw_utilities-0.8.7.tar` & `dycw_utilities-0.8.8.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.envrc
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.rgiginore
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/conftest.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/noxfile.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/requirements-dev.txt
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.github/workflows/push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/conftest.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_airium.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_atomicwrites.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_beartype.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_bidict.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_class_name.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_clean_dir.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_cryptography.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_cvxpy.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_datetime.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_email.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_enum.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_errors.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_fastapi.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_fastparquet.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_fpdf2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_getpass.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_git.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_hashlib.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_hatch.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_iterables.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_json.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_logging.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_memory_profiler.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_modules.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_monitor_memory.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_more_itertools.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_os.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pathlib.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pickle.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pqdm.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pyinstrument.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pypi_server.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pytest.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_pytest_check.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_random.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_re.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_scipy.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_semver.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_sentinel.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_socket.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_subprocess.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_sys.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_tempfile.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_text.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_timer.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_tqdm.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_typed_settings.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_types.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_typing.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_warnings.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_zipfile.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/test_zoneinfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/attrs/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/attrs/test_attrs.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/attrs/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/click/__init__.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/click/test_click.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/click/test_luigi.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/click/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/holoviews/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/holoviews/test_holoviews.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/holoviews/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_hypothesis.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_luigi.py
--rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_numpy.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_pandas.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_semver.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_sqlalchemy.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/hypothesis/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/loguru/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/loguru/script_to_test_luigi.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/loguru/test_loguru.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/__init__.py
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/test_attrs.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/test_luigi.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/test_semver.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/test_server.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/luigi/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/math/__init__.py
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/math/test_math.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/math/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/standalone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/outer_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/outer_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/subpackage/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/subpackage/inner_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/subpackage/inner_2.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_with/subpackage/inner_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_without/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_without/module_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/modules/package_without/module_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/numpy/__init__.py
--rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/numpy/test_numpy.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/numpy/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/pandas/__init__.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/pandas/test_pandas.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/pandas/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/sqlalchemy/test_fastparquet.py
--rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/sqlalchemy/test_pandas.py
--rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/sqlalchemy/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/xarray/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/xarray/test_typing.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/xarray/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/zarr/__init__.py
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/zarr/test_xarray.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/tests/zarr/test_zarr.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/airium.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/atomicwrites.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/beartype.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/bidict.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/class_name.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/cryptography.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/cvxpy.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/datetime.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/email.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/enum.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/errors.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/fastapi.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/fastparquet.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/fpdf2.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/getpass.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/git.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hashlib.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hatch.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/iterables.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/json.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/logging.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/loguru.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/memory_profiler.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/modules.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/more_itertools.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/os.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pathlib.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pickle.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pqdm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/py.typed
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pyinstrument.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pytest.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pytest_check.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/random.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/re.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/scipy.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/semver.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/sentinel.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/socket.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/subprocess.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/sys.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/tempfile.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/text.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/timer.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/tqdm.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/typed_settings.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/types.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/typing.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/warnings.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/zipfile.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/zoneinfo.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/attrs/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/attrs/xarray.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/clean_dir/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/clean_dir/__main__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/clean_dir/classes.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/click/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/click/luigi.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/click/sqlalchemy.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/holoviews/__init__.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/holoviews/xarray.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/luigi.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/numpy.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/pandas.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/semver.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/sqlalchemy.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/typing.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/hypothesis/xarray.py
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/__init__.py
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/attrs.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/semver.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/sqlalchemy.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/server/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/server/__main__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/luigi/server/classes.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/math/__init__.py
--rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/math/typing.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/monitor_memory/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/monitor_memory/__main__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/monitor_memory/classes.py
--rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/numpy/__init__.py
--rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/numpy/typing.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pandas/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pandas/typing.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pypi_server/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pypi_server/__main__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/pypi_server/classes.py
--rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/sqlalchemy/fastparquet.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/sqlalchemy/pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/xarray/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/xarray/typing.py
--rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/zarr/__init__.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/utilities/zarr/xarray.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/.gitignore
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/README.md
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dycw_utilities-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.envrc
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.rgiginore
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/conftest.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/noxfile.py
+-rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/requirements-dev.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.github/workflows/push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/conftest.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_airium.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_atomicwrites.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_beartype.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_bidict.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_class_name.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_clean_dir.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_cryptography.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_cvxpy.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_datetime.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_email.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_enum.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_errors.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fastapi.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fastparquet.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fpdf2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_getpass.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_git.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_hashlib.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_hatch.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_iterables.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_json.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_logging.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_memory_profiler.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_modules.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_monitor_memory.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_more_itertools.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_os.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pathlib.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pickle.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pqdm.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pyinstrument.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pypi_server.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pytest.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pytest_check.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_random.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_re.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_scipy.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_semver.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_sentinel.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_socket.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_subprocess.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_sys.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_tempfile.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_text.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_timer.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_tqdm.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_typed_settings.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_types.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_typing.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_warnings.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_zipfile.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_zoneinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/test_attrs.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/__init__.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_click.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_luigi.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/__init__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/test_holoviews.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_hypothesis.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_luigi.py
+-rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_numpy.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_pandas.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_semver.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_sqlalchemy.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/script_to_test_luigi.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/test_loguru.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/__init__.py
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_attrs.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_luigi.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_semver.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_server.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/__init__.py
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/test_math.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/standalone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/outer_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/outer_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_2.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/module_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/module_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/test_numpy.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/__init__.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/test_pandas.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_fastparquet.py
+-rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_pandas.py
+-rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/test_typing.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/__init__.py
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/test_xarray.py
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/test_zarr.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/airium.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/atomicwrites.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/beartype.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/bidict.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/class_name.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/cryptography.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/cvxpy.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/datetime.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/email.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/enum.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/errors.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fastapi.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fastparquet.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fpdf2.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/getpass.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/git.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hashlib.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hatch.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/iterables.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/json.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/logging.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/loguru.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/memory_profiler.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/modules.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/more_itertools.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/os.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pathlib.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pickle.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pqdm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/py.typed
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pyinstrument.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pytest.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pytest_check.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/random.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/re.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/scipy.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/semver.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sentinel.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/socket.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/subprocess.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sys.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/tempfile.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/text.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/timer.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/tqdm.py
+-rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/typed_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/types.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/typing.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/warnings.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zipfile.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zoneinfo.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/attrs/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/attrs/xarray.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/__main__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/classes.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/luigi.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/sqlalchemy.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/holoviews/__init__.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/holoviews/xarray.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/luigi.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/numpy.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/pandas.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/semver.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/sqlalchemy.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/typing.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/xarray.py
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/__init__.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/attrs.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/semver.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/sqlalchemy.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/classes.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/math/__init__.py
+-rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/math/typing.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/__main__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/classes.py
+-rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/numpy/__init__.py
+-rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/numpy/typing.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pandas/__init__.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pandas/typing.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/__main__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/classes.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/fastparquet.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/xarray/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/xarray/typing.py
+-rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zarr/__init__.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zarr/xarray.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.gitignore
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/README.md
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/PKG-INFO
```

### Comparing `dycw_utilities-0.8.7/.pre-commit-config.yaml` & `dycw_utilities-0.8.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/noxfile.py` & `dycw_utilities-0.8.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/requirements-dev.txt` & `dycw_utilities-0.8.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/.github/workflows/pull-request.yml` & `dycw_utilities-0.8.8/.github/workflows/pull-request.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/.github/workflows/push.yml` & `dycw_utilities-0.8.8/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_airium.py` & `dycw_utilities-0.8.8/tests/test_airium.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_atomicwrites.py` & `dycw_utilities-0.8.8/tests/test_atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_beartype.py` & `dycw_utilities-0.8.8/tests/test_beartype.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_bidict.py` & `dycw_utilities-0.8.8/tests/test_bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_class_name.py` & `dycw_utilities-0.8.8/tests/test_class_name.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_clean_dir.py` & `dycw_utilities-0.8.8/tests/test_clean_dir.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_cryptography.py` & `dycw_utilities-0.8.8/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_cvxpy.py` & `dycw_utilities-0.8.8/tests/test_cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_datetime.py` & `dycw_utilities-0.8.8/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_email.py` & `dycw_utilities-0.8.8/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_enum.py` & `dycw_utilities-0.8.8/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_errors.py` & `dycw_utilities-0.8.8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_fastapi.py` & `dycw_utilities-0.8.8/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_fastparquet.py` & `dycw_utilities-0.8.8/tests/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_fpdf2.py` & `dycw_utilities-0.8.8/tests/test_fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_git.py` & `dycw_utilities-0.8.8/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_hashlib.py` & `dycw_utilities-0.8.8/tests/test_hashlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_iterables.py` & `dycw_utilities-0.8.8/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_json.py` & `dycw_utilities-0.8.8/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_modules.py` & `dycw_utilities-0.8.8/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_monitor_memory.py` & `dycw_utilities-0.8.8/tests/test_monitor_memory.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_more_itertools.py` & `dycw_utilities-0.8.8/tests/test_more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_os.py` & `dycw_utilities-0.8.8/tests/test_os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pathlib.py` & `dycw_utilities-0.8.8/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pickle.py` & `dycw_utilities-0.8.8/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pqdm.py` & `dycw_utilities-0.8.8/tests/test_pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pypi_server.py` & `dycw_utilities-0.8.8/tests/test_pypi_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pytest.py` & `dycw_utilities-0.8.8/tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_pytest_check.py` & `dycw_utilities-0.8.8/tests/test_pytest_check.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_re.py` & `dycw_utilities-0.8.8/tests/test_re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_scipy.py` & `dycw_utilities-0.8.8/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_subprocess.py` & `dycw_utilities-0.8.8/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_tempfile.py` & `dycw_utilities-0.8.8/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_text.py` & `dycw_utilities-0.8.8/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_timer.py` & `dycw_utilities-0.8.8/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_tqdm.py` & `dycw_utilities-0.8.8/tests/test_tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_typed_settings.py` & `dycw_utilities-0.8.8/tests/test_typed_settings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_types.py` & `dycw_utilities-0.8.8/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_warnings.py` & `dycw_utilities-0.8.8/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/test_zipfile.py` & `dycw_utilities-0.8.8/tests/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/attrs/test_attrs.py` & `dycw_utilities-0.8.8/tests/attrs/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/attrs/test_xarray.py` & `dycw_utilities-0.8.8/tests/attrs/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/click/test_click.py` & `dycw_utilities-0.8.8/tests/click/test_click.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/click/test_luigi.py` & `dycw_utilities-0.8.8/tests/click/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/click/test_sqlalchemy.py` & `dycw_utilities-0.8.8/tests/click/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/holoviews/test_holoviews.py` & `dycw_utilities-0.8.8/tests/holoviews/test_holoviews.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/holoviews/test_xarray.py` & `dycw_utilities-0.8.8/tests/holoviews/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_hypothesis.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_luigi.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_numpy.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_pandas.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_semver.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_sqlalchemy.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/hypothesis/test_xarray.py` & `dycw_utilities-0.8.8/tests/hypothesis/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/loguru/script_to_test_luigi.py` & `dycw_utilities-0.8.8/tests/loguru/script_to_test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/loguru/test_loguru.py` & `dycw_utilities-0.8.8/tests/loguru/test_loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/luigi/test_attrs.py` & `dycw_utilities-0.8.8/tests/luigi/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/luigi/test_luigi.py` & `dycw_utilities-0.8.8/tests/luigi/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/luigi/test_server.py` & `dycw_utilities-0.8.8/tests/luigi/test_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/luigi/test_sqlalchemy.py` & `dycw_utilities-0.8.8/tests/luigi/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/math/test_math.py` & `dycw_utilities-0.8.8/tests/math/test_math.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/math/test_typing.py` & `dycw_utilities-0.8.8/tests/math/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/numpy/test_numpy.py` & `dycw_utilities-0.8.8/tests/numpy/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/numpy/test_typing.py` & `dycw_utilities-0.8.8/tests/numpy/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/pandas/test_pandas.py` & `dycw_utilities-0.8.8/tests/pandas/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/pandas/test_typing.py` & `dycw_utilities-0.8.8/tests/pandas/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/sqlalchemy/test_fastparquet.py` & `dycw_utilities-0.8.8/tests/sqlalchemy/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/sqlalchemy/test_pandas.py` & `dycw_utilities-0.8.8/tests/sqlalchemy/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/sqlalchemy/test_sqlalchemy.py` & `dycw_utilities-0.8.8/tests/sqlalchemy/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/xarray/test_typing.py` & `dycw_utilities-0.8.8/tests/xarray/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/zarr/test_xarray.py` & `dycw_utilities-0.8.8/tests/zarr/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/tests/zarr/test_zarr.py` & `dycw_utilities-0.8.8/tests/zarr/test_zarr.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/atomicwrites.py` & `dycw_utilities-0.8.8/utilities/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/bidict.py` & `dycw_utilities-0.8.8/utilities/bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/cryptography.py` & `dycw_utilities-0.8.8/utilities/cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/cvxpy.py` & `dycw_utilities-0.8.8/utilities/cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/datetime.py` & `dycw_utilities-0.8.8/utilities/datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/email.py` & `dycw_utilities-0.8.8/utilities/email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/enum.py` & `dycw_utilities-0.8.8/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/errors.py` & `dycw_utilities-0.8.8/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/fastapi.py` & `dycw_utilities-0.8.8/utilities/fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/fastparquet.py` & `dycw_utilities-0.8.8/utilities/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/fpdf2.py` & `dycw_utilities-0.8.8/utilities/fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/git.py` & `dycw_utilities-0.8.8/utilities/git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hatch.py` & `dycw_utilities-0.8.8/utilities/hatch.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/iterables.py` & `dycw_utilities-0.8.8/utilities/iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/json.py` & `dycw_utilities-0.8.8/utilities/json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/logging.py` & `dycw_utilities-0.8.8/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/loguru.py` & `dycw_utilities-0.8.8/utilities/loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/memory_profiler.py` & `dycw_utilities-0.8.8/utilities/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/modules.py` & `dycw_utilities-0.8.8/utilities/modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/more_itertools.py` & `dycw_utilities-0.8.8/utilities/more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/os.py` & `dycw_utilities-0.8.8/utilities/os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pickle.py` & `dycw_utilities-0.8.8/utilities/pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pqdm.py` & `dycw_utilities-0.8.8/utilities/pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pyinstrument.py` & `dycw_utilities-0.8.8/utilities/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pytest.py` & `dycw_utilities-0.8.8/utilities/pytest.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/re.py` & `dycw_utilities-0.8.8/utilities/re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/scipy.py` & `dycw_utilities-0.8.8/utilities/scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/sentinel.py` & `dycw_utilities-0.8.8/utilities/sentinel.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/subprocess.py` & `dycw_utilities-0.8.8/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/tempfile.py` & `dycw_utilities-0.8.8/utilities/tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/text.py` & `dycw_utilities-0.8.8/utilities/text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/timer.py` & `dycw_utilities-0.8.8/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/tqdm.py` & `dycw_utilities-0.8.8/utilities/tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/typed_settings.py` & `dycw_utilities-0.8.8/utilities/typed_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     TypeArgsMaker,
     TypeHandler,
     TypeHandlerFunc,
 )
 from typed_settings.click_utils import ClickHandler
 from typed_settings.click_utils import click_options as _click_options
 from typed_settings.loaders import Loader
+from typed_settings.types import AUTO, _Auto
 
 from utilities.click import Date, DateTime, Time, Timedelta
 from utilities.click import Enum as ClickEnum
 from utilities.datetime import (
     ensure_date,
     ensure_datetime,
     ensure_time,
@@ -60,17 +61,26 @@
 @beartype
 def load_settings(
     cls: type[_T],
     /,
     *,
     appname: str = "appname",
     config_files: Iterable[PathLike] = _CONFIG_FILES,
+    config_file_section: Union[str, _Auto] = AUTO,
+    config_files_var: Union[None, str, _Auto] = AUTO,
+    env_prefix: Union[None, str, _Auto] = AUTO,
 ) -> _T:
     """Load a settings object with the extended converter."""
-    loaders = _get_loaders(appname=appname, config_files=config_files)
+    loaders = _get_loaders(
+        appname=appname,
+        config_files=config_files,
+        config_file_section=config_file_section,
+        config_files_var=config_files_var,
+        env_prefix=env_prefix,
+    )
     converter = _make_converter()
     return _load_settings(cast(Any, cls), loaders, converter=converter)
 
 
 @beartype
 def click_options(
     cls: type[Any],
@@ -90,21 +100,32 @@
         converter=converter,
         type_args_maker=type_args_maker,
         argname=argname,
     )
 
 
 def _get_loaders(
-    *, appname: str = "appname", config_files: Iterable[PathLike] = _CONFIG_FILES
+    *,
+    appname: str = "appname",
+    config_files: Iterable[PathLike] = _CONFIG_FILES,
+    config_file_section: Union[str, _Auto] = AUTO,
+    config_files_var: Union[None, str, _Auto] = AUTO,
+    env_prefix: Union[None, str, _Auto] = AUTO,
 ) -> list[Loader]:
     # cannot @beartype as Loader is a protocol
     if search("_", appname):
         msg = f"{appname=}"
         raise AppNameContainsUnderscoreError(msg)
-    return default_loaders(appname, config_files=config_files)
+    return default_loaders(
+        appname,
+        config_files=config_files,
+        config_file_section=config_file_section,
+        config_files_var=config_files_var,
+        env_prefix=env_prefix,
+    )
 
 
 class AppNameContainsUnderscoreError(ValueError):
     """Raised when the appname contains a space."""
 
 
 @beartype
```

### Comparing `dycw_utilities-0.8.7/utilities/types.py` & `dycw_utilities-0.8.8/utilities/types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/warnings.py` & `dycw_utilities-0.8.8/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/zipfile.py` & `dycw_utilities-0.8.8/utilities/zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/attrs/__init__.py` & `dycw_utilities-0.8.8/utilities/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/clean_dir/__init__.py` & `dycw_utilities-0.8.8/utilities/clean_dir/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/clean_dir/classes.py` & `dycw_utilities-0.8.8/utilities/clean_dir/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/click/__init__.py` & `dycw_utilities-0.8.8/utilities/click/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/click/luigi.py` & `dycw_utilities-0.8.8/utilities/click/luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/click/sqlalchemy.py` & `dycw_utilities-0.8.8/utilities/click/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/holoviews/__init__.py` & `dycw_utilities-0.8.8/utilities/holoviews/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/holoviews/xarray.py` & `dycw_utilities-0.8.8/utilities/holoviews/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/__init__.py` & `dycw_utilities-0.8.8/utilities/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/numpy.py` & `dycw_utilities-0.8.8/utilities/hypothesis/numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/pandas.py` & `dycw_utilities-0.8.8/utilities/hypothesis/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/semver.py` & `dycw_utilities-0.8.8/utilities/hypothesis/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/sqlalchemy.py` & `dycw_utilities-0.8.8/utilities/hypothesis/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/hypothesis/xarray.py` & `dycw_utilities-0.8.8/utilities/hypothesis/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/__init__.py` & `dycw_utilities-0.8.8/utilities/luigi/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/attrs.py` & `dycw_utilities-0.8.8/utilities/luigi/attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/semver.py` & `dycw_utilities-0.8.8/utilities/luigi/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/sqlalchemy.py` & `dycw_utilities-0.8.8/utilities/luigi/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/server/__init__.py` & `dycw_utilities-0.8.8/utilities/luigi/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/luigi/server/classes.py` & `dycw_utilities-0.8.8/utilities/luigi/server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/math/__init__.py` & `dycw_utilities-0.8.8/utilities/math/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/math/typing.py` & `dycw_utilities-0.8.8/utilities/math/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/monitor_memory/__init__.py` & `dycw_utilities-0.8.8/utilities/monitor_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/monitor_memory/classes.py` & `dycw_utilities-0.8.8/utilities/monitor_memory/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/numpy/__init__.py` & `dycw_utilities-0.8.8/utilities/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/numpy/typing.py` & `dycw_utilities-0.8.8/utilities/numpy/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pandas/__init__.py` & `dycw_utilities-0.8.8/utilities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pandas/typing.py` & `dycw_utilities-0.8.8/utilities/pandas/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pypi_server/__init__.py` & `dycw_utilities-0.8.8/utilities/pypi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/pypi_server/classes.py` & `dycw_utilities-0.8.8/utilities/pypi_server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/sqlalchemy/__init__.py` & `dycw_utilities-0.8.8/utilities/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/sqlalchemy/fastparquet.py` & `dycw_utilities-0.8.8/utilities/sqlalchemy/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/sqlalchemy/pandas.py` & `dycw_utilities-0.8.8/utilities/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/xarray/typing.py` & `dycw_utilities-0.8.8/utilities/xarray/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/zarr/__init__.py` & `dycw_utilities-0.8.8/utilities/zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/utilities/zarr/xarray.py` & `dycw_utilities-0.8.8/utilities/zarr/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/.gitignore` & `dycw_utilities-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/README.md` & `dycw_utilities-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/pyproject.toml` & `dycw_utilities-0.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.7/PKG-INFO` & `dycw_utilities-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dycw-utilities
-Version: 0.8.7
+Version: 0.8.8
 Author-email: Derek Wan <d.wan@icloud.com>
 Requires-Python: >=3.9
 Requires-Dist: beartype>=0.13.0
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: airium
 Requires-Dist: airium>=0.2.5; extra == 'airium'
 Provides-Extra: atomicwrites
```

