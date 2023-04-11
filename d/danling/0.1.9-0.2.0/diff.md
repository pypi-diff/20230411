# Comparing `tmp/danling-0.1.9.tar.gz` & `tmp/danling-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.1.9.tar", last modified: Tue Apr  4 04:21:12 2023, max compression
+gzip compressed data, was "danling-0.2.0.tar", last modified: Tue Apr 11 13:46:07 2023, max compression
```

## Comparing `danling-0.1.9.tar` & `danling-0.2.0.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.430591 danling-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.406589 danling-0.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 04:21:03.000000 danling-0.1.9/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.406589 danling-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-04 04:21:03.000000 danling-0.1.9/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-04 04:21:03.000000 danling-0.1.9/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-04 04:21:03.000000 danling-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.406589 danling-0.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-04 04:21:03.000000 danling-0.1.9/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-04 04:21:12.430591 danling-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-04 04:21:03.000000 danling-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-04 04:21:03.000000 danling-0.1.9/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-04 04:21:03.000000 danling-0.1.9/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 04:21:11.000000 danling-0.1.9/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 04:21:03.000000 danling-0.1.9/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-04 04:21:03.000000 danling-0.1.9/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-04 04:21:03.000000 danling-0.1.9/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-04 04:21:03.000000 danling-0.1.9/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 04:21:03.000000 danling-0.1.9/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 04:21:03.000000 danling-0.1.9/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-04 04:21:03.000000 danling-0.1.9/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-04 04:21:03.000000 danling-0.1.9/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13145 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21016 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-04 04:21:03.000000 danling-0.1.9/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-04 04:21:03.000000 danling-0.1.9/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-04 04:21:03.000000 danling-0.1.9/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-04 04:21:03.000000 danling-0.1.9/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-04 04:21:03.000000 danling-0.1.9/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 04:21:03.000000 danling-0.1.9/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-04 04:21:03.000000 danling-0.1.9/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-04 04:21:03.000000 danling-0.1.9/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-04 04:21:03.000000 danling-0.1.9/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.410590 danling-0.1.9/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-04 04:21:12.000000 danling-0.1.9/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-04 04:21:12.000000 danling-0.1.9/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 04:21:12.000000 danling-0.1.9/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-04 04:21:12.000000 danling-0.1.9/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 04:21:12.000000 danling-0.1.9/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 04:21:03.000000 danling-0.1.9/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 04:21:03.000000 danling-0.1.9/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-04 04:21:03.000000 danling-0.1.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 04:21:03.000000 danling-0.1.9/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 04:21:03.000000 danling-0.1.9/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 04:21:03.000000 danling-0.1.9/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-04 04:21:03.000000 danling-0.1.9/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 04:21:03.000000 danling-0.1.9/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-04 04:21:03.000000 danling-0.1.9/docs/runner/bases.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 04:21:03.000000 danling-0.1.9/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-04 04:21:03.000000 danling-0.1.9/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-04 04:21:03.000000 danling-0.1.9/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-04 04:21:03.000000 danling-0.1.9/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-04 04:21:03.000000 danling-0.1.9/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-04 04:21:03.000000 danling-0.1.9/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-04 04:21:03.000000 danling-0.1.9/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-04 04:21:03.000000 danling-0.1.9/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-04 04:21:03.000000 danling-0.1.9/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-04 04:21:03.000000 danling-0.1.9/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.406589 danling-0.1.9/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.414590 danling-0.1.9/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.426591 danling-0.1.9/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.426591 danling-0.1.9/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.430591 danling-0.1.9/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-04 04:21:03.000000 danling-0.1.9/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-04 04:21:03.000000 danling-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 04:21:03.000000 danling-0.1.9/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 04:21:03.000000 danling-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 04:21:12.430591 danling-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 04:21:03.000000 danling-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:21:12.430591 danling-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-04 04:21:03.000000 danling-0.1.9/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.849398 danling-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-11 13:46:03.000000 danling-0.2.0/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-11 13:46:03.000000 danling-0.2.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 13:46:03.000000 danling-0.2.0/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-11 13:46:03.000000 danling-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-11 13:46:03.000000 danling-0.2.0/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-11 13:46:07.849398 danling-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-11 13:46:03.000000 danling-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-11 13:46:03.000000 danling-0.2.0/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 13:46:03.000000 danling-0.2.0/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 13:46:07.000000 danling-0.2.0/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-11 13:46:03.000000 danling-0.2.0/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 13:46:03.000000 danling-0.2.0/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-11 13:46:03.000000 danling-0.2.0/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-11 13:46:03.000000 danling-0.2.0/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 13:46:03.000000 danling-0.2.0/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 13:46:03.000000 danling-0.2.0/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 13:46:03.000000 danling-0.2.0/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-11 13:46:03.000000 danling-0.2.0/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 13:46:07.000000 danling-0.2.0/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 13:46:03.000000 danling-0.2.0/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 13:46:03.000000 danling-0.2.0/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 13:46:03.000000 danling-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-11 13:46:03.000000 danling-0.2.0/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.833397 danling-0.2.0/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 13:46:03.000000 danling-0.2.0/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:46:03.000000 danling-0.2.0/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:46:03.000000 danling-0.2.0/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 13:46:03.000000 danling-0.2.0/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 13:46:03.000000 danling-0.2.0/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 13:46:03.000000 danling-0.2.0/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 13:46:03.000000 danling-0.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.829397 danling-0.2.0/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.837397 danling-0.2.0/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.845398 danling-0.2.0/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 13:46:03.000000 danling-0.2.0/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 13:46:03.000000 danling-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 13:46:03.000000 danling-0.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 13:46:03.000000 danling-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:46:07.849398 danling-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:46:03.000000 danling-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:46:07.849398 danling-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-11 13:46:03.000000 danling-0.2.0/tests/test_runner.py
```

### Comparing `danling-0.1.9/.github/workflows/docs.yaml` & `danling-0.2.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/.github/workflows/push.yaml` & `danling-0.2.0/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/.gitignore` & `danling-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.Apache2` & `danling-0.2.0/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.BSD2` & `danling-0.2.0/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.BSD3` & `danling-0.2.0/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.BSD4` & `danling-0.2.0/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.GPL2` & `danling-0.2.0/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.GPL3` & `danling-0.2.0/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.MIT` & `danling-0.2.0/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/LICENSES/LICENSE.Unlicense` & `danling-0.2.0/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/PKG-INFO` & `danling-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.1.9/README.md` & `danling-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/anaconda-project.yml` & `danling-0.2.0/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/__init__.py` & `danling-0.2.0/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/metrics/average_meter.py` & `danling-0.2.0/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/metrics/average_meters.py` & `danling-0.2.0/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/__init__.py` & `danling-0.2.0/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/mlp/dense.py` & `danling-0.2.0/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/mlp/mlp.py` & `danling-0.2.0/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/__init__.py` & `danling-0.2.0/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.0/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.0/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/decoder.py` & `danling-0.2.0/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/encoder.py` & `danling-0.2.0/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.0/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.0/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.2.0/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/registry.py` & `danling-0.2.0/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/runner/README.md` & `danling-0.2.0/danling/runner/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 # Runner
 
 The Runner of DanLing sets up the basic environment for running neural networks.
 
 ## Components
 
