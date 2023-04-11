# Comparing `tmp/ddev-1.6.0.tar.gz` & `tmp/ddev-2.0.0.tar.gz`

## Comparing `ddev-1.6.0.tar` & `ddev-2.0.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ddev-1.6.0/.flake8
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ddev-1.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-1.6.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/config/__init__.py
--rw-r--r--   0        0        0    40934 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/config/test_model.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/repo/test_config.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/test_json.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/validation/__init__.py
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ddev-1.6.0/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ddev-1.6.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-1.6.0/README.md
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ddev-1.6.0/hatch.toml
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 ddev-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 ddev-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ddev-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/config/__init__.py
+-rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/config/test_model.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ddev-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-2.0.0/README.md
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ddev-2.0.0/hatch.toml
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 ddev-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 ddev-2.0.0/PKG-INFO
```

### Comparing `ddev-1.6.0/CHANGELOG.md` & `ddev-2.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG - ddev
 
+## 2.0.0 / 2023-04-11
+
+* [Changed] Replace flake8 and isort with Ruff. See [#14212](https://github.com/DataDog/integrations-core/pull/14212).
+
 ## 1.6.0 / 2023-03-31
 
 * [Added] Add GitHub Actions workflows. See [#14187](https://github.com/DataDog/integrations-core/pull/14187).
 
 ## 1.5.0 / 2023-03-23
 
 * [Added] Bump datadog-checks-dev to 18.x. See [#14225](https://github.com/DataDog/integrations-core/pull/14225).
```

### Comparing `ddev-1.6.0/src/ddev/cli/__init__.py` & `ddev-2.0.0/src/ddev/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/application.py` & `ddev-2.0.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/terminal.py` & `ddev-2.0.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/config/__init__.py` & `ddev-2.0.0/src/ddev/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/env/__init__.py` & `ddev-2.0.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/meta/__init__.py` & `ddev-2.0.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-2.0.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/release/__init__.py` & `ddev-2.0.0/src/ddev/cli/release/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/release/agent/__init__.py` & `ddev-2.0.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/release/show/__init__.py` & `ddev-2.0.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/status/__init__.py` & `ddev-2.0.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/validate/__init__.py` & `ddev-2.0.0/src/ddev/cli/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/validate/ci.py` & `ddev-2.0.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/cli/validate/manifest.py` & `ddev-2.0.0/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/config/file.py` & `ddev-2.0.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/config/model.py` & `ddev-2.0.0/src/ddev/config/model.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/config/utils.py` & `ddev-2.0.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/integration/core.py` & `ddev-2.0.0/src/ddev/integration/core.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/repo/core.py` & `ddev-2.0.0/src/ddev/repo/core.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/fs.py` & `ddev-2.0.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/git.py` & `ddev-2.0.0/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/json.py` & `ddev-2.0.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/platform.py` & `ddev-2.0.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/structures.py` & `ddev-2.0.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-2.0.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/src/ddev/validation/tracker.py` & `ddev-2.0.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/conftest.py` & `ddev-2.0.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from contextlib import ExitStack
 from typing import Generator
 
 import pytest
 import vcr
 from click.testing import CliRunner as __CliRunner
 from datadog_checks.dev.tooling.utils import set_root
-
 from ddev.config.constants import AppEnvVars, ConfigEnvVars
 from ddev.config.file import ConfigFile
 from ddev.repo.core import Repository
 from ddev.utils.ci import running_in_ci
 from ddev.utils.fs import Path, temp_directory
 from ddev.utils.platform import Platform
```

### Comparing `ddev-1.6.0/tests/test__utils.py` & `ddev-2.0.0/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/cli/config/test_find.py` & `ddev-2.0.0/tests/cli/config/test_find.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 import pytest
-
 from ddev.config.constants import ConfigEnvVars
 
 
 def test_copy(ddev, config_file, mocker):
     mock = mocker.patch('pyperclip.copy')
     result = ddev('config', 'find', '-c')
```

### Comparing `ddev-1.6.0/tests/cli/config/test_restore.py` & `ddev-2.0.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/cli/config/test_set.py` & `ddev-2.0.0/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/cli/config/test_show.py` & `ddev-2.0.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/cli/status/test_status.py` & `ddev-2.0.0/tests/cli/status/test_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import pytest
-
 from ddev.config.constants import AppEnvVars
 from ddev.utils.structures import EnvVars
 
 
 def test_repo_configured_default(ddev, helpers, repository):
     result = ddev('status')
```

### Comparing `ddev-1.6.0/tests/cli/validate/test_manifest.py` & `ddev-2.0.0/tests/cli/validate/test_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import json
 
 import pytest
-
 from ddev.utils.structures import EnvVars
 
 
 @pytest.fixture(scope='module', autouse=True)
 def terminal_width():
     with EnvVars({'COLUMNS': '200'}):
         yield
```

### Comparing `ddev-1.6.0/tests/config/test_model.py` & `ddev-2.0.0/tests/config/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 import pytest
-
 from ddev.config.model import ConfigurationError, RootConfig
 
 
 def test_default():
     config = RootConfig({})
     config.parse_fields()
```

### Comparing `ddev-1.6.0/tests/helpers/api.py` & `ddev-2.0.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/integration/test_core.py` & `ddev-2.0.0/tests/integration/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/repo/test_core.py` & `ddev-2.0.0/tests/repo/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 import pytest
-
 from ddev.integration.core import Integration
 from ddev.repo.config import RepositoryConfig
 from ddev.repo.constants import NOT_SHIPPABLE
 from ddev.repo.core import IntegrationRegistry, Repository
 
 
 def test_attributes(local_repo):
```

### Comparing `ddev-1.6.0/tests/utils/test_fs.py` & `ddev-2.0.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/utils/test_git.py` & `ddev-2.0.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/utils/test_json.py` & `ddev-2.0.0/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/utils/test_platform.py` & `ddev-2.0.0/tests/utils/test_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import pytest
-
 from ddev.utils.platform import Platform
 
 
 @pytest.mark.requires_windows
 class TestWindows:
     def test_tag(self):
         assert Platform().windows is True
```

### Comparing `ddev-1.6.0/tests/utils/test_structures.py` & `ddev-2.0.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/tests/validation/test_tracker.py` & `ddev-2.0.0/tests/validation/test_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import pytest
+from ddev.validation.tracker import ValidationTracker
 from rich.console import Console
 from rich.style import Style
 from rich.tree import Tree
 
-from ddev.validation.tracker import ValidationTracker
-
 
 def get_tracker():
     return ValidationTracker(
         Console(),
         Tree('validate test', style=Style.parse('bold')),
         success_style=Style.parse('bold cyan'),
         error_style=Style.parse('bold red'),
```

### Comparing `ddev-1.6.0/.gitignore` & `ddev-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/README.md` & `ddev-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-1.6.0/PKG-INFO` & `ddev-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 1.6.0
+Version: 2.0.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
-Requires-Dist: datadog-checks-dev[cli]~=18.0
+Requires-Dist: datadog-checks-dev[cli]~=19.0
 Requires-Dist: hatch>=1.6.3
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
 Requires-Dist: pyperclip
 Requires-Dist: rich>=12.5.1
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
```