-For readability and maintainability, there are three levels of Runner:
+For readability and maintainability, there are three levels of Runner + a RunnerState.
 
-### [`RunnerBase`][danling.runner.bases.RunnerBase]
+The RunnerState stores all the information that is critical for a run and is stored in the checkpoint (e.g. `epochs`, `run_id`, etc.).
+With RunnerState and corresponding weights, you can resume a run from any point.
 
-[`RunnerBase`][danling.runner.bases.RunnerBase] gives you a basic instinct on what attributes and properties are provided by the Runner.
+The Runner contains all runtime information that is irrelevant to the checkpoint (e.g. `world_size`, `rank`, etc.).
+
+### [`RunnerState`][danling.runner.runner_state.RunnerState]
+
+[`RunnerState`][danling.runner.runner_state.RunnerState] stores the state of a run.
+
+All attributes stored in `RunnerState` will be saved in the checkpoint, and thus should be json serialisable.
+Except for `@property` of json serialisable attributes.
+
+### [`RunnerBase`][danling.runner.runner_base.RunnerBase]
+
+[`RunnerBase`][danling.runner.abstract_base_runner.RunnerBase] gives you a basic instinct on what attributes and properties are provided by the Runner.
 
 It works in an AbstractBaseClass manner and should neither be used directly nor be inherited from.
 
 ### [`BaseRunner`][danling.runner.BaseRunner]
 
 [`BaseRunner`][danling.runner.BaseRunner] contains core methods of general basic functionality,
 such as `init_logging`, `append_result`, `print_result`.
@@ -76,7 +88,26 @@
 
 To help you manage your experiments, DanLing will automatically generate directories for you.
 
 `dir` is the directory of a certain run, defaults to `{dir/name-id}`.
 All run files should be under this directory.
 
 In particular, `checkpoint_dir`, which defaults to `dir/checkpoint_dir_name` contains all checkpoint files.
+
+As a result, your `project_root` should looks like following:
+
+```bash
+- {project_root}
+-     |- {name}-{id} (equivalents to {experiment_name}-{run_name}-{experiment_id}-{run_id}-{uuid})
+-       |
+-       |- {checkpoint_dir_name}
+-       |    |
+-       |    |- best.pth
+-       |    |- latest.pth
+-       |    |- epoch-10.pth
+-       |
+-       |- run.log
+-       |- runner.yaml
+-       |- results.json
+-       |- latest.json
+-       |- best.json
+```
```

### Comparing `danling-0.1.9/danling/runner/base_runner.py` & `danling-0.2.0/danling/runner/base_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-import atexit
 import logging
 import logging.config
 import os
 import random
 import shutil
 from typing import Callable, Mapping, Optional, Tuple, Union
 from warnings import warn
 
 import numpy as np
 from chanfig import FlatDict, NestedDict
 
 from danling.utils import catch
 
-from .bases import RunnerBase
+from .runner_base import RunnerBase
 from .utils import on_main_process
 
 
 class BaseRunner(RunnerBase):
     r"""
     Base class for running a neural network.
 
@@ -40,16 +39,14 @@
             self.set_deterministic()
         if self.log:
             self.init_logging()
         self.init_print()
         if self.tensorboard:
             self.init_tensorboard()
 
-        atexit.register(self.print_result)
-
     @on_main_process
     def init_logging(self) -> None:
         r"""
         Set up logging.
         """
 
         # Why is setting up proper logging so !@?#! ugly?
@@ -138,15 +135,16 @@
                 This avoids same data augmentation are applied on every processes.
 
                 Defaults to `self.rank`.
 
                 Set to `False` to disable this feature.
         """
 
-        seed = self.seed
+        if seed is None:
+            seed = self.seed
         if bias is None:
             bias = self.rank
         if bias:
             seed += bias
         np.random.seed(seed)
         random.seed(seed)
 
@@ -198,17 +196,17 @@
 
         if self.optimizer is not None:
             self.optimizer.step()
             if zero_grad:
                 self.optimizer.zero_grad()
         if self.scheduler is not None:
             self.scheduler.step()
-        self.steps += 1
+        self.state.steps += 1
         # TODO: Support `drop_last = False`
-        self.iters += self.batch_size_equivalent
+        self.state.iters += self.batch_size_equivalent
 
     def state_dict(self, cls: Callable = dict) -> Mapping:
         r"""
         Return dict of all attributes for checkpoint.
         """
 
         raise NotImplementedError
```

### Comparing `danling-0.1.9/danling/runner/torch_runner.py` & `danling-0.2.0/danling/runner/torch_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,48 +23,46 @@
         accelerator (Accelerator):
         accelerate: Defaults to `{}`.
             if is `None`, will not use `accelerate`.
     """
 
     # pylint: disable=R0902
 
-    accelerator: Accelerator
-    accelerate: Mapping[str, Any]
-
-    def __init__(self, *args, **kwargs) -> None:
-        self.accelerate = {}
-        super().__init__(*args, **kwargs)
+    accelerator: Accelerator = None  # type: ignore
+    accelerate: Mapping[str, Any] = None  # type: ignore
 
     def init_distributed(self) -> None:
         r"""
         Set up distributed training.
 
         Initialise process group and set up DDP variables.
         """
 
+        if self.accelerate is None:
+            self.accelerate = {}
         self.accelerator = Accelerator(**self.accelerate)
         if self.distributed:
-            object_list = [self.id, self.uuid]
+            object_list = [self.state.id]
             dist.broadcast_object_list(object_list)
-            self.id, self.uuid = object_list[0], object_list[1]
+            self.state.id = object_list[0]
 
     @on_main_process
     def init_tensorboard(self, *args, **kwargs) -> None:
         r"""
         Set up Tensoraoard SummaryWriter.
         """
         from torch.utils.tensorboard.writer import SummaryWriter  # pylint: disable=C0415
 
         if "log_dir" not in kwargs:
             kwargs["log_dir"] = self.dir
 
         self.writer = SummaryWriter(*args, **kwargs)
         self.writer.add_scalar = catch(OSError, verbose=False)(self.writer.add_scalar)  # type: ignore
 
-    def set_seed(self, seed: Optional[int] = None, bias: Optional[int] = None) -> None:
+    def set_seed(self, seed: int = None, bias: Optional[int] = None) -> None:  # type: ignore
         r"""
         Set up random seed.
 
         Args:
             seed: Random seed to set.
                 Defaults to `self.seed` (`config.seed`).
 
@@ -82,16 +80,16 @@
         if self.distributed:
             object_list = [seed]
             dist.broadcast_object_list(object_list)
             seed = object_list[0]
         if bias is None:
             bias = self.rank
         if bias:
-            seed += bias
-        self.seed = seed
+            seed += bias  # type: ignore
+        self.state.seed = seed
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
     def set_deterministic(self) -> None:
         r"""
@@ -108,15 +106,15 @@
         Return dict of all attributes for checkpoint.
         """
 
         if self.model is None:
             raise ValueError("Model must be defined when calling state_dict")
         model = self.accelerator.unwrap_model(self.model)
         return cls(
-            runner=self.dict(),
+            runner=self.state.dict(),
             model=model.state_dict(),
             optimizer=self.optimizer.state_dict() if self.optimizer else None,
             scheduler=self.scheduler.state_dict() if self.scheduler else None,
         )
 
     def prepare(self, *args, device_placement: Optional[List[bool]] = None) -> None:
         r"""
@@ -228,10 +226,14 @@
         r"""
         Reduce tensor.
         """
 
         return self.accelerator.reduce(tensor, reduction=reduction)
 
     def __getattr__(self, name: str) -> Any:
+        try:
+            return super().__getattr__(name)
+        except AttributeError:
+            pass
         if self.accelerator is not None and hasattr(self.accelerator, name):
             return getattr(self.accelerator, name)
-        return super().__getattr__(name)
+        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
```

### Comparing `danling-0.1.9/danling/runner/utils.py` & `danling-0.2.0/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/tensors/nested_tensor.py` & `danling-0.2.0/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/tensors/torch_func_registry.py` & `danling-0.2.0/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/utils/basex.py` & `danling-0.2.0/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/utils/decorators.py` & `danling-0.2.0/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling/utils/io.py` & `danling-0.2.0/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/danling.egg-info/PKG-INFO` & `danling-0.2.0/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.1.9/danling.egg-info/SOURCES.txt` & `danling-0.2.0/danling.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 danling/modules/transformer/pos_embed/pos_embed.py
 danling/optim/__init__.py
 danling/optim/lr_scheduler/__init__.py
 danling/optim/lr_scheduler/lr_scheduler.py
 danling/runner/README.md
 danling/runner/__init__.py
 danling/runner/base_runner.py
-danling/runner/bases.py
+danling/runner/runner_base.py
+danling/runner/runner_state.py
 danling/runner/torch_runner.py
 danling/runner/utils.py
 danling/tensors/__init__.py
 danling/tensors/nested_tensor.py
 danling/tensors/torch_func_registry.py
 danling/utils/__init__.py
 danling/utils/basex.py
@@ -64,16 +65,17 @@
 docs/index.md
 docs/manifest.webmanifest
 docs/package.md
 docs/registry.md
 docs/blog/index.md
 docs/metrics/average_meter.md
 docs/runner/base_runner.md
-docs/runner/bases.md
 docs/runner/index.md
+docs/runner/runner_base.md
+docs/runner/runner_state.md
 docs/runner/torch_runner.md
 docs/runner/utils.md
 docs/tensors/nested_tensor.md
 docs/tensors/pn_tensor.md
 docs/tensors/torch_func_registry.md
 docs/utils/basex.md
 docs/utils/decorators.md
```

### Comparing `danling-0.1.9/mkdocs.yml` & `danling-0.2.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 repo_name: DanLing
 repo_url: https://github.com/ZhiyuanChen/DanLing
 
 nav:
   - DanLing: index.md
   - Runner:
       - runner/index.md
-      - RunnerBase: runner/bases.md
+      - RunnerState: runner/runner_state.md
+      - RunnerBase: runner/runner_base.md
       - BaseRunner: runner/base_runner.md
       - TorchRunner: runner/torch_runner.md
       - Utilities: runner/utils.md
   - Tensors:
     - NestedTensor: tensors/nested_tensor.md
     - PNTensor: tensors/pn_tensor.md
     - TorchFuncRegistry: tensors/torch_func_registry.md
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 site_name: DanLing site_url: https://danling.org site_author: DanLing
 Contributors site_description: Easier Configuration copyright: All rights
 reserved © 2021-2023, DanLing Contributors repo_name: DanLing repo_url: https:/
 /github.com/ZhiyuanChen/DanLing nav: - DanLing: index.md - Runner: - runner/
-index.md - RunnerBase: runner/bases.md - BaseRunner: runner/base_runner.md -
-TorchRunner: runner/torch_runner.md - Utilities: runner/utils.md - Tensors: -
-NestedTensor: tensors/nested_tensor.md - PNTensor: tensors/pn_tensor.md -
-TorchFuncRegistry: tensors/torch_func_registry.md - Registry: registry.md -
-Metrics: - AverageMeter: metrics/average_meter.md - Utils: - Decorator: utils/
+index.md - RunnerState: runner/runner_state.md - RunnerBase: runner/
+runner_base.md - BaseRunner: runner/base_runner.md - TorchRunner: runner/
+torch_runner.md - Utilities: runner/utils.md - Tensors: - NestedTensor:
+tensors/nested_tensor.md - PNTensor: tensors/pn_tensor.md - TorchFuncRegistry:
+tensors/torch_func_registry.md - Registry: registry.md - Metrics: -
+AverageMeter: metrics/average_meter.md - Utils: - Decorator: utils/
 decorators.md - IO: utils/io.md - basex: utils/basex.md - package: package.md #
 - Blog: blog/index.md theme: name: material custom_dir: overrides language:
 "zh" palette: - media: "(prefers-color-scheme: dark)" scheme: slate primary:
 blue grey accent: teal toggle: icon: material/brightness-4 name: Switch to
 light mode - media: "(prefers-color-scheme: light)" scheme: default primary:
 blue grey accent: teal toggle: icon: material/brightness-7 name: Switch to dark
 mode logo: "assets/images/logo.png" favicon: "assets/images/logo.ico" features:
```

### Comparing `danling-0.1.9/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.0/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.0/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.0/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.0/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/assets/images/favicon.ico` & `danling-0.2.0/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/assets/images/logo.png` & `danling-0.2.0/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/overrides/main.html` & `danling-0.2.0/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/pyproject.toml` & `danling-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.1.9/tests/test_runner.py` & `danling-0.2.0/tests/test_runner.py`

 * *Files identical despite different names*

