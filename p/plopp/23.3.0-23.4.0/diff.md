# Comparing `tmp/plopp-23.3.0.tar.gz` & `tmp/plopp-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plopp-23.3.0.tar", last modified: Thu Mar  9 09:16:55 2023, max compression
+gzip compressed data, was "plopp-23.4.0.tar", last modified: Tue Apr 11 12:29:14 2023, max compression
```

## Comparing `plopp-23.3.0.tar` & `plopp-23.4.0.tar`

### file list

```diff
@@ -1,191 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.323700 plopp-23.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-03-09 09:16:37.000000 plopp-23.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-03-09 09:16:37.000000 plopp-23.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-03-09 09:16:37.000000 plopp-23.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-03-09 09:16:37.000000 plopp-23.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-03-09 09:16:37.000000 plopp-23.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-03-09 09:16:37.000000 plopp-23.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-03-09 09:16:37.000000 plopp-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-03-09 09:16:55.323700 plopp-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-03-09 09:16:37.000000 plopp-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-03-09 09:16:37.000000 plopp-23.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.291699 plopp-23.3.0/docs/_static/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_static/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.295699 plopp-23.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.295699 plopp-23.3.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.295699 plopp-23.3.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/faq.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.295699 plopp-23.3.0/docs/about/reference/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/reference/matplotlib.rst
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/reference/plotly.rst
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/reference/pythreejs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/about/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.299699 plopp-23.3.0/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/image-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/inspector-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8577 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/line-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/saving-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/scatter3d-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/slicer-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/basics/super-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8831 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.299699 plopp-23.3.0/docs/customization/
--rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/customization/subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5236 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/customization/tweaking-figures.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.299699 plopp-23.3.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (122)    17409 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/custom-interfaces.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.299699 plopp-23.3.0/docs/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)     4846 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/gallery/masking-a-range.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/gallery/nyc-taxi.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     7018 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/gallery/rectangle-selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/gallery/scatter3d-with-threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/examples/gallery.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-03-09 09:16:37.000000 plopp-23.3.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-03-09 09:16:37.000000 plopp-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.303699 plopp-23.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/mini.in
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/mini.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/noplotly.in
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/noplotly.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-09 09:16:37.000000 plopp-23.3.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.303699 plopp-23.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-03-09 09:16:37.000000 plopp-23.3.0/resources/logo-plopp-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-03-09 09:16:55.323700 plopp-23.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.283699 plopp-23.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.303699 plopp-23.3.0/src/plopp/
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.307699 plopp-23.3.0/src/plopp/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.307699 plopp-23.3.0/src/plopp/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     5961 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/interactive.py
--rw-r--r--   0 runner    (1001) docker     (122)     8832 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/line.py
--rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/matplotlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.307699 plopp-23.3.0/src/plopp/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/plotly/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/plotly/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     8998 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/plotly/line.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.311699 plopp-23.3.0/src/plopp/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/pythreejs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6981 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/pythreejs/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/pythreejs/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/pythreejs/outline.py
--rw-r--r--   0 runner    (1001) docker     (122)     5041 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/backends/pythreejs/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.311699 plopp-23.3.0/src/plopp/core/
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3014 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/limits.py
--rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6202 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.311699 plopp-23.3.0/src/plopp/data/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/data/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.315699 plopp-23.3.0/src/plopp/functions/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3479 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/inspector.py
--rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/slicer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/functions/superplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.315699 plopp-23.3.0/src/plopp/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/basefig.py
--rw-r--r--   0 runner    (1001) docker     (122)     9811 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/colormapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/figimage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/figline.py
--rw-r--r--   0 runner    (1001) docker     (122)     6774 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/figscatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/graphics/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/src/plopp/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/checkboxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    12003 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/cut3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5541 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/drawing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/slice.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     4246 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7454 2023-03-09 09:16:37.000000 plopp-23.3.0/src/plopp/widgets/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.307699 plopp-23.3.0/src/plopp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-03-09 09:16:55.000000 plopp-23.3.0/src/plopp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4667 2023-03-09 09:16:55.000000 plopp-23.3.0/src/plopp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 09:16:55.000000 plopp-23.3.0/src/plopp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-09 09:16:55.000000 plopp-23.3.0/src/plopp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-09 09:16:55.000000 plopp-23.3.0/src/plopp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.287699 plopp-23.3.0/tests/backends/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/tests/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3680 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_image_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_interactive_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/matplotlib/mpl_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/tests/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/plotly/plotly_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/plotly/plotly_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3847 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/plotly/plotly_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/tests/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/pythreejs/pythreejs_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/pythreejs/pythreejs_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.319699 plopp-23.3.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/core/graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/core/limits_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/core/model_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.323700 plopp-23.3.0/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/common_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/inspector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8015 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/plot_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/scatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3203 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/slicer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/functions/superplot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.323700 plopp-23.3.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     5362 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/graphics/colormapper_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4802 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/graphics/figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/graphics/figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/graphics/figscatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/high_level_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/minimal_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 09:16:55.323700 plopp-23.3.0/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/widgets/box_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/widgets/checkboxes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/widgets/cut3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-03-09 09:16:37.000000 plopp-23.3.0/tests/widgets/slice_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-03-09 09:16:37.000000 plopp-23.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.577211 plopp-23.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-04-11 12:28:58.000000 plopp-23.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 12:28:58.000000 plopp-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-11 12:28:58.000000 plopp-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-04-11 12:29:14.617212 plopp-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:28:58.000000 plopp-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-04-11 12:28:58.000000 plopp-23.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_static/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    18766 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/faq.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/about/reference/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/matplotlib.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/plotly.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/pythreejs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/image-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/inspector-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/line-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/saving-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/scatter3d-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/slicer-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/super-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9238 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/customization/
+-rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/customization/subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/customization/tweaking-figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    19809 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/custom-interfaces.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/masking-a-range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/nyc-taxi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     6988 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/rectangle-selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/scatter3d-with-slider.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/scatter3d-with-threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/getting-started/numpy-pandas-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/getting-started/overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-04-11 12:28:58.000000 plopp-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/mini.in
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/mini.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/noplotly.in
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/noplotly.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-04-11 12:28:58.000000 plopp-23.4.0/resources/logo-plopp-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-11 12:29:14.617212 plopp-23.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.573211 plopp-23.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/src/plopp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12570 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5557 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8124 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/line.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.597211 plopp-23.4.0/src/plopp/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8089 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/outline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.597211 plopp-23.4.0/src/plopp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/limits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7013 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.601211 plopp-23.4.0/src/plopp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.601211 plopp-23.4.0/src/plopp/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6627 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/superplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.605212 plopp-23.4.0/src/plopp/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/basefig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9762 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figimage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6637 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figscatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/src/plopp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/checkboxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11209 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/cut3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3935 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.577211 plopp-23.4.0/tests/backends/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_interactive_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)     8670 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/inspector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9973 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/scatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/slicer_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/superplot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     5308 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/colormapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5911 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figscatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/high_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/minimal_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/box_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/checkboxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/cut3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/slice_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-04-11 12:28:58.000000 plopp-23.4.0/tox.ini
```

### Comparing `plopp-23.3.0/.github/workflows/ci.yml` & `plopp-23.4.0/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   formatting:
     name: Formatting and static analysis
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.9
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
       - uses: stefanzweifel/git-auto-commit-action@v4
         with:
           commit_message: Apply automatic formatting
 
@@ -33,15 +33,15 @@
     name: Tests
     needs: formatting
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.9
       - run: sudo apt install --yes graphviz graphviz-dev
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox
 
   docs:
     needs: tests
```

### Comparing `plopp-23.3.0/.github/workflows/docs.yml` & `plopp-23.4.0/.github/workflows/docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       - run: sudo apt install --yes graphviz pandoc
       - uses: actions/checkout@v3
         with:
           ref: ${{ inputs.version }}
           fetch-depth: 0  # history required so setuptools_scm can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.9
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
           tox --skip-pkg-install -e docs -- plopp==${VERSION}
           echo "target=$(python docs/version.py --repo=plopp --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
```

### Comparing `plopp-23.3.0/.github/workflows/release.yml` & `plopp-23.4.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
@@ -66,30 +66,30 @@
     steps:
       - uses: actions/download-artifact@v2
       - uses: conda-incubator/setup-miniconda@v2
       - run: conda install -c conda-forge --yes anaconda-client
       - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
       - uses: actions/setup-python@v3
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   manage-versions:
     name: Manage Versions
     runs-on: ubuntu-20.04
     outputs:
       version-new: ${{ steps.version.outputs.new }}
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.9
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
         run: |
           echo "::set-output name=new::$(python docs/version.py --repo=plopp --version=${GITHUB_REF_NAME} --action=is-new)"
           echo "::set-output name=replaced::$(python docs/version.py --repo=plopp --version=${GITHUB_REF_NAME} --action=get-replaced)"
```

### Comparing `plopp-23.3.0/.pre-commit-config.yaml` & `plopp-23.4.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,18 @@
         args: [ --markdown-linebreak-ext=md ]
         exclude: '\.svg'
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
-  - repo: https://github.com/pre-commit/mirrors-yapf
-    rev: v0.32.0
+  - repo: https://github.com/psf/black
+    rev: 23.1.0
     hooks:
-      - id: yapf
-        args: [ "-i", "-r" ]
-        types: [ "python" ]
-        additional_dependencies: [ "toml" ]
+      - id: black
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
```

### Comparing `plopp-23.3.0/LICENSE` & `plopp-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/PKG-INFO` & `plopp-23.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.3.0
+Version: 23.4.0
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.3.0/README.md` & `plopp-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_static/favicon.ico` & `plopp-23.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png` & `plopp-23.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_static/logo.svg` & `plopp-23.4.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_templates/scipp-class-template.rst` & `plopp-23.4.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_templates/scipp-module-template.rst` & `plopp-23.4.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/_templates/sections/header-article.html` & `plopp-23.4.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/about/about.rst` & `plopp-23.4.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/about/faq.ipynb` & `plopp-23.4.0/docs/about/faq.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/about/reference.rst` & `plopp-23.4.0/docs/about/reference.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 Graphics
 ========
 
 .. autosummary::
    :toctree: generated
 
+   graphics.Camera
    graphics.ColorMapper
    graphics.FigImage
    graphics.FigLine
    graphics.FigScatter3d
    graphics.figure1d
    graphics.figure2d
    graphics.figure3d
```

### Comparing `plopp-23.3.0/docs/basics/image-plot.ipynb` & `plopp-23.4.0/docs/basics/image-plot.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989054951690821%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import plopp as pp')], delete: [2, 1]}}, 13: {'source': "*

 * *            '[\'da.plot(\\n\', \'    crop={\\n\', "        \'x\': {\'min\': sc.scalar(20, '*

 * *            'unit=\'m\'), \'max\': sc.scalar(35, unit=\'m\')},\\n", "        \'y\': {\'min\': '*

 * *            'sc.scalar(10, unit=\'m\')},\\n", \'    }\\n\', \')\']}, 21: {\'source\': {insert: '*

 * *            '[(1, "da.coords[\'x2\'] = da.coords[\'x\'] ** 2\\n"), (2, "da.coords[\'y2\'] = '*

 * *            'da.coords[\'y\'] ** […]*

```diff
@@ -12,16 +12,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "b39377b6-a67b-4f35-92bb-b0f9be2b0b0e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
-                "import plopp as pp\n",
-                "pp.patch_scipp()"
+                "import plopp as pp"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8487626a-2461-40c2-b0cd-42c6f82c9fab",
             "metadata": {},
             "source": [
@@ -122,17 +121,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a430e707-71ad-4276-ae67-bf1caa989224",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da.plot(crop={'x': {'min': sc.scalar(20, unit='m'),\n",
-                "                     'max': sc.scalar(35, unit='m')},\n",
-                "              'y': {'min': sc.scalar(10, unit='m')}})"
+                "da.plot(\n",
+                "    crop={\n",
+                "        'x': {'min': sc.scalar(20, unit='m'), 'max': sc.scalar(35, unit='m')},\n",
+                "        'y': {'min': sc.scalar(10, unit='m')},\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3e112469-76b6-4cdf-8494-9806e641fb25",
             "metadata": {},
             "source": [
@@ -202,16 +204,16 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "1b1714d6-c981-4b9d-bdbb-f96ec32e1d5e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = pp.data.data2d()\n",
-                "da.coords['x2'] = da.coords['x']**2\n",
-                "da.coords['y2'] = da.coords['y']**2\n",
+                "da.coords['x2'] = da.coords['x'] ** 2\n",
+                "da.coords['y2'] = da.coords['y'] ** 2\n",
                 "pp.plot(da, coords=['x2', 'y2'])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b16b749d-0130-4ecf-964e-036d84a73317",
             "metadata": {},
```

### Comparing `plopp-23.3.0/docs/basics/inspector-plot.ipynb` & `plopp-23.4.0/docs/basics/inspector-plot.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942380150713485%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(1, "p = pp.inspector(da, dim=\'z\', '*

 * *            'orientation=\'vertical\')")], delete: [1]}}, 3: {\'source\': {insert: [(11, \'\\n\'), '*

 * *            "(15, '\\n'), (17, '    f1.children = [\\n'), (18, '        f1.top_bar,\\n'), (19, "*

 * *            "'        HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]),\\n'), (20, '        "*

 * *            "f1.bottom_bar,\\n'), (21, '    ]\\n'), (23, '    f2.children = [\\n'), (24, '        "*

 * *            "f2.top_bar,\\n'), (25 […]*

```diff
@@ -34,15 +34,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "f152c042-c22a-44c2-8ab1-f712cf8f8de8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = pp.data.data3d()\n",
-                "p = pp.inspector(da, orientation='vertical')"
+                "p = pp.inspector(da, dim='z', orientation='vertical')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9dea0be0-1bd0-453e-8c91-fb7b5706341f",
             "metadata": {
@@ -58,20 +58,31 @@
                 "tool = p.children[0].toolbar['inspect']\n",
                 "tool.value = True\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x, y = 40 * np.random.random(2)\n",
                 "    tool._tool.click(x, y)\n",
                 "\n",
+                "\n",
                 "def update(pl):\n",
                 "    from ipywidgets import HBox\n",
+                "\n",
                 "    f1 = pl.children[0]\n",
-                "    f1.children = [f1.top_bar, HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]), f1.bottom_bar]\n",
+                "    f1.children = [\n",
+                "        f1.top_bar,\n",
+                "        HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]),\n",
+                "        f1.bottom_bar,\n",
+                "    ]\n",
                 "    f2 = pl.children[1]\n",
-                "    f2.children = [f2.top_bar, HBox([f2.left_bar, f2.canvas.to_image(), f2.right_bar]), f2.bottom_bar]\n",
+                "    f2.children = [\n",
+                "        f2.top_bar,\n",
+                "        HBox([f2.left_bar, f2.canvas.to_image(), f2.right_bar]),\n",
+                "        f2.bottom_bar,\n",
+                "    ]\n",
+                "\n",
                 "\n",
                 "update(p)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -149,14 +160,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/basics/line-plot.ipynb` & `plopp-23.4.0/docs/basics/line-plot.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666667%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import plopp as pp')], delete: [2, 1]}}, 12: {'source': "*

 * *            '["da.plot(vmin=sc.scalar(-0.5, unit=\'m/s\'), vmax=sc.scalar(1.5, unit=\'m/s\'))"]}, '*

 * *            '16: {\'source\': ["da.plot(crop={\'x\': {\'min\': sc.scalar(20, unit=\'m\'), \'max\': '*

 * *            'sc.scalar(40, unit=\'m\')}})"]}, 24: {\'source\': [\'pp.plot(\\n\', "    {\'a\': da, '*

 * *            '\'b\': 0.2 * da},\\n", "    color={\'a\': \'red\', \'b\': \'black\'},\\n", "    '*

 * *            'li […]*

```diff
@@ -12,16 +12,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "b39377b6-a67b-4f35-92bb-b0f9be2b0b0e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
-                "import plopp as pp\n",
-                "pp.patch_scipp()"
+                "import plopp as pp"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8487626a-2461-40c2-b0cd-42c6f82c9fab",
             "metadata": {},
             "source": [
@@ -120,16 +119,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "18b8d395-ce0a-4181-8b3f-2c7e0d91618f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da.plot(vmin=sc.scalar(-0.5, unit='m/s'),\n",
-                "        vmax=sc.scalar(1.5, unit='m/s'))"
+                "da.plot(vmin=sc.scalar(-0.5, unit='m/s'), vmax=sc.scalar(1.5, unit='m/s'))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e1b8596a-e5d6-43ae-b0d5-3b501cf75774",
             "metadata": {},
             "source": [
@@ -158,16 +156,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a430e707-71ad-4276-ae67-bf1caa989224",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da.plot(crop={'x': {'min': sc.scalar(20, unit='m'),\n",
-                "                    'max': sc.scalar(40, unit='m')}})"
+                "da.plot(crop={'x': {'min': sc.scalar(20, unit='m'), 'max': sc.scalar(40, unit='m')}})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4905d6a7-d5b3-4665-b03b-4005685ffad1",
             "metadata": {},
             "source": [
@@ -239,18 +236,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f22cf6e0-91aa-453e-8a96-46079d3b09a7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot({'a': da, 'b': 0.2 * da},\n",
-                "        color={'a': 'red', 'b': 'black'},\n",
-                "        linestyle={'a': 'solid', 'b': 'dashed'},\n",
-                "        marker=None)"
+                "pp.plot(\n",
+                "    {'a': da, 'b': 0.2 * da},\n",
+                "    color={'a': 'red', 'b': 'black'},\n",
+                "    linestyle={'a': 'solid', 'b': 'dashed'},\n",
+                "    marker=None,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e485478c-3652-44fc-8b47-f368dad095cb",
             "metadata": {},
             "source": [
@@ -327,15 +326,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "bfcd768c-cc4f-4973-ba55-30c4b7da2d73",
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = pp.data.data1d()\n",
-                "da.coords['x2'] = da.coords['x']**2\n",
+                "da.coords['x2'] = da.coords['x'] ** 2\n",
                 "pp.plot(da, coords=['x2'])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "123c2b07-ad46-485b-9842-8a754d1fc44b",
             "metadata": {},
```

### Comparing `plopp-23.3.0/docs/basics/saving-figures.ipynb` & `plopp-23.4.0/docs/basics/saving-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/basics/scatter3d-plot.ipynb` & `plopp-23.4.0/docs/basics/scatter3d-plot.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991590711805556%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(15, "        \'position\': sc.vectors(\\n"), (16, '*

 * *            '"            dims=[\'row\'], unit=\'m\', values=position.reshape(nclusters * '*

 * *            'npercluster, 3)\\n"), (17, \'        )\\n\'), (18, \'    },\\n\'), (19, \')\\n\')], '*

 * *            'delete: [17, 16, 15]}}, 7: {\'source\': {insert: [(9, "        \'time\': '*

 * *            'sc.array(dims=[\'row\'], unit=\'s\', values=time),\\n"), (10, \'    },\\n\'), (11, '*

 * *            "')\\n')], delete: [10, 9]}}}" […]*

```diff
@@ -52,17 +52,19 @@
                 "    r = 20.0 * np.random.normal(size=[npercluster, 3])\n",
                 "    position[n, :] = r + center\n",
                 "    values[n, :] = np.linalg.norm(r, axis=1) + n\n",
                 "\n",
                 "da = sc.DataArray(\n",
                 "    data=sc.array(dims=['row'], values=values.flatten(), unit='K'),\n",
                 "    coords={\n",
-                "        'position': sc.vectors(dims=['row'], unit='m',\n",
-                "                               values=position.reshape(nclusters*npercluster, 3))\n",
-                "    })\n",
+                "        'position': sc.vectors(\n",
+                "            dims=['row'], unit='m', values=position.reshape(nclusters * npercluster, 3)\n",
+                "        )\n",
+                "    },\n",
+                ")\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d054e1a6-e503-43e8-9a9b-2ec73c5ef6e5",
             "metadata": {},
@@ -102,16 +104,17 @@
                 "y = np.sin(time)\n",
                 "\n",
                 "da = sc.DataArray(\n",
                 "    data=sc.array(dims=['row'], values=time),\n",
                 "    coords={\n",
                 "        'x': sc.array(dims=['row'], unit='m', values=x),\n",
                 "        'y': sc.array(dims=['row'], unit='m', values=y),\n",
-                "        'time': sc.array(dims=['row'], unit='s', values=time)\n",
-                "    })\n",
+                "        'time': sc.array(dims=['row'], unit='s', values=time),\n",
+                "    },\n",
+                ")\n",
                 "\n",
                 "pp.scatter3d(da, x='x', y='y', z='time', figsize=(550, 400), pixel_size=0.2)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `plopp-23.3.0/docs/basics/slicer-plot.ipynb` & `plopp-23.4.0/docs/basics/slicer-plot.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}}"}*

```diff
@@ -18,14 +18,15 @@
             "execution_count": null,
             "id": "00f7ac7c-794e-4b71-8dcd-c147fee1ffa4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
+                "\n",
                 "da = pp.data.data3d()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "04bcabe8-0863-44aa-878b-f02b2b0e37bd",
             "metadata": {},
```

### Comparing `plopp-23.3.0/docs/basics/super-plot.ipynb` & `plopp-23.4.0/docs/basics/super-plot.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989335317460317%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 4: {'source': {insert: [(1, '\\n'), (9, "*

 * *            "'f.children = [\\n'), (10, '    f.top_bar,\\n'), (11, '    HBox([f.left_bar, "*

 * *            "f.canvas.to_image(), f.right_bar]),\\n'), (12, '    f.bottom_bar,\\n'), (13, ']')], "*

 * *            'delete: [8]}}}'}*

```diff
@@ -20,14 +20,15 @@
             "execution_count": null,
             "id": "00f7ac7c-794e-4b71-8dcd-c147fee1ffa4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
+                "\n",
                 "da = pp.data.data2d()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "04bcabe8-0863-44aa-878b-f02b2b0e37bd",
             "metadata": {},
@@ -51,22 +52,27 @@
             "id": "6deecdb6-a7af-4754-b02e-5e82da1eca68",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "from ipywidgets import HBox\n",
+                "\n",
                 "b = p.children[0].children[1].children[0]\n",
                 "sl = p.children[1].controls['y']['slider']\n",
                 "b.click()\n",
                 "sl.value = 20\n",
                 "b.click()\n",
                 "sl.value = 30\n",
                 "f = p.children[0].children[0]\n",
-                "f.children = [f.top_bar, HBox([f.left_bar, f.canvas.to_image(), f.right_bar]), f.bottom_bar]"
+                "f.children = [\n",
+                "    f.top_bar,\n",
+                "    HBox([f.left_bar, f.canvas.to_image(), f.right_bar]),\n",
+                "    f.bottom_bar,\n",
+                "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00b5ac9c-364c-4403-ba2b-7895cbc61d36",
             "metadata": {},
```

### Comparing `plopp-23.3.0/docs/conf.py` & `plopp-23.4.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,42 +38,39 @@
     l1 = []
     l1.append({"type": "link", "text": "scipp", "url": f"{base}"})
     l1.append({"type": "link", "text": "plopp", "url": f"{base}/plopp"})
     l1.append({"type": "link", "text": "scippnexus", "url": f"{base}/scippnexus"})
     l1.append({"type": "link", "text": "scippneutron", "url": f"{base}/scippneutron"})
     l1.append({"type": "link", "text": "ess", "url": f"{base}/ess"})
     header_buttons = context["header_buttons"]
-    header_buttons.append({
-        "type": "group",
-        "buttons": l1,
-        "icon": "fa fa-caret-down",
-        "text": "Related projects"
-    })
+    header_buttons.append(
+        {
+            "type": "group",
+            "buttons": l1,
+            "icon": "fa fa-caret-down",
+            "text": "Related projects",
+        }
+    )
     releases = version_info.minor_releases(first='0.1')
     if outdated:
         current = f"{long_version} (outdated)"
         latest = "latest"
         entries = ['.'.join(long_version.split('.')[:2])]
     else:
         current = f"{long_version} (latest)"
         latest = f"{releases[0]} (latest)"
         entries = releases[1:]
     lines = [{"type": "link", "text": latest, "url": f"{base}/{project}"}]
     for r in entries:
-        lines.append({
-            "type": "link",
-            "text": f"{r}",
-            "url": f"{base}/{project}/release/{r}"
-        })
-    header_buttons.append({
-        "type": "group",
-        "buttons": lines,
-        "icon": "fa fa-caret-down",
-        "text": current
-    })
+        lines.append(
+            {"type": "link", "text": f"{r}", "url": f"{base}/{project}/release/{r}"}
+        )
+    header_buttons.append(
+        {"type": "group", "buttons": lines, "icon": "fa fa-caret-down", "text": current}
+    )
 
 
 sphinx_book_theme.add_launch_buttons = add_buttons
 
 html_show_sourcelink = True
 
 extensions = [
@@ -101,15 +98,15 @@
 """  # noqa: E501
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipp': ('https://scipp.github.io/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
-    'xarray': ('https://xarray.pydata.org/en/stable/', None)
+    'xarray': ('https://xarray.pydata.org/en/stable/', None),
 }
 
 # autodocs includes everything, even irrelevant API internals. autosummary
 # looks more suitable in the long run when the API grows.
 # For a nice example see how xarray handles its API documentation.
 autosummary_generate = True
 
@@ -188,15 +185,16 @@
 }
 
 if outdated:
     html_theme_options["announcement"] = (
         f"⚠️ You are viewing the documentation for an old version of {project}. "
         f"Switch to <a href='https://scipp.github.io/{project}' "
         "style='color:white;text-decoration:underline;'"
-        ">latest</a> version. ⚠️")
+        ">latest</a> version. ⚠️"
+    )
 
 html_logo = "_static/logo.svg"
 html_favicon = "_static/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
@@ -226,16 +224,23 @@
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'scipp', u'scipp Documentation', author, 'scipp',
-     'One line description of project.', 'Miscellaneous'),
+    (
+        master_doc,
+        'scipp',
+        u'scipp Documentation',
+        author,
+        'scipp',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # -- Options for Matplotlib in notebooks ----------------------------------
 
 nbsphinx_execute_arguments = [
     "--Session.metadata=scipp_sphinx_build=True",
 ]
@@ -245,30 +250,41 @@
 doctest_global_setup = '''
 import numpy as np
 import scipp as sc
 '''
 
 # Using normalize whitespace because many __str__ functions in scipp produce
 # extraneous empty lines and it would look strange to include them in the docs.
-doctest_default_flags = doctest.ELLIPSIS | doctest.IGNORE_EXCEPTION_DETAIL | \
-                        doctest.DONT_ACCEPT_TRUE_FOR_1 | \
-                        doctest.NORMALIZE_WHITESPACE
+doctest_default_flags = (
+    doctest.ELLIPSIS
+    | doctest.IGNORE_EXCEPTION_DETAIL
+    | doctest.DONT_ACCEPT_TRUE_FOR_1
+    | doctest.NORMALIZE_WHITESPACE
+)
 
 # -- Options for linkcheck ------------------------------------------------
 
 linkcheck_ignore = [
     # Specific lines in Github blobs cannot be found by linkcheck.
     r'https?://github\.com/.*?/blob/[a-f0-9]+/.+?#',
 ]
 
 # -- Options for nbsphinx gallery------------------------------------------
-
+notebook_root = os.path.join('examples', 'gallery')
+thumbnail_root = os.path.join('_static', 'gallery')
 nbsphinx_thumbnails = {
-    'examples/gallery/nyc-taxi':
-    '_static/gallery/nyc-taxi-thumbnail.png',
-    'examples/gallery/masking-a-range':
-    '_static/gallery/masking-a-range-thumbnail.png',
-    'examples/gallery/rectangle-selection':
-    '_static/gallery/rectangle-selection-thumbnail.png',
-    'examples/gallery/scatter3d-with-threshold':
-    '_static/gallery/scatter3d-with-threshold-thumbnail.png',
+    os.path.join(notebook_root, 'nyc-taxi'): os.path.join(
+        thumbnail_root, 'nyc-taxi-thumbnail.png'
+    ),
+    os.path.join(notebook_root, 'masking-a-range'): os.path.join(
+        thumbnail_root, 'masking-a-range-thumbnail.png'
+    ),
+    os.path.join(notebook_root, 'rectangle-selection'): os.path.join(
+        thumbnail_root, 'rectangle-selection-thumbnail.png'
+    ),
+    os.path.join(notebook_root, 'scatter3d-with-threshold'): os.path.join(
+        thumbnail_root, 'scatter3d-with-threshold-thumbnail.png'
+    ),
+    os.path.join(notebook_root, 'scatter3d-with-slider'): os.path.join(
+        thumbnail_root, 'scatter3d-with-slider-thumbnail.png'
+    ),
 }
```

### Comparing `plopp-23.3.0/docs/customization/subplots.ipynb` & `plopp-23.4.0/docs/customization/subplots.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/docs/customization/tweaking-figures.ipynb` & `plopp-23.4.0/docs/customization/tweaking-figures.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998139880952381%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(1, 'b = a + sc.array(dims=a.dims, "*

 * *            "values=np.random.random(a.shape[0]) - 0.5, unit=a.unit)\\n')], delete: [3, 2, 1]}}}"}*

```diff
@@ -127,17 +127,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "a14f634b-7512-4f2b-a555-921482e24acc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "a = pp.data.data1d() * 5.0\n",
-                "b = a + sc.array(dims=a.dims,\n",
-                "                 values=np.random.random(a.shape[0]) - 0.5,\n",
-                "                 unit=a.unit)\n",
+                "b = a + sc.array(dims=a.dims, values=np.random.random(a.shape[0]) - 0.5, unit=a.unit)\n",
                 "\n",
                 "fig = plt.figure(figsize=(5, 4))\n",
                 "ax0 = fig.add_axes([0.0, 0.2, 1.0, 0.8])\n",
                 "ax1 = fig.add_axes([0.0, 0.0, 1.0, 0.2])\n",
                 "\n",
                 "pp.plot({'a': a, 'b': b}, ax=ax0)\n",
                 "pp.plot(a - b, ax=ax1)\n",
```

### Comparing `plopp-23.3.0/docs/examples/custom-interfaces.ipynb` & `plopp-23.4.0/docs/examples/custom-interfaces.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9739534886976676%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(6, 'z = 3.0 * np.sin(np.sqrt(x**2 + y.reshape(ny, 1) ** 2) "*

 * *            '/ 10.0) + noise + 300.0\\n\'), (8, \'da = sc.DataArray(\\n\'), (9, "    '*

 * *            'data=sc.array(dims=[\'y\', \'x\'], values=z, unit=\'K\'),\\n"), (10, \'    '*

 * *            'coords={\\n\'), (11, "        \'x\': sc.array(dims=[\'x\'], values=x, '*

 * *            'unit=\'m\'),\\n"), (12, "        \'y\': sc.array(dims=[\'y\'], values=y, '*

 * *            'unit=\'m\'),\\n"), (13, \'    },\\n\'), (14, \')\ […]*

```diff
@@ -41,19 +41,23 @@
             "source": [
                 "nx = 200\n",
                 "ny = 150\n",
                 "\n",
                 "x = np.arange(float(nx))\n",
                 "y = np.arange(float(ny))\n",
                 "noise = np.random.random((ny, nx))\n",
-                "z = 3.0 * np.sin(np.sqrt(x**2 + y.reshape(ny, 1)**2) / 10.0) + noise + 300.0\n",
+                "z = 3.0 * np.sin(np.sqrt(x**2 + y.reshape(ny, 1) ** 2) / 10.0) + noise + 300.0\n",
                 "\n",
-                "da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=z, unit='K'),\n",
-                "                  coords={'x': sc.array(dims=['x'], values=x, unit='m'),\n",
-                "                          'y': sc.array(dims=['y'], values=y, unit='m')})\n",
+                "da = sc.DataArray(\n",
+                "    data=sc.array(dims=['y', 'x'], values=z, unit='K'),\n",
+                "    coords={\n",
+                "        'x': sc.array(dims=['x'], values=x, unit='m'),\n",
+                "        'y': sc.array(dims=['y'], values=y, unit='m'),\n",
+                "    },\n",
+                ")\n",
                 "\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6a96bf2d-3849-4c90-8c67-3838cf50b429",
@@ -62,30 +66,29 @@
                 "## A set of connected nodes\n",
                 "\n",
                 "In `plopp`, think of each element in your interface as a set of interconnected nodes in a graph.\n",
                 "Each node can have parent nodes, children nodes, and also views attached to them (e.g. figures).\n",
                 "\n",
                 "At the most basic level, a graph will contain a node (white rectangle) that provides the input data,\n",
                 "and a view (grey ellipse) which will be a figure to display the data visually.\n",
-                "Note that the figure takes as input the `input_node`."
+                "Note that the figure takes as input the `data_node`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "424ad72b-5f66-46a2-ad29-9ec67847b5f3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
+                "data_node = pp.Node(da)\n",
                 "\n",
-                "fig = pp.figure2d(in_node)\n",
+                "fig = pp.figure2d(data_node)\n",
                 "\n",
-                "pp.show_graph(in_node)  # display the graph"
+                "pp.show_graph(data_node)  # display the graph"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4e299e9a-da48-47bd-bbae-33572c241e79",
             "metadata": {},
             "source": [
@@ -110,72 +113,85 @@
             "id": "dadc1065-0c73-4f87-a6a3-f81723ce00dc",
             "metadata": {},
             "source": [
                 "### Nodes are callables\n",
                 "\n",
                 "Nodes in the graph have to be constructed from callables.\n",
                 "When a view requests data from a parent node, the callable is called.\n",
-                "Typically, the callables will be a function that take in a data array as an input,\n",
+                "Typically, the callable will be a function that takes in a data array as an input,\n",
                 "and returns a data array as an output.\n",
                 "\n",
                 "Keeping your inputs and outputs as data arrays is useful because figure views will only accept data arrays as input.\n",
                 "That said, nodes that produce other outputs are very common, for example when using interactive widgets.\n",
                 "\n",
                 "In the small example above, the node at the top of the graph has no parents,\n",
-                "and its callable is simply a `lambda` function with no arguments that just returns the input data."
+                "and its callable is simply a `lambda` function with no arguments that just returns the input data.\n",
+                "\n",
+                "Calling any node will return the output from its internal callable\n",
+                "(this is very similar to [Dask's](https://docs.dask.org/en/stable/delayed.html) `delayed.compute()` method).\n",
+                "In our example above, calling `data_node` will simply return the initial data array"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cf2828c1-b3c7-411f-b965-f56835b6f13e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "data_node()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9ecf2cbe-7478-4a6b-94b9-b25574b2c9c3",
             "metadata": {},
             "source": [
+                "But for more complex graphs, the call will walk the tree, requesting all the pieces of data it needs to compute the final result.\n",
+                "\n",
                 "## Expanding the graph\n",
                 "\n",
                 "Next, say we wish to add a gaussian smoothing step in our graph, before showing the data on the figure.\n",
-                "We start with the same `input_node`, but add a second node that performs the smoothing operation before attaching the figure.\n",
-                "Because the `gaussian_filter` function requires a kernel width `sigma` as input, which we set to 5."
+                "We start with the same `data_node`, but add a second node that performs the smoothing operation before attaching the figure.\n",
+                "Because the `gaussian_filter` function requires a kernel width `sigma` as input, we set it to 5 via a keyword argument\n",
+                "(note here that it is not necessary to wrap it into a `Node`, this will automatically be handled internally)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "20abc54f-ec99-4113-9aef-fb7e4133c6aa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
+                "from scipp.scipy.ndimage import gaussian_filter\n",
+                "\n",
+                "data_node = pp.Node(da)\n",
                 "\n",
-                "try:\n",
-                "    from scipp.scipy.ndimage import gaussian_filter\n",
-                "except ImportError:\n",
-                "    from scipp.ndimage import gaussian_filter\n",
-                "smooth_node = pp.node(gaussian_filter, sigma=5)(in_node)\n",
-                "smooth_node.name = 'Smoothing'\n",
+                "smooth_node = pp.Node(gaussian_filter, data_node, sigma=5)\n",
                 "\n",
                 "fig = pp.figure2d(smooth_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dcd46e8d-947c-4866-b9c1-a0a70ee56774",
             "metadata": {},
             "source": [
-                "The resulting graph has an input node, a smoothing node, and a figure:"
+                "The resulting graph has two input nodes (one for the data array and one for the kernel width), a smoothing node, and a figure:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5cf353e2-6968-4741-becc-926bc3c16f34",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(data_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b46191da-9516-402f-8f01-ad86014d8bc9",
             "metadata": {},
             "source": [
@@ -199,55 +215,53 @@
             "source": [
                 "## Adding interactive widgets\n",
                 "\n",
                 "In the example above, the kernel size `sigma` for the gaussian smoothing was frozen to `5`.\n",
                 "But we would actually want to control this via a slider widget.\n",
                 "\n",
                 "In this case, the smoothing node now needs two inputs: the raw data, and the `sigma`.\n",
-                "It gets the raw data from the `input_node`, and the `sigma` from a `widget_node`,\n",
+                "It gets the raw data from the `data_node`, and the `sigma` from a `widget_node`,\n",
                 "which is coupled to a slider from the `ipywidgets` library."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c483edcd-f28c-48c7-a6f4-958964a03bc8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
-                "\n",
                 "import ipywidgets as ipw\n",
+                "\n",
+                "data_node = pp.Node(da)\n",
+                "\n",
                 "slider = ipw.IntSlider(min=1, max=20)\n",
                 "slider_node = pp.widget_node(slider)\n",
-                "slider_node.name = 'Slider node'\n",
                 "\n",
-                "smooth_node = pp.node(gaussian_filter)(in_node, sigma=slider_node)\n",
-                "smooth_node.name = 'Smoothing'\n",
+                "smooth_node = pp.Node(gaussian_filter, data_node, sigma=slider_node)\n",
                 "\n",
                 "fig = pp.figure2d(smooth_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c671a291-bf40-40f7-9e03-75dbd77997b2",
             "metadata": {},
             "source": [
-                "As expected, the smoothing node now has two parent nodes:"
+                "As expected, the smoothing node now has a widget as one of its parent nodes instead of the fixed-value input node:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "743c2fdb-9782-439e-9e25-e3afe5960ad3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(fig)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "08ce4da8-21ea-4aa4-bedc-4b38f01fdcdd",
             "metadata": {},
             "source": [
@@ -271,16 +285,16 @@
             "source": [
                 "When a change occurs in one of the nodes, all the nodes below it in the graph are notified about the change (the children nodes receive a notification, and they, in turn, notify their own children).\n",
                 "It is then up to each view to decide whether they are interested in the notification or not (usually, most views are interested in all notifications from parents).\n",
                 "If they are, they request data from their parent nodes, which in turn request data from their parents, and so on, until the request has reached the top of the graph.\n",
                 "\n",
                 "As a result, when the slider is dragged, the smoothing node gets notified and tells the figure that a change has occurred.\n",
                 "The figure tells `smooth_node` that it wants updated data.\n",
-                "`smooth_node` asks nodes `in_node` and `slider_node` for their data.\n",
-                "`in_node` returns the raw data, while `slider_node` returns the integer value for the kernel size.\n",
+                "`smooth_node` asks nodes `data_node` and `slider_node` for their data.\n",
+                "`data_node` returns the raw data, while `slider_node` returns the integer value for the kernel size.\n",
                 "`smooth_node` then simply sends the inputs to the `gaussian_filter` function, and forwards the result to the figure."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b3a07b8f-7212-491f-a878-e854f23496e6",
             "metadata": {},
@@ -310,32 +324,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "686b3cdf-33b5-4e45-85b9-b2266211c0bc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
+                "data_node = pp.Node(da)\n",
                 "\n",
                 "slider = ipw.IntSlider(min=1, max=20, value=10)\n",
                 "slider_node = pp.widget_node(slider)\n",
-                "slider_node.name = 'Slider node'\n",
                 "\n",
-                "smooth_node = pp.node(gaussian_filter)(in_node, sigma=slider_node)\n",
-                "smooth_node.name = 'Smoothing'\n",
+                "smooth_node = pp.Node(gaussian_filter, data_node, sigma=slider_node)\n",
                 "\n",
                 "fig2d = pp.figure2d(smooth_node)\n",
                 "\n",
                 "# Sum the raw data along the vertical dimension\n",
-                "sum_raw = pp.node(sc.sum, dim='y')(in_node)\n",
-                "sum_raw.name = 'Summing raw data'\n",
+                "sum_raw = pp.Node(sc.sum, data_node, dim='y')\n",
                 "# Sum the smoothed data along the vertical dimension\n",
-                "sum_smoothed = pp.node(sc.sum, dim='y')(smooth_node)\n",
-                "sum_smoothed.name = 'Summing smoothed data'\n",
+                "sum_smoothed = pp.Node(sc.sum, smooth_node, dim='y')\n",
                 "# Give two nodes to a figure to display both on the same axes\n",
                 "fig1d = pp.figure1d(sum_raw, sum_smoothed)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "36c9ea09-8701-465c-beec-f55d371192ee",
@@ -348,15 +357,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "81ae3b91-9622-48ca-bc90-f5cbce5ea426",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(slider_node)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d908a930-a1dc-4e7b-90f4-be8cb7e11d88",
             "metadata": {},
@@ -369,15 +378,15 @@
             "cell_type": "markdown",
             "id": "4b595fcb-02b8-4fa3-be16-3512e65b2c6a",
             "metadata": {},
             "source": [
                 "Because the slider only affects the smoothing part of the graph,\n",
                 "only the orange markers will update when we drag the slider.\n",
                 "\n",
-                "## Multiple controls\n",
+                "## Multiple controls and the `node` decorator\n",
                 "\n",
                 "In this section, masks will be added to the raw data,\n",
                 "and a widget made of checkboxes will be used to toggle the masks on and off.\n",
                 "\n",
                 "We make a slightly different interface, where we remove the gaussian smoothing,\n",
                 "and instead use the slider to slice rows in the input data."
             ]
@@ -386,35 +395,34 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "29a6345c-d530-4278-8896-b6baca81d2aa",
             "metadata": {},
             "outputs": [],
             "source": [
                 "da.masks['below_300'] = da.data < sc.scalar(300.0, unit='K')\n",
-                "da.masks['large_x'] = da.coords['x'] > sc.scalar(150., unit='m')\n",
+                "da.masks['large_x'] = da.coords['x'] > sc.scalar(150.0, unit='m')\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a966d595-0487-44a3-a718-66ff1f6d4cf6",
+            "id": "38984bbe-b161-4cfd-8994-e69774497555",
             "metadata": {},
             "source": [
-                "The input node remains the same:"
+                "The data node remains the same:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9d6777a3-e345-4b4d-93d0-8eb4f5a34cfc",
+            "id": "13347965-3359-486c-99ec-8670f7b4797d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'"
+                "data_node = pp.Node(da)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7ae9ce63-4318-4646-8cbe-d15014f48fb4",
             "metadata": {},
             "source": [
@@ -426,14 +434,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "ecaea2a3-2a66-42c6-b3c9-369b26aa4c50",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from plopp.widgets import Checkboxes, Box\n",
+                "\n",
                 "masks_widget = Checkboxes(da.masks.keys())\n",
                 "masks_widget"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1a0a4ce7-5ab2-4187-b89c-2e0df7a3e86e",
@@ -455,41 +464,42 @@
         {
             "cell_type": "markdown",
             "id": "69510b9d-8bbb-4e7d-8c39-dde70d88b3db",
             "metadata": {},
             "source": [
                 "We make a node from the checkboxes widget using `widget_node` once again.\n",
                 "\n",
-                "The `node` function can be called directly by supplying a callable to it,\n",
-                "but it can also be used as a function decorator.\n",
+                "We can supply custom functions to the `Node` constructor,\n",
+                "but it is often useful to decorate our functions with the `plopp.node` decorator,\n",
+                "and then call the functions directly.\n",
                 "\n",
                 "We therefore define a function that will hide masks depending on the checkboxes values,\n",
-                "and decorate it with `@pp.node` so that it can accept `in_node` and `masks_node` as inputs."
+                "and decorate it with `@pp.node` so that it can accept `data_node` and `masks_node` as inputs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "06483d83-a20f-419e-bf54-d30d7badf7be",
             "metadata": {},
             "outputs": [],
             "source": [
                 "masks_node = pp.widget_node(masks_widget)\n",
-                "masks_node.name = 'Masks checkboxes'\n",
+                "\n",
                 "\n",
                 "@pp.node\n",
                 "def hide_masks(data_array, masks):\n",
                 "    out = data_array.copy(deep=False)\n",
                 "    for name, value in masks.items():\n",
                 "        if name in out.masks and (not value):\n",
                 "            del out.masks[name]\n",
                 "    return out\n",
                 "\n",
-                "hide_node = hide_masks(in_node, masks=masks_node)\n",
-                "hide_node.name = 'Hide/show masks'"
+                "\n",
+                "hide_node = hide_masks(data_array=data_node, masks=masks_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8d6f05d3-b618-427f-ad39-dcaf3ba3f093",
             "metadata": {},
             "source": [
@@ -504,22 +514,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "@pp.node\n",
                 "def slice_y(data_array, index):\n",
                 "    return data_array['y', index]\n",
                 "\n",
+                "\n",
                 "slider = ipw.IntSlider(min=0, max=da.sizes['y'] - 1)\n",
                 "slider_node = pp.widget_node(slider)\n",
-                "slider_node.name = 'Slider node'\n",
                 "\n",
                 "slice_node = slice_y(hide_node, index=slider_node)\n",
-                "slice_node.name = 'Slice horizontal row'\n",
                 "\n",
-                "pp.show_graph(in_node)"
+                "pp.show_graph(masks_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6e53a3c6-37eb-4a68-8431-50294dbb789d",
             "metadata": {},
             "source": [
@@ -533,15 +542,15 @@
             "id": "b8acfe84-4061-4639-ab44-22edd71d4259",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig2d = pp.figure2d(hide_node)\n",
                 "fig1d = pp.figure1d(slice_node)\n",
                 "\n",
-                "pp.show_graph(in_node)"
+                "pp.show_graph(masks_node)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0beec3e5-1deb-4efe-bbd5-7679789feb7d",
             "metadata": {},
@@ -552,15 +561,101 @@
         },
         {
             "cell_type": "markdown",
             "id": "a963de68-ce9f-4c3a-a9e3-dd40a7458223",
             "metadata": {},
             "source": [
                 "Note that the masks update on both the 1D and 2D figures,\n",
-                "because the checkboxes widget lies at the very top of the graph."
+                "because the checkboxes widget lies at the very top of the graph.\n",
+                "\n",
+                "## Operators\n",
+                "\n",
+                "Nodes also have operators, and simple operations can be implemented in a short-hand way, instead of defining functions such as `add` or `multiply`.\n",
+                "Consider for example"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e58f5f5e-9c52-41eb-9d61-1419c0baf541",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "a = pp.Node(np.array([1, 2, 3, 4, 5]))\n",
+                "b = pp.Node(np.array([6, 7, 8, 9, 10]))\n",
+                "\n",
+                "c = a + b\n",
+                "c()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ddfef22b-c4ed-4c89-98f6-67cf47c36854",
+            "metadata": {},
+            "source": [
+                "Operators also work with normal Python objects, which simply get wrapped in a node:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "19acdd96-9377-4de1-b4fb-516ab39208ac",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "c = a * 33.0\n",
+                "c()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "daace072-f3f1-4093-9263-3b23b44a8b81",
+            "metadata": {},
+            "source": [
+                "### A short example"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a4e38e0d-4e67-4791-972a-05874ad04fcd",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "noise = 0.5 * (np.random.random(100) - 0.5)\n",
+                "signal = np.sin(0.1 * np.arange(100.0)) + noise\n",
+                "\n",
+                "# Noisy data\n",
+                "a = pp.Node(\n",
+                "    sc.DataArray(\n",
+                "        data=sc.array(dims=['time'], values=signal),\n",
+                "        coords={'time': sc.arange('time', 100.0, unit='s')},\n",
+                "    )\n",
+                ")\n",
+                "fig = pp.figure1d(a)\n",
+                "fig"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "9747ac74-cd16-41e2-a82c-9f23b3a59530",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "b = pp.Node(\n",
+                "    sc.DataArray(\n",
+                "        data=sc.array(dims=['time'], values=noise),\n",
+                "        coords={'time': sc.arange('time', 100.0, unit='s')},\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "# Remove noise from signal\n",
+                "diff = a - b\n",
+                "pp.figure1d(diff)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -571,14 +666,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/examples/gallery/masking-a-range.ipynb` & `plopp-23.4.0/docs/examples/gallery/masking-a-range.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928093633286648%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'spread = 30.0\\n'), (11, '    yc = np.random.choice([ny "*

 * *            "/ 4, ny / 2, 3 * ny / 4])\\n'), (12, '    xy = np.random.normal(\\n'), (13, '        "*

 * *            "loc=(xc, yc), scale=spread * np.random.random(), size=[per_peak, 2]\\n'), (14, '    "*

 * *            ')\\n\'), (18, \'da = sc.DataArray(\\n\'), (19, "    data=sc.array(dims=[\'y\', '*

 * *            '\'x\'], values=a, unit=\'counts\'),\\n"), (20, \'    coords={\\n\'), (21, "        '*

 * *            '\'x\':  […]*

```diff
@@ -39,34 +39,37 @@
             "execution_count": null,
             "id": "9d367a8e-9587-4b46-bb74-9e4c8eaa60ef",
             "metadata": {},
             "outputs": [],
             "source": [
                 "npeaks = 200\n",
                 "per_peak = 500\n",
-                "spread = 30.\n",
+                "spread = 30.0\n",
                 "ny = 300\n",
                 "nx = 300\n",
                 "a = np.ones((ny, nx))\n",
                 "\n",
                 "xbins = np.arange(nx + 1)\n",
                 "ybins = np.arange(ny + 1)\n",
                 "for n in range(npeaks):\n",
                 "    xc = np.random.random() * nx\n",
-                "    yc = np.random.choice([ny/4, ny/2, 3*ny/4])\n",
-                "    xy = np.random.normal(loc=(xc, yc),\n",
-                "                          scale=spread * np.random.random(),\n",
-                "                          size=[per_peak, 2])\n",
+                "    yc = np.random.choice([ny / 4, ny / 2, 3 * ny / 4])\n",
+                "    xy = np.random.normal(\n",
+                "        loc=(xc, yc), scale=spread * np.random.random(), size=[per_peak, 2]\n",
+                "    )\n",
                 "    h, ye, xe = np.histogram2d(xy[:, 1], xy[:, 0], bins=(ybins, xbins))\n",
                 "    a += h\n",
                 "\n",
-                "da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=a, unit='counts'),\n",
-                "                  coords={'x': sc.array(dims=['x'], values=xbins, unit='cm'),\n",
-                "                          'y': sc.array(dims=['y'], values=ybins, unit='cm')}\n",
-                "                 )"
+                "da = sc.DataArray(\n",
+                "    data=sc.array(dims=['y', 'x'], values=a, unit='counts'),\n",
+                "    coords={\n",
+                "        'x': sc.array(dims=['x'], values=xbins, unit='cm'),\n",
+                "        'y': sc.array(dims=['y'], values=ybins, unit='cm'),\n",
+                "    },\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0e5010d1-1710-476e-91c0-a01c281bfcf6",
             "metadata": {},
             "source": [
@@ -78,56 +81,52 @@
             "execution_count": null,
             "id": "346e8cc8-3874-464e-ad49-dcfb5ad92770",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ydim = 'y'\n",
                 "\n",
-                "# A function that will add a mask outside of selected range\n",
+                "\n",
+                "@pp.node\n",
                 "def add_mask(da, trunc_range):\n",
+                "    \"\"\"A function that will add a mask outside of selected range.\"\"\"\n",
                 "    min_tr, max_tr = trunc_range\n",
                 "    out = da.copy(deep=False)\n",
                 "    out.masks[ydim] = sc.zeros(sizes={ydim: da.sizes[ydim]}, dtype=bool)\n",
                 "    out.masks[ydim].values[:min_tr] = True\n",
                 "    out.masks[ydim].values[max_tr:] = True\n",
                 "    return out\n",
                 "\n",
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
                 "\n",
                 "# Make a range slider\n",
-                "slider = ipw.IntRangeSlider(max=da.sizes[ydim]-1,\n",
-                "                            description='y indices',\n",
-                "                            layout={'width': '400px'})\n",
-                "\n",
+                "slider = ipw.IntRangeSlider(\n",
+                "    max=da.sizes[ydim] - 1, description='y indices', layout={'width': '400px'}\n",
+                ")\n",
                 "slider_node = pp.widget_node(slider)\n",
-                "slider_node.name = 'Slider node'\n",
                 "\n",
                 "# Add mask\n",
-                "mask_node = pp.node(add_mask)(in_node, trunc_range=slider_node)\n",
-                "mask_node.name = 'Add masks'\n",
+                "mask_node = add_mask(da, trunc_range=slider_node)\n",
                 "\n",
                 "# Node that sums along the y dimension\n",
-                "sum_node = pp.node(sc.sum, dim=ydim)(mask_node)\n",
-                "sum_node.name = 'Sum Y'\n",
+                "sum_node = pp.Node(sc.sum, mask_node, dim=ydim)\n",
                 "\n",
                 "# Make figures\n",
                 "fig2d = pp.figure2d(mask_node, norm='log')\n",
                 "fig1d = pp.figure1d(sum_node, grid=True, ls='solid', marker='')\n",
                 "ipw.VBox([slider, fig2d, fig1d])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7201be42-c726-43cd-b6ad-65cf8f2941b3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(fig1d)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "37373128-b948-4100-a761-87229730c62a",
             "metadata": {
@@ -152,14 +151,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/examples/gallery/nyc-taxi.ipynb` & `plopp-23.4.0/docs/examples/gallery/nyc-taxi.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923657614087302%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(5, 'from scipp.scipy.ndimage import gaussian_filter\\n')], "*

 * *            'delete: [8, 7, 6, 5]}}, 2: {\'source\': {insert: [(5, "slice_node = pp.Node(lambda '*

 * *            'da, ind: da[\'hour\', ind], da=data, ind=slider_node)\\n"), (11, "sum_lat = '*

 * *            'pp.Node(sc.sum, slice_node, dim=\'latitude\')\\n"), (14, \'smooth = '*

 * *            "pp.Node(gaussian_filter, sum_lat, sigma=5)\\n')], delete: [23, 22, 19, 18, 12, 11, "*

 * *            "10, 7, 3, 2, 1, 0]}}, 4: {'so […]*

```diff
@@ -28,55 +28,43 @@
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import scipp as sc\n",
                 "import plopp as pp\n",
                 "from plopp import widgets\n",
                 "from plopp.data import examples\n",
-                "try:\n",
-                "    from scipp.scipy.ndimage import gaussian_filter\n",
-                "except ImportError:\n",
-                "    from scipp.ndimage import gaussian_filter\n",
+                "from scipp.scipy.ndimage import gaussian_filter\n",
                 "import ipywidgets as ipw\n",
                 "\n",
                 "data = sc.io.open_hdf5(examples.nyc_taxi())\n",
                 "data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a8b1129c-5258-49de-a2fe-4e5d51af29ca",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Input data node\n",
-                "in_node = pp.input_node(data)\n",
-                "in_node.name = 'Input data'\n",
-                "\n",
                 "# Slider node that provides index to slice\n",
                 "slider = ipw.IntSlider(description='Hour:', min=0, max=23)\n",
                 "slider_node = pp.widget_node(slider)\n",
-                "slider_node.name = 'Slider widget'\n",
                 "\n",
                 "# Node that actually does the slicing\n",
-                "slice_node = pp.node(\n",
-                "    lambda da, ind: da['hour', ind])(da=in_node, ind=slider_node)\n",
-                "slice_node.name = 'Slice by hour'\n",
+                "slice_node = pp.Node(lambda da, ind: da['hour', ind], da=data, ind=slider_node)\n",
                 "\n",
                 "# Add a 2D figure to show the NYC map\n",
                 "fig2d = pp.figure2d(slice_node, norm='log')\n",
                 "\n",
                 "# Add a node after the slicing to sum along the latitude dimension\n",
-                "sum_lat = pp.node(sc.sum, dim='latitude')(slice_node)\n",
-                "sum_lat.name = 'Sum along latitude'\n",
+                "sum_lat = pp.Node(sc.sum, slice_node, dim='latitude')\n",
                 "\n",
                 "# Add a node after the sum that performs as Gaussian smoothing\n",
-                "smooth = pp.node(gaussian_filter, sigma=5)(sum_lat)\n",
-                "smooth.name = 'Gaussian smoothing'\n",
+                "smooth = pp.Node(gaussian_filter, sum_lat, sigma=5)\n",
                 "\n",
                 "# Add a 1D figure that will display both raw sum and smoothed data\n",
                 "fig1d = pp.figure1d(sum_lat, smooth, norm='log')\n",
                 "\n",
                 "widgets.Box([slider, fig2d, fig1d])  # Container box"
             ]
         },
@@ -91,15 +79,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4290d222-946b-49f1-b42d-e1404c0326c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(fig1d)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "28ee06c2-ed57-45b0-aaff-0667f23479b3",
             "metadata": {
@@ -125,14 +113,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/examples/gallery/rectangle-selection.ipynb` & `plopp-23.4.0/docs/examples/gallery/rectangle-selection.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930006757005339%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'spread = 30.0\\n'), (11, '    yc = np.random.choice([ny "*

 * *            "/ 4, ny / 2, 3 * ny / 4])\\n'), (12, '    xy = np.random.normal(\\n'), (13, '        "*

 * *            "loc=(xc, yc), scale=spread * np.random.random(), size=[per_peak, 2]\\n'), (14, '    "*

 * *            ')\\n\'), (18, \'da = sc.DataArray(\\n\'), (19, "    data=sc.array(dims=[\'y\', '*

 * *            '\'x\'], values=a, unit=\'counts\'),\\n"), (20, \'    coords={\\n\'), (21, "        '*

 * *            '\'x\':  […]*

```diff
@@ -39,34 +39,37 @@
             "execution_count": null,
             "id": "3c05fe5b-483a-438e-a7ba-a64b24a33b61",
             "metadata": {},
             "outputs": [],
             "source": [
                 "npeaks = 200\n",
                 "per_peak = 500\n",
-                "spread = 30.\n",
+                "spread = 30.0\n",
                 "ny = 300\n",
                 "nx = 300\n",
                 "a = np.ones((ny, nx))\n",
                 "\n",
                 "xbins = np.arange(nx + 1)\n",
                 "ybins = np.arange(ny + 1)\n",
                 "for n in range(npeaks):\n",
                 "    xc = np.random.random() * nx\n",
-                "    yc = np.random.choice([ny/4, ny/2, 3*ny/4])\n",
-                "    xy = np.random.normal(loc=(xc, yc),\n",
-                "                          scale=spread * np.random.random(),\n",
-                "                          size=[per_peak, 2])\n",
+                "    yc = np.random.choice([ny / 4, ny / 2, 3 * ny / 4])\n",
+                "    xy = np.random.normal(\n",
+                "        loc=(xc, yc), scale=spread * np.random.random(), size=[per_peak, 2]\n",
+                "    )\n",
                 "    h, ye, xe = np.histogram2d(xy[:, 1], xy[:, 0], bins=(ybins, xbins))\n",
                 "    a += h\n",
                 "\n",
-                "da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=a, unit='counts'),\n",
-                "                  coords={'x': sc.array(dims=['x'], values=xbins, unit='cm'),\n",
-                "                          'y': sc.array(dims=['y'], values=ybins, unit='cm')}\n",
-                "                 )"
+                "da = sc.DataArray(\n",
+                "    data=sc.array(dims=['y', 'x'], values=a, unit='counts'),\n",
+                "    coords={\n",
+                "        'x': sc.array(dims=['x'], values=xbins, unit='cm'),\n",
+                "        'y': sc.array(dims=['y'], values=ybins, unit='cm'),\n",
+                "    },\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "402753eb-bb08-4e6c-9299-a021231010eb",
             "metadata": {},
             "source": [
@@ -83,14 +86,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from plopp.widgets.drawing import DrawingTool\n",
                 "from functools import partial\n",
                 "from mpltoolbox import Rectangles\n",
                 "\n",
+                "\n",
                 "def vertical_sum(da, rect_info):\n",
                 "    \"\"\"\n",
                 "    Function that slices the data according to the\n",
                 "    rectangle size/position, and sums along the\n",
                 "    vertical dimension.\n",
                 "    \"\"\"\n",
                 "    x = rect_info['x']\n",
@@ -107,27 +111,27 @@
                 "    Convert the raw rectangle info to a dict containing the dimensions of\n",
                 "    each axis, and values with units.\n",
                 "    \"\"\"\n",
                 "    return lambda: {\n",
                 "        'x': {\n",
                 "            'dim': figure.dims['x'],\n",
                 "            'left': sc.scalar(artist.xy[0], unit=figure.canvas.xunit),\n",
-                "            'right': sc.scalar(artist.xy[0] + artist.width, unit=figure.canvas.xunit)\n",
+                "            'right': sc.scalar(artist.xy[0] + artist.width, unit=figure.canvas.xunit),\n",
                 "        },\n",
                 "        'y': {\n",
                 "            'dim': figure.dims['y'],\n",
                 "            'bottom': sc.scalar(artist.xy[1], unit=figure.canvas.yunit),\n",
-                "            'top': sc.scalar(artist.xy[1] + artist.height, unit=figure.canvas.yunit)\n",
+                "            'top': sc.scalar(artist.xy[1] + artist.height, unit=figure.canvas.yunit),\n",
                 "        },\n",
                 "    }\n",
                 "\n",
-                "RectangleTool = partial(DrawingTool,\n",
-                "                        tool=Rectangles,\n",
-                "                        get_artist_info=_get_rect_info,\n",
-                "                        icon='vector-square')"
+                "\n",
+                "RectangleTool = partial(\n",
+                "    DrawingTool, tool=Rectangles, get_artist_info=_get_rect_info, icon='vector-square'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e4671098-831c-4272-8174-725d006266e5",
             "metadata": {},
             "source": [
@@ -140,21 +144,20 @@
             "execution_count": null,
             "id": "6acd8916-8ba8-4065-9cbe-5d76a74ce281",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from plopp.widgets import Box\n",
                 "\n",
-                "in_node = pp.input_node(da)\n",
-                "in_node.name = 'Input node'\n",
+                "data_node = pp.Node(da)\n",
                 "\n",
-                "f2d = pp.figure2d(in_node, norm='log')\n",
+                "f2d = pp.figure2d(data_node, norm='log')\n",
                 "f1d = pp.figure1d()\n",
                 "\n",
-                "r = RectangleTool(figure=f2d, input_node=in_node, func=vertical_sum, destination=f1d)\n",
+                "r = RectangleTool(figure=f2d, input_node=data_node, func=vertical_sum, destination=f1d)\n",
                 "f2d.toolbar['roi'] = r\n",
                 "\n",
                 "box = Box([f2d, f1d])"
             ]
         },
         {
             "cell_type": "code",
@@ -169,18 +172,27 @@
                 "\n",
                 "r._tool.click(50, 200)\n",
                 "r._tool.click(200, 250)\n",
                 "r._tool.click(30, 50)\n",
                 "r._tool.click(250, 170)\n",
                 "\n",
                 "from ipywidgets import HBox\n",
+                "\n",
                 "f1 = box[0]\n",
-                "f1.children = [f1.top_bar, HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]), f1.bottom_bar]\n",
+                "f1.children = [\n",
+                "    f1.top_bar,\n",
+                "    HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]),\n",
+                "    f1.bottom_bar,\n",
+                "]\n",
                 "f2 = box[1]\n",
-                "f2.children = [f2.top_bar, HBox([f2.left_bar, f2.canvas.to_image(), f2.right_bar]), f2.bottom_bar]"
+                "f2.children = [\n",
+                "    f2.top_bar,\n",
+                "    HBox([f2.left_bar, f2.canvas.to_image(), f2.right_bar]),\n",
+                "    f2.bottom_bar,\n",
+                "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f0004b44-743b-473a-8276-4f438ba9f802",
             "metadata": {},
@@ -192,15 +204,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c5cf73d9-2a93-42c0-8854-944dcd9be1f8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.show_graph(in_node)"
+                "pp.show_graph(data_node)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "01b502c8-d10c-45ff-8447-a9fd7121781f",
             "metadata": {
@@ -225,14 +237,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/examples/gallery/scatter3d-with-threshold.ipynb` & `plopp-23.4.0/docs/examples/gallery/scatter3d-with-threshold.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333333%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(7, "da = sc.DataArray(sc.sin(x) * sc.sin(y) * sc.sin(z), '*

 * *            'coords={\'x\': x, \'y\': y, \'z\': z})\\n")], delete: [7]}}}'}*

```diff
@@ -24,15 +24,15 @@
                 "import scipp as sc\n",
                 "import plopp as pp\n",
                 "\n",
                 "x = sc.linspace('x', 0.0, 10.0, num=40, unit='rad')\n",
                 "y = sc.linspace('y', 0.0, 10.0, num=40, unit='rad')\n",
                 "z = sc.linspace('z', 0.0, 10.0, num=40, unit='rad')\n",
                 "\n",
-                "da = sc.DataArray(sc.sin(x)*sc.sin(y)*sc.sin(z), coords={'x':x, 'y':y, 'z':z})\n",
+                "da = sc.DataArray(sc.sin(x) * sc.sin(y) * sc.sin(z), coords={'x': x, 'y': y, 'z': z})\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7dfb69b0-3049-4b49-bc44-d335bb6f4008",
             "metadata": {},
```

### Comparing `plopp-23.3.0/docs/examples/gallery.ipynb` & `plopp-23.4.0/docs/examples/gallery.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9938616071428572%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, '* [3-D scatter plot with "*

 * *            "threshold](gallery/scatter3d-with-threshold.ipynb)\\n'), (4, '* [3-D scatter plot "*

 * *            "with slider](gallery/scatter3d-with-slider.ipynb)')], delete: [3]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -16,15 +16,16 @@
                     "nbsphinx-gallery"
                 ]
             },
             "source": [
                 "* [Interactive histogramming](gallery/nyc-taxi.ipynb)\n",
                 "* [Masking a range](gallery/masking-a-range.ipynb)\n",
                 "* [Rectangle selection](gallery/rectangle-selection.ipynb)\n",
-                "* [3-D scatter plot with threshold](gallery/scatter3d-with-threshold.ipynb)"
+                "* [3-D scatter plot with threshold](gallery/scatter3d-with-threshold.ipynb)\n",
+                "* [3-D scatter plot with slider](gallery/scatter3d-with-slider.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -36,13 +37,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-23.3.0/docs/index.rst` & `plopp-23.4.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 ============
 
 - If you have questions that are not answered by these documentation pages, ask on `GitHub discussions <https://github.com/scipp/plopp/discussions>`_.
   Please include a self-contained reproducible example if possible.
 - Report bugs (including unclear, missing, or wrong documentation!), suggest features or view the source code `on GitHub <https://github.com/scipp/plopp>`_.
 
 .. toctree::
+   :caption: Getting started
+   :maxdepth: 3
+   :hidden:
+
+   getting-started/overview
+   getting-started/numpy-pandas-xarray
+
+.. toctree::
    :caption: Basic Usage
    :maxdepth: 3
    :hidden:
 
    basics/line-plot
    basics/image-plot
    basics/slicer-plot
```

#### html2text {}

```diff
@@ -13,15 +13,17 @@
 install plopp[all] Using conda ----------- You can install from ``conda`` using
 .. code-block:: sh conda install -c conda-forge -c scipp plopp Get in touch
 ============ - If you have questions that are not answered by these
 documentation pages, ask on `GitHub discussions
 github.com/scipp/plopp/discussions>`_. Please include a self-contained
 reproducible example if possible. - Report bugs (including unclear, missing, or
 wrong documentation!), suggest features or view the source code `on GitHub
-github.com/scipp/plopp>`_. .. toctree:: :caption: Basic Usage :maxdepth: 3 :
-hidden: basics/line-plot basics/image-plot basics/slicer-plot basics/inspector-
-plot basics/super-plot basics/scatter3d-plot basics/saving-figures .. toctree::
-:caption: Custom figures :maxdepth: 3 :hidden: customization/subplots
-customization/tweaking-figures .. toctree:: :caption: Examples :maxdepth: 3 :
-hidden: examples/custom-interfaces examples/gallery .. toctree:: :caption:
-About :maxdepth: 3 :hidden: about/reference about/faq about/about Release notes
+github.com/scipp/plopp>`_. .. toctree:: :caption: Getting started :maxdepth: 3
+:hidden: getting-started/overview getting-started/numpy-pandas-xarray ..
+toctree:: :caption: Basic Usage :maxdepth: 3 :hidden: basics/line-plot basics/
+image-plot basics/slicer-plot basics/inspector-plot basics/super-plot basics/
+scatter3d-plot basics/saving-figures .. toctree:: :caption: Custom figures :
+maxdepth: 3 :hidden: customization/subplots customization/tweaking-figures ..
+toctree:: :caption: Examples :maxdepth: 3 :hidden: examples/custom-interfaces
+examples/gallery .. toctree:: :caption: About :maxdepth: 3 :hidden: about/
+reference about/faq about/about Release notes
 github.com/scipp/plopp/releases>
```

### Comparing `plopp-23.3.0/docs/version.py` & `plopp-23.4.0/docs/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             versions.append(parse(t.name))
         except InvalidVersion:
             pass
     return sorted(versions, reverse=True)
 
 
 class VersionInfo:
-
     def __init__(self):
         self._releases = _get_releases()
 
     def _to_version(self, version) -> Version:
         if isinstance(version, str):
             try:
                 return parse(version)
@@ -88,23 +87,24 @@
     elif action == 'get-target':
         print(info.target(version))
     return 0
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Process some integers.')
-    parser.add_argument('--action',
-                        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
-                        required=True,
-                        help='Action to perform: Check whether this major or minor '
-                        'release exists or is new (is-latest), check whether this is a '
-                        'new major or minor release (is-new), get the version this is '
-                        'replacing (get-replaced), get the target folder for '
-                        'publishing the docs (get-target). In all cases the '
-                        'patch/micro version is ignored.')
-    parser.add_argument('--version',
-                        dest='version',
-                        required=True,
-                        help='Version the action refers to')
+    parser.add_argument(
+        '--action',
+        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
+        required=True,
+        help='Action to perform: Check whether this major or minor '
+        'release exists or is new (is-latest), check whether this is a '
+        'new major or minor release (is-new), get the version this is '
+        'replacing (get-replaced), get the target folder for '
+        'publishing the docs (get-target). In all cases the '
+        'patch/micro version is ignored.',
+    )
+    parser.add_argument(
+        '--version', dest='version', required=True, help='Version the action refers to'
+    )
 
     args = parser.parse_args()
     sys.exit(main(**vars(args)))
```

### Comparing `plopp-23.3.0/pyproject.toml` & `plopp-23.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # Excluding tests because bandit doesn't like `assert`.
 exclude_dirs = ["docs/conf.py", "tests", "install"]
 
 [tool.codespell]
 ignore-words-list = "elemt"
 skip = "./.git,./install,./build,./.tox,*/*_cache,*/.virtual_documents,*/.ipynb_checkpoints,*.pdf,*.svg"
 
+[tool.black]
+skip-string-normalization = true
+
 [tool.isort]
 skip_gitignore = true
-line_length = 88
-multi_line_output = 2  # for compatibility with yapf
+profile = "black"
 
 [tool.mypy]
 mypy_path = "src"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 minversion = "7.0"
```

### Comparing `plopp-23.3.0/requirements/ci.txt` & `plopp-23.4.0/requirements/ci.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-# SHA1:bd04ac356d400038fce201257b22d93954dbc415
+# SHA1:27725fab811331ce61f689bd6e27c641e802b3f0
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.2.0
+cachetools==5.3.0
     # via tox
 certifi==2022.12.7
     # via requests
 chardet==5.1.0
     # via tox
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.10.7
     # via
     #   tox
     #   virtualenv
+gitdb==4.0.10
+    # via gitpython
+gitpython==3.1.31
+    # via -r requirements/ci.in
 idna==3.4
     # via requests
-packaging==22.0
+packaging==23.0
     # via
     #   pyproject-api
     #   tox
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
-pyproject-api==1.4.0
+pyproject-api==1.5.1
     # via tox
-requests==2.28.1
+requests==2.28.2
     # via -r requirements/ci.in
+smmap==5.0.0
+    # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.2.4
+tox==4.4.8
     # via -r requirements/ci.in
-urllib3==1.26.13
+urllib3==1.26.15
     # via requests
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via tox
```

### Comparing `plopp-23.3.0/requirements/mini.txt` & `plopp-23.4.0/requirements/mini.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 #
 #    pip-compile-multi
 #
 attrs==22.2.0
     # via pytest
 confuse==2.0.0
     # via scipp
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 graphlib-backport==1.0.3
     # via scipp
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
-numpy==1.24.1
+numpy==1.24.2
     # via scipp
-packaging==22.0
+packaging==23.0
     # via pytest
 pluggy==1.0.0
     # via pytest
-pytest==7.2.0
+pytest==7.2.2
     # via -r requirements/mini.in
 pyyaml==6.0
     # via confuse
-scipp==23.1.1
+scipp==23.3.1
     # via -r requirements/mini.in
 tomli==2.0.1
     # via pytest
```

### Comparing `plopp-23.3.0/requirements/static.txt` & `plopp-23.4.0/requirements/static.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 #
 #    pip-compile-multi
 #
 cfgv==3.3.1
     # via pre-commit
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.10.7
     # via virtualenv
-identify==2.5.13
+identify==2.5.22
     # via pre-commit
 nodeenv==1.7.0
     # via pre-commit
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.2.1
     # via -r requirements/static.in
 pyyaml==6.0
     # via pre-commit
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `plopp-23.3.0/requirements/test.txt` & `plopp-23.4.0/requirements/test.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-# SHA1:62ffaa0ef12ab2b5241d4902e702d869f8daba1e
+# SHA1:9d2a19ef95d8f42022966bea7982ed8fa1d11f6d
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-contourpy==1.0.6
+attrs==22.2.0
+    # via pytest
+contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
-fonttools==4.38.0
+fonttools==4.39.3
     # via matplotlib
 graphviz==0.20.1
     # via -r requirements/test.in
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
-ipympl==0.9.2
+ipympl==0.9.3
     # via -r requirements/test.in
+ipython-genutils==0.2.0
+    # via ipympl
 kaleido==0.2.1
     # via -r requirements/test.in
 kiwisolver==1.4.4
     # via matplotlib
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via ipympl
+pandas==1.5.3
+    # via
+    #   -r requirements/test.in
+    #   xarray
 pillow==9.4.0
     # via
     #   ipympl
     #   matplotlib
-plotly==5.11.0
+plotly==5.14.0
     # via -r requirements/test.in
 pluggy==1.0.0
     # via pytest
 pyparsing==3.0.9
     # via matplotlib
-pytest==7.2.0
+pytest==7.2.2
     # via -r requirements/test.in
-scipy==1.10.0
+pytz==2023.3
+    # via pandas
+scipy==1.10.1
     # via -r requirements/test.in
-tenacity==8.1.0
+tenacity==8.2.2
     # via plotly
 tomli==2.0.1
     # via pytest
+xarray==2023.3.0
+    # via -r requirements/test.in
```

### Comparing `plopp-23.3.0/resources/logo-plopp-2022.svg` & `plopp-23.4.0/resources/logo-plopp-2022.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/setup.cfg` & `plopp-23.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,11 @@
 [options.package_data]
 plopp = py.typed
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
-[yapf]
-based_on_style = pep8
-column_limit = 88
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `plopp-23.3.0/src/plopp/__init__.py` & `plopp-23.4.0/src/plopp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,44 +13,47 @@
 from .backends.manager import BackendManager
 
 backends = BackendManager()
 
 from . import data
 from .core import Node, View, input_node, node, show_graph, widget_node
 from .functions import inspector, plot, scatter3d, slicer, superplot
-from .graphics import figure1d, figure2d, figure3d
+from .graphics import Camera, figure1d, figure2d, figure3d
 
 
 def patch_scipp():
     """
     Running this replaces the ``plot`` function from Scipp with the plopp ``plot``
     wrapper. This patches the ``Variable``, ``DataArray``, ``Dataset`` classes,
     as well as the main ``plot`` function in the Scipp module.
     """
     import scipp as sc
+
     setattr(sc.Variable, 'plot', plot)
     setattr(sc.DataArray, 'plot', plot)
     setattr(sc.Dataset, 'plot', plot)
     setattr(sc, 'plot', plot)
 
 
 def unpatch_scipp():
     """
     Running this reverts the patching operation in :func:`patch_scipp`.
     """
     import scipp as sc
     from scipp.plotting import plot as pl
+
     setattr(sc.Variable, 'plot', pl)
     setattr(sc.DataArray, 'plot', pl)
     setattr(sc.Dataset, 'plot', pl)
     setattr(sc, 'plot', pl)
 
 
 def show():
     """
     A function to display all the currently opened figures (note that this only applies
     to the figures created via the Matplotlib backend).
     See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.show.html for more
     details.
     """
     import matplotlib.pyplot as plt
+
     plt.show()
```

### Comparing `plopp-23.3.0/src/plopp/backends/manager.py` & `plopp-23.4.0/src/plopp/backends/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
 class BackendManager:
-
     def __init__(self):
         self._mapping = {'2d': 'matplotlib', '3d': 'pythreejs'}
         self._backends = {}
         self._sync()
 
     def __getitem__(self, key):
         return self._mapping[key]
@@ -24,23 +23,26 @@
 
     def items(self):
         return self._mapping.items()
 
     def _sync(self):
         if self._mapping['2d'] == 'matplotlib':
             from .matplotlib import MatplotlibBackend
+
             self._backends['2d'] = MatplotlibBackend()
         elif self._mapping['2d'] == 'plotly':
             from .plotly import PlotlyBackend
+
             self._backends['2d'] = PlotlyBackend()
         else:
             raise ValueError(f'Unsupported 2d backend \'{self._mapping["2d"]}\'.')
 
         if self._mapping['3d'] == 'pythreejs':
             from .pythreejs import PythreejsBackend
+
             self._backends['3d'] = PythreejsBackend()
         else:
             raise ValueError(f'Unsupported 3d backend \'{self._mapping["3d"]}\'.')
 
     def is_interactive(self):
         return self._backends['2d'].is_interactive()
 
@@ -73,15 +75,16 @@
         return _image(*args, **kwargs)
 
     def point_cloud(self, *args, **kwargs):
         try:
             _point_cloud = self._backends['3d'].point_cloud
         except AttributeError:
             raise ValueError(
-                f'Unsupported backend \'{self["3d"]}\' for point_cloud (3D).')
+                f'Unsupported backend \'{self["3d"]}\' for point_cloud (3D).'
+            )
         return _point_cloud(*args, **kwargs)
 
     def figure1d(self, *args, **kwargs):
         try:
             _figure1d = self._backends['2d'].figure1d
         except AttributeError:
             raise ValueError(f'Unsupported backend \'{self["2d"]}\' for figure1d.')
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/__init__.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
 def _make_figure(*args, **kwargs):
     from .utils import is_interactive_backend
+
     if is_interactive_backend():
         from .interactive import InteractiveFig
+
         return InteractiveFig(*args, **kwargs)
     else:
         from .static import StaticFig
+
         return StaticFig(*args, **kwargs)
 
 
 class MatplotlibBackend:
-
     def is_interactive(self):
         """
         Returns ``True`` if the backend currently in use allows for interactive figures.
         """
         from .utils import is_interactive_backend
+
         return is_interactive_backend()
 
     def canvas2d(self, *args, **kwargs):
         """
         See :class:`canvas.Canvas` for details.
         """
         from .canvas import Canvas as CanvasMpl
+
         return CanvasMpl(*args, **kwargs)
 
     def line(self, *args, **kwargs):
         """
         See :class:`line.Line` for details.
         """
         from .line import Line as LineMpl
+
         return LineMpl(*args, **kwargs)
 
     def image(self, *args, **kwargs):
         """
         See :class:`image.Image` for details.
         """
         from .image import Image as ImageMpl
+
         return ImageMpl(*args, **kwargs)
 
     def figure1d(self, *args, **kwargs):
         """
         See :class:`static.StaticFig` and :class:`interactive.InteractiveFig` for
         details.
         """
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/canvas.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/canvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,26 +48,27 @@
         unit.
     aspect:
         The aspect ratio for the axes.
     cbar:
         Add axes to host a colorbar if ``True``.
     """
 
-    def __init__(self,
-                 ax: plt.Axes = None,
-                 cax: plt.Axes = None,
-                 figsize: Optional[Tuple[float, float]] = None,
-                 title: str = None,
-                 grid: bool = False,
-                 vmin: Union[sc.Variable, int, float] = None,
-                 vmax: Union[sc.Variable, int, float] = None,
-                 aspect: Literal['auto', 'equal'] = 'auto',
-                 cbar: bool = False,
-                 **ignored):
-
+    def __init__(
+        self,
+        ax: plt.Axes = None,
+        cax: plt.Axes = None,
+        figsize: Optional[Tuple[float, float]] = None,
+        title: str = None,
+        grid: bool = False,
+        vmin: Union[sc.Variable, int, float] = None,
+        vmax: Union[sc.Variable, int, float] = None,
+        aspect: Literal['auto', 'equal'] = 'auto',
+        cbar: bool = False,
+        **ignored,
+    ):
         # Note on the `**ignored`` keyword arguments: the figure which owns the canvas
         # creates both the canvas and an artist object (Line or Image). The figure
         # accepts keyword arguments, and has to somehow forward them to the canvas and
         # the artist. Since the figure has no detailed knowledge of the underlying
         # backend that implements the canvas, it cannot have specific arguments (such
         # as `ax` for specifying Matplotlib axes).
         # Instead, we forward all the kwargs from the figure to both the canvas and the
@@ -82,15 +83,16 @@
         self.yunit = None
         self._own_axes = False
 
         if self.ax is None:
             self._own_axes = True
             with silent_mpl_figure():
                 self.fig, self.ax = plt.subplots(
-                    figsize=(6., 4.) if figsize is None else figsize)
+                    figsize=(6.0, 4.0) if figsize is None else figsize
+                )
             if self.is_widget():
                 self.fig.canvas.toolbar_visible = False
                 self.fig.canvas.header_visible = False
         else:
             self.fig = self.ax.get_figure()
 
         if cbar and self.cax is None:
@@ -110,14 +112,15 @@
         return hasattr(self.fig.canvas, "on_widget_constructed")
 
     def to_image(self):
         """
         Convert the underlying Matplotlib figure to an image widget from ``ipywidgets``.
         """
         from ipywidgets import Image
+
         return Image(value=fig_to_bytes(self.fig), format='png')
 
     def to_widget(self):
         if self.is_widget() and not is_sphinx_build():
             return self.fig.canvas
         else:
             return self.to_image()
@@ -141,32 +144,40 @@
             self._xmax = max(self._xmax, xmax)
             self._ymin = min(self._ymin, ymin)
             self._ymax = max(self._ymax, ymax)
         for c in self.ax.collections:
             if isinstance(c, QuadMesh):
                 coords = c.get_coordinates()
                 left, right = fix_empty_range(
-                    find_limits(sc.array(dims=['x', 'y'], values=coords[..., 0]),
-                                scale=self.xscale))
+                    find_limits(
+                        sc.array(dims=['x', 'y'], values=coords[..., 0]),
+                        scale=self.xscale,
+                    )
+                )
                 bottom, top = fix_empty_range(
-                    find_limits(sc.array(dims=['x', 'y'], values=coords[..., 1]),
-                                scale=self.yscale))
+                    find_limits(
+                        sc.array(dims=['x', 'y'], values=coords[..., 1]),
+                        scale=self.yscale,
+                    )
+                )
                 self._xmin = min(self._xmin, left.value)
                 self._xmax = max(self._xmax, right.value)
                 self._ymin = min(self._ymin, bottom.value)
                 self._ymax = max(self._ymax, top.value)
         if self._user_vmin is not None:
             self._ymin = maybe_variable_to_number(self._user_vmin, unit=self.yunit)
         if self._user_vmax is not None:
             self._ymax = maybe_variable_to_number(self._user_vmax, unit=self.yunit)
 
-        self.ax.set_xlim(_none_if_not_finite(self._xmin),
-                         _none_if_not_finite(self._xmax))
-        self.ax.set_ylim(_none_if_not_finite(self._ymin),
-                         _none_if_not_finite(self._ymax))
+        self.ax.set_xlim(
+            _none_if_not_finite(self._xmin), _none_if_not_finite(self._xmax)
+        )
+        self.ax.set_ylim(
+            _none_if_not_finite(self._ymin), _none_if_not_finite(self._ymax)
+        )
         self.draw()
 
     def draw(self):
         """
         Make a draw call to the underlying figure.
         """
         self.fig.canvas.draw_idle()
@@ -197,109 +208,148 @@
 
         Parameters
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
         for xy, lims in limits.items():
-            getattr(self.ax, f'set_{xy}lim')(*[
-                maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
-                for m in ('min', 'max') if m in lims
-            ])
+            getattr(self.ax, f'set_{xy}lim')(
+                *[
+                    maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
+                    for m in ('min', 'max')
+                    if m in lims
+                ]
+            )
 
     @property
     def title(self) -> str:
+        """
+        Get or set the title of the plot.
+        """
         return self.ax.get_title()
 
     @title.setter
     def title(self, text: str):
         self.ax.set_title(text)
 
     @property
     def xlabel(self) -> str:
+        """
+        Get or set the label of the x-axis.
+        """
         return self.ax.get_xlabel()
 
     @xlabel.setter
     def xlabel(self, lab: str):
         self.ax.set_xlabel(lab)
 
     @property
     def ylabel(self) -> str:
+        """
+        Get or set the label of the y-axis.
+        """
         return self.ax.get_ylabel()
 
     @ylabel.setter
     def ylabel(self, lab: str):
         self.ax.set_ylabel(lab)
 
     @property
     def cblabel(self) -> str:
+        """
+        Get or set the label of the colorbar.
+        """
         return self.cax.get_ylabel()
 
     @cblabel.setter
     def cblabel(self, lab: str):
         self.cax.set_ylabel(lab)
 
     @property
     def xscale(self) -> str:
+        """
+        Get or set the scale of the x-axis ('linear' or 'log').
+        """
         return self.ax.get_xscale()
 
     @xscale.setter
     def xscale(self, scale: Literal['linear', 'log']):
         self.ax.set_xscale(scale)
 
     @property
     def yscale(self) -> str:
+        """
+        Get or set the scale of the y-axis ('linear' or 'log').
+        """
         return self.ax.get_yscale()
 
     @yscale.setter
     def yscale(self, scale: Literal['linear', 'log']):
         self.ax.set_yscale(scale)
 
     @property
     def xmin(self) -> float:
+        """
+        Get or set the lower (left) bound of the x-axis.
+        """
         return self.ax.get_xlim()[0]
 
     @xmin.setter
     def xmin(self, value: float):
         self.ax.set_xlim(value, self.xmax)
 
     @property
     def xmax(self) -> float:
+        """
+        Get or set the upper (right) bound of the x-axis.
+        """
         return self.ax.get_xlim()[1]
 
     @xmax.setter
     def xmax(self, value: float):
         self.ax.set_xlim(self.xmin, value)
 
     @property
     def xrange(self) -> Tuple[float, float]:
+        """
+        Get or set the range/limits of the x-axis.
+        """
         return self.ax.get_xlim()
 
     @xrange.setter
     def xrange(self, value: Tuple[float, float]):
         self.ax.set_xlim(value)
 
     @property
     def ymin(self) -> float:
+        """
+        Get or set the lower (bottom) bound of the y-axis.
+        """
         return self.ax.get_ylim()[0]
 
     @ymin.setter
     def ymin(self, value: float):
         self.ax.set_ylim(value, self.ymax)
 
     @property
     def ymax(self) -> float:
+        """
+        Get or set the upper (top) bound of the y-axis.
+        """
         return self.ax.get_ylim()[1]
 
     @ymax.setter
     def ymax(self, value: float):
         self.ax.set_ylim(self.ymin, value)
 
     @property
     def yrange(self) -> Tuple[float, float]:
+        """
+        Get or set the range/limits of the y-axis.
+        """
         return self.ax.get_ylim()
 
     @yrange.setter
     def yrange(self, value: Tuple[float, float]):
         self.ax.set_ylim(value)
 
     def reset_mode(self):
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/image.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,22 @@
     z = _maybe_repeat_values(data=data, dim_1d=dim_1d, dim_2d=dim_2d)
     if dim_2d is None:
         return coords['x'], coords['y'], z
 
     # Broadcast 1d coord to 2d and repeat along 1d dim
     # TODO: It may be more efficient here to first repeat and then broadcast, but
     # the current order is simpler in implementation.
-    broadcasted_coord = repeat(sc.broadcast(coords[dim_1d[0]],
-                                            sizes={
-                                                **coords[dim_2d[0]].sizes,
-                                                **coords[dim_1d[0]].sizes
-                                            }).transpose(data.dims),
-                               dim=dim_1d[1],
-                               n=2)
+    broadcasted_coord = repeat(
+        sc.broadcast(
+            coords[dim_1d[0]],
+            sizes={**coords[dim_2d[0]].sizes, **coords[dim_1d[0]].sizes},
+        ).transpose(data.dims),
+        dim=dim_1d[1],
+        n=2,
+    )
     # Repeat 2d coord along 1d dim
     repeated_coord = repeat(coords[dim_2d[0]].transpose(data.dims), dim=dim_1d[1], n=2)
     out = {dim_1d[0]: broadcasted_coord[dim_1d[1], 1:-1], dim_2d[0]: repeated_coord}
     return out['x'], out['y'], z
 
 
 class Image:
@@ -66,21 +67,22 @@
         The shading to use for the ``pcolormesh``.
     rasterized:
         Rasterize the mesh/image if ``True``.
     **kwargs:
         Additional arguments are forwarded to Matplotlib's ``pcolormesh``.
     """
 
-    def __init__(self,
-                 canvas: Canvas,
-                 data: sc.DataArray,
-                 shading: str = 'auto',
-                 rasterized: bool = True,
-                 **kwargs):
-
+    def __init__(
+        self,
+        canvas: Canvas,
+        data: sc.DataArray,
+        shading: str = 'auto',
+        rasterized: bool = True,
+        **kwargs,
+    ):
         self._canvas = canvas
         self._ax = self._canvas.ax
         self._data = data
         self._id = uuid.uuid4().hex
         # Because all keyword arguments from the figure are forwarded to both the canvas
         # and the line, we need to remove the arguments that belong to the canvas.
         kwargs.pop('ax', None)
@@ -92,33 +94,37 @@
 
         to_dim_search = {}
         string_labels = {}
         bin_edge_coords = {}
         for i, k in enumerate('yx'):
             to_dim_search[k] = {
                 'dim': self._data.dims[i],
-                'var': self._data.meta[self._data.dims[i]]
+                'var': self._data.meta[self._data.dims[i]],
             }
             bin_edge_coords[k] = coord_as_bin_edges(self._data, self._data.dims[i])
             if self._data.meta[self._data.dims[i]].dtype == str:
                 string_labels[k] = self._data.meta[self._data.dims[i]]
 
         self._dim_1d, self._dim_2d = _get_dims_of_1d_and_2d_coords(to_dim_search)
         self._mesh = None
 
-        x, y, z = _from_data_array_to_pcolormesh(data=self._data.data,
-                                                 coords=bin_edge_coords,
-                                                 dim_1d=self._dim_1d,
-                                                 dim_2d=self._dim_2d)
-        self._mesh = self._ax.pcolormesh(x.values,
-                                         y.values,
-                                         z.values,
-                                         shading=shading,
-                                         rasterized=rasterized,
-                                         **kwargs)
+        x, y, z = _from_data_array_to_pcolormesh(
+            data=self._data.data,
+            coords=bin_edge_coords,
+            dim_1d=self._dim_1d,
+            dim_2d=self._dim_2d,
+        )
+        self._mesh = self._ax.pcolormesh(
+            x.values,
+            y.values,
+            z.values,
+            shading=shading,
+            rasterized=rasterized,
+            **kwargs,
+        )
         self._mesh.set_array(None)
 
         for xy, var in string_labels.items():
             getattr(self._ax, f'set_{xy}ticks')(np.arange(float(var.shape[0])))
             getattr(self._ax, f'set_{xy}ticklabels')(var.values)
 
         if need_grid:
@@ -126,23 +132,29 @@
 
     @property
     def data(self):
         """
         Get the Mesh's data in a form that may have been tweaked, compared to the
         original data, in the case of a two-dimensional coordinate.
         """
-        out = sc.DataArray(data=_maybe_repeat_values(
-            data=self._data.data, dim_1d=self._dim_1d, dim_2d=self._dim_2d))
+        out = sc.DataArray(
+            data=_maybe_repeat_values(
+                data=self._data.data, dim_1d=self._dim_1d, dim_2d=self._dim_2d
+            )
+        )
         if self._data.masks:
-            out.masks['one_mask'] = _maybe_repeat_values(data=sc.broadcast(
-                merge_masks(self._data.masks),
-                dims=self._data.dims,
-                shape=self._data.shape),
-                                                         dim_1d=self._dim_1d,
-                                                         dim_2d=self._dim_2d)
+            out.masks['one_mask'] = _maybe_repeat_values(
+                data=sc.broadcast(
+                    merge_masks(self._data.masks),
+                    dims=self._data.dims,
+                    shape=self._data.shape,
+                ),
+                dim_1d=self._dim_1d,
+                dim_2d=self._dim_2d,
+            )
         return out
 
     def set_colors(self, rgba: np.ndarray):
         """
         Set the mesh's rgba colors:
 
         Parameters
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/interactive.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 
 class InteractiveFig(VBox):
     """
     Create an interactive figure.
     """
 
     def __init__(self, *args, FigConstructor, **kwargs):
-
         self._fig = FigConstructor(*args, **kwargs)
-        self.toolbar = make_toolbar_canvas2d(canvas=self._fig.canvas,
-                                             colormapper=getattr(
-                                                 self._fig, 'colormapper', None))
+        self.toolbar = make_toolbar_canvas2d(
+            canvas=self._fig.canvas, colormapper=getattr(self._fig, 'colormapper', None)
+        )
         self.left_bar = VBar([self.toolbar])
         self.right_bar = VBar()
         self.bottom_bar = HBar()
         self.top_bar = HBar()
 
-        super().__init__([
-            self.top_bar,
-            HBox([self.left_bar,
-                  self._fig.canvas.to_widget(), self.right_bar]), self.bottom_bar
-        ])
+        super().__init__(
+            [
+                self.top_bar,
+                HBox([self.left_bar, self._fig.canvas.to_widget(), self.right_bar]),
+                self.bottom_bar,
+            ]
+        )
 
     @property
     def fig(self):
         """
         Get the underlying Matplotlib figure.
         """
         return self._fig.canvas.fig
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/line.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/line.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         The initial data to create the line from.
     number:
         The canvas keeps track of how many lines have been added to it. This number is
         used to set the color and marker parameters of the line.
     """
 
     def __init__(self, canvas: Canvas, data: sc.DataArray, number: int = 0, **kwargs):
-
         self._canvas = canvas
         self._ax = self._canvas.ax
         self._data = data
         # Because all keyword arguments from the figure are forwarded to both the canvas
         # and the line, we need to remove the arguments that belong to the canvas.
         kwargs.pop('ax', None)
 
@@ -66,20 +65,22 @@
         aliases = {'ls': 'linestyle', 'lw': 'linewidth', 'c': 'color'}
         for key, alias in aliases.items():
             if key in args:
                 args[alias] = args.pop(key)
 
         self._make_line(data=self._make_data(), number=number, **args)
 
-    def _make_line(self,
-                   data: Dict,
-                   number: int,
-                   errorbars: bool = True,
-                   mask_color: str = 'black',
-                   **kwargs):
+    def _make_line(
+        self,
+        data: Dict,
+        number: int,
+        errorbars: bool = True,
+        mask_color: str = 'black',
+        **kwargs,
+    ):
         """
         Create either plot markers or a step function, depending on whether the data
         contains bin edges or not.
 
         Parameters
         ----------
         data:
@@ -97,103 +98,102 @@
             - ``matplotlib.pyplot.plot`` for data with a non bin-edge coordinate
             - ``matplotlib.pyplot.step`` for data with a bin-edge coordinate
         """
 
         default_step_style = {
             'linestyle': 'solid',
             'linewidth': 1.5,
-            'color': f'C{number}'
+            'color': f'C{number}',
         }
         markers = list(Line2D.markers.keys())
         default_plot_style = {
             'linestyle': 'none',
             'linewidth': 1.5,
             'marker': markers[(number + 2) % len(markers)],
-            'color': f'C{number}'
+            'color': f'C{number}',
         }
 
         if data["hist"]:
-            self._line = self._ax.step(data['values']['x'],
-                                       data['values']['y'],
-                                       label=self.label,
-                                       zorder=10,
-                                       **{
-                                           **default_step_style,
-                                           **kwargs
-                                       })[0]
+            self._line = self._ax.step(
+                data['values']['x'],
+                data['values']['y'],
+                label=self.label,
+                zorder=10,
+                **{**default_step_style, **kwargs},
+            )[0]
 
             self._mask = self._ax.step(data['mask']['x'], data['mask']['y'])[0]
             self._mask.update_from(self._line)
             self._mask.set_color(mask_color)
             self._mask.set_label(None)
             self._mask.set_linewidth(self._mask.get_linewidth() * 3)
             self._mask.set_zorder(self._mask.get_zorder() - 1)
             self._mask.set_visible(data['mask']['visible'])
         else:
-            self._line = self._ax.plot(data['values']['x'],
-                                       data['values']['y'],
-                                       label=self.label,
-                                       zorder=10,
-                                       **{
-                                           **default_plot_style,
-                                           **kwargs
-                                       })[0]
-            self._mask = self._ax.plot(data['mask']['x'],
-                                       data['mask']['y'],
-                                       zorder=11,
-                                       mec=mask_color,
-                                       mfc="None",
-                                       mew=3.0,
-                                       linestyle="none",
-                                       marker=self._line.get_marker(),
-                                       visible=data['mask']['visible'])[0]
+            self._line = self._ax.plot(
+                data['values']['x'],
+                data['values']['y'],
+                label=self.label,
+                zorder=10,
+                **{**default_plot_style, **kwargs},
+            )[0]
+            self._mask = self._ax.plot(
+                data['mask']['x'],
+                data['mask']['y'],
+                zorder=11,
+                mec=mask_color,
+                mfc="None",
+                mew=3.0,
+                linestyle="none",
+                marker=self._line.get_marker(),
+                visible=data['mask']['visible'],
+            )[0]
 
         # Add error bars
         if errorbars and (data['stddevs'] is not None):
-            self._error = self._ax.errorbar(data['stddevs']['x'],
-                                            data['stddevs']['y'],
-                                            yerr=data['stddevs']['e'],
-                                            color=self._line.get_color(),
-                                            zorder=10,
-                                            fmt="none")
+            self._error = self._ax.errorbar(
+                data['stddevs']['x'],
+                data['stddevs']['y'],
+                yerr=data['stddevs']['e'],
+                color=self._line.get_color(),
+                zorder=10,
+                fmt="none",
+            )
 
         if self.label:
             self._ax.legend()
 
     def _make_data(self) -> dict:
         x = self._data.meta[self._dim]
         y = self._data.data
         hist = len(x) != len(y)
         error = None
         mask = {'x': x.values, 'y': y.values, 'visible': False}
         if self._data.variances is not None:
             error = {
                 'x': sc.midpoints(x).values if hist else x.values,
                 'y': y.values,
-                'e': sc.stddevs(y).values
+                'e': sc.stddevs(y).values,
             }
         if len(self._data.masks):
             one_mask = merge_masks(self._data.masks).values
             mask = {
                 'x': x.values,
                 'y': np.where(one_mask, y.values, np.nan),
-                'visible': True
+                'visible': True,
             }
         if hist:
             y = sc.concat([y[0:1], y], dim=self._dim)
             if mask is not None:
                 mask['y'] = np.concatenate([mask['y'][0:1], mask['y']])
         return {
-            'values': {
-                'x': x.values,
-                'y': y.values
-            },
+            'values': {'x': x.values, 'y': y.values},
             'stddevs': error,
             'mask': mask,
-            'hist': hist
+            'hist': hist,
         }
 
     def update(self, new_values: sc.DataArray):
         """
         Update the x and y positions of the data points from new data.
 
         Parameters
@@ -210,17 +210,20 @@
             self._mask.set_visible(True)
         else:
             self._mask.set_visible(False)
 
         if (self._error is not None) and (new_values['stddevs'] is not None):
             coll = self._error.get_children()[0]
             coll.set_segments(
-                self._change_segments_y(new_values['stddevs']['x'],
-                                        new_values['stddevs']['y'],
-                                        new_values['stddevs']['e']))
+                self._change_segments_y(
+                    new_values['stddevs']['x'],
+                    new_values['stddevs']['y'],
+                    new_values['stddevs']['e'],
+                )
+            )
 
     def _change_segments_y(self, x: ArrayLike, y: ArrayLike, e: ArrayLike) -> ArrayLike:
         """
         Update the positions of the errorbars when `update_data` is called.
         """
         arr1 = np.repeat(x, 2)
         arr2 = np.array([y - e, y + e]).T.flatten()
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/static.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 class StaticFig:
     """
     Create a static figure to represent one-dimensional data.
     """
 
     def __init__(self, *args, FigConstructor, **kwargs):
-
         self._fig = FigConstructor(*args, **kwargs)
 
     def _repr_mimebundle_(self, include=None, exclude=None) -> dict:
         """
         Mimebundle display representation for jupyter notebooks.
         """
         out = {'text/plain': 'Figure'}
```

### Comparing `plopp-23.3.0/src/plopp/backends/matplotlib/utils.py` & `plopp-23.4.0/src/plopp/backends/matplotlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 
 
 def require_interactive_backend(func: str):
     """
     Raise an error if the current backend in use is non-interactive.
     """
     if not is_interactive_backend():
-        raise RuntimeError(f"The {func} can only be used with the interactive widget "
-                           "backend. Use `%matplotlib widget` at the start of your "
-                           "notebook.")
+        raise RuntimeError(
+            f"The {func} can only be used with the interactive widget "
+            "backend. Use `%matplotlib widget` at the start of your "
+            "notebook."
+        )
 
 
 def _running_in_jupyter() -> bool:
     """
     Detect whether Python is running in Jupyter.
 
     Note that this includes not only Jupyter notebooks
@@ -79,13 +81,14 @@
 def is_sphinx_build() -> bool:
     """
     Returns ``True`` if we are running inside a sphinx documentation build.
     """
     if not _running_in_jupyter():
         return False
     from IPython import get_ipython
+
     ipy = get_ipython()
     cfg = ipy.config
     meta = cfg["Session"]["metadata"]
     if hasattr(meta, "to_dict"):
         meta = meta.to_dict()
     return meta.get("scipp_sphinx_build", False)
```

### Comparing `plopp-23.3.0/src/plopp/backends/plotly/__init__.py` & `plopp-23.4.0/src/plopp/backends/plotly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
 class PlotlyBackend:
-
     def is_interactive(self):
         """
         Returns ``True`` if the backend currently in use allows for interactive figures.
         """
         return True
 
     def canvas2d(self, *args, **kwargs):
         """
         See :class:`canvas.Canvas` for details.
         """
         from .canvas import Canvas as CanvasPlotly
+
         return CanvasPlotly(*args, **kwargs)
 
     def line(self, *args, **kwargs):
         """
         See :class:`line.Line` for details.
         """
         from .line import Line as LinePlotly
+
         return LinePlotly(*args, **kwargs)
 
     def figure1d(self, *args, **kwargs):
         """
         See :class:`figure.Figure` for details.
         """
         from .figure import Figure as FigPlotly
+
         return FigPlotly(*args, **kwargs)
```

### Comparing `plopp-23.3.0/src/plopp/backends/plotly/canvas.py` & `plopp-23.4.0/src/plopp/backends/plotly/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,51 +28,53 @@
         The maximum value for the vertical axis. If a number (without a unit) is
         supplied, it is assumed that the unit is the same as the current vertical axis
         unit.
     cbar:
         Add axes to host a colorbar if ``True``.
     """
 
-    def __init__(self,
-                 figsize: Tuple[float, float] = None,
-                 title: str = None,
-                 vmin: Union[sc.Variable, int, float] = None,
-                 vmax: Union[sc.Variable, int, float] = None,
-                 cbar: bool = False,
-                 **ignored):
-
+    def __init__(
+        self,
+        figsize: Tuple[float, float] = None,
+        title: str = None,
+        vmin: Union[sc.Variable, int, float] = None,
+        vmax: Union[sc.Variable, int, float] = None,
+        cbar: bool = False,
+        **ignored,
+    ):
         # Note on the `**ignored`` keyword arguments: the figure which owns the canvas
         # creates both the canvas and an artist object (Line or Image). The figure
         # accepts keyword arguments, and has to somehow forward them to the canvas and
         # the artist. Since the figure has no detailed knowledge of the underlying
         # backend that implements the canvas, it cannot have specific arguments (such
         # as `layout` for specifying a Plotly layout).
         # Instead, we forward all the kwargs from the figure to both the canvas and the
         # artist, and filter out the artist kwargs with `**ignored`.
 
         import plotly.graph_objects as go
+
         self.fig = go.FigureWidget(
             layout={
                 'modebar_remove': [
-                    'zoom', 'pan', 'select', 'toImage', 'zoomIn', 'zoomOut',
-                    'autoScale', 'resetScale', 'lasso2d'
+                    'zoom',
+                    'pan',
+                    'select',
+                    'toImage',
+                    'zoomIn',
+                    'zoomOut',
+                    'autoScale',
+                    'resetScale',
+                    'lasso2d',
                 ],
-                'margin': {
-                    'l': 0,
-                    'r': 0,
-                    't': 0 if title is None else 40,
-                    'b': 0
-                },
-                'dragmode':
-                False,
-                'width':
-                600 if figsize is None else figsize[0],
-                'height':
-                400 if figsize is None else figsize[1]
-            })
+                'margin': {'l': 0, 'r': 0, 't': 0 if title is None else 40, 'b': 0},
+                'dragmode': False,
+                'width': 600 if figsize is None else figsize[0],
+                'height': 400 if figsize is None else figsize[1],
+            }
+        )
         self.figsize = figsize
         self._user_vmin = vmin
         self._user_vmax = vmax
         self.xunit = None
         self.yunit = None
         self._own_axes = False
         if title:
@@ -85,20 +87,23 @@
         """
         Auto-scale the axes ranges to show all data in the canvas.
         """
         ymin = None
         ymax = None
         if (self._user_vmin is not None) or (self._user_vmax is not None):
             if None in (self._user_vmin, self._user_vmax):
-                raise ValueError('With the Plotly backend, you have to specify both '
-                                 'vmin and vmax.')
+                raise ValueError(
+                    'With the Plotly backend, you have to specify both '
+                    'vmin and vmax.'
+                )
             ymin = maybe_variable_to_number(self._user_vmin, unit=self.yunit)
             ymax = maybe_variable_to_number(self._user_vmax, unit=self.yunit)
-            self.fig.update_layout(yaxis={'autorange': False},
-                                   xaxis={'autorange': True})
+            self.fig.update_layout(
+                yaxis={'autorange': False}, xaxis={'autorange': True}
+            )
             self.fig.update_yaxes(range=[ymin, ymax])
         else:
             self.fig.update_layout(yaxis={'autorange': True}, xaxis={'autorange': True})
 
     def save(self, filename: str):
         """
         Save the figure to file.
@@ -123,106 +128,142 @@
 
         Parameters
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
         for xy, lims in limits.items():
-            getattr(self.fig, f'update_{xy}axes')(range=[
-                maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
-                for m in ('min', 'max') if m in lims
-            ])
+            getattr(self.fig, f'update_{xy}axes')(
+                range=[
+                    maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
+                    for m in ('min', 'max')
+                    if m in lims
+                ]
+            )
 
     @property
     def title(self) -> str:
+        """
+        Get or set the title of the plot.
+        """
         return self.fig.layout.title
 
     @title.setter
     def title(self, text: str):
         layout = self.fig.layout
         if not text:
             layout.margin.t = 0
         elif layout.margin.t == 0:
             layout.margin.t = 40
         layout.title = text
 
     @property
     def xlabel(self) -> str:
+        """
+        Get or set the label of the x-axis.
+        """
         return self.fig.layout.xaxis.title
 
     @xlabel.setter
     def xlabel(self, lab: str):
         self.fig.layout.xaxis.title = lab
 
     @property
     def ylabel(self) -> str:
+        """
+        Get or set the label of the y-axis.
+        """
         return self.fig.layout.yaxis.title
 
     @ylabel.setter
     def ylabel(self, lab: str):
         self.fig.layout.yaxis.title = lab
 
     @property
     def xscale(self) -> str:
+        """
+        Get or set the scale of the x-axis ('linear' or 'log').
+        """
         return self.fig.layout.xaxis.type
 
     @xscale.setter
     def xscale(self, scale: Literal['linear', 'log']):
         self.fig.update_xaxes(type=scale)
 
     @property
     def yscale(self) -> str:
+        """
+        Get or set the scale of the y-axis ('linear' or 'log').
+        """
         return self.fig.layout.yaxis.type
 
     @yscale.setter
     def yscale(self, scale: Literal['linear', 'log']):
         self.fig.update_yaxes(type=scale)
 
     @property
     def xmin(self) -> float:
+        """
+        Get or set the lower (left) bound of the x-axis.
+        """
         return self.fig.layout.xaxis.range[0]
 
     @xmin.setter
     def xmin(self, value: float):
         self.fig.layout.xaxis.range = [value, self.xmax]
 
     @property
     def xmax(self) -> float:
+        """
+        Get or set the upper (right) bound of the x-axis.
+        """
         return self.fig.layout.xaxis.range[1]
 
     @xmax.setter
     def xmax(self, value: float):
         self.fig.layout.xaxis.range = [self.xmin, value]
 
     @property
     def xrange(self) -> Tuple[float, float]:
+        """
+        Get or set the range/limits of the x-axis.
+        """
         return self.fig.layout.xaxis.range
 
     @xrange.setter
     def xrange(self, value: Tuple[float, float]):
         self.fig.layout.xaxis.range = value
 
     @property
     def ymin(self) -> float:
+        """
+        Get or set the lower (bottom) bound of the y-axis.
+        """
         return self.fig.layout.yaxis.range[0]
 
     @ymin.setter
     def ymin(self, value: float):
         self.fig.layout.yaxis.range = [value, self.ymax]
 
     @property
     def ymax(self) -> float:
+        """
+        Get or set the upper (top) bound of the y-axis.
+        """
         return self.fig.layout.yaxis.range[1]
 
     @ymax.setter
     def ymax(self, value: float):
         self.fig.layout.yaxis.range = [self.ymin, value]
 
     @property
     def yrange(self) -> Tuple[float, float]:
+        """
+        Get or set the range/limits of the y-axis.
+        """
         return self.fig.layout.yaxis.range
 
     @yrange.setter
     def yrange(self, value: Tuple[float, float]):
         self.fig.layout.yaxis.range = value
 
     def reset_mode(self):
```

### Comparing `plopp-23.3.0/src/plopp/backends/plotly/figure.py` & `plopp-23.4.0/src/plopp/backends/plotly/figure.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 
 class Figure(VBox):
     """
     Create an interactive figure to represent one-dimensional data.
     """
 
     def __init__(self, *args, FigConstructor, **kwargs):
-
         self._fig = FigConstructor(*args, **kwargs)
         self.toolbar = make_toolbar_canvas2d(canvas=self._fig.canvas)
         self.left_bar = VBar([self.toolbar])
         self.right_bar = VBar()
         self.bottom_bar = HBar()
         self.top_bar = HBar()
 
-        super().__init__([
-            self.top_bar,
-            HBox([self.left_bar,
-                  self._fig.canvas.to_widget(), self.right_bar]), self.bottom_bar
-        ])
+        super().__init__(
+            [
+                self.top_bar,
+                HBox([self.left_bar, self._fig.canvas.to_widget(), self.right_bar]),
+                self.bottom_bar,
+            ]
+        )
 
     @property
     def canvas(self):
         return self._fig.canvas
 
     @property
     def artists(self):
```

### Comparing `plopp-23.3.0/src/plopp/backends/plotly/line.py` & `plopp-23.4.0/src/plopp/backends/plotly/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         The initial data to create the line from.
     number:
         The canvas keeps track of how many lines have been added to it. This number is
         used to set the color and marker parameters of the line.
     """
 
     def __init__(self, canvas: Canvas, data: sc.DataArray, number: int = 0, **kwargs):
-
         self._fig = canvas.fig
         self._data = data
 
         args = _parse_dicts_in_kwargs(kwargs, name=data.name)
 
         self._line = None
         self._mask = None
@@ -55,22 +54,24 @@
         self._dim = self._data.dim
         self._unit = self._data.unit
         self._coord = self._data.meta[self._dim]
         self._id = uuid.uuid4().hex
 
         self._make_line(data=self._make_data(), number=number, **args)
 
-    def _make_line(self,
-                   data: Dict,
-                   number: int,
-                   errorbars: bool = True,
-                   mask_color: str = 'black',
-                   mode='markers',
-                   marker=None,
-                   **kwargs):
+    def _make_line(
+        self,
+        data: Dict,
+        number: int,
+        errorbars: bool = True,
+        mask_color: str = 'black',
+        mode='markers',
+        marker=None,
+        **kwargs
+    ):
         """
         Create either plot markers or a step function, depending on whether the data
         contains bin edges or not.
 
         Parameters
         ----------
         data:
@@ -100,56 +101,59 @@
         if data["hist"]:
             line_shape = 'vh'
             mode = 'lines'
 
         marker_style = default_marker_style if marker is None else marker
         line_style = {**default_line_style, **kwargs}
 
-        self._line = go.Scatter(x=np.asarray(data['values']['x']),
-                                y=np.asarray(data['values']['y']),
-                                name=self.label,
-                                mode=mode,
-                                marker=marker_style,
-                                line_shape=line_shape,
-                                line=line_style)
+        self._line = go.Scatter(
+            x=np.asarray(data['values']['x']),
+            y=np.asarray(data['values']['y']),
+            name=self.label,
+            mode=mode,
+            marker=marker_style,
+            line_shape=line_shape,
+            line=line_style,
+        )
 
         if errorbars and (data['stddevs'] is not None):
-            self._error = go.Scatter(x=np.asarray(data['stddevs']['x']),
-                                     y=np.asarray(data['stddevs']['y']),
-                                     line=line_style,
-                                     name=self.label,
-                                     mode='markers',
-                                     marker={'opacity': 0},
-                                     error_y={
-                                         'type': 'data',
-                                         'array': data['stddevs']['e']
-                                     },
-                                     showlegend=False)
+            self._error = go.Scatter(
+                x=np.asarray(data['stddevs']['x']),
+                y=np.asarray(data['stddevs']['y']),
+                line=line_style,
+                name=self.label,
+                mode='markers',
+                marker={'opacity': 0},
+                error_y={'type': 'data', 'array': data['stddevs']['e']},
+                showlegend=False,
+            )
 
         marker_line_style = {'width': 3, 'color': mask_color}
         if 'line' in marker_style:
             marker_style['line'].update(marker_line_style)
         else:
             marker_style['line'] = marker_line_style
         if 'width' in line_style:
             line_style['width'] *= 5
         else:
             line_style['width'] = 5
         if data["hist"]:
             line_style['color'] = mask_color
 
-        self._mask = go.Scatter(x=np.asarray(data['mask']['x']),
-                                y=np.asarray(data['mask']['y']),
-                                name=self.label,
-                                mode=mode,
-                                marker=marker_style,
-                                line_shape=line_shape,
-                                line=line_style,
-                                visible=data['mask']['visible'],
-                                showlegend=False)
+        self._mask = go.Scatter(
+            x=np.asarray(data['mask']['x']),
+            y=np.asarray(data['mask']['y']),
+            name=self.label,
+            mode=mode,
+            marker=marker_style,
+            line_shape=line_shape,
+            line=line_style,
+            visible=data['mask']['visible'],
+            showlegend=False,
+        )
 
         # Below, we need to re-define the line because it seems that the Scatter trace
         # that ends up in the figure is a copy of the one above.
         # Plotly has no concept of zorder, so we need to add the traces in a specific
         # order
         if data["hist"]:
             self._fig.add_trace(self._mask)
@@ -178,35 +182,32 @@
         hist = len(x) != len(y)
         error = None
         mask = {'x': x.values, 'y': y.values, 'visible': False}
         if self._data.variances is not None:
             error = {
                 'x': sc.midpoints(x).values if hist else x.values,
                 'y': y.values,
-                'e': sc.stddevs(y).values
+                'e': sc.stddevs(y).values,
             }
         if len(self._data.masks):
             one_mask = merge_masks(self._data.masks).values
             mask = {
                 'x': x.values,
                 'y': np.where(one_mask, y.values, np.nan),
-                'visible': True
+                'visible': True,
             }
         if hist:
             y = sc.concat([y[0:1], y], dim=self._dim)
             if mask is not None:
                 mask['y'] = np.concatenate([mask['y'][0:1], mask['y']])
         return {
-            'values': {
-                'x': x.values,
-                'y': y.values
-            },
+            'values': {'x': x.values, 'y': y.values},
             'stddevs': error,
             'mask': mask,
-            'hist': hist
+            'hist': hist,
         }
 
     def update(self, new_values: sc.DataArray):
         """
         Update the x and y positions of the data points from new data.
 
         Parameters
@@ -214,27 +215,26 @@
         new_values:
             New data to update the line values, masks, errorbars from.
         """
         self._data = new_values
         new_values = self._make_data()
 
         with self._fig.batch_update():
-            self._line.update({
-                'x': new_values['values']['x'],
-                'y': new_values['values']['y']
-            })
+            self._line.update(
+                {'x': new_values['values']['x'], 'y': new_values['values']['y']}
+            )
 
             if (self._error is not None) and (new_values['stddevs'] is not None):
-                self._error.update({
-                    'x': new_values['stddevs']['x'],
-                    'y': new_values['stddevs']['y'],
-                    'error_y': {
-                        'array': new_values['stddevs']['e']
+                self._error.update(
+                    {
+                        'x': new_values['stddevs']['x'],
+                        'y': new_values['stddevs']['y'],
+                        'error_y': {'array': new_values['stddevs']['e']},
                     }
-                })
+                )
 
             if new_values['mask']['visible']:
                 update = {'x': new_values['mask']['x'], 'y': new_values['mask']['y']}
                 self._mask.update(update)
                 self._mask.visible = True
             else:
                 self._mask.visible = False
```

### Comparing `plopp-23.3.0/src/plopp/backends/pythreejs/__init__.py` & `plopp-23.4.0/src/plopp/backends/pythreejs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
 class PythreejsBackend:
-
     def is_interactive(self):
         """
         Returns ``True`` if the backend currently in use allows for interactive figures.
         """
         return True
 
     def canvas3d(self, *args, **kwargs):
         """
         See :class:`canvas.Canvas` for details.
         """
         from .canvas import Canvas as CanvasP3js
+
         return CanvasP3js(*args, **kwargs)
 
     def point_cloud(self, *args, **kwargs):
         """
         See :class:`point_cloud.PointCloud` for details.
         """
         from .point_cloud import PointCloud as PointCloudP3js
+
         return PointCloudP3js(*args, **kwargs)
 
     def figure3d(self, *args, **kwargs):
         """
         See :class:`figure.Figure` for details.
         """
         from .figure import Figure as FigP3js
+
         return FigP3js(*args, **kwargs)
```

### Comparing `plopp-23.3.0/src/plopp/backends/pythreejs/canvas.py` & `plopp-23.4.0/src/plopp/backends/pythreejs/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from copy import copy
-from typing import Any, Tuple
+from typing import Any, Optional, Tuple
 
 import ipywidgets as ipw
 import numpy as np
-from scipp import Variable
+import scipp as sc
+
+from ...graphics import Camera
 
 
 class Canvas:
     """
     WebGL canvas used to render 3D graphics.
     It is based on the ``pythreejs`` library. It provides a scene, camera, controls,
     as well as functions for controlling the camera.
@@ -20,99 +22,127 @@
     Parameters
     ----------
     figsize:
         The width and height of the renderer in pixels.
     title:
         The title to be placed above the figure. It is possible to use HTML formatting
         to customize the title appearance.
+    camera:
+        Initial camera configuration (position, target).
     """
 
-    def __init__(self, figsize: Tuple[int, int] = (600, 400), title: str = None):
-
-        # TODO: the title is still unused.
-
+    def __init__(
+        self,
+        figsize: Tuple[int, int] = (600, 400),
+        title: Optional[str] = None,
+        camera: Optional[Camera] = None,
+    ):
         import pythreejs as p3
 
         self.xunit = None
         self.yunit = None
         self.zunit = None
         self.outline = None
         self.axticks = None
         self.figsize = np.asarray(figsize)
         self._title_text = title
         self._title = self._make_title()
         width, height = self.figsize
-
+        self._user_camera = Camera() if camera is None else camera
         self.camera = p3.PerspectiveCamera(aspect=width / height)
         self.camera_backup = {}
         self.axes_3d = p3.AxesHelper()
         self.outline = None
-        self.scene = p3.Scene(children=[self.camera, self.axes_3d],
-                              background="#f0f0f0")
+        self.scene = p3.Scene(
+            children=[self.camera, self.axes_3d], background="#f0f0f0"
+        )
         self.controls = p3.OrbitControls(controlling=self.camera)
-        self.renderer = p3.Renderer(camera=self.camera,
-                                    scene=self.scene,
-                                    controls=[self.controls],
-                                    width=width,
-                                    height=height)
+        self.renderer = p3.Renderer(
+            camera=self.camera,
+            scene=self.scene,
+            controls=[self.controls],
+            width=width,
+            height=height,
+        )
 
     def to_widget(self):
         return self.renderer
 
-    def make_outline(self, limits: Tuple[Variable, Variable, Variable]):
+    def make_outline(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Create an outline box with ticklabels, given a range in the XYZ directions.
         """
         from .outline import Outline
+
         if self.outline is not None:
             self.remove(self.outline)
         self.outline = Outline(limits=limits)
         self.add(self.outline)
         self._update_camera(limits=limits)
         self.axes_3d.scale = [self.camera.far] * 3
 
-    def _update_camera(self, limits: Tuple[Variable, Variable, Variable]):
+    def _update_camera(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Update the camera position when a new object is added to the canvas.
         The camera will look at the mean position of all the objects, and its position
         will be far enough from the center to see all the objects.
         This 'Home' position will be backed up so it can be used when resetting the
         camera via the ``home`` function.
         """
+        if not self._user_camera.has_units():
+            self._user_camera.set_units(self.xunit, self.yunit, self.zunit)
+
         center = [var.mean().value for var in limits]
-        distance_from_center = 1.2
+        distance_fudge_factor = 1.2
         box_size = np.array([(limits[i][1] - limits[i][0]).value for i in range(3)])
-        camera_position = list(np.array(center) + distance_from_center * box_size)
-        camera_lookat = tuple(center)
-        self.camera.position = camera_position
-        cam_pos_norm = np.linalg.norm(self.camera.position)
+        self.camera.position = self._user_camera.get(
+            'position', list(np.array(center) + distance_fudge_factor * box_size)
+        )
+        camera_dist = np.linalg.norm(np.array(self.camera.position) - np.array(center))
         box_mean_size = np.linalg.norm(box_size)
-        self.camera.near = 0.01 * box_mean_size
-        self.camera.far = 5.0 * cam_pos_norm
+        self.camera.near = self._user_camera.get('near', 0.01 * box_mean_size)
+        camera_to_origin = np.linalg.norm(
+            np.array(self.camera.position) - np.array([0, 0, 0])
+        )
+        center_to_origin = np.linalg.norm(np.array(center) - np.array([0, 0, 0]))
+        self.camera.far = self._user_camera.get(
+            'far',
+            5 * max(box_mean_size, camera_dist, camera_to_origin, center_to_origin),
+        )
+        camera_lookat = tuple(self._user_camera.get('look_at', center))
         self.controls.target = camera_lookat
         self.camera.lookAt(camera_lookat)
 
         # Save camera settings
         self.camera_backup["reset"] = copy(self.camera.position)
+        self.camera_backup["look_at"] = copy(camera_lookat)
         self.camera_backup["center"] = tuple(copy(center))
         self.camera_backup["x_normal"] = [
-            center[0] - distance_from_center * box_mean_size, center[1], center[2]
+            center[0] - distance_fudge_factor * box_mean_size,
+            center[1],
+            center[2],
         ]
         self.camera_backup["y_normal"] = [
-            center[0], center[1] - distance_from_center * box_mean_size, center[2]
+            center[0],
+            center[1] - distance_fudge_factor * box_mean_size,
+            center[2],
         ]
         self.camera_backup["z_normal"] = [
-            center[0], center[1], center[2] - distance_from_center * box_mean_size
+            center[0],
+            center[1],
+            center[2] - distance_fudge_factor * box_mean_size,
         ]
 
     def home(self):
         """
         Reset the camera position.
         """
-        self.move_camera(position=self.camera_backup["reset"])
+        self.move_camera(
+            position=self.camera_backup["reset"], look_at=self.camera_backup["look_at"]
+        )
 
     def camera_x_normal(self):
         """
         View scene along the X normal.
         """
         self._camera_normal(position=self.camera_backup["x_normal"].copy(), ind=0)
 
@@ -133,26 +163,32 @@
         Move camera to requested normal, and flip if current position is equal
         to the requested position.
         """
         if np.allclose(self.camera.position, position):
             position[ind] = 2.0 * self.camera_backup["center"][ind] - position[ind]
         self.move_camera(position=position)
 
-    def move_camera(self, position: Tuple[float, float, float]):
+    def move_camera(
+        self,
+        position: Tuple[float, float, float],
+        look_at: Optional[Tuple[float, float, float]] = None,
+    ):
         """
         Move the camera to the supplied position.
 
         Parameters
         ----------
         position:
             The new camera position.
         """
         self.camera.position = position
-        self.controls.target = self.camera_backup["center"]
-        self.camera.lookAt(self.camera_backup["center"])
+        if look_at is None:
+            look_at = self.camera_backup["center"]
+        self.controls.target = look_at
+        self.camera.lookAt(look_at)
 
     def toggle_outline(self):
         """
         Toggle the visibility of the outline box.
         """
         self.outline.visible = not self.outline.visible
 
@@ -172,22 +208,27 @@
         """
         Remove an object from the ``scene``.
         """
         self.scene.remove(obj)
 
     def _make_title(self):
         if self._title_text:
-            html = (f'<div style="text-align: center; width: {self.figsize[0]}px">'
-                    f'{self._title_text}</div>')
+            html = (
+                f'<div style="text-align: center; width: {self.figsize[0]}px">'
+                f'{self._title_text}</div>'
+            )
         else:
             html = None
         return ipw.HTML(html)
 
     @property
     def title(self) -> str:
+        """
+        Get or set the title of the plot.
+        """
         return self._title_text
 
     @title.setter
     def title(self, text: str):
         self._title_text = text
         self._title = self._make_title()
```

### Comparing `plopp-23.3.0/src/plopp/backends/pythreejs/figure.py` & `plopp-23.4.0/src/plopp/backends/pythreejs/figure.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 
 class Figure(VBox):
     """
     Create a figure to represent three-dimensional data.
     """
 
     def __init__(self, *args, FigConstructor, **kwargs):
-
         self._fig = FigConstructor(*args, **kwargs)
-        self.toolbar = make_toolbar_canvas3d(canvas=self._fig.canvas,
-                                             colormapper=self._fig.colormapper)
+        self.toolbar = make_toolbar_canvas3d(
+            canvas=self._fig.canvas, colormapper=self._fig.colormapper
+        )
         self.left_bar = VBar([self.toolbar])
         self.right_bar = VBar([self._fig.colormapper.to_widget()])
         self.bottom_bar = HBar()
         self.top_bar = HBar([self._fig.canvas._title])
 
-        super().__init__([
-            self.top_bar,
-            HBox([self.left_bar,
-                  self._fig.canvas.to_widget(), self.right_bar]), self.bottom_bar
-        ])
+        super().__init__(
+            [
+                self.top_bar,
+                HBox([self.left_bar, self._fig.canvas.to_widget(), self.right_bar]),
+                self.bottom_bar,
+            ]
+        )
 
     @property
     def canvas(self):
         return self._fig.canvas
 
     @property
     def artists(self):
@@ -75,17 +77,19 @@
         filename:
             Name of the output HTML file.
         """
         ext = os.path.splitext(filename)[1]
         if ext.lower() != '.html':
             raise ValueError('File extension must be .html for saving 3d figures.')
         from ipywidgets.embed import dependency_state, embed_minimal_html
+
         out = HBox([self._fig.canvas.to_widget(), self.right_bar])
         # Garbage collection for embedded html output:
         # https://github.com/jupyter-widgets/pythreejs/issues/217
         state = dependency_state(out)
         # convert and write to file
         embed_minimal_html(
             filename,
             out,
             title=self._fig.canvas.title if self._fig.canvas.title else 'figure3d',
-            state=state)
+            state=state,
+        )
```

### Comparing `plopp-23.3.0/src/plopp/backends/pythreejs/outline.py` & `plopp-23.4.0/src/plopp/backends/pythreejs/outline.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,46 +14,51 @@
 def _get_delta(x: Variable, axis: int) -> float:
     """
     Compute the difference between two bounds along a given axis.
     """
     return (x[axis][1] - x[axis][0]).value
 
 
-def _get_offsets(limits: Tuple[Variable, Variable, Variable], axis: int,
-                 ind: int) -> np.ndarray:
+def _get_offsets(
+    limits: Tuple[Variable, Variable, Variable], axis: int, ind: int
+) -> np.ndarray:
     """
     Compute offsets for 3 dimensions, along the edges of the box.
     """
     offsets = np.array([limits[i][ind].value for i in range(3)])
     offsets[axis] = 0
     return offsets
 
 
 def _make_geometry(limits: Tuple[Variable, Variable, Variable]) -> p3.EdgesGeometry:
     """
     Make a geometry to represent the edges of a cubic box.
     """
     return p3.EdgesGeometry(
-        p3.BoxBufferGeometry(width=_get_delta(limits, axis=0),
-                             height=_get_delta(limits, axis=1),
-                             depth=_get_delta(limits, axis=2)))
+        p3.BoxBufferGeometry(
+            width=_get_delta(limits, axis=0),
+            height=_get_delta(limits, axis=1),
+            depth=_get_delta(limits, axis=2),
+        )
+    )
 
 
-def _make_sprite(string: str,
-                 position: Tuple[float, float, float],
-                 color: str = "black",
-                 size: float = 1.0) -> p3.Sprite:
+def _make_sprite(
+    string: str,
+    position: Tuple[float, float, float],
+    color: str = "black",
+    size: float = 1.0,
+) -> p3.Sprite:
     """
     Make a text-based sprite for axis tick.
     """
-    sm = p3.SpriteMaterial(map=p3.TextTexture(string=string,
-                                              color=color,
-                                              size=300,
-                                              squareTexture=True),
-                           transparent=True)
+    sm = p3.SpriteMaterial(
+        map=p3.TextTexture(string=string, color=color, size=300, squareTexture=True),
+        transparent=True,
+    )
     return p3.Sprite(material=sm, position=position, scale=[size, size, size])
 
 
 class Outline(p3.Group):
     """
     Create an object that draws a rectangular outline, given some limits for the XYZ
     dimensions. Along the lower edges of the cube are added some tick labels and axes
@@ -67,65 +72,79 @@
         for the outline. Each variable also has a dimension, which is to be used as the
         dimension for that direction, as well as a unit, which will be used to label
         the corresponding axis.
     tick_size:
         A number to scale the tick size.
     """
 
-    def __init__(self,
-                 limits: Tuple[Variable, Variable, Variable],
-                 tick_size: float = None):
-
+    def __init__(
+        self, limits: Tuple[Variable, Variable, Variable], tick_size: float = None
+    ):
         center = [var.mean().value for var in limits]
         if tick_size is None:
             tick_size = 0.05 * np.mean([_get_delta(limits, axis=i) for i in range(3)])
 
-        self.box = p3.LineSegments(geometry=_make_geometry(limits),
-                                   material=p3.LineBasicMaterial(color='#000000'),
-                                   position=center)
+        self.box = p3.LineSegments(
+            geometry=_make_geometry(limits),
+            material=p3.LineBasicMaterial(color='#000000'),
+            position=center,
+        )
 
         self.ticks = self._make_ticks(limits=limits, tick_size=tick_size)
-        self.labels = self._make_labels(limits=limits,
-                                        center=center,
-                                        tick_size=tick_size)
+        self.labels = self._make_labels(
+            limits=limits, center=center, tick_size=tick_size
+        )
 
         super().__init__()
         for obj in (self.box, self.ticks, self.labels):
             self.add(obj)
 
-    def _make_ticks(self, limits: Tuple[Variable, Variable, Variable],
-                    tick_size: float) -> p3.Group:
+    def _make_ticks(
+        self, limits: Tuple[Variable, Variable, Variable], tick_size: float
+    ) -> p3.Group:
         """
         Create tick labels on outline edges
         """
         ticks_group = p3.Group()
         iden = np.identity(3, dtype=np.float32)
         ticker_ = ticker.MaxNLocator(5)
         for axis in range(3):
             ticks = ticker_.tick_values(limits[axis][0].value, limits[axis][1].value)
             for tick in ticks:
                 if limits[axis][0].value <= tick <= limits[axis][1].value:
                     tick_pos = iden[axis] * tick + _get_offsets(limits, axis, 0)
                     ticks_group.add(
-                        _make_sprite(string=value_to_string(tick, precision=1),
-                                     position=tick_pos.tolist(),
-                                     size=tick_size))
+                        _make_sprite(
+                            string=value_to_string(tick, precision=1),
+                            position=tick_pos.tolist(),
+                            size=tick_size,
+                        )
+                    )
         return ticks_group
 
-    def _make_labels(self, limits: Tuple[Variable, Variable, Variable],
-                     center: List[float], tick_size: float) -> p3.Group:
+    def _make_labels(
+        self,
+        limits: Tuple[Variable, Variable, Variable],
+        center: List[float],
+        tick_size: float,
+    ) -> p3.Group:
         """
         Create axes labels (coord dimension and unit) on outline edges
         """
         labels_group = p3.Group()
         for axis in range(3):
             axis_label = f'{limits[axis].dim} [{limits[axis].unit}]'
             # Offset labels 5% beyond axis ticks to reduce overlap
             delta = 0.05
             labels_group.add(
-                _make_sprite(string=axis_label,
-                             position=(np.roll([1, 0, 0], axis) * center[axis] +
-                                       (1.0 + delta) * _get_offsets(limits, axis, 0) -
-                                       delta * _get_offsets(limits, axis, 1)).tolist(),
-                             size=tick_size * 0.3 * len(axis_label)))
+                _make_sprite(
+                    string=axis_label,
+                    position=(
+                        np.roll([1, 0, 0], axis) * center[axis]
+                        + (1.0 + delta) * _get_offsets(limits, axis, 0)
+                        - delta * _get_offsets(limits, axis, 1)
+                    ).tolist(),
+                    size=tick_size * 0.3 * len(axis_label),
+                )
+            )
 
         return labels_group
```

### Comparing `plopp-23.3.0/src/plopp/backends/pythreejs/point_cloud.py` & `plopp-23.4.0/src/plopp/backends/pythreejs/point_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 import numpy as np
 import scipp as sc
 
 
 def _check_ndim(data):
     if data.ndim != 1:
-        raise ValueError('PointCloud only accepts one dimensional data, '
-                         f'found {data.ndim} dimensions. You should flatten your data '
-                         '(using scipp.flatten) before sending it to the point cloud.')
+        raise ValueError(
+            'PointCloud only accepts one dimensional data, '
+            f'found {data.ndim} dimensions. You should flatten your data '
+            '(using scipp.flatten) before sending it to the point cloud.'
+        )
 
 
 class PointCloud:
     """
     Artist to represent a three-dimensional point cloud/scatter plot.
 
     Parameters
@@ -31,22 +33,24 @@
         The initial data to create the line from.
     pixel_size:
         The size of the markers.
     opacity:
         The opacity of the points.
     """
 
-    def __init__(self,
-                 *,
-                 x: str,
-                 y: str,
-                 z: str,
-                 data: sc.DataArray,
-                 pixel_size: Union[sc.Variable, float, int] = 1,
-                 opacity: float = 1):
+    def __init__(
+        self,
+        *,
+        x: str,
+        y: str,
+        z: str,
+        data: sc.DataArray,
+        pixel_size: Union[sc.Variable, float, int] = 1,
+        opacity: float = 1,
+    ):
         """
         Make a point cloud using pythreejs
         """
         import pythreejs as p3
 
         _check_ndim(data)
         self._data = data
@@ -57,40 +61,50 @@
 
         self._pixel_size = pixel_size
         if hasattr(self._pixel_size, 'unit'):
             if len(set([self._data.meta[dim].unit for dim in [x, y, z]])) > 1:
                 raise ValueError(
                     f'The supplied pixel_size has unit {self._pixel_size.unit}, but '
                     'the spatial coordinates do not all have the same units. In this '
-                    'case the pixel_size should just be a float with no unit.')
+                    'case the pixel_size should just be a float with no unit.'
+                )
             else:
                 self._pixel_size = self._pixel_size.to(
-                    dtype=float, unit=self._data.meta[x].unit).value
+                    dtype=float, unit=self._data.meta[x].unit
+                ).value
 
         self.geometry = p3.BufferGeometry(
             attributes={
-                'position':
-                p3.BufferAttribute(array=np.array([
-                    self._data.meta[self._x].values.astype('float32'), self._data.meta[
-                        self._y].values.astype('float32'), self._data.meta[
-                            self._z].values.astype('float32')
-                ]).T),
-                'color':
-                p3.BufferAttribute(array=np.zeros(
-                    [self._data.meta[self._x].shape[0], 3], dtype='float32'))
-            })
+                'position': p3.BufferAttribute(
+                    array=np.array(
+                        [
+                            self._data.meta[self._x].values.astype('float32'),
+                            self._data.meta[self._y].values.astype('float32'),
+                            self._data.meta[self._z].values.astype('float32'),
+                        ]
+                    ).T
+                ),
+                'color': p3.BufferAttribute(
+                    array=np.zeros(
+                        [self._data.meta[self._x].shape[0], 3], dtype='float32'
+                    )
+                ),
+            }
+        )
 
         # TODO: a device pixel_ratio should probably be read from a config file
         pixel_ratio = 1.0
         # Note that an additional factor of 2.5 (obtained from trial and error) seems to
         # be required to get the sizes right in the scene.
-        self.material = p3.PointsMaterial(vertexColors='VertexColors',
-                                          size=2.5 * self._pixel_size * pixel_ratio,
-                                          transparent=True,
-                                          opacity=opacity)
+        self.material = p3.PointsMaterial(
+            vertexColors='VertexColors',
+            size=2.5 * self._pixel_size * pixel_ratio,
+            transparent=True,
+            opacity=opacity,
+        )
         self.points = p3.Points(geometry=self.geometry, material=self.material)
 
     def set_colors(self, rgba):
         """
         Set the point cloud's rgba colors:
 
         Parameters
@@ -119,17 +133,19 @@
         xcoord = self._data.meta[self._x]
         ycoord = self._data.meta[self._y]
         zcoord = self._data.meta[self._z]
         half_pixel = 0.5 * self._pixel_size
         dx = sc.scalar(half_pixel, unit=xcoord.unit)
         dy = sc.scalar(half_pixel, unit=ycoord.unit)
         dz = sc.scalar(half_pixel, unit=zcoord.unit)
-        return (sc.concat([xcoord.min() - dx, xcoord.max() + dx], dim=self._x),
-                sc.concat([ycoord.min() - dy, ycoord.max() + dy], dim=self._y),
-                sc.concat([zcoord.min() - dz, zcoord.max() + dz], dim=self._z))
+        return (
+            sc.concat([xcoord.min() - dx, xcoord.max() + dx], dim=self._x),
+            sc.concat([ycoord.min() - dy, ycoord.max() + dy], dim=self._y),
+            sc.concat([zcoord.min() - dz, zcoord.max() + dz], dim=self._z),
+        )
 
     @property
     def opacity(self):
         """
         Get the material opacity.
         """
         return self.material.opacity
```

### Comparing `plopp-23.3.0/src/plopp/core/graph.py` & `plopp-23.4.0/src/plopp/core/graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,89 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from html import escape
+from itertools import chain
 
-from .model import Node
+from .node import Node
 
 
 def _make_graphviz_digraph(*args, **kwargs):
     try:
         from graphviz import Digraph
     except ImportError:
         raise RuntimeError(
             "Failed to import `graphviz`. "
             "Use `pip install graphviz` (requires installed `graphviz` executable) or "
-            "`conda install -c conda-forge python-graphviz`.")
+            "`conda install -c conda-forge python-graphviz`."
+        )
     return Digraph(*args, **kwargs)
 
 
-def _walk_graph(start, nodes, edges, views, hide_views):
-    label = escape(str(
-        start.func)) + '\nid = ' + start.id if start.name is None else escape(
-            start.name)
+def _walk_graph(start, nodes, edges, views, labels, hide_views):
+    label = (
+        escape(str(start.func)) + '\nid = ' + start.id
+        if start.name is None
+        else escape(start.name)
+    )
     nodes[start.id] = label
     for child in start.children:
         if start.id not in edges:
             edges[start.id] = {child.id}
         else:
             edges[start.id].add(child.id)
-        _walk_graph(start=child,
-                    nodes=nodes,
-                    edges=edges,
-                    views=views,
-                    hide_views=hide_views)
-    for parent in start.parents + list(start.kwparents.values()):
+        _walk_graph(
+            start=child,
+            nodes=nodes,
+            edges=edges,
+            views=views,
+            labels=labels,
+            hide_views=hide_views,
+        )
+    for arg_name, parent in chain(
+        ((f'arg_{i}', p) for i, p in enumerate(start.parents)), start.kwparents.items()
+    ):
         key = parent.id
+        if key not in labels:
+            labels[key] = arg_name
         if key not in nodes:
             if key not in edges:
                 edges[key] = {start.id}
             else:
                 edges[key].add(start.id)
-            _walk_graph(start=parent,
-                        nodes=nodes,
-                        edges=edges,
-                        views=views,
-                        hide_views=hide_views)
+            _walk_graph(
+                start=parent,
+                nodes=nodes,
+                edges=edges,
+                views=views,
+                labels=labels,
+                hide_views=hide_views,
+            )
+
     if not hide_views:
         for view in start.views:
             views[view.id] = view.__class__.__name__
             if start.id not in edges:
                 edges[start.id] = {view.id}
             else:
                 edges[start.id].add(view.id)
 
 
-def _make_graph(dot, nodes, edges, views):
+def _make_graph(dot, nodes, edges, labels, views):
     for key, lab in nodes.items():
         dot.node(key, label=lab)
     for key, lab in views.items():
         dot.node(key, label=lab, shape='ellipse', style='filled', color='lightgrey')
     for parent, children in edges.items():
         for child in children:
-            dot.edge(parent, child)
+            dot.edge(
+                parent,
+                child,
+                label=labels.get(parent, '') if child not in views else '',
+            )
     return dot
 
 
 def show_graph(node: Node, hide_views: bool = False):
     """
     Display the connected nodes and views as a graph.
 
@@ -82,13 +101,20 @@
         A visual representation of the graph generated with Graphviz.
     """
     dot = _make_graphviz_digraph(strict=True)
     dot.attr('node', shape='box', height='0.1')
     nodes = {}
     edges = {}
     views = {}
-    _walk_graph(start=node,
-                nodes=nodes,
-                edges=edges,
-                views=views,
-                hide_views=hide_views)
-    return _make_graph(dot=dot, nodes=nodes, edges=edges, views=views)
+    labels = {}
+    # If input is a View, get the underlying node
+    if hasattr(node, 'graph_nodes'):
+        node = list(node.graph_nodes.values())[0]
+    _walk_graph(
+        start=node,
+        nodes=nodes,
+        edges=edges,
+        views=views,
+        labels=labels,
+        hide_views=hide_views,
+    )
+    return _make_graph(dot=dot, nodes=nodes, edges=edges, labels=labels, views=views)
```

### Comparing `plopp-23.3.0/src/plopp/core/limits.py` & `plopp-23.4.0/src/plopp/core/limits.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 from typing import Literal, Tuple
 
 import numpy as np
 from scipp import Variable, scalar
 
 
-def find_limits(x: Variable,
-                scale: Literal['linear', 'log'] = 'linear') -> Tuple[Variable, ...]:
+def find_limits(
+    x: Variable, scale: Literal['linear', 'log'] = 'linear'
+) -> Tuple[Variable, ...]:
     """
     Find sensible limits, depending on linear or log scale.
     If there are no finite values in the array, return NaN for both min and max values.
     """
     v = x.values
     finite_inds = np.isfinite(v)
     if np.sum(finite_inds) == 0:
```

### Comparing `plopp-23.3.0/src/plopp/core/model.py` & `plopp-23.4.0/src/plopp/core/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,134 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from __future__ import annotations
+
 import uuid
-from functools import partial
+import warnings
 from itertools import chain
-from typing import Any, Callable
+from typing import Any, Union
+
+from .system import VisibleDeprecationWarning
+from .view import View
+
+
+# TODO: Remove this in v23.05.0
+def input_node(obj: Any) -> Node:
+    """
+    Create a simple node that returns the supplied object when data is requested from
+    it. This node has no parents, and typically lives at the top of a graph to provide
+    the raw input data.
+
+    .. deprecated:: v23.04.0
+       Use :class:`Node` instead.
+
+    Parameters
+    ----------
+    obj:
+        The object to return when data is requested from the node.
+    """
+    warnings.warn(
+        "plopp.input_node has been deprecated "
+        "and will be removed in Plopp v23.05.0. "
+        "Use plopp.Node instead.",
+        VisibleDeprecationWarning,
+    )
+    n = Node(lambda: obj)
+    n.name = f'Input <{type(obj).__name__}>'
+    return n
 
 
 class Node:
     """
     A node that can have parent and children nodes, to create a graph.
-    A node must be constructed from a callable ``func``.
+    A node can be constructed from a callable ``func``, or a raw object. In the case
+    of a raw object, a node wrapping the object will be created.
 
     Parameters
     ----------
     func:
-        The callable that is called when data is requested from the node.
+        The callable that is called when data is requested from the node. This can also
+        be a raw object, in which case this becomes a callable that returns the object.
     *parents:
         Positional arguments that represent the positional arguments of the function
         ``func``.
     *kwparents:
         Keyword arguments that represent the keyword arguments of the function ``func``.
     """
 
-    def __init__(self, func: Callable, *parents, **kwparents):
-        if not callable(func):
-            raise ValueError("A node can only be created using a callable func.")
-        self.func = func
-        self._id = str(uuid.uuid1())
+    def __init__(self, func: Any, *parents, **kwparents):
+        func_is_callable = callable(func)
+        self._input_value = None
+        if func_is_callable:
+            self.func = func
+        else:
+            self._input_value = func
+            self.func = lambda: func
+        self._id = uuid.uuid4().hex
         self.children = []
         self.views = []
-        self.parents = list(parents)
-        self.kwparents = dict(kwparents)
+        self.parents = [p if isinstance(p, Node) else Node(p) for p in parents]
+        self.kwparents = {
+            key: p if isinstance(p, Node) else Node(p) for key, p in kwparents.items()
+        }
         for parent in chain(self.parents, self.kwparents.values()):
             parent.add_child(self)
         self._data = None
-        self.name = None
+
+        if func_is_callable:
+            # Set automatic name from function name and arguments
+            args_string = ', '.join(
+                chain(
+                    (f'arg_{i}' for i in range(len(self.parents))),
+                    self.kwparents.keys(),
+                )
+            )
+            fname = getattr(self.func, "__name__", str(self.func))
+            self.name = f'{fname}({args_string})'
+        else:
+            val_str = f'={repr(func)}' if isinstance(func, (int, float, str)) else ""
+            self.name = f'Input <{type(func).__name__}{val_str}>'
 
     def __call__(self):
         return self.request_data()
 
     @property
-    def id(self):
+    def id(self) -> str:
         """
         The unique uuid of the node. This differs from the ``name`` which can be any
         string.
         """
         return self._id
 
+    @property
+    def input_value(self) -> Any:
+        """
+        The input value of the node, if it is an input node.
+        """
+        return self._input_value
+
+    @property
+    def is_input_node(self) -> bool:
+        """
+        Whether the node is an input node.
+        """
+        return self._input_value is not None
+
     def remove(self):
         """
         Remove the node from the graph.
         This attempts to remove clear the list of parents of the node.
         The operation fails is the node has children, as removing it would leave the
         graph in an ill-defined state.
         """
         if self.children:
             raise RuntimeError(
-                f"Cannot delete node because it has children {self.children}.")
+                f"Cannot delete node because it has children {self.children}."
+            )
         for view in self.views:
             del view.graph_nodes[self.id]
         for parent in chain(self.parents, self.kwparents.values()):
             parent.children.remove(self)
         self.views.clear()
         self.parents.clear()
         self.kwparents.clear()
@@ -72,27 +139,26 @@
         parents, and passes those results as arguments to the node's own ``func``.
         The result from calling the function is cached, to limit the number of times
         the graph is traversed.
         """
         if self._data is None:
             args = (parent.request_data() for parent in self.parents)
             kwargs = {
-                key: parent.request_data()
-                for key, parent in self.kwparents.items()
+                key: parent.request_data() for key, parent in self.kwparents.items()
             }
             self._data = self.func(*args, **kwargs)
         return self._data
 
-    def add_child(self, child):
+    def add_child(self, child: Node):
         """
         Add a child to the node.
         """
         self.children.append(child)
 
-    def add_view(self, view):
+    def add_view(self, view: View):
         """
         Add a view to the node.
         """
         self.views.append(view)
         view.graph_nodes[self.id] = self
 
     def notify_children(self, message: Any):
@@ -119,62 +185,33 @@
         ----------
         message:
             The message to pass to the views.
         """
         for view in self.views:
             view.notify_view({"node_id": self.id, "message": message})
 
+    def __repr__(self) -> str:
+        return f"Node(name={self.name})"
 
-def node(func: Callable, *args, **kwargs) -> Callable:
-    """
-    Create a :class:`Node` from a callable.
-    The additional arguments will be parent nodes to the returned node.
-    This can also be used as a decorator.
+    def __add__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x + y, self, other)
 
-    Parameters
-    ----------
-    func:
-        The callable to create the :class:`Node`.
-    """
-    partialized = partial(func, *args, **kwargs)
+    def __radd__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x + y, other, self)
 
-    def make_node(*args, **kwargs):
-        return Node(partialized, *args, **kwargs)
+    def __sub__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x - y, self, other)
 
-    return make_node
+    def __rsub__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x - y, other, self)
 
+    def __mul__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x * y, self, other)
 
-def input_node(obj: Any):
-    """
-    Create a simple node that returns the supplied object when data is requested from
-    it. This node has no parents, and typically lives at the top of a graph to provide
-    the raw input data.
-
-    Parameters
-    ----------
-    obj:
-        The object to return when data is requested from the node.
-    """
-    return Node(lambda: obj)
+    def __rmul__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x * y, other, self)
 
+    def __truediv__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x / y, self, other)
 
-def widget_node(widget) -> Node:
-    """
-    Create a node from a widget. When data is requested from it, it will return the
-    ``.value`` attribute of the supplied widget.
-    In addition, all of its children will be notified when the ``value`` of the widget
-    changes.
-
-    Parameters
-    ----------
-    widget:
-        The widget used to construct the node. This can be a widget from the
-        ``ipywidgets`` library, or a custom widget.
-    """
-    n = Node(func=lambda: widget.value)
-    # TODO: Our custom widgets have a '_plopp_observe' method instead of 'observe'
-    # because inheriting from VBox causes errors when overriding the 'observe' method
-    # (see https://bit.ly/3SggPVS).
-    func = widget._plopp_observe_ if hasattr(widget,
-                                             '_plopp_observe_') else widget.observe
-    func(n.notify_children, names="value")
-    return n
+    def __rtruediv__(self, other: Union[Node, Any]) -> Node:
+        return Node(lambda x, y: x / y, other, self)
```

### Comparing `plopp-23.3.0/src/plopp/core/utils.py` & `plopp-23.4.0/src/plopp/core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,32 +60,44 @@
     """
     index = x.dims.index(dim) + 1
     dummy_dim = uuid.uuid4().hex
     new_dims = list(x.dims)
     new_dims.insert(index, dummy_dim)
     new_shape = list(x.shape)
     new_shape.insert(index, n)
-    return x.broadcast(dims=new_dims, shape=new_shape).flatten(dims=[dim, dummy_dim],
-                                                               to=dim)
+    return x.broadcast(dims=new_dims, shape=new_shape).flatten(
+        dims=[dim, dummy_dim], to=dim
+    )
 
 
-def number_to_variable(x: Union[int, float, sc.Variable], unit: str) -> sc.Variable:
-    """
-    Convert the input int or float to a variable.
+def maybe_number_to_variable(
+    x: Union[int, float, sc.Variable], unit: Optional[str] = None
+) -> sc.Variable:
+    """
+    If the input is a raw number, convert to a variable.
+    If a unit is requested, perform the conversion to that unit before returning.
+    If the input is a variable, return it (potentially converted to the requested unit).
 
     Parameters
     ----------
     x:
         The input int or float.
+    unit:
+        The unit to use for the output variable.
     """
-    return sc.scalar(x, unit=unit) if isinstance(x, (int, float)) else x.to(unit=unit)
+    return (
+        sc.scalar(x, unit=unit)
+        if isinstance(x, (int, float))
+        else (x.to(unit=unit) if unit is not None else x)
+    )
 
 
-def maybe_variable_to_number(x: Union[int, float, sc.Variable],
-                             unit=None) -> Union[int, float]:
+def maybe_variable_to_number(
+    x: Union[int, float, sc.Variable], unit=None
+) -> Union[int, float]:
     """
     If the input is a variable, return its value.
     If a unit is requested, perform the conversion to that unit first.
     If the input is a number, return it unchanged.
 
     Parameters
     ----------
@@ -132,16 +144,17 @@
     val:
         The input number.
     precision:
         The number of decimal places to use for the string output.
     """
     if (not isinstance(val, float)) or (val == 0):
         text = str(val)
-    elif (abs(val) >= 10.0**(precision+1)) or \
-         (abs(val) <= 10.0**(-precision-1)):
+    elif (abs(val) >= 10.0 ** (precision + 1)) or (
+        abs(val) <= 10.0 ** (-precision - 1)
+    ):
         text = "{val:.{prec}e}".format(val=val, prec=precision)
     else:
         text = "{}".format(val)
         if len(text) > precision + 2 + (text[0] == '-'):
             text = "{val:.{prec}f}".format(val=val, prec=precision)
     return text
 
@@ -164,24 +177,27 @@
     case of a bin-edge coordinate) to a string.
 
     Parameters
     ----------
     x:
         The input variable (of length 1 or 2).
     """
-    out = value_to_string(x.values)
+    vals = x.values
+    if vals.shape:
+        out = ':'.join([value_to_string(v) for v in vals])
+    else:
+        out = value_to_string(float(vals))
     if x.unit is not None:
         out += f" [{x.unit}]"
     return out
 
 
-def make_compatible(x: sc.Variable,
-                    *,
-                    unit: Union[str, None],
-                    dim: Optional[str] = None):
+def make_compatible(
+    x: sc.Variable, *, unit: Union[str, None], dim: Optional[str] = None
+):
     """
     Raise exception if the dimensions of the supplied variable do not contain the
     requested dimension.
     Then, if the variable unit differs from the requested unit, attempt a conversion.
 
     Parameters
     ----------
@@ -191,15 +207,18 @@
         Attempt unit conversion to this unit if the input variable has a different unit.
     dim:
         If supplied, check that the dim is found in the input variable's dimensions.
     """
     if (dim is not None) and (dim not in x.dims):
         raise sc.DimensionError(
             f'The supplied variable has dimension {x.dims} which is '
-            f'incompatible with the requested dimension {dim}.')
+            f'incompatible with the requested dimension {dim}.'
+        )
     if x.unit != unit:
         if unit is not None:
             return x.to(unit=unit, dtype=float)
         else:
-            raise sc.UnitError(f'The supplied variable has unit {x.unit} which is '
-                               'incompatible with the requested unit None/<no unit>.')
+            raise sc.UnitError(
+                f'The supplied variable has unit {x.unit} which is '
+                'incompatible with the requested unit None/<no unit>.'
+            )
     return x
```

### Comparing `plopp-23.3.0/src/plopp/core/view.py` & `plopp-23.4.0/src/plopp/core/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Parameters
     ----------
     *nodes:
         The nodes that are attached to the view.
     """
 
     def __init__(self, *nodes):
-        self._id = str(uuid.uuid1())
+        self._id = uuid.uuid4().hex
         self.graph_nodes = {}
         for node in nodes:
             node.add_view(self)
 
     @abstractmethod
     def notify_view(self, _):
         """
```

### Comparing `plopp-23.3.0/src/plopp/data/examples.py` & `plopp-23.4.0/src/plopp/data/examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 _version = '1'
 
 
 @lru_cache(maxsize=1)
 def _make_pooch():
     import pooch
+
     return pooch.create(
         path=pooch.os_cache('plopp'),
         env='PLOPP_DATA_DIR',
         base_url='https://public.esss.dk/groups/scipp/plopp/{version}/',
         version=_version,
-        registry={'nyc_taxi_data.h5': 'md5:fc0867ec061e4ac0cbe5975a665a0eea'})
+        registry={'nyc_taxi_data.h5': 'md5:fc0867ec061e4ac0cbe5975a665a0eea'},
+    )
 
 
 _pooch = _make_pooch()
 
 
 def get_path(name: str) -> str:
     """
```

### Comparing `plopp-23.3.0/src/plopp/data/factory.py` & `plopp-23.4.0/src/plopp/data/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 import numpy as np
 import scipp as sc
 
 default_dim_list = ['x', 'y', 'z', 'time', 'temperature']
 
 
-def variable(ndim: int = 1,
-             variances: bool = False,
-             dtype: str = 'float64',
-             unit: str = 'm/s',
-             dims: Optional[List[str]] = None,
-             dim_list: List[str] = default_dim_list) -> sc.Variable:
+def variable(
+    ndim: int = 1,
+    variances: bool = False,
+    dtype: str = 'float64',
+    unit: str = 'm/s',
+    dims: Optional[List[str]] = None,
+    dim_list: List[str] = default_dim_list,
+) -> sc.Variable:
     """
     Generate a sample ``Variable`` containing data based on a sine function.
 
     Parameters
     ----------
     ndim:
         The number of dimensions.
@@ -46,25 +48,27 @@
     var = sc.array(dims=dims, values=a, unit=unit, dtype=dtype)
     if variances:
         var.variances = np.abs(np.random.normal(a * 0.1, 0.05))
 
     return var
 
 
-def data_array(ndim: int = 1,
-               variances: bool = False,
-               binedges: bool = False,
-               labels: bool = False,
-               masks: bool = False,
-               attrs: bool = False,
-               ragged: bool = False,
-               dtype: str = 'float64',
-               unit: str = 'm/s',
-               dims: Optional[List[str]] = None,
-               dim_list: List[str] = default_dim_list) -> sc.DataArray:
+def data_array(
+    ndim: int = 1,
+    variances: bool = False,
+    binedges: bool = False,
+    labels: bool = False,
+    masks: bool = False,
+    attrs: bool = False,
+    ragged: bool = False,
+    dtype: str = 'float64',
+    unit: str = 'm/s',
+    dims: Optional[List[str]] = None,
+    dim_list: List[str] = default_dim_list,
+) -> sc.DataArray:
     """
     Generate a sample ``DataArray`` containing data based on a sine function, with
     coordinates. Optionally add masks, labels, attributes.
     It is also possible to turn the coordinates into bin-edges, or make a ragged (2d)
     coordinate.
 
     Parameters
@@ -91,54 +95,59 @@
         List of dimension labels. If ``None``, they will be auto-generated.
     dim_list:
         List of dimension labels to use if no ``dims`` are provided.
     """
 
     coord_units = dict(zip(dim_list, ['m', 'm', 'm', 's', 'K']))
 
-    data = variable(ndim=ndim,
-                    variances=variances,
-                    dims=dims,
-                    dtype=dtype,
-                    unit=unit,
-                    dim_list=dim_list)
+    data = variable(
+        ndim=ndim,
+        variances=variances,
+        dims=dims,
+        dtype=dtype,
+        unit=unit,
+        dim_list=dim_list,
+    )
 
     coord_dict = {
-        data.dims[i]: sc.arange(data.dims[i],
-                                data.shape[i] + binedges,
-                                unit=coord_units[data.dims[i]],
-                                dtype=np.float64)
+        data.dims[i]: sc.arange(
+            data.dims[i],
+            data.shape[i] + binedges,
+            unit=coord_units[data.dims[i]],
+            dtype=np.float64,
+        )
         for i in range(ndim)
     }
     attr_dict = {}
     mask_dict = {}
 
     if labels:
-        coord_dict["lab"] = sc.linspace(data.dims[0],
-                                        101.,
-                                        105.,
-                                        data.shape[0],
-                                        unit='s')
+        coord_dict["lab"] = sc.linspace(
+            data.dims[0], 101.0, 105.0, data.shape[0], unit='s'
+        )
     if attrs:
-        attr_dict["attr"] = sc.linspace(data.dims[0], 10., 77., data.shape[0], unit='s')
+        attr_dict["attr"] = sc.linspace(
+            data.dims[0], 10.0, 77.0, data.shape[0], unit='s'
+        )
     if masks:
-        mask_dict["mask"] = sc.array(dims=data.dims,
-                                     values=np.where(data.values > 0, True, False))
+        mask_dict["mask"] = sc.array(
+            dims=data.dims, values=np.where(data.values > 0, True, False)
+        )
 
     if ragged:
         grid = []
         for i, dim in enumerate(data.dims):
             if binedges and (i < ndim - 1):
                 grid.append(coord_dict[dim].values[:-1])
             else:
                 grid.append(coord_dict[dim].values)
         mesh = np.meshgrid(*grid, indexing="ij")
-        coord_dict[data.dims[-1]] = sc.array(dims=data.dims,
-                                             values=mesh[-1] +
-                                             np.indices(mesh[-1].shape)[0])
+        coord_dict[data.dims[-1]] = sc.array(
+            dims=data.dims, values=mesh[-1] + np.indices(mesh[-1].shape)[0]
+        )
     return sc.DataArray(data=data, coords=coord_dict, attrs=attr_dict, masks=mask_dict)
 
 
 def dataset(entries: List[str] = None, **kwargs) -> sc.Dataset:
     """
     Generate a sample ``Dataset``. See :func:`data_array` for more options.
 
@@ -170,21 +179,23 @@
     seed:
         The seed for the random number generator.
     """
     rng = np.random.default_rng(seed)
     position = scale * rng.standard_normal(size=[npoints, 3])
     values = np.linalg.norm(position, axis=1)
     vec = sc.vectors(dims=['row'], unit='m', values=position)
-    return sc.DataArray(data=sc.array(dims=['row'], values=values, unit='K'),
-                        coords={
-                            'position': vec,
-                            'x': vec.fields.x,
-                            'y': vec.fields.y,
-                            'z': vec.fields.z
-                        })
+    return sc.DataArray(
+        data=sc.array(dims=['row'], values=values, unit='K'),
+        coords={
+            'position': vec,
+            'x': vec.fields.x,
+            'y': vec.fields.y,
+            'z': vec.fields.z,
+        },
+    )
 
 
 def data1d(**kwargs):
     return data_array(ndim=1, **kwargs)
 
 
 def data2d(**kwargs):
```

### Comparing `plopp-23.3.0/src/plopp/functions/common.py` & `plopp-23.4.0/src/plopp/functions/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,115 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import warnings
-from typing import Dict, List, Optional, Union
+from collections.abc import Mapping
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import scipp as sc
 
 from .. import backends
-from ..core.utils import number_to_variable
+from ..core.utils import maybe_number_to_variable
 
 
 def require_interactive_backend(func: str):
     """
     Raise an error if the current backend in use is non-interactive.
     """
     if not backends.is_interactive():
-        raise RuntimeError(f"The {func} can only be used with an interactive backend "
-                           "backend. Use `%matplotlib widget` at the start of your "
-                           "notebook.")
+        raise RuntimeError(
+            f"The {func} can only be used with an interactive backend "
+            "backend. Use `%matplotlib widget` at the start of your "
+            "notebook."
+        )
+
+
+def from_compatible_lib(obj: Any) -> Any:
+    """
+    Convert from a compatible library, if possible.
+    """
+    if 'pandas' in str(type(obj)):
+        return sc.compat.from_pandas(obj)
+    if 'xarray' in str(type(obj)):
+        return sc.compat.from_xarray(obj)
+    return obj
 
 
 def _to_data_array(
-        obj: Union[list, np.ndarray, sc.Variable, sc.DataArray]) -> sc.DataArray:
+    obj: Union[list, np.ndarray, sc.Variable, sc.DataArray]
+) -> sc.DataArray:
     """
     Convert an input to a DataArray, potentially adding fake coordinates if they are
     missing.
     """
     out = obj
     if isinstance(out, list):
         out = np.array(out)
     if isinstance(out, np.ndarray):
         dims = [f"axis-{i}" for i in range(len(out.shape))]
         out = sc.Variable(dims=dims, values=out)
     if isinstance(out, sc.Variable):
         out = sc.DataArray(data=out)
+    out = from_compatible_lib(out)
     if not isinstance(out, sc.DataArray):
         raise ValueError(f"Cannot convert input of type {type(obj)} to a DataArray.")
     out = out.copy(deep=False)
     for dim, size in out.sizes.items():
         if dim not in out.meta:
             out.coords[dim] = sc.arange(dim, size, unit=None)
     return out
 
 
 def _to_variable_if_not_none(x: sc.Variable, unit: str) -> Union[None, sc.Variable]:
     """
     Convert input to the required unit if it is not ``None``.
     """
     if x is not None:
-        return number_to_variable(x, unit=unit)
+        return maybe_number_to_variable(x, unit=unit)
 
 
 def _check_size(da: sc.DataArray):
     """
     Prevent slow figure rendering by raising an error if the data array exceeds a
     default size.
     """
     limits = {1: 1_000_000, 2: 2500 * 2500}
     if da.ndim not in limits:
         raise ValueError("plot can only handle 1d and 2d data.")
     if np.prod(da.shape) > limits[da.ndim]:
-        raise ValueError(f"Plotting data of size {da.shape} may take very long or use "
-                         "an excessive amount of memory. This is therefore disabled by "
-                         "default. To bypass this check, use `ignore_size=True`.")
+        raise ValueError(
+            f"Plotting data of size {da.shape} may take very long or use "
+            "an excessive amount of memory. This is therefore disabled by "
+            "default. To bypass this check, use `ignore_size=True`."
+        )
 
 
 def check_not_binned(obj):
     if obj.bins is not None:
         params = ', '.join([f'{dim}=100' for dim in obj.dims])
         raise ValueError(
             "Cannot plot binned data, it must be histogrammed first, "
             f"e.g., using ``obj.hist()`` or obj.hist({params})``."
             "See https://scipp.github.io/generated/functions/scipp.hist.html for "
-            "more details.")
+            "more details."
+        )
 
 
 def _all_dims_sorted(var, order='ascending'):
     return all([sc.allsorted(var, dim, order=order) for dim in var.dims])
 
 
-def preprocess(obj: Union[np.ndarray, sc.Variable, sc.DataArray],
-               crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
-               name: str = '',
-               ignore_size: bool = False,
-               coords: Optional[List[str]] = None):
+def preprocess(
+    obj: Union[np.ndarray, sc.Variable, sc.DataArray],
+    crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
+    name: str = '',
+    ignore_size: bool = False,
+    coords: Optional[List[str]] = None,
+) -> sc.DataArray:
     """
     Pre-process input data for plotting.
     This involves:
 
       - converting the input to a data array
       - filling in missing dimension coords if needed
       - slicing out the parts that are not needed if cropping is requested
@@ -118,32 +139,52 @@
         # on the figure (this mostly arises in the case of a 2d image with no bin-edge
         # coord). Therefore, we convert the value-based range to slicing indices, and
         # then extend the lower and upper bounds by 1.
         smin = _to_variable_if_not_none(sl.get('min'), unit=out.meta[dim].unit)
         smax = _to_variable_if_not_none(sl.get('max'), unit=out.meta[dim].unit)
         start = max(out[dim, :smin].sizes[dim] - 1, 0)
         width = out[dim, smin:smax].sizes[dim]
-        out = out[dim, start:start + width + 2]
+        out = out[dim, start : start + width + 2]
     if not ignore_size:
         _check_size(out)
     if coords is not None:
         renamed_dims = {}
         if isinstance(coords, str):
             coords = [coords]
         for dim in coords:
             underlying = out.meta[dim].dims[-1]
             renamed_dims[underlying] = dim
         out = out.rename_dims(**renamed_dims)
     for name, coord in out.coords.items():
         if coord.ndim > 0:
             try:
-                if not (_all_dims_sorted(coord, order='ascending')
-                        or _all_dims_sorted(coord, order='descending')):
+                if not (
+                    _all_dims_sorted(coord, order='ascending')
+                    or _all_dims_sorted(coord, order='descending')
+                ):
                     warnings.warn(
                         'The input contains a coordinate with unsorted values '
                         f'({name}). The results may be unpredictable. '
                         'Coordinates can be sorted using '
                         '`scipp.sort(data, dim="to_be_sorted", order="ascending")`.',
-                        UserWarning)
+                        UserWarning,
+                    )
             except sc.DTypeError:
                 pass
     return out
+
+
+def preprocess_multi(obj, **kwargs) -> List[sc.DataArray]:
+    """
+    Pre-process potentially multiple input data for plotting.
+    See :func:`preprocess` for details.
+
+    Parameters
+    ----------
+    obj:
+        The input objects that will be converted to data arrays.
+    """
+    to_preprocess = from_compatible_lib(obj)
+    if isinstance(to_preprocess, (Mapping, sc.Dataset)):
+        return [preprocess(item, name=name, **kwargs) for name, item in obj.items()]
+    else:
+        return [preprocess(obj, **kwargs)]
```

### Comparing `plopp-23.3.0/src/plopp/functions/inspector.py` & `plopp-23.4.0/src/plopp/functions/inspector.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,42 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from typing import Dict, Literal, Union
 
 import scipp as sc
 from numpy import ndarray
 
-from ..core import input_node, node
+from ..core import Node
 from ..core.utils import coord_as_bin_edges
 from ..graphics import figure1d, figure2d
 from .common import preprocess, require_interactive_backend
 
 
-def slice_xy(da, xy):
+def _slice_xy(da, xy):
     x = xy['x']
     y = xy['y']
     return da[y['dim'], y['value']][x['dim'], x['value']]
 
 
-def inspector(obj: Union[ndarray, sc.Variable, sc.DataArray],
-              dim: str = None,
-              *,
-              operation: Literal['sum', 'mean', 'min', 'max'] = 'sum',
-              orientation: Literal['horizontal', 'vertical'] = 'horizontal',
-              crop: Dict[str, Dict[str, sc.Variable]] = None,
-              **kwargs):
+def _apply_op(da, op, dim):
+    out = getattr(sc, op)(da, dim=dim)
+    if out.name:
+        out.name = f'{op} of {out.name}'
+    return out
+
+
+def inspector(
+    obj: Union[ndarray, sc.Variable, sc.DataArray],
+    dim: str = None,
+    *,
+    operation: Literal['sum', 'mean', 'min', 'max'] = 'sum',
+    orientation: Literal['horizontal', 'vertical'] = 'horizontal',
+    crop: Dict[str, Dict[str, sc.Variable]] = None,
+    **kwargs,
+):
     """
     Inspector takes in a three-dimensional input and applies a reduction operation
     (``'sum'`` by default) along one of the dimensions specified by ``dim``.
     It displays the result as a two-dimensional image.
     In addition, an 'inspection' tool is available in the toolbar which allows to place
     markers on the image which perform slicing at that position to retain only the third
     dimension and displays the resulting one-dimensional slice on the right hand side
@@ -64,31 +73,34 @@
 
     Returns
     -------
     :
         A :class:`Box` which will contain two :class:`Figure` and one slider widget.
     """
     if obj.ndim != 3:
-        raise ValueError('The inspector plot currently only work with '
-                         f'three-dimensional data, found {obj.ndim} dims.')
+        raise ValueError(
+            'The inspector plot currently only work with '
+            f'three-dimensional data, found {obj.ndim} dims.'
+        )
     require_interactive_backend('inspector')
 
     da = preprocess(obj, crop=crop, ignore_size=True)
-    in_node = input_node(da)
+    in_node = Node(da)
     if dim is None:
         dim = da.dims[-1]
 
     # Convert dimension coords to bin edges
     for d in set(da.dims) - {dim}:
         da.coords[d] = coord_as_bin_edges(da, d)
 
-    op_node = node(getattr(sc, operation), dim=dim)(in_node)
+    op_node = Node(_apply_op, da=in_node, op=operation, dim=dim)
     f2d = figure2d(op_node, **{**{'crop': crop}, **kwargs})
     f1d = figure1d()
 
     from ..widgets import Box, PointsTool
-    pts = PointsTool(figure=f2d, input_node=in_node, func=slice_xy, destination=f1d)
+
+    pts = PointsTool(figure=f2d, input_node=in_node, func=_slice_xy, destination=f1d)
     f2d.toolbar['inspect'] = pts
     out = [f2d, f1d]
     if orientation == 'horizontal':
         out = [out]
     return Box(out)
```

### Comparing `plopp-23.3.0/src/plopp/functions/plot.py` & `plopp-23.4.0/src/plopp/functions/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from collections.abc import Mapping
 from typing import Dict, List, Literal, Optional, Tuple, Union
 
 from numpy import ndarray
-from scipp import Dataset, Variable
+from scipp import Variable
 from scipp.typing import VariableLike
 
-from ..core import input_node
+from ..core import Node
 from ..graphics import figure1d, figure2d
-from .common import preprocess
+from .common import preprocess_multi
 
 
-def plot(obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
-         *,
-         aspect: Literal['auto', 'equal'] = 'auto',
-         cbar: bool = True,
-         coords: Optional[List[str]] = None,
-         crop: Optional[Dict[str, Dict[str, Variable]]] = None,
-         errorbars: bool = True,
-         figsize: Tuple[float, float] = None,
-         grid: bool = False,
-         ignore_size: bool = False,
-         mask_color: str = 'black',
-         norm: Literal['linear', 'log'] = 'linear',
-         scale: Optional[Dict[str, str]] = None,
-         title: Optional[str] = None,
-         vmin: Optional[Union[Variable, int, float]] = None,
-         vmax: Optional[Union[Variable, int, float]] = None,
-         **kwargs):
+def plot(
+    obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
+    *,
+    aspect: Literal['auto', 'equal'] = 'auto',
+    cbar: bool = True,
+    coords: Optional[List[str]] = None,
+    crop: Optional[Dict[str, Dict[str, Variable]]] = None,
+    errorbars: bool = True,
+    figsize: Tuple[float, float] = None,
+    grid: bool = False,
+    ignore_size: bool = False,
+    mask_color: str = 'black',
+    norm: Literal['linear', 'log'] = 'linear',
+    scale: Optional[Dict[str, str]] = None,
+    title: Optional[str] = None,
+    vmin: Optional[Union[Variable, int, float]] = None,
+    vmax: Optional[Union[Variable, int, float]] = None,
+    **kwargs,
+):
     """Plot a Scipp object.
 
     Parameters
     ----------
     obj:
         The object to be plotted.
     aspect:
@@ -91,50 +92,50 @@
         'grid': grid,
         'norm': norm,
         'scale': scale,
         'title': title,
         'vmin': vmin,
         'vmax': vmax,
         'figsize': figsize,
-        **kwargs
+        **kwargs,
     }
 
-    if isinstance(obj, (Mapping, Dataset)):
-        data_arrays = [
-            preprocess(item,
-                       crop=crop,
-                       name=name,
-                       ignore_size=ignore_size,
-                       coords=coords) for name, item in obj.items()
-        ]
-    else:
-        data_arrays = [
-            preprocess(obj, crop=crop, ignore_size=ignore_size, coords=coords)
-        ]
+    data_arrays = preprocess_multi(
+        obj, crop=crop, ignore_size=ignore_size, coords=coords
+    )
 
     ndims = set()
     for da in data_arrays:
         ndims.add(da.ndim)
     if len(ndims) > 1:
-        raise ValueError('All items given to the plot function must have the same '
-                         f'number of dimensions. Found dimensions {ndims}.')
+        raise ValueError(
+            'All items given to the plot function must have the same '
+            f'number of dimensions. Found dimensions {ndims}.'
+        )
     ndim = ndims.pop()
     if ndim == 1:
-        return figure1d(*[input_node(da) for da in data_arrays],
-                        errorbars=errorbars,
-                        mask_color=mask_color,
-                        **common_args)
+        return figure1d(
+            *[Node(da) for da in data_arrays],
+            errorbars=errorbars,
+            mask_color=mask_color,
+            **common_args,
+        )
     elif ndim == 2:
         if len(data_arrays) > 1:
             raise ValueError(
                 'The plot function can only plot a single 2d data entry. If you want '
                 'to create multiple figures, see the documentation on subplots at '
                 'https://scipp.github.io/plopp/customization/subplots.html. If you '
                 'want to plot two images onto the same axes, use the lower-level '
-                'plopp.figure2d function.')
-        return figure2d(*[input_node(da) for da in data_arrays],
-                        aspect=aspect,
-                        cbar=cbar,
-                        **common_args)
+                'plopp.figure2d function.'
+            )
+        return figure2d(
+            *[Node(da) for da in data_arrays],
+            aspect=aspect,
+            cbar=cbar,
+            **common_args,
+        )
     else:
-        raise ValueError('The plot function can only plot 1d and 2d data, got input '
-                         f'with {ndim} dimensions')
+        raise ValueError(
+            'The plot function can only plot 1d and 2d data, got input '
+            f'with {ndim} dimensions'
+        )
```

### Comparing `plopp-23.3.0/src/plopp/functions/scatter3d.py` & `plopp-23.4.0/src/plopp/functions/scatter3d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Literal, Tuple, Union
+from typing import Literal, Optional, Tuple, Union
 
 import scipp as sc
 
-from ..core import input_node
-from .common import check_not_binned
-
-
-def scatter3d(da: sc.DataArray,
-              *,
-              x: str = None,
-              y: str = None,
-              z: str = None,
-              pos: str = None,
-              figsize: Tuple[int, int] = (600, 400),
-              norm: Literal['linear', 'log'] = 'linear',
-              title: str = None,
-              vmin: Union[sc.Variable, int, float] = None,
-              vmax: Union[sc.Variable, int, float] = None,
-              cmap: str = 'viridis',
-              **kwargs):
+from ..core import Node
+from ..graphics import Camera
+from .common import check_not_binned, from_compatible_lib
+
+
+def scatter3d(
+    obj: sc.DataArray,
+    *,
+    x: str = None,
+    y: str = None,
+    z: str = None,
+    pos: str = None,
+    figsize: Tuple[int, int] = (600, 400),
+    norm: Literal['linear', 'log'] = 'linear',
+    title: str = None,
+    vmin: Union[sc.Variable, int, float] = None,
+    vmax: Union[sc.Variable, int, float] = None,
+    cmap: str = 'viridis',
+    camera: Optional[Camera] = None,
+    **kwargs,
+):
     """Make a three-dimensional scatter plot.
 
     To specify the positions of the scatter points, you can use:
 
     - a single coordinate inside the supplied data array that has dtype ``vector3``
       (use the ``pos`` parameter to specify the name of the coordinate).
     - three coordinates from the data array, whose names are specified using the
       ``x``, ``y``, and ``z`` arguments.
 
     Note that if ``pos`` is used, ``x``, ``y``, and ``z`` must all be ``None``.
 
     Parameters
     ----------
-    da:
+    obj:
         The data array containing the data and the coordinates.
     x:
         The name of the coordinate that is to be used for the X positions.
         Default is 'x'.
     y:
         The name of the coordinate that is to be used for the Y positions.
         Default is 'y'.
@@ -57,14 +61,16 @@
         The figure title.
     vmin:
         Lower bound for the colorscale.
     vmax:
         Upper bound for the colorscale.
     cmap:
         The name of the colormap.
+    camera:
+        Initial camera configuration (position, target).
 
     Returns
     -------
     :
         A three-dimensional interactive scatter plot.
     """
     from ..graphics import figure3d
@@ -73,43 +79,51 @@
     if 'ax' in kwargs:
         raise ValueError(
             'Keyword "ax" detected. Embedding 3D scatter plots inside Matplotlib axes '
             'is not supported. See '
             'https://scipp.github.io/plopp/customization/subplots.html#FAQ:-subplots-with-3D-scatter-plots'  # noqa: E501
         )
 
+    da = from_compatible_lib(obj)
     check_not_binned(da)
 
     if pos is not None:
         if any((x, y, z)):
-            raise ValueError(f'If pos ({pos}) is defined, all of '
-                             f'x ({x}), y ({y}), and z ({z}) must be None.')
+            raise ValueError(
+                f'If pos ({pos}) is defined, all of '
+                f'x ({x}), y ({y}), and z ({z}) must be None.'
+            )
         coords = {
             (x := f'{pos}.x'): da.meta[pos].fields.x,
             (y := f'{pos}.y'): da.meta[pos].fields.y,
-            (z := f'{pos}.z'): da.meta[pos].fields.z
+            (z := f'{pos}.z'): da.meta[pos].fields.z,
         }
     else:
         x = x if x is not None else 'x'
         y = y if y is not None else 'y'
         z = z if z is not None else 'z'
         coords = {k: da.meta[k] for k in (x, y, z)}
 
     to_plot = sc.DataArray(data=da.data, masks=da.masks, coords=coords)
     if to_plot.ndim != 1:
         to_plot = to_plot.flatten(to=uuid.uuid4().hex)
-    fig = figure3d(input_node(to_plot),
-                   x=x,
-                   y=y,
-                   z=z,
-                   figsize=figsize,
-                   norm=norm,
-                   title=title,
-                   vmin=vmin,
-                   vmax=vmax,
-                   cmap=cmap,
-                   **kwargs)
+    fig = figure3d(
+        Node(to_plot),
+        x=x,
+        y=y,
+        z=z,
+        figsize=figsize,
+        norm=norm,
+        title=title,
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        camera=camera,
+        **kwargs,
+    )
     tri_cutter = TriCutTool(fig)
-    fig.toolbar['cut3d'] = ToggleTool(callback=tri_cutter.toggle_visibility,
-                                      icon='cube',
-                                      tooltip='Hide/show spatial cutting tool')
+    fig.toolbar['cut3d'] = ToggleTool(
+        callback=tri_cutter.toggle_visibility,
+        icon='cube',
+        tooltip='Hide/show spatial cutting tool',
+    )
     return Box([fig, tri_cutter])
```

### Comparing `plopp-23.3.0/src/plopp/functions/slicer.py` & `plopp-23.4.0/src/plopp/functions/slicer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from typing import Dict, List, Union
 
 import scipp as sc
 from numpy import ndarray
 from scipp.typing import VariableLike
 
-from ..core import input_node, widget_node
+from ..core import Node, widget_node
 from ..graphics import figure1d, figure2d
-from .common import preprocess, require_interactive_backend
+from .common import preprocess_multi, require_interactive_backend
 
 
 class Slicer:
     """
     Class that slices out dimensions from the data and displays the resulting data as
     either a 1D line or a 2D image.
 
@@ -37,68 +37,63 @@
     crop:
         Set the axis limits. Limits should be given as a dict with one entry per
         dimension to be cropped.
     **kwargs:
         The additional arguments are forwarded to the underlying 1D or 2D figures.
     """
 
-    def __init__(self,
-                 obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike,
-                                                                   ndarray]]],
-                 keep: List[str] = None,
-                 *,
-                 crop: Dict[str, Dict[str, sc.Variable]] = None,
-                 **kwargs):
-
-        if isinstance(obj, (dict, sc.Dataset)):
-            ds = sc.Dataset({
-                key: preprocess(da, crop=crop, ignore_size=True)
-                for key, da in obj.items()
-            })
-        else:
-            da = preprocess(obj, crop=crop, ignore_size=True)
-            ds = sc.Dataset({da.name: da})
+    def __init__(
+        self,
+        obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
+        keep: List[str] = None,
+        *,
+        crop: Dict[str, Dict[str, sc.Variable]] = None,
+        **kwargs,
+    ):
+        data_arrays = preprocess_multi(obj, crop=crop, ignore_size=True)
+        ds = sc.Dataset({da.name: da for da in data_arrays})
 
         if keep is None:
-            keep = ds.dims[-(2 if ds.ndim > 2 else 1):]
+            keep = ds.dims[-(2 if ds.ndim > 2 else 1) :]
 
         if isinstance(keep, str):
             keep = [keep]
 
         if len(keep) == 0:
             raise ValueError(
-                'Slicer plot: the list of dims to be kept cannot be empty.')
+                'Slicer plot: the list of dims to be kept cannot be empty.'
+            )
         if not all(dim in ds.dims for dim in keep):
             raise ValueError(
                 f"Slicer plot: one or more of the requested dims to be kept {keep} "
-                f"were not found in the input's dimensions {ds.dims}.")
+                f"were not found in the input's dimensions {ds.dims}."
+            )
 
         from ..widgets import SliceWidget, slice_dims
 
-        self.data_nodes = [input_node(da) for da in ds.values()]
+        self.data_nodes = [Node(da) for da in ds.values()]
 
-        self.slider = SliceWidget(
-            sizes={dim: size
-                   for dim, size in ds.sizes.items() if dim not in keep},
-            coords=ds.meta)
+        self.slider = SliceWidget(ds, dims=[dim for dim in ds.dims if dim not in keep])
         self.slider_node = widget_node(self.slider)
         self.slice_nodes = [
             slice_dims(data_node, self.slider_node) for data_node in self.data_nodes
         ]
         if len(keep) == 1:
             self.figure = figure1d(*self.slice_nodes, crop=crop, **kwargs)
         elif len(keep) == 2:
             self.figure = figure2d(*self.slice_nodes, crop=crop, **kwargs)
 
 
-def slicer(obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
-           keep: List[str] = None,
-           *,
-           crop: Dict[str, Dict[str, sc.Variable]] = None,
-           **kwargs):
+def slicer(
+    obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
+    keep: List[str] = None,
+    *,
+    crop: Dict[str, Dict[str, sc.Variable]] = None,
+    **kwargs,
+):
     """
     Plot a multi-dimensional object by slicing one or more of the dimensions.
     This will produce one slider per sliced dimension, below the figure.
 
     Parameters
     ----------
     obj:
@@ -120,8 +115,9 @@
     -------
     :
         A :class:`Box` which will contain a :class:`Figure` and slider widgets.
     """
     require_interactive_backend('slicer')
     sl = Slicer(obj=obj, keep=keep, crop=crop, **kwargs)
     from ..widgets import Box
+
     return Box([sl.figure, sl.slider])
```

### Comparing `plopp-23.3.0/src/plopp/functions/superplot.py` & `plopp-23.4.0/src/plopp/functions/superplot.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,40 +26,45 @@
         The node that generates the input data.
     """
 
     def __init__(self, data_node: Node, slider_node: Node, fig: View):
         import ipywidgets as ipw
 
         from ..widgets.box import VBar
+
         self._data_node = data_node
         self._slider_node = slider_node
         self._fig = fig
         self._lines = {}
         self.button = ipw.Button(description='Save line')
         self.button.on_click(self.save_line)
         self.container = VBar()
         self.widget = VBar([self.button, self.container], layout={'width': '350px'})
 
     def _update_container(self):
         self.container.children = [line['tool'] for line in self._lines.values()]
 
     def save_line(self, change: Dict[str, Any] = None):
         from ..widgets import ColorTool
+
         line_id = uuid.uuid4().hex
         data = self._data_node.request_data()
         self._fig.update(data, key=line_id)
         slice_values = self._slider_node.request_data()
-        text = ', '.join(f'{k}: {coord_element_to_string(data.meta[k])}'
-                         for k, it in slice_values.items())
+        text = ', '.join(
+            f'{k}: {coord_element_to_string(data.meta[k])}'
+            for k, it in slice_values.items()
+        )
         line = self._fig.artists[line_id]
         tool = ColorTool(text=text, color=to_hex(line.color))
         self._lines[line_id] = {'line': line, 'tool': tool}
         self._update_container()
-        tool.color.observe(partial(self.change_line_color, line_id=line_id),
-                           names='value')
+        tool.color.observe(
+            partial(self.change_line_color, line_id=line_id), names='value'
+        )
         tool.button.on_click(partial(self.remove_line, line_id=line_id))
 
     def change_line_color(self, change: Dict[str, Any], line_id: str):
         self._lines[line_id]['line'].color = change['new']
 
     def remove_line(self, change: Dict[str, Any], line_id: str):
         self._lines[line_id]['line'].remove()
@@ -94,39 +99,46 @@
         dimension to be cropped. Each entry should be a nested dict containing scalar
         values for `'min'` and/or `'max'`. Example:
         `da.plot(crop={'time': {'min': 2 * sc.Unit('s'), 'max': 40 * sc.Unit('s')}})`
     **kwargs:
         See :py:func:`plopp.plot` for the full list of line customization arguments.
     """
 
-    def __init__(self,
-                 obj: Union[sc.typing.VariableLike, ndarray],
-                 keep: Optional[str] = None,
-                 *,
-                 crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
-                 **kwargs):
+    def __init__(
+        self,
+        obj: Union[sc.typing.VariableLike, ndarray],
+        keep: Optional[str] = None,
+        *,
+        crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
+        **kwargs,
+    ):
         da = preprocess(obj, crop=crop, ignore_size=True)
         if keep is None:
             keep = da.dims[-1]
         if isinstance(keep, (list, tuple)):
             raise TypeError(
-                "The keep argument must be a single string, not a list or tuple.")
+                "The keep argument must be a single string, not a list or tuple."
+            )
         self.slicer = Slicer(da, keep=[keep], crop=crop, **kwargs)
-        self.linesavetool = LineSaveTool(data_node=self.slicer.slice_nodes[0],
-                                         slider_node=self.slicer.slider_node,
-                                         fig=self.slicer.figure)
+        self.linesavetool = LineSaveTool(
+            data_node=self.slicer.slice_nodes[0],
+            slider_node=self.slicer.slider_node,
+            fig=self.slicer.figure,
+        )
         self.figure = self.slicer.figure
         self.slider = self.slicer.slider
 
 
-def superplot(obj: Union[sc.typing.VariableLike, ndarray],
-              keep: Optional[str] = None,
-              *,
-              crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
-              **kwargs):
+def superplot(
+    obj: Union[sc.typing.VariableLike, ndarray],
+    keep: Optional[str] = None,
+    *,
+    crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
+    **kwargs,
+):
     """
     Plot a multi-dimensional object as a one-dimensional line, slicing all but one
     dimension. This will produce one slider per sliced dimension, below the figure.
     In addition, a tool for saving the currently displayed line is added on the right
     hand side of the figure.
 
     Parameters
@@ -150,8 +162,9 @@
     :
         A :class:`widgets.Box` which will contain a :class:`graphics.FigLine`, slider
         widgets and a tool to save/delete lines.
     """
     require_interactive_backend('superplot')
     sp = Superplot(obj=obj, keep=keep, crop=crop, **kwargs)
     from ..widgets import Box
+
     return Box([[sp.figure, sp.linesavetool.widget], sp.slider])
```

### Comparing `plopp-23.3.0/src/plopp/graphics/basefig.py` & `plopp-23.4.0/src/plopp/graphics/basefig.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/src/plopp/graphics/colormapper.py` & `plopp-23.4.0/src/plopp/graphics/colormapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,25 +83,26 @@
         supplied, it is assumed that the unit is the same as the data unit.
     nan_color:
         The color used for representing NAN values.
     figsize:
         The size of the figure next to which the colorbar will be displayed.
     """
 
-    def __init__(self,
-                 canvas: Optional[Any] = None,
-                 cbar: bool = True,
-                 cmap: str = 'viridis',
-                 mask_cmap: str = 'gray',
-                 norm: Literal['linear', 'log'] = 'linear',
-                 vmin: Optional[Union[sc.Variable, int, float]] = None,
-                 vmax: Optional[Union[sc.Variable, int, float]] = None,
-                 nan_color: Optional[str] = None,
-                 figsize: Optional[Tuple[float, float]] = None):
-
+    def __init__(
+        self,
+        canvas: Optional[Any] = None,
+        cbar: bool = True,
+        cmap: str = 'viridis',
+        mask_cmap: str = 'gray',
+        norm: Literal['linear', 'log'] = 'linear',
+        vmin: Optional[Union[sc.Variable, int, float]] = None,
+        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        nan_color: Optional[str] = None,
+        figsize: Optional[Tuple[float, float]] = None,
+    ):
         self.cax = canvas.cax if canvas is not None else None
         self.cmap = _get_cmap(cmap, nan_color=nan_color)
         self.mask_cmap = _get_cmap(mask_cmap, nan_color=nan_color)
         self.user_vmin = vmin
         self.user_vmax = vmax
         self.vmin = np.inf
         self.vmax = np.NINF
@@ -134,14 +135,15 @@
         return self.artists[key]
 
     def to_widget(self):
         """
         Convert the colorbar into a widget for use with other ``ipywidgets``.
         """
         import ipywidgets as ipw
+
         self.widget = ipw.HTML()
         self._update_colorbar_widget()
         return self.widget
 
     def _update_colorbar_widget(self):
         """
         Upon an updated colorscale range, we need to update the image inside the widget.
@@ -225,16 +227,18 @@
             The data array to use to update the colorscale range.
         key:
             The id of the node that provided this data.
         """
         if self.unit is None:
             self.unit = data.unit
         elif data.unit != self.unit:
-            raise ValueError(f'Incompatible unit: colormapper has unit {self.unit}, '
-                             f'new data has unit {data.unit}.')
+            raise ValueError(
+                f'Incompatible unit: colormapper has unit {self.unit}, '
+                f'new data has unit {data.unit}.'
+            )
 
         if self.name is None:
             self.name = data.name
         elif data.name != self.name:
             self.name = ''
         if self.cax is not None:
             text = self.name
```

### Comparing `plopp-23.3.0/src/plopp/graphics/figimage.py` & `plopp-23.4.0/src/plopp/graphics/figimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,49 +62,49 @@
         Format of the figure displayed in the Jupyter notebook. If ``None``, a SVG is
         created as long as the number of markers in the figure is not too large. If too
         many markers are drawn, a PNG image is created instead.
     **kwargs:
         All other kwargs are forwarded to the Image artist.
     """
 
-    def __init__(self,
-                 *nodes,
-                 cmap: str = 'viridis',
-                 mask_cmap: str = 'gray',
-                 norm: Literal['linear', 'log'] = 'linear',
-                 vmin: Optional[Union[sc.Variable, int, float]] = None,
-                 vmax: Optional[Union[sc.Variable, int, float]] = None,
-                 scale: Optional[Dict[str, str]] = None,
-                 aspect: Literal['auto', 'equal'] = 'auto',
-                 grid: bool = False,
-                 crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
-                 cbar: bool = True,
-                 title: Optional[str] = None,
-                 figsize: Optional[Tuple[float, float]] = None,
-                 format: Optional[Literal['svg', 'png']] = None,
-                 **kwargs):
-
+    def __init__(
+        self,
+        *nodes,
+        cmap: str = 'viridis',
+        mask_cmap: str = 'gray',
+        norm: Literal['linear', 'log'] = 'linear',
+        vmin: Optional[Union[sc.Variable, int, float]] = None,
+        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        scale: Optional[Dict[str, str]] = None,
+        aspect: Literal['auto', 'equal'] = 'auto',
+        grid: bool = False,
+        crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
+        cbar: bool = True,
+        title: Optional[str] = None,
+        figsize: Optional[Tuple[float, float]] = None,
+        format: Optional[Literal['svg', 'png']] = None,
+        **kwargs
+    ):
         super().__init__(*nodes)
 
         self._scale = {} if scale is None else scale
         self._kwargs = kwargs
         self._repr_format = format
-        self.canvas = backends.canvas2d(cbar=cbar,
-                                        aspect=aspect,
-                                        grid=grid,
-                                        title=title,
-                                        figsize=figsize,
-                                        **kwargs)
-        self.colormapper = ColorMapper(cmap=cmap,
-                                       cbar=cbar,
-                                       mask_cmap=mask_cmap,
-                                       norm=norm,
-                                       vmin=vmin,
-                                       vmax=vmax,
-                                       canvas=self.canvas)
+        self.canvas = backends.canvas2d(
+            cbar=cbar, aspect=aspect, grid=grid, title=title, figsize=figsize, **kwargs
+        )
+        self.colormapper = ColorMapper(
+            cmap=cmap,
+            cbar=cbar,
+            mask_cmap=mask_cmap,
+            norm=norm,
+            vmin=vmin,
+            vmax=vmax,
+            canvas=self.canvas,
+        )
 
         self.render()
         self.canvas.autoscale()
         if crop is not None:
             self.crop(**crop)
         self.canvas.finalize()
 
@@ -128,27 +128,27 @@
         ycoord = new_values.coords[ydim]
         if not self.dims:
             self.dims.update({"x": xdim, "y": ydim})
             self.canvas.xunit = xcoord.unit
             self.canvas.yunit = ycoord.unit
             self.colormapper.unit = new_values.unit
         else:
-            new_values.data = make_compatible(new_values.data,
-                                              unit=self.colormapper.unit)
-            new_values.coords[xdim] = make_compatible(xcoord,
-                                                      dim=self.dims['x'],
-                                                      unit=self.canvas.xunit)
-            new_values.coords[ydim] = make_compatible(ycoord,
-                                                      dim=self.dims['y'],
-                                                      unit=self.canvas.yunit)
+            new_values.data = make_compatible(
+                new_values.data, unit=self.colormapper.unit
+            )
+            new_values.coords[xdim] = make_compatible(
+                xcoord, dim=self.dims['x'], unit=self.canvas.xunit
+            )
+            new_values.coords[ydim] = make_compatible(
+                ycoord, dim=self.dims['y'], unit=self.canvas.yunit
+            )
 
         self.colormapper.update(data=new_values, key=key)
 
         if key not in self.artists:
-
             image = backends.image(canvas=self.canvas, data=new_values, **self._kwargs)
             self.artists[key] = image
             self.colormapper[key] = image
             self.dims.update({"x": new_values.dims[1], "y": new_values.dims[0]})
 
             self.canvas.xunit = new_values.meta[new_values.dims[1]].unit
             self.canvas.yunit = new_values.meta[new_values.dims[0]].unit
```

### Comparing `plopp-23.3.0/src/plopp/graphics/figline.py` & `plopp-23.4.0/src/plopp/graphics/figline.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,45 +56,48 @@
     **kwargs:
         All other kwargs are forwarded to Matplotlib:
 
         - ``matplotlib.pyplot.plot`` for 1d data with a non bin-edge coordinate
         - ``matplotlib.pyplot.step`` for 1d data with a bin-edge coordinate
     """
 
-    def __init__(self,
-                 *nodes,
-                 norm: Literal['linear', 'log'] = 'linear',
-                 vmin: Optional[Union[sc.Variable, int, float]] = None,
-                 vmax: Optional[Union[sc.Variable, int, float]] = None,
-                 scale: Optional[Dict[str, str]] = None,
-                 errorbars: bool = True,
-                 mask_color: str = 'black',
-                 aspect: Literal['auto', 'equal'] = 'auto',
-                 grid: bool = False,
-                 crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
-                 title: Optional[str] = None,
-                 figsize: Tuple[float, float] = None,
-                 format: Optional[Literal['svg', 'png']] = None,
-                 **kwargs):
-
+    def __init__(
+        self,
+        *nodes,
+        norm: Literal['linear', 'log'] = 'linear',
+        vmin: Optional[Union[sc.Variable, int, float]] = None,
+        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        scale: Optional[Dict[str, str]] = None,
+        errorbars: bool = True,
+        mask_color: str = 'black',
+        aspect: Literal['auto', 'equal'] = 'auto',
+        grid: bool = False,
+        crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
+        title: Optional[str] = None,
+        figsize: Tuple[float, float] = None,
+        format: Optional[Literal['svg', 'png']] = None,
+        **kwargs
+    ):
         super().__init__(*nodes)
 
         self._scale = {} if scale is None else scale
         self._errorbars = errorbars
         self._mask_color = mask_color
         self._kwargs = kwargs
         self._repr_format = format
-        self.canvas = backends.canvas2d(cbar=False,
-                                        aspect=aspect,
-                                        grid=grid,
-                                        figsize=figsize,
-                                        title=title,
-                                        vmin=vmin,
-                                        vmax=vmax,
-                                        **kwargs)
+        self.canvas = backends.canvas2d(
+            cbar=False,
+            aspect=aspect,
+            grid=grid,
+            figsize=figsize,
+            title=title,
+            vmin=vmin,
+            vmax=vmax,
+            **kwargs
+        )
         self.canvas.yscale = norm
 
         self.render()
         self.canvas.autoscale()
         if crop is not None:
             self.crop(**crop)
         self.canvas.finalize()
@@ -117,26 +120,27 @@
         coord = new_values.coords[dim]
         if not self.dims:
             self.dims['x'] = dim
             self.canvas.xunit = coord.unit
             self.canvas.yunit = new_values.unit
         else:
             new_values.data = make_compatible(new_values.data, unit=self.canvas.yunit)
-            new_values.coords[dim] = make_compatible(coord,
-                                                     dim=self.dims['x'],
-                                                     unit=self.canvas.xunit)
+            new_values.coords[dim] = make_compatible(
+                coord, dim=self.dims['x'], unit=self.canvas.xunit
+            )
 
         if key not in self.artists:
-
-            line = backends.line(canvas=self.canvas,
-                                 data=new_values,
-                                 number=len(self.artists),
-                                 errorbars=self._errorbars,
-                                 mask_color=self._mask_color,
-                                 **self._kwargs)
+            line = backends.line(
+                canvas=self.canvas,
+                data=new_values,
+                number=len(self.artists),
+                errorbars=self._errorbars,
+                mask_color=self._mask_color,
+                **self._kwargs
+            )
             self.artists[key] = line
 
             self.canvas.xlabel = name_with_unit(var=new_values.meta[self.dims['x']])
             self.canvas.ylabel = name_with_unit(var=new_values.data, name="")
 
             if self.dims['x'] in self._scale:
                 self.canvas.xscale = self._scale[self.dims['x']]
```

### Comparing `plopp-23.3.0/src/plopp/graphics/figscatter3d.py` & `plopp-23.4.0/src/plopp/graphics/figscatter3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Literal, Tuple, Union
+from typing import Literal, Optional, Tuple, Union
 
 import scipp as sc
 
 from .. import backends
 from ..core.utils import make_compatible
+from ..graphics import Camera
 from .basefig import BaseFig
 from .colormapper import ColorMapper
 
 
 class FigScatter3d(BaseFig):
     """
     Figure that makes a visual representation of three-dimensional scatter data.
@@ -42,47 +43,53 @@
     vmax:
         Upper bound for the colorbar. If a number (without a unit) is supplied, it is
         assumed that the unit is the same as the data unit.
     title:
         The figure title.
     figsize:
         The width and height of the figure, in pixels.
+    camera:
+        Initial camera configuration (position, target).
     **kwargs:
         All other kwargs are forwarded to the PointCloud artist.
     """
 
-    def __init__(self,
-                 *nodes,
-                 x: str = 'x',
-                 y: str = 'y',
-                 z: str = 'z',
-                 cmap: str = 'viridis',
-                 mask_cmap: str = 'gray',
-                 norm: Literal['linear', 'log'] = 'linear',
-                 vmin: Union[sc.Variable, int, float] = None,
-                 vmax: Union[sc.Variable, int, float] = None,
-                 figsize: Tuple[int, int] = (600, 400),
-                 title: str = None,
-                 **kwargs):
-
+    def __init__(
+        self,
+        *nodes,
+        x: str = 'x',
+        y: str = 'y',
+        z: str = 'z',
+        cmap: str = 'viridis',
+        mask_cmap: str = 'gray',
+        norm: Literal['linear', 'log'] = 'linear',
+        vmin: Optional[Union[sc.Variable, int, float]] = None,
+        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        figsize: Tuple[int, int] = (600, 400),
+        title: Optional[str] = None,
+        camera: Optional[Camera] = None,
+        **kwargs
+    ):
         super().__init__(*nodes)
 
         self._x = x
         self._y = y
         self._z = z
         self._kwargs = kwargs
 
-        self.canvas = backends.canvas3d(figsize=figsize, title=title)
-        self.colormapper = ColorMapper(cmap=cmap,
-                                       mask_cmap=mask_cmap,
-                                       norm=norm,
-                                       vmin=vmin,
-                                       vmax=vmax,
-                                       nan_color="#f0f0f0",
-                                       figsize=self.canvas.figsize)
+        self.canvas = backends.canvas3d(figsize=figsize, title=title, camera=camera)
+        self.colormapper = ColorMapper(
+            cmap=cmap,
+            mask_cmap=mask_cmap,
+            norm=norm,
+            vmin=vmin,
+            vmax=vmax,
+            nan_color="#f0f0f0",
+            figsize=self.canvas.figsize,
+        )
 
         self._original_artists = [n.id for n in nodes]
         self.render()
 
     def update(self, new_values: sc.DataArray, key: str, draw=True):
         """
         Add new point cloud or update point cloud array with new values.
@@ -102,31 +109,33 @@
         if not self.dims:
             self.dims.update({'x': self._x, 'y': self._y, 'z': self._z})
             self.canvas.xunit = xcoord.unit
             self.canvas.yunit = ycoord.unit
             self.canvas.zunit = zcoord.unit
             self.colormapper.unit = new_values.unit
         else:
-            new_values.data = make_compatible(new_values.data,
-                                              unit=self.colormapper.unit)
+            new_values.data = make_compatible(
+                new_values.data, unit=self.colormapper.unit
+            )
             new_values.coords[self._x] = new_values.coords[self._x].to(
-                unit=self.canvas.xunit, copy=False)
+                unit=self.canvas.xunit, copy=False
+            )
             new_values.coords[self._y] = new_values.coords[self._y].to(
-                unit=self.canvas.yunit, copy=False)
+                unit=self.canvas.yunit, copy=False
+            )
             new_values.coords[self._z] = new_values.coords[self._z].to(
-                unit=self.canvas.zunit, copy=False)
+                unit=self.canvas.zunit, copy=False
+            )
 
         self.colormapper.update(data=new_values, key=key)
 
         if key not in self.artists:
-            pts = backends.point_cloud(data=new_values,
-                                       x=self._x,
-                                       y=self._y,
-                                       z=self._z,
-                                       **self._kwargs)
+            pts = backends.point_cloud(
+                data=new_values, x=self._x, y=self._y, z=self._z, **self._kwargs
+            )
             self.artists[key] = pts
             self.colormapper[key] = pts
             self.canvas.add(pts.points)
             if key in self._original_artists:
                 self.canvas.make_outline(limits=self.get_limits())
 
         self.artists[key].update(new_values=new_values)
@@ -152,17 +161,19 @@
                 ymin = ylims[0]
             if ymax is None or ylims[1] > ymax:
                 ymax = ylims[1]
             if zmin is None or zlims[0] < zmin:
                 zmin = zlims[0]
             if zmax is None or zlims[1] > zmax:
                 zmax = zlims[1]
-        return (sc.concat([xmin, xmax],
-                          dim=self._x), sc.concat([ymin, ymax], dim=self._y),
-                sc.concat([zmin, zmax], dim=self._z))
+        return (
+            sc.concat([xmin, xmax], dim=self._x),
+            sc.concat([ymin, ymax], dim=self._y),
+            sc.concat([zmin, zmax], dim=self._z),
+        )
 
     def set_opacity(self, alpha: float):
         """
         Update the opacity of the original children (not the cuts).
 
         Parameters
         ----------
```

### Comparing `plopp-23.3.0/src/plopp/graphics/figure.py` & `plopp-23.4.0/src/plopp/graphics/figure.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     style:
         The type of figure to create.
 
     Examples
     --------
     Create an input node and attach a figure1d as a view:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure1d(in_node)
 
     Visualize two data arrays on the same figure:
 
-      >>> a_node = pp.input_node(a)
-      >>> b_node = pp.input_node(b)
+      >>> a_node = pp.Node(a)
+      >>> b_node = pp.Node(b)
       >>> fig = pp.figure1d(a_node, b_node)
 
     With a customization argument to make the vertical scale logarithmic:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure1d(in_node, norm='log')
     """
 
     if style == 'line':
         from .figline import FigLine
 
         return backends.figure1d(*args, FigConstructor=FigLine, **kwargs)
@@ -55,20 +55,20 @@
     style:
         The type of figure to create.
 
     Examples
     --------
     Create an input node and attach a figure2d as a view:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure2d(in_node)
 
     With a customization argument to make the color scale logarithmic:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure2d(in_node, norm='log')
     """
 
     if style == 'image':
         from .figimage import FigImage
 
         return backends.figure2d(*args, FigConstructor=FigImage, **kwargs)
@@ -87,20 +87,20 @@
     style:
         The type of figure to create.
 
     Examples
     --------
     Create an input node and attach a figure3d as a view:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure3d(in_node)
 
     With a customization argument to make the color scale logarithmic:
 
-      >>> in_node = pp.input_node(da)
+      >>> in_node = pp.Node(da)
       >>> fig = pp.figure3d(in_node, norm='log')
     """
 
     if style == 'scatter':
         from .figscatter3d import FigScatter3d
 
         return backends.figure3d(*args, FigConstructor=FigScatter3d, **kwargs)
```

### Comparing `plopp-23.3.0/src/plopp/widgets/box.py` & `plopp-23.4.0/src/plopp/widgets/box.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/src/plopp/widgets/checkboxes.py` & `plopp-23.4.0/src/plopp/widgets/checkboxes.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,32 +23,37 @@
 
     def __init__(self, entries: List[str], description: str = "", value: bool = True):
         self.checkboxes = {}
         self._lock = False
         self.description = ipw.Label(value=description)
 
         for key in entries:
-            self.checkboxes[key] = ipw.Checkbox(value=value,
-                                                description=f"{escape(key)}",
-                                                indent=False,
-                                                layout={"width": "initial"})
+            self.checkboxes[key] = ipw.Checkbox(
+                value=value,
+                description=f"{escape(key)}",
+                indent=False,
+                layout={"width": "initial"},
+            )
 
         to_hbox = [
             self.description,
-            ipw.HBox(list(self.checkboxes.values()),
-                     layout=ipw.Layout(flex_flow='row wrap'))
+            ipw.HBox(
+                list(self.checkboxes.values()), layout=ipw.Layout(flex_flow='row wrap')
+            ),
         ]
 
         if len(self.checkboxes) > 1:
             # Add a master button to control all masks in one go
-            self.toggle_all_button = ipw.ToggleButton(value=value,
-                                                      description="Toggle all",
-                                                      disabled=False,
-                                                      button_style="",
-                                                      layout={"width": "initial"})
+            self.toggle_all_button = ipw.ToggleButton(
+                value=value,
+                description="Toggle all",
+                disabled=False,
+                button_style="",
+                layout={"width": "initial"},
+            )
             for cbox in self.checkboxes.values():
                 ipw.jsdlink((self.toggle_all_button, 'value'), (cbox, 'value'))
             to_hbox.insert(1, self.toggle_all_button)
 
         super().__init__(to_hbox)
 
     def _plopp_observe_(self, callback: Callable, **kwargs):
```

### Comparing `plopp-23.3.0/src/plopp/widgets/cut3d.py` & `plopp-23.4.0/src/plopp/widgets/cut3d.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,93 +88,101 @@
         Color of the cut's outline.
     linewidth:
         Width of the line delineating the outline.
     **kwargs:
         The kwargs are forwarded to the ToggleButton from ``ipywidgets``.
     """
 
-    def __init__(self,
-                 view: View,
-                 limits: Tuple[sc.Variable, sc.Variable, sc.Variable],
-                 direction: Literal['x', 'y', 'z'],
-                 value: bool = False,
-                 color: str = 'red',
-                 linewidth: float = 1.5,
-                 **kwargs):
-
+    def __init__(
+        self,
+        view: View,
+        limits: Tuple[sc.Variable, sc.Variable, sc.Variable],
+        direction: Literal['x', 'y', 'z'],
+        value: bool = False,
+        color: str = 'red',
+        linewidth: float = 1.5,
+        **kwargs,
+    ):
         import pythreejs as p3
+
         self._limits = limits
         self._direction = direction
         axis = 'xyz'.index(self._direction)
         self._dim = self._limits[axis].dim
         self._unit = self._limits[axis].unit
         self._view = view
 
         w_axis = 2 if self._direction == 'x' else 0
         h_axis = 2 if self._direction == 'y' else 1
         width = (self._limits[w_axis][1] - self._limits[w_axis][0]).value
         height = (self._limits[h_axis][1] - self._limits[h_axis][0]).value
 
         self.outline = p3.LineSegments(
-            geometry=p3.EdgesGeometry(p3.PlaneBufferGeometry(width=width,
-                                                             height=height)),
-            material=p3.LineBasicMaterial(color=color, linewidth=linewidth))
+            geometry=p3.EdgesGeometry(
+                p3.PlaneBufferGeometry(width=width, height=height)
+            ),
+            material=p3.LineBasicMaterial(color=color, linewidth=linewidth),
+        )
         if self._direction == 'x':
             self.outline.rotateY(0.5 * np.pi)
         if self._direction == 'y':
             self.outline.rotateX(0.5 * np.pi)
 
         center = [var.mean().value for var in self._limits]
         self.outline.position = center
         self.outline.visible = value
 
         self.thickness = 0.01
         self._thickness_step = self.thickness * 0.25
 
         self.button = ipw.ToggleButton(value=value, **kwargs)
-        self.slider = ipw.FloatSlider(min=limits[axis][0].value,
-                                      max=limits[axis][1].value,
-                                      value=center[axis],
-                                      layout={
-                                          'width': '150px',
-                                          'padding': '0px'
-                                      },
-                                      disabled=not value,
-                                      readout=False)
+        self.slider = ipw.FloatSlider(
+            min=limits[axis][0].value,
+            max=limits[axis][1].value,
+            value=center[axis],
+            layout={'width': '150px', 'padding': '0px'},
+            disabled=not value,
+            readout=False,
+        )
         self.slider.step = (self.slider.max - self.slider.min) * self.thickness * 0.5
-        self.readout = ipw.FloatText(layout={'width': '70px'},
-                                     step=self.slider.step,
-                                     disabled=not value)
+        self.readout = ipw.FloatText(
+            layout={'width': '70px'}, step=self.slider.step, disabled=not value
+        )
         self.unit_label = ipw.Label(f'[{self._unit}]')
         ipw.jslink((self.slider, "value"), (self.readout, "value"))
 
-        self.plus_minus = PlusMinusTool(plus={
-            'callback': self.increase_thickness,
-            'tooltip': 'Increase cut thickness',
-            'disabled': not value
-        },
-                                        minus={
-                                            'callback': self.decrease_thickness,
-                                            'tooltip': 'Decrease cut thickness',
-                                            'disabled': not value
-                                        })
+        self.plus_minus = PlusMinusTool(
+            plus={
+                'callback': self.increase_thickness,
+                'tooltip': 'Increase cut thickness',
+                'disabled': not value,
+            },
+            minus={
+                'callback': self.decrease_thickness,
+                'tooltip': 'Decrease cut thickness',
+                'disabled': not value,
+            },
+        )
 
         self.button.observe(self.toggle, names='value')
         self.slider.observe(self.move, names='value')
         self.slider.observe(self.update_cut, names='value')
 
         self._nodes = list(self._view.graph_nodes.values())
         self.select_nodes = {}
 
-        super().__init__([
-            ipw.VBox([self.button, self.plus_minus]),
-            ipw.VBox(
-                [self.slider, ipw.HBox([self.readout, self.unit_label])],
-                layout={'align_items': 'center'})
-        ])
+        super().__init__(
+            [
+                ipw.VBox([self.button, self.plus_minus]),
+                ipw.VBox(
+                    [self.slider, ipw.HBox([self.readout, self.unit_label])],
+                    layout={'align_items': 'center'},
+                ),
+            ]
+        )
 
     def toggle(self, change: Dict[str, Any]):
         """
         Toggle the tool on and off.
         """
         self.outline.visible = change['new']
         for widget in (self.slider, self.plus_minus, self.readout):
@@ -200,16 +208,17 @@
         """
 
         def select(da, s):
             return da[s]
 
         for n in self._nodes:
             da = n.request_data()
-            delta = sc.scalar((self.slider.max - self.slider.min) * self.thickness,
-                              unit=self._unit)
+            delta = sc.scalar(
+                (self.slider.max - self.slider.min) * self.thickness, unit=self._unit
+            )
             pos = sc.scalar(self.slider.value, unit=self._unit)
             selection = sc.abs(da.meta[self._dim] - pos) < delta
             if selection.sum().value > 0:
                 self.select_nodes[n.id] = node(partial(select, s=selection))(da=n)
                 self.select_nodes[n.id].add_view(self._view)
                 self._view.update(
                     self.select_nodes[n.id].request_data(),
@@ -267,60 +276,72 @@
     Parameters
     ----------
     fig:
         The 3d figure that contains the point clouds to be cut.
     """
 
     def __init__(self, fig: View):
-
         self._fig = fig
         limits = self._fig.get_limits()
-        self.cut_x = Cut3dTool(view=self._fig,
-                               direction='x',
-                               limits=limits,
-                               description='X',
-                               icon='cube',
-                               **BUTTON_LAYOUT)
-        self.cut_y = Cut3dTool(view=self._fig,
-                               direction='y',
-                               limits=limits,
-                               description='Y',
-                               icon='cube',
-                               **BUTTON_LAYOUT)
-        self.cut_z = Cut3dTool(view=self._fig,
-                               direction='z',
-                               limits=limits,
-                               description='Z',
-                               icon='cube',
-                               **BUTTON_LAYOUT)
+        self.cut_x = Cut3dTool(
+            view=self._fig,
+            direction='x',
+            limits=limits,
+            description='X',
+            icon='cube',
+            **BUTTON_LAYOUT,
+        )
+        self.cut_y = Cut3dTool(
+            view=self._fig,
+            direction='y',
+            limits=limits,
+            description='Y',
+            icon='cube',
+            **BUTTON_LAYOUT,
+        )
+        self.cut_z = Cut3dTool(
+            view=self._fig,
+            direction='z',
+            limits=limits,
+            description='Z',
+            icon='cube',
+            **BUTTON_LAYOUT,
+        )
 
         self._fig.canvas.add(
-            [self.cut_x.outline, self.cut_y.outline, self.cut_z.outline])
+            [self.cut_x.outline, self.cut_y.outline, self.cut_z.outline]
+        )
 
-        self.opacity = ipw.BoundedFloatText(min=0,
-                                            max=0.5,
-                                            step=0.01,
-                                            disabled=True,
-                                            value=0.03,
-                                            style={'description_width': 'initial'},
-                                            layout={
-                                                'width': '50px',
-                                                'padding': '0px 0px 0px 0px'
-                                            })
+        self.opacity = ipw.BoundedFloatText(
+            min=0,
+            max=0.5,
+            step=0.01,
+            disabled=True,
+            value=0.03,
+            style={'description_width': 'initial'},
+            layout={'width': '50px', 'padding': '0px 0px 0px 0px'},
+        )
         self.opacity.observe(self._set_opacity, names='value')
 
         self.cut_x.button.observe(self._toggle_opacity, names='value')
         self.cut_y.button.observe(self._toggle_opacity, names='value')
         self.cut_z.button.observe(self._toggle_opacity, names='value')
 
         space = ipw.HBox([], layout={'width': '10px'})
-        super().__init__([
-            self.cut_x, space, self.cut_y, space, self.cut_z, space,
-            ipw.VBox([ipw.Label('Opacity:'), self.opacity])
-        ])
+        super().__init__(
+            [
+                self.cut_x,
+                space,
+                self.cut_y,
+                space,
+                self.cut_z,
+                space,
+                ipw.VBox([ipw.Label('Opacity:'), self.opacity]),
+            ]
+        )
         self.layout.display = 'none'
 
     def _toggle_opacity(self, _):
         """
         If any cut is active, set the opacity of the original children (not the cuts) to
         a low value. If all cuts are inactive, set the opacity back to 1.
         """
```

### Comparing `plopp-23.3.0/src/plopp/widgets/drawing.py` & `plopp-23.4.0/src/plopp/widgets/drawing.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from ..core import Node, View, node
 from .tools import ToggleTool
 
 
 def is_figure(x):
     from ..backends.matplotlib.interactive import InteractiveFig
+
     return isinstance(x, InteractiveFig)
 
 
 class DrawingTool(ToggleTool):
     """
     Interface between Plopp and Mpltoolbox.
 
@@ -39,24 +40,25 @@
         by the ``destination``.
     value:
         Activate the tool upon creation if ``True``.
     **kwargs:
         Additional arguments are forwarded to the ``ToggleTool`` constructor.
     """
 
-    def __init__(self,
-                 figure: View,
-                 input_node: Node,
-                 tool: Any,
-                 func: Callable,
-                 destination: Union[View, Node],
-                 get_artist_info: Callable,
-                 value: bool = False,
-                 **kwargs):
-
+    def __init__(
+        self,
+        figure: View,
+        input_node: Node,
+        tool: Any,
+        func: Callable,
+        destination: Union[View, Node],
+        get_artist_info: Callable,
+        value: bool = False,
+        **kwargs,
+    ):
         super().__init__(callback=self.start_stop, value=value, **kwargs)
 
         self._figure = figure
         self._destination_is_fig = is_figure(self._figure)
         self._input_node = input_node
         self._draw_nodes = {}
         self._output_nodes = {}
@@ -76,16 +78,17 @@
         artist.nodeid = nodeid
         output_node = node(self._func)(self._input_node, draw_node)
         output_node.name = f'Output node {len(self._output_nodes)}'
         self._output_nodes[nodeid] = output_node
         if self._destination_is_fig:
             output_node.add_view(self._destination._fig)
             self._destination.update(new_values=output_node(), key=output_node.id)
-            self._destination.artists[output_node.id].color = artist.color if hasattr(
-                artist, 'color') else artist.edgecolor
+            self._destination.artists[output_node.id].color = (
+                artist.color if hasattr(artist, 'color') else artist.edgecolor
+            )
         elif isinstance(self._destination, Node):
             self._destination.parents.append(output_node)
 
     def update_node(self, artist):
         n = self._draw_nodes[artist.nodeid]
         n.func = self._get_artist_info(artist=artist, figure=self._figure)
         n.notify_children(artist)
@@ -113,36 +116,39 @@
     """
     Convert the raw (x, y) position of a point to a dict containing the dimensions of
     each axis, and scalar values with units.
     """
     return lambda: {
         'x': {
             'dim': figure.dims['x'],
-            'value': sc.scalar(artist.x, unit=figure.canvas.xunit)
+            'value': sc.scalar(artist.x, unit=figure.canvas.xunit),
         },
         'y': {
             'dim': figure.dims['y'],
-            'value': sc.scalar(artist.y, unit=figure.canvas.yunit)
+            'value': sc.scalar(artist.y, unit=figure.canvas.yunit),
         },
     }
 
 
 def _make_points(**kwargs):
     """
     Intermediate function needed for giving to `partial` to avoid making mpltoolbox a
     hard dependency.
     """
     from mpltoolbox import Points
+
     return Points(**kwargs)
 
 
-PointsTool = partial(DrawingTool,
-                     tool=partial(_make_points, mec='w'),
-                     get_artist_info=_get_points_info,
-                     icon='crosshairs')
+PointsTool = partial(
+    DrawingTool,
+    tool=partial(_make_points, mec='w'),
+    get_artist_info=_get_points_info,
+    icon='crosshairs',
+)
 """
 Tool to add point markers onto a figure.
 
 Parameters
 ----------
 figure:
     The figure where the tool will draw things (points, lines, shapes...).
```

### Comparing `plopp-23.3.0/src/plopp/widgets/slice.py` & `plopp-23.4.0/src/plopp/widgets/slice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, List
 
 import ipywidgets as ipw
 import scipp as sc
 
 from ..core import node
 from ..core.utils import coord_element_to_string
 from .box import VBar
@@ -16,49 +16,58 @@
     Widgets containing a slider for each of the requested dimensions.
     The widget uses the input data array to determine the range each slider should have.
     Each slider also comes with a checkbox to toggle on and off the slider's continuous
     update.
 
     Parameters
     ----------
-    data_array:
+    da:
         The input data array.
     dims:
         The dimensions to make sliders for.
     """
 
-    def __init__(self, sizes: Dict[str, int], coords: Dict[str, sc.Variable]):
-
-        self._slider_dims = list(sizes.keys())
+    def __init__(self, da: sc.DataArray, dims: List[str]):
+        if isinstance(dims, str):
+            dims = [dims]
+        self._slider_dims = dims
         self.controls = {}
         self.view = None
         children = []
 
         for dim in self._slider_dims:
-            coord = coords[dim]
-            slider = ipw.IntSlider(step=1,
-                                   description=dim,
-                                   min=0,
-                                   max=sizes[dim] - 1,
-                                   continuous_update=True,
-                                   readout=False,
-                                   layout={"width": "200px"},
-                                   style={'description_width': 'initial'})
-            continuous_update = ipw.Checkbox(value=True,
-                                             tooltip="Continuous update",
-                                             indent=False,
-                                             layout={"width": "20px"})
+            coord = (
+                da.meta[dim]
+                if dim in da.meta
+                else sc.arange(dim, da.sizes[dim], unit=None)
+            )
+            slider = ipw.IntSlider(
+                step=1,
+                description=dim,
+                min=0,
+                max=da.sizes[dim] - 1,
+                continuous_update=True,
+                readout=False,
+                layout={"width": "200px"},
+                style={'description_width': 'initial'},
+            )
+            continuous_update = ipw.Checkbox(
+                value=True,
+                tooltip="Continuous update",
+                indent=False,
+                layout={"width": "20px"},
+            )
             label = ipw.Label(value=coord_element_to_string(coord[dim, 0]))
             ipw.jslink((continuous_update, 'value'), (slider, 'continuous_update'))
 
             self.controls[dim] = {
                 'continuous': continuous_update,
                 'slider': slider,
                 'label': label,
-                'coord': coord
+                'coord': coord,
             }
             slider.observe(self._update_label, names='value')
             children.append(ipw.HBox([continuous_update, slider, label]))
 
         super().__init__(children)
 
     def _update_label(self, change: Dict[str, Any]):
```

### Comparing `plopp-23.3.0/src/plopp/widgets/toolbar.py` & `plopp-23.4.0/src/plopp/widgets/toolbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         del self.tools[key]
         self._update_children()
 
     def _update_children(self):
         self.children = list(self.tools.values())
 
 
-def make_toolbar_canvas2d(canvas: Any,
-                          colormapper: Optional[ColorMapper] = None) -> Toolbar:
+def make_toolbar_canvas2d(
+    canvas: Any, colormapper: Optional[ColorMapper] = None
+) -> Toolbar:
     """
     Create a toolbar for a 2D canvas.
     If the colormapper is defined, add a button to toggle the norm of the colormapper.
 
     Parameters
     ----------
     canvas:
@@ -65,64 +66,61 @@
     tool_list = {
         'home': tools.HomeTool(canvas.autoscale),
         'panzoom': tools.PanZoomTool(canvas.panzoom),
         'logx': tools.LogxTool(canvas.logx, value=canvas.xscale == 'log'),
         'logy': tools.LogyTool(canvas.logy, value=canvas.yscale == 'log'),
     }
     if colormapper is not None:
-        tool_list['lognorm'] = tools.LogNormTool(colormapper.toggle_norm,
-                                                 value=colormapper.norm == 'log')
+        tool_list['lognorm'] = tools.LogNormTool(
+            colormapper.toggle_norm, value=colormapper.norm == 'log'
+        )
     tool_list['save'] = tools.SaveTool(canvas.download_figure)
     return Toolbar(tools=tool_list)
 
 
-def make_toolbar_canvas3d(canvas: Any,
-                          colormapper: Optional[ColorMapper] = None) -> Toolbar:
+def make_toolbar_canvas3d(
+    canvas: Any, colormapper: Optional[ColorMapper] = None
+) -> Toolbar:
     """
     Create a toolbar for a 3D canvas.
     If the colormapper is defined, add a button to toggle the norm of the colormapper.
 
     Parameters
     ----------
     canvas:
         The 3D canvas to operate on.
     colormapper:
         The colormapper which controls the colors of the artists in the canvas.
     """
     tool_list = {
-        'home':
-        tools.HomeTool(canvas.home),
-        'camerax':
-        tools.CameraTool(canvas.camera_x_normal,
-                         description='X',
-                         tooltip='Camera to X normal. '
-                         'Click twice to flip the view direction.'),
-        'cameray':
-        tools.CameraTool(canvas.camera_y_normal,
-                         description='Y',
-                         tooltip='Camera to Y normal. '
-                         'Click twice to flip the view direction.'),
-        'cameraz':
-        tools.CameraTool(canvas.camera_z_normal,
-                         description='Z',
-                         tooltip='Camera to Z normal. '
-                         'Click twice to flip the view direction.')
+        'home': tools.HomeTool(canvas.home),
+        'camerax': tools.CameraTool(
+            canvas.camera_x_normal,
+            description='X',
+            tooltip='Camera to X normal. ' 'Click twice to flip the view direction.',
+        ),
+        'cameray': tools.CameraTool(
+            canvas.camera_y_normal,
+            description='Y',
+            tooltip='Camera to Y normal. ' 'Click twice to flip the view direction.',
+        ),
+        'cameraz': tools.CameraTool(
+            canvas.camera_z_normal,
+            description='Z',
+            tooltip='Camera to Z normal. ' 'Click twice to flip the view direction.',
+        ),
     }
     if colormapper is not None:
-        tool_list['lognorm'] = tools.LogNormTool(colormapper.toggle_norm,
-                                                 value=colormapper.norm == 'log')
-    tool_list.update({
-        'box':
-        tools.OutlineTool(canvas.toggle_outline),
-        'axes':
-        tools.AxesTool(canvas.toggle_axes3d),
-        'size':
-        tools.PlusMinusTool(plus={
-            'callback': canvas.bigger,
-            'tooltip': 'Increase canvas size'
-        },
-                            minus={
-                                'callback': canvas.smaller,
-                                'tooltip': 'Decrease canvas size'
-                            })
-    })
+        tool_list['lognorm'] = tools.LogNormTool(
+            colormapper.toggle_norm, value=colormapper.norm == 'log'
+        )
+    tool_list.update(
+        {
+            'box': tools.OutlineTool(canvas.toggle_outline),
+            'axes': tools.AxesTool(canvas.toggle_axes3d),
+            'size': tools.PlusMinusTool(
+                plus={'callback': canvas.bigger, 'tooltip': 'Increase canvas size'},
+                minus={'callback': canvas.smaller, 'tooltip': 'Decrease canvas size'},
+            ),
+        }
+    )
     return Toolbar(tools=tool_list)
```

### Comparing `plopp-23.3.0/src/plopp/widgets/tools.py` & `plopp-23.4.0/src/plopp/widgets/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         self.observe(self, names='value')
 
     def __call__(self, *ignored):
         self.callback()
 
 
 class PlusMinusTool(ipw.HBox):
-
     def __init__(self, plus, minus):
         layout = {'width': '16px', 'padding': '0px'}
         self.callback = {'plus': plus.pop('callback'), 'minus': minus.pop('callback')}
         self._plus = ipw.Button(icon='plus', **{**{'layout': layout}, **plus})
         self._minus = ipw.Button(icon='minus', **{**{'layout': layout}, **minus})
         self._plus.on_click(self.plus)
         self._minus.on_click(self.minus)
@@ -101,36 +100,35 @@
     value:
         If given, the value of the button with the corresponding option will be set to
         True.
     **kwargs:
         All other kwargs are forwarded to ipywidgets.ToggleButton.
     """
 
-    def __init__(self,
-                 callback: Callable,
-                 options: List[str],
-                 icons: Optional[List[str]] = None,
-                 tooltips: List[str] = None,
-                 descriptions: List[str] = None,
-                 value: Optional[str] = None,
-                 **kwargs):
-
+    def __init__(
+        self,
+        callback: Callable,
+        options: List[str],
+        icons: Optional[List[str]] = None,
+        tooltips: List[str] = None,
+        descriptions: List[str] = None,
+        value: Optional[str] = None,
+        **kwargs
+    ):
         self.callback = callback
         self._options = options
         self._buttons = {}
         for i, key in enumerate(self._options):
             tb = ipw.ToggleButton(
                 icon=icons[i] if icons is not None else None,
                 tooltip=tooltips[i] if tooltips is not None else None,
                 description=descriptions[i] if descriptions is not None else '',
                 value=key == value,
-                **{
-                    **BUTTON_LAYOUT,
-                    **kwargs
-                })
+                **{**BUTTON_LAYOUT, **kwargs}
+            )
             tb._option = key
             tb.observe(self, names='value')
             self._buttons[key] = tb
         self._lock = False
         super().__init__(list(self._buttons.values()))
 
     def __call__(self, change: dict):
@@ -156,36 +154,37 @@
 
 LogxTool = partial(ToggleTool, description='logx', tooltip='Toggle X axis scale')
 """Toggle horizontal axis scale tool."""
 
 LogyTool = partial(ToggleTool, description='logy', tooltip='Toggle Y axis scale')
 """Toggle vertical axis scale tool."""
 
-LogNormTool = partial(ToggleTool,
-                      description='log',
-                      tooltip='Toggle colorscale normalization')
+LogNormTool = partial(
+    ToggleTool, description='log', tooltip='Toggle colorscale normalization'
+)
 """Toggle normalization scale tool."""
 
 SaveTool = partial(ButtonTool, icon='save', tooltip='Save figure')
 """Save figure to png tool."""
 
 CameraTool = partial(ButtonTool, icon='camera', tooltip='Autoscale view')
 """Tool for changing the position of the camera in a 3d scene."""
 
-OutlineTool = partial(ToggleTool,
-                      value=True,
-                      icon='codepen',
-                      tooltip='Toggle outline visibility')
+OutlineTool = partial(
+    ToggleTool, value=True, icon='codepen', tooltip='Toggle outline visibility'
+)
 """Toggle outline visibility tool"""
 
-AxesTool = partial(ToggleTool,
-                   value=True,
-                   description='\u27C0',
-                   style={'font_weight': 'bold'},
-                   tooltip='Toggle visibility of XYZ axes')
+AxesTool = partial(
+    ToggleTool,
+    value=True,
+    description='\u27C0',
+    style={'font_weight': 'bold'},
+    tooltip='Toggle visibility of XYZ axes',
+)
 """Toggle RGB axes helper visibility tool"""
 
 
 class PanZoomTool(MultiToggleTool):
     """
     Tool to control the panning and zooming actions on a Matplotlib figure.
 
@@ -195,20 +194,22 @@
         The canvas to act upon.
     value:
         Set the initially selected button. No button selected if ``None``.
     """
 
     def __init__(self, callback: Callable, value: bool = None, **kwargs):
         self._callback = callback
-        super().__init__(callback=self._panzoom,
-                         options=['pan', 'zoom'],
-                         icons=['arrows', 'search-plus'],
-                         tooltips=['Pan', 'Zoom'],
-                         value=value,
-                         **kwargs)
+        super().__init__(
+            callback=self._panzoom,
+            options=['pan', 'zoom'],
+            icons=['arrows', 'search-plus'],
+            tooltips=['Pan', 'Zoom'],
+            value=value,
+            **kwargs
+        )
 
     def _panzoom(self):
         self._callback(self.value)
 
 
 class ColorTool(ipw.HBox):
     """
@@ -222,13 +223,12 @@
     color:
         Initial color.
     """
 
     def __init__(self, text: str, color: str):
         layout = ipw.Layout(display="flex", justify_content="flex-end", width='150px')
         self.text = ipw.Label(value=text, layout=layout)
-        self.color = ipw.ColorPicker(concise=True,
-                                     value=color,
-                                     description='',
-                                     layout={'width': "30px"})
+        self.color = ipw.ColorPicker(
+            concise=True, value=color, description='', layout={'width': "30px"}
+        )
         self.button = ipw.Button(icon='times', **BUTTON_LAYOUT)
         super().__init__([self.text, self.color, self.button])
```

### Comparing `plopp-23.3.0/src/plopp.egg-info/PKG-INFO` & `plopp-23.4.0/src/plopp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.3.0
+Version: 23.4.0
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.3.0/src/plopp.egg-info/SOURCES.txt` & `plopp-23.4.0/src/plopp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 conda/meta.yaml
 docs/conf.py
 docs/index.rst
 docs/version.py
 docs/_static/favicon.ico
 docs/_static/logo.svg
 docs/_static/gallery/README.txt
+docs/_static/gallery/scatter3d-with-slider-thumbnail.png
 docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
 docs/_templates/scipp-class-template.rst
 docs/_templates/scipp-module-template.rst
 docs/_templates/sections/header-article.html
 docs/about/about.rst
 docs/about/faq.ipynb
 docs/about/reference.rst
@@ -36,15 +37,18 @@
 docs/customization/subplots.ipynb
 docs/customization/tweaking-figures.ipynb
 docs/examples/custom-interfaces.ipynb
 docs/examples/gallery.ipynb
 docs/examples/gallery/masking-a-range.ipynb
 docs/examples/gallery/nyc-taxi.ipynb
 docs/examples/gallery/rectangle-selection.ipynb
+docs/examples/gallery/scatter3d-with-slider.ipynb
 docs/examples/gallery/scatter3d-with-threshold.ipynb
+docs/getting-started/numpy-pandas-xarray.ipynb
+docs/getting-started/overview.ipynb
 requirements/base.in
 requirements/base.txt
 requirements/ci.in
 requirements/ci.txt
 requirements/docs.in
 requirements/docs.txt
 requirements/mini.in
@@ -80,16 +84,18 @@
 src/plopp/backends/pythreejs/__init__.py
 src/plopp/backends/pythreejs/canvas.py
 src/plopp/backends/pythreejs/figure.py
 src/plopp/backends/pythreejs/outline.py
 src/plopp/backends/pythreejs/point_cloud.py
 src/plopp/core/__init__.py
 src/plopp/core/graph.py
+src/plopp/core/helpers.py
 src/plopp/core/limits.py
-src/plopp/core/model.py
+src/plopp/core/node.py
+src/plopp/core/system.py
 src/plopp/core/utils.py
 src/plopp/core/view.py
 src/plopp/data/__init__.py
 src/plopp/data/examples.py
 src/plopp/data/factory.py
 src/plopp/data/testing.py
 src/plopp/functions/__init__.py
@@ -97,14 +103,15 @@
 src/plopp/functions/inspector.py
 src/plopp/functions/plot.py
 src/plopp/functions/scatter3d.py
 src/plopp/functions/slicer.py
 src/plopp/functions/superplot.py
 src/plopp/graphics/__init__.py
 src/plopp/graphics/basefig.py
+src/plopp/graphics/camera.py
 src/plopp/graphics/colormapper.py
 src/plopp/graphics/figimage.py
 src/plopp/graphics/figline.py
 src/plopp/graphics/figscatter3d.py
 src/plopp/graphics/figure.py
 src/plopp/widgets/__init__.py
 src/plopp/widgets/box.py
@@ -129,15 +136,15 @@
 tests/backends/plotly/plotly_figure_test.py
 tests/backends/plotly/plotly_line_test.py
 tests/backends/pythreejs/pythreejs_canvas_test.py
 tests/backends/pythreejs/pythreejs_figure_test.py
 tests/backends/pythreejs/pythreejs_point_cloud_test.py
 tests/core/graph_test.py
 tests/core/limits_test.py
-tests/core/model_test.py
+tests/core/node_test.py
 tests/core/utils_test.py
 tests/core/views.py
 tests/functions/common_test.py
 tests/functions/inspector_test.py
 tests/functions/plot_test.py
 tests/functions/scatter3d_test.py
 tests/functions/slicer_test.py
```

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_canvas_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_canvas_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,50 +46,56 @@
     canvas = Canvas()
     canvas.xunit = 'm'
     canvas.yunit = 'm'
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     ymin = sc.scalar(5.5, unit='m')
     ymax = sc.scalar(22.3, unit='m')
-    canvas.crop(x={
-        'min': xmin,
-        'max': xmax,
-    }, y={
-        'min': ymin,
-        'max': ymax,
-    })
+    canvas.crop(
+        x={
+            'min': xmin,
+            'max': xmax,
+        },
+        y={
+            'min': ymin,
+            'max': ymax,
+        },
+    )
     assert canvas.ax.get_xlim() == (xmin.value, xmax.value)
     assert canvas.ax.get_ylim() == (ymin.value, ymax.value)
 
 
 def test_crop_unit_conversion():
     canvas = Canvas()
     canvas.xunit = 'cm'
     canvas.yunit = 'cm'
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(3.3, unit='m')
     canvas.crop(x={'min': xmin, 'max': xmax})
-    assert canvas.ax.get_xlim() == (210., 330.)
+    assert canvas.ax.get_xlim() == (210.0, 330.0)
 
 
 def test_crop_no_variable():
     canvas = Canvas()
     canvas.xunit = 'm'
     canvas.yunit = 'm'
     xmin = 2.1
     xmax = 102.0
     ymin = 5.5
     ymax = 22.3
-    canvas.crop(x={
-        'min': xmin,
-        'max': xmax,
-    }, y={
-        'min': ymin,
-        'max': ymax,
-    })
+    canvas.crop(
+        x={
+            'min': xmin,
+            'max': xmax,
+        },
+        y={
+            'min': ymin,
+            'max': ymax,
+        },
+    )
     assert canvas.ax.get_xlim() == (xmin, xmax)
     assert canvas.ax.get_ylim() == (ymin, ymax)
 
 
 @pytest.mark.parametrize('ext', ['jpg', 'png', 'pdf', 'svg'])
 def test_save_to_disk(ext):
     canvas = Canvas()
```

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_figimage_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_figimage_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 
-from plopp import input_node
+from plopp import Node
 from plopp.data.testing import data_array
 from plopp.graphics.figimage import FigImage
 
 
 def test_cbar():
     da = data_array(ndim=2, binedges=True)
-    fig = FigImage(input_node(da), cbar=False)
+    fig = FigImage(Node(da), cbar=False)
     assert fig.canvas.cax is None
 
 
 def test_update_on_one_mesh_changes_colors_on_second_mesh():
     da1 = data_array(ndim=2)
     da2 = 3.0 * data_array(ndim=2)
     da2.coords['xx'] += sc.scalar(50.0, unit='m')
-    a = input_node(da1)
-    b = input_node(da2)
+    a = Node(da1)
+    b = Node(da2)
     f = FigImage(a, b)
     old_b_colors = f.artists[b.id]._mesh.get_facecolors()
     a.func = lambda: da1 * 1.1
     a.notify_children('updated a')
     # No change because the update did not change the colorbar limits
     assert np.allclose(old_b_colors, f.artists[b.id]._mesh.get_facecolors())
     a.func = lambda: da1 * 5.0
     a.notify_children('updated a')
     assert not np.allclose(old_b_colors, f.artists[b.id]._mesh.get_facecolors())
 
 
 def test_with_string_coord():
     strings = ['a', 'b', 'c', 'd', 'e']
-    da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
-                      coords={
-                          'x': sc.array(dims=['x'], values=strings, unit='s'),
-                          'y': sc.arange('y', 5., unit='m')
-                      })
-    fig = FigImage(input_node(da))
+    da = sc.DataArray(
+        data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
+        coords={
+            'x': sc.array(dims=['x'], values=strings, unit='s'),
+            'y': sc.arange('y', 5.0, unit='m'),
+        },
+    )
+    fig = FigImage(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_with_strings_as_bin_edges():
     strings = ['a', 'b', 'c', 'd', 'e', 'f']
-    da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
-                      coords={
-                          'x': sc.array(dims=['x'], values=strings, unit='s'),
-                          'y': sc.arange('y', 6., unit='m')
-                      })
-    fig = FigImage(input_node(da))
+    da = sc.DataArray(
+        data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
+        coords={
+            'x': sc.array(dims=['x'], values=strings, unit='s'),
+            'y': sc.arange('y', 6.0, unit='m'),
+        },
+    )
+    fig = FigImage(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_with_strings_as_bin_edges_other_coord_is_bin_centers():
     strings = ['a', 'b', 'c', 'd', 'e', 'f']
-    da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
-                      coords={
-                          'x': sc.array(dims=['x'], values=strings, unit='s'),
-                          'y': sc.arange('y', 5., unit='m')
-                      })
-    fig = FigImage(input_node(da))
+    da = sc.DataArray(
+        data=sc.array(dims=['y', 'x'], values=np.random.random((5, 5))),
+        coords={
+            'x': sc.array(dims=['x'], values=strings, unit='s'),
+            'y': sc.arange('y', 5.0, unit='m'),
+        },
+    )
+    fig = FigImage(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_kwargs_are_forwarded_to_artist():
     da = data_array(ndim=2)
-    fig = FigImage(input_node(da), rasterized=True)
+    fig = FigImage(Node(da), rasterized=True)
     artist = list(fig.artists.values())[0]
     assert artist._mesh.get_rasterized()
-    fig = FigImage(input_node(da), rasterized=False)
+    fig = FigImage(Node(da), rasterized=False)
     artist = list(fig.artists.values())[0]
     assert not artist._mesh.get_rasterized()
 
 
 def test_figsize():
     da = data_array(ndim=2)
     size = (8.1, 8.3)
-    fig = FigImage(input_node(da), figsize=size)
+    fig = FigImage(Node(da), figsize=size)
     assert np.allclose(fig.canvas.fig.get_size_inches(), size)
 
 
 def test_grid():
     da = data_array(ndim=2)
-    fig = FigImage(input_node(da), grid=True)
+    fig = FigImage(Node(da), grid=True)
     assert fig.canvas.ax.xaxis.get_gridlines()[0].get_visible()
 
 
 def test_ax():
     fig, ax = plt.subplots()
     assert len(ax.collections) == 0
     da = data_array(ndim=2)
-    _ = FigImage(input_node(da), ax=ax)
+    _ = FigImage(Node(da), ax=ax)
     assert len(ax.collections) == 1
 
 
 def test_cax():
     fig, ax = plt.subplots()
     cax = fig.add_axes([0.9, 0.02, 0.05, 0.98])
     assert len(cax.collections) == 0
     da = data_array(ndim=2)
-    _ = FigImage(input_node(da), ax=ax, cax=cax)
+    _ = FigImage(Node(da), ax=ax, cax=cax)
     assert len(cax.collections) > 0
```

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_figline_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_figline_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 
-from plopp import input_node
+from plopp import Node
 from plopp.data.testing import data_array
 from plopp.graphics.figline import FigLine
 
 
 def test_with_string_coord():
     strings = ['a', 'b', 'c', 'd', 'e']
-    da = sc.DataArray(data=sc.arange('x', 5.),
-                      coords={'x': sc.array(dims=['x'], values=strings, unit='m')})
-    fig = FigLine(input_node(da))
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0),
+        coords={'x': sc.array(dims=['x'], values=strings, unit='m')},
+    )
+    fig = FigLine(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_with_strings_as_bin_edges():
     strings = ['a', 'b', 'c', 'd', 'e', 'f']
-    da = sc.DataArray(data=sc.arange('x', 5.),
-                      coords={'x': sc.array(dims=['x'], values=strings, unit='m')})
-    fig = FigLine(input_node(da))
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0),
+        coords={'x': sc.array(dims=['x'], values=strings, unit='m')},
+    )
+    fig = FigLine(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_figsize():
     da = data_array(ndim=1)
     size = (6.1, 3.3)
-    fig = FigLine(input_node(da), figsize=size)
+    fig = FigLine(Node(da), figsize=size)
     assert np.allclose(fig.canvas.fig.get_size_inches(), size)
 
 
 def test_grid():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da), grid=True)
+    fig = FigLine(Node(da), grid=True)
     assert fig.canvas.ax.xaxis.get_gridlines()[0].get_visible()
 
 
 def test_ax():
     fig, ax = plt.subplots()
     assert len(ax.lines) == 0
     da = data_array(ndim=1)
-    _ = FigLine(input_node(da), ax=ax)
+    _ = FigLine(Node(da), ax=ax)
     assert len(ax.lines) > 0
```

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_figure_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_image_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_image_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_interactive_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_interactive_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from plopp import input_node
+from plopp import Node
 from plopp.backends.matplotlib.interactive import InteractiveFig
 from plopp.data.testing import data_array
 from plopp.graphics.figimage import FigImage
 from plopp.graphics.figline import FigLine
 
 
 def test_logx_1d_toolbar_button(use_ipympl):
     da = data_array(ndim=1)
-    fig = InteractiveFig(input_node(da), FigConstructor=FigLine, scale={'xx': 'log'})
+    fig = InteractiveFig(Node(da), FigConstructor=FigLine, scale={'xx': 'log'})
     assert fig.toolbar['logx'].value
 
 
 def test_logy_1d_toolbar_button(use_ipympl):
     da = data_array(ndim=1)
-    fig = InteractiveFig(input_node(da), FigConstructor=FigLine, norm='log')
+    fig = InteractiveFig(Node(da), FigConstructor=FigLine, norm='log')
     assert fig.toolbar['logy'].value
 
 
 def test_logxy_2d_toolbar_buttons(use_ipympl):
     da = data_array(ndim=2)
-    fig = InteractiveFig(input_node(da),
-                         FigConstructor=FigImage,
-                         scale={
-                             'xx': 'log',
-                             'yy': 'log'
-                         })
+    fig = InteractiveFig(
+        Node(da), FigConstructor=FigImage, scale={'xx': 'log', 'yy': 'log'}
+    )
     assert fig.toolbar['logx'].value
     assert fig.toolbar['logy'].value
 
 
 def test_log_norm_2d_toolbar_button(use_ipympl):
     da = data_array(ndim=2)
-    fig = InteractiveFig(input_node(da), FigConstructor=FigImage, norm='log')
+    fig = InteractiveFig(Node(da), FigConstructor=FigImage, norm='log')
     assert fig.toolbar['lognorm'].value
```

### Comparing `plopp-23.3.0/tests/backends/matplotlib/mpl_line_test.py` & `plopp-23.4.0/tests/backends/matplotlib/mpl_line_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,21 @@
     y1 = np.array(coll.get_segments())[:, 0, 1]
     y2 = np.array(coll.get_segments())[:, 1, 1]
     assert np.allclose(y1, (da.data * 2.5 - sc.stddevs(da.data)).values)
     assert np.allclose(y2, (da.data * 2.5 + sc.stddevs(da.data)).values)
 
 
 def test_line_datetime_binedges_with_errorbars():
-    t = np.arange(np.datetime64('2017-03-16T20:58:17'),
-                  np.datetime64('2017-03-16T21:15:17'), 20)
+    t = np.arange(
+        np.datetime64('2017-03-16T20:58:17'), np.datetime64('2017-03-16T21:15:17'), 20
+    )
     time = sc.array(dims=['time'], values=t)
     v = np.random.rand(time.sizes['time'] - 1)
-    da = sc.DataArray(data=sc.array(dims=['time'], values=10 * v, variances=v),
-                      coords={'time': time})
+    da = sc.DataArray(
+        data=sc.array(dims=['time'], values=10 * v, variances=v), coords={'time': time}
+    )
     # Checking for the locations of the errorbars is slightly strange, as the
     # get_segments() method from the LineCollection gives x values as floats, not
     # datetime, and comparing with the original data is thus difficult as the floats
     # do not seem immediately convertible to datetimes.
     # Hence, we simply check if the Line can be created without raising an exception.
     Line(canvas=Canvas(), data=da)
```

### Comparing `plopp-23.3.0/tests/backends/plotly/plotly_canvas_test.py` & `plopp-23.4.0/tests/backends/plotly/plotly_canvas_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,50 +38,56 @@
     canvas = Canvas()
     canvas.xunit = 'm'
     canvas.yunit = 'm'
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     ymin = sc.scalar(5.5, unit='m')
     ymax = sc.scalar(22.3, unit='m')
-    canvas.crop(x={
-        'min': xmin,
-        'max': xmax,
-    }, y={
-        'min': ymin,
-        'max': ymax,
-    })
+    canvas.crop(
+        x={
+            'min': xmin,
+            'max': xmax,
+        },
+        y={
+            'min': ymin,
+            'max': ymax,
+        },
+    )
     assert canvas.xrange == (xmin.value, xmax.value)
     assert canvas.yrange == (ymin.value, ymax.value)
 
 
 def test_crop_unit_conversion():
     canvas = Canvas()
     canvas.xunit = 'cm'
     canvas.yunit = 'cm'
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(3.3, unit='m')
     canvas.crop(x={'min': xmin, 'max': xmax})
-    assert canvas.xrange == (210., 330.)
+    assert canvas.xrange == (210.0, 330.0)
 
 
 def test_crop_no_variable():
     canvas = Canvas()
     canvas.xunit = 'm'
     canvas.yunit = 'm'
     xmin = 2.1
     xmax = 102.0
     ymin = 5.5
     ymax = 22.3
-    canvas.crop(x={
-        'min': xmin,
-        'max': xmax,
-    }, y={
-        'min': ymin,
-        'max': ymax,
-    })
+    canvas.crop(
+        x={
+            'min': xmin,
+            'max': xmax,
+        },
+        y={
+            'min': ymin,
+            'max': ymax,
+        },
+    )
     assert canvas.xrange == (xmin, xmax)
     assert canvas.yrange == (ymin, ymax)
 
 
 @pytest.mark.parametrize('ext', ['jpg', 'png', 'pdf', 'svg', 'html'])
 def test_save_to_disk(ext):
     canvas = Canvas()
```

### Comparing `plopp-23.3.0/tests/backends/plotly/plotly_figure_test.py` & `plopp-23.4.0/tests/backends/plotly/plotly_figure_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import pytest
 
-from plopp import input_node
+from plopp import Node
 from plopp.backends.plotly.figure import Figure
 from plopp.data.testing import data_array
 from plopp.graphics.figline import FigLine
 
 pytest.importorskip("plotly")
 
 
 def test_logx_1d_toolbar_button():
     da = data_array(ndim=1)
-    fig = Figure(input_node(da), FigConstructor=FigLine, scale={'xx': 'log'})
+    fig = Figure(Node(da), FigConstructor=FigLine, scale={'xx': 'log'})
     assert fig.toolbar['logx'].value
 
 
 def test_logy_1d_toolbar_button():
     da = data_array(ndim=1)
-    fig = Figure(input_node(da), FigConstructor=FigLine, norm='log')
+    fig = Figure(Node(da), FigConstructor=FigLine, norm='log')
     assert fig.toolbar['logy'].value
```

### Comparing `plopp-23.3.0/tests/backends/plotly/plotly_line_test.py` & `plopp-23.4.0/tests/backends/plotly/plotly_line_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,19 +93,21 @@
     new_values.variances = da.variances * 4.0
     line.update(new_values)
     assert np.allclose(line._line.y, da.values)
     assert np.allclose(line._error.error_y['array'], sc.stddevs(da.data).values * 2.0)
 
 
 def test_line_datetime_binedges_with_errorbars():
-    t = np.arange(np.datetime64('2017-03-16T20:58:17'),
-                  np.datetime64('2017-03-16T21:15:17'), 20)
+    t = np.arange(
+        np.datetime64('2017-03-16T20:58:17'), np.datetime64('2017-03-16T21:15:17'), 20
+    )
     time = sc.array(dims=['time'], values=t)
     v = np.random.rand(time.sizes['time'] - 1)
-    da = sc.DataArray(data=sc.array(dims=['time'], values=10 * v, variances=v),
-                      coords={'time': time})
+    da = sc.DataArray(
+        data=sc.array(dims=['time'], values=10 * v, variances=v), coords={'time': time}
+    )
     xint = t.astype(int)
     xmid = (0.5 * (xint[1:] + xint[:-1])).astype(int)
     expected = np.array(xmid, dtype=t.dtype)
     line = Line(canvas=Canvas(), data=da)
     # Note that allclose does not work on datetime dtypes
     assert np.allclose(line._error.x.astype(int), expected.astype(int))
```

### Comparing `plopp-23.3.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py` & `plopp-23.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from plopp.data.testing import scatter
 
 
 def test_creation():
     da = scatter()
     cloud = PointCloud(data=da, x='x', y='y', z='z')
     assert sc.identical(cloud._data, da)
-    assert np.allclose(cloud.geometry.attributes['position'].array,
-                       da.coords['position'].values)
+    assert np.allclose(
+        cloud.geometry.attributes['position'].array, da.coords['position'].values
+    )
 
 
 def test_update():
     da = scatter()
     cloud = PointCloud(data=da, x='x', y='y', z='z')
     cloud.update(da)
     assert sc.identical(cloud._data, da)
@@ -37,15 +38,15 @@
     assert sc.identical(ylims[1], da.meta['y'].max() + sc.scalar(0.5 * pix, unit='m'))
     assert sc.identical(zlims[0], da.meta['z'].min() - sc.scalar(0.5 * pix, unit='m'))
     assert sc.identical(zlims[1], da.meta['z'].max() + sc.scalar(0.5 * pix, unit='m'))
 
 
 def test_get_limits_flat_panel():
     da = scatter()
-    da.coords['z'] *= 0.
+    da.coords['z'] *= 0.0
     pix = 0.5
     cloud = PointCloud(data=da, x='x', y='y', z='z', pixel_size=pix)
     xlims, ylims, zlims = cloud.get_limits()
     assert sc.identical(xlims[0], da.meta['x'].min() - sc.scalar(0.5 * pix, unit='m'))
     assert sc.identical(xlims[1], da.meta['x'].max() + sc.scalar(0.5 * pix, unit='m'))
     assert sc.identical(ylims[0], da.meta['y'].min() - sc.scalar(0.5 * pix, unit='m'))
     assert sc.identical(ylims[1], da.meta['y'].max() + sc.scalar(0.5 * pix, unit='m'))
@@ -64,19 +65,17 @@
     cloud = PointCloud(data=da, x='x', y='y', z='z', pixel_size=sc.scalar(2, unit='m'))
     assert cloud.material.size == 2.0 * reference.material.size
 
 
 def test_pixel_size_unit_conversion():
     da = scatter()
     reference = PointCloud(data=da, x='x', y='y', z='z', pixel_size=1)
-    cloud = PointCloud(data=da,
-                       x='x',
-                       y='y',
-                       z='z',
-                       pixel_size=sc.scalar(350, unit='cm'))
+    cloud = PointCloud(
+        data=da, x='x', y='y', z='z', pixel_size=sc.scalar(350, unit='cm')
+    )
     assert cloud.material.size == 3.5 * reference.material.size
     with pytest.raises(sc.UnitError):
         PointCloud(data=da, x='x', y='y', z='z', pixel_size=sc.scalar(350, unit='s'))
 
 
 def test_pixel_size_cannot_have_units_when_spatial_dimensions_have_different_units():
     da = scatter()
@@ -90,19 +89,21 @@
     cloud = PointCloud(data=da, x='x', y='y', z='z', pixel_size=2.5)
     assert cloud.material.size == 2.5 * reference.material.size
 
 
 def test_creation_raises_when_data_is_not_1d():
     da = scatter()
     da2d = sc.broadcast(da, sizes={**da.sizes, **{'time': 10}})
-    with pytest.raises(ValueError,
-                       match='PointCloud only accepts one dimensional data'):
+    with pytest.raises(
+        ValueError, match='PointCloud only accepts one dimensional data'
+    ):
         PointCloud(data=da2d, x='x', y='y', z='z')
 
 
 def test_update_raises_when_data_is_not_1d():
     da = scatter()
     cloud = PointCloud(data=da, x='x', y='y', z='z')
     da2d = sc.broadcast(da, sizes={**da.sizes, **{'time': 10}})
-    with pytest.raises(ValueError,
-                       match='PointCloud only accepts one dimensional data'):
+    with pytest.raises(
+        ValueError, match='PointCloud only accepts one dimensional data'
+    ):
         cloud.update(da2d)
```

### Comparing `plopp-23.3.0/tests/conftest.py` & `plopp-23.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/core/graph_test.py` & `plopp-23.4.0/tests/core/graph_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,82 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from views import SimpleView
 
-from plopp import input_node, node, show_graph
+from plopp import Node, show_graph
 
 
 def has_edge(graph, node1, node2):
     """
     Check if graph contains a given edge.
     """
     tail_name = graph._quote_edge(node1)
     head_name = graph._quote_edge(node2)
-    return graph._edge(tail=tail_name, head=head_name, attr='') in graph.body
+    for key in graph.body:
+        print(
+            graph._edge(tail=tail_name, head=head_name, attr=''),
+            key.split(' [label')[0],
+        )
+        if (
+            graph._edge(tail=tail_name, head=head_name, attr='').strip()
+            == key.split(' [label')[0].strip()
+        ):
+            return True
+    return False
 
 
 def test_two_nodes_parent_child():
     # [ a ]
     #   |
     # [ b ]
-    a = input_node(5)
-    b = node(lambda x: x - 2)(a)
+    a = Node(5)
+    b = Node(lambda x: x - 2, a)
     g = show_graph(a)
     assert has_edge(g, a.id, b.id)
 
 
 def test_two_children():
     #    [ a ]
     #     / \
     #    /   \
     # [ b ] [ c ]
-    a = input_node(5)
-    b = node(lambda x: x - 2)(a)
-    c = node(lambda x: x + 2)(a)
+    a = Node(5)
+    b = Node(lambda x: x - 2, a)
+    c = Node(lambda x: x + 2, a)
     g = show_graph(a)
     assert has_edge(g, a.id, b.id)
     assert has_edge(g, a.id, c.id)
 
 
 def test_two_parents():
     # [ a ] [ b ]
     #    \   /
     #     \ /
     #    [ c ]
-    a = input_node(5)
-    b = input_node(9)
-    c = node(lambda x, y: x + y)(a, b)
+    a = Node(5)
+    b = Node(9)
+    c = Node(lambda x, y: x + y, a, b)
     g = show_graph(a)
     assert has_edge(g, a.id, c.id)
     assert has_edge(g, b.id, c.id)
 
 
 def test_two_parents_two_children():
     # [ a ] [ b ]
     #    \   / |
     #     \ /  |
     #    [ c ] |
     #       \  |
     #        \/
     #      [ d ]
-    a = input_node(5)
-    b = input_node(9)
-    c = node(lambda x, y: x + y)(a, b)
-    d = node(lambda x, y: x - y)(c, b)
+    a = Node(5)
+    b = Node(9)
+    c = Node(lambda x, y: x + y, a, b)
+    d = Node(lambda x, y: x - y, c, b)
     g = show_graph(a)
     assert has_edge(g, a.id, c.id)
     assert has_edge(g, b.id, c.id)
     assert has_edge(g, c.id, d.id)
     assert has_edge(g, b.id, d.id)
 
 
@@ -75,20 +85,20 @@
     #      /     \
     #     /       \
     #    /         \
     # [ b ] [ d ] [ c ]
     #    \   / \   /
     #     \ /   \ /
     #    [ e ] [ f ]
-    a = input_node(0)
-    b = node(lambda x: x + 1)(a)
-    c = node(lambda x: x + 2)(a)
-    d = input_node(4)
-    e = node(lambda x, y: x + y)(b, d)
-    f = node(lambda x, y: x + y)(c, d)
+    a = Node(0)
+    b = Node(lambda x: x + 1, a)
+    c = Node(lambda x: x + 2, a)
+    d = Node(4)
+    e = Node(lambda x, y: x + y, b, d)
+    f = Node(lambda x, y: x + y, c, d)
     g = show_graph(a)
     assert has_edge(g, a.id, b.id)
     assert has_edge(g, a.id, c.id)
     assert has_edge(g, b.id, e.id)
     assert has_edge(g, d.id, e.id)
     assert has_edge(g, d.id, f.id)
     assert has_edge(g, c.id, f.id)
@@ -98,15 +108,15 @@
     #    [ a ]
     #     / \
     #    /   \
     # [ b ] [ View ]
     #   |
     #   |
     # [ View ]
-    a = input_node(5)
-    b = node(lambda x: x - 2)(x=a)
+    a = Node(5)
+    b = Node(lambda x: x - 2, x=a)
     av = SimpleView(a)
     bv = SimpleView(b)
     g = show_graph(a)
     assert has_edge(g, a.id, b.id)
     assert has_edge(g, a.id, av.id)
     assert has_edge(g, b.id, bv.id)
```

### Comparing `plopp-23.3.0/tests/core/limits_test.py` & `plopp-23.4.0/tests/core/limits_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,80 +5,80 @@
 import pytest
 import scipp as sc
 
 from plopp.core.limits import find_limits, fix_empty_range
 
 
 def test_find_limits():
-    x = sc.arange('x', 11., unit='m')
+    x = sc.arange('x', 11.0, unit='m')
     lims = find_limits(x)
-    assert sc.identical(lims[0], sc.scalar(0., unit='m'))
-    assert sc.identical(lims[1], sc.scalar(10., unit='m'))
+    assert sc.identical(lims[0], sc.scalar(0.0, unit='m'))
+    assert sc.identical(lims[1], sc.scalar(10.0, unit='m'))
 
 
 def test_find_limits_log():
-    x = sc.arange('x', 11., unit='m')
+    x = sc.arange('x', 11.0, unit='m')
     lims = find_limits(x, scale='log')
-    assert sc.identical(lims[0], sc.scalar(1., unit='m'))
-    assert sc.identical(lims[1], sc.scalar(10., unit='m'))
+    assert sc.identical(lims[0], sc.scalar(1.0, unit='m'))
+    assert sc.identical(lims[1], sc.scalar(10.0, unit='m'))
 
 
 def test_find_limits_log_int():
     x = sc.arange('x', 11, unit='m')
     lims = find_limits(x, scale='log')
     assert sc.identical(lims[0], sc.scalar(1, unit='m'))
     assert sc.identical(lims[1], sc.scalar(10, unit='m'))
 
 
 def test_find_limits_with_nan():
-    x = sc.arange('x', 11., unit='m')
+    x = sc.arange('x', 11.0, unit='m')
     x.values[5] = np.nan
     lims = find_limits(x)
-    assert sc.identical(lims[0], sc.scalar(0., unit='m'))
-    assert sc.identical(lims[1], sc.scalar(10., unit='m'))
+    assert sc.identical(lims[0], sc.scalar(0.0, unit='m'))
+    assert sc.identical(lims[1], sc.scalar(10.0, unit='m'))
 
 
 def test_find_limits_with_inf():
-    x = sc.arange('x', 11., unit='m')
+    x = sc.arange('x', 11.0, unit='m')
     x.values[5] = np.inf
     lims = find_limits(x)
-    assert sc.identical(lims[0], sc.scalar(0., unit='m'))
-    assert sc.identical(lims[1], sc.scalar(10., unit='m'))
+    assert sc.identical(lims[0], sc.scalar(0.0, unit='m'))
+    assert sc.identical(lims[1], sc.scalar(10.0, unit='m'))
 
 
 def test_find_limits_with_ninf():
-    x = sc.arange('x', 11., unit='m')
+    x = sc.arange('x', 11.0, unit='m')
     x.values[5] = np.NINF
     lims = find_limits(x)
-    assert sc.identical(lims[0], sc.scalar(0., unit='m'))
-    assert sc.identical(lims[1], sc.scalar(10., unit='m'))
+    assert sc.identical(lims[0], sc.scalar(0.0, unit='m'))
+    assert sc.identical(lims[1], sc.scalar(10.0, unit='m'))
 
 
 def test_find_limits_no_finite_values_raises():
     x = sc.array(dims=['x'], values=[np.nan, np.inf, np.NINF, np.nan], unit='m')
     with pytest.raises(ValueError, match="No finite values were found in array"):
         _ = find_limits(x)
 
 
 def test_fix_empty_range():
-    a = sc.scalar(5., unit='m')
-    b = sc.scalar(10., unit='m')
+    a = sc.scalar(5.0, unit='m')
+    b = sc.scalar(10.0, unit='m')
     lims = fix_empty_range((a, b))
     assert sc.identical(lims[0], a)
     assert sc.identical(lims[1], b)
 
 
 def test_fix_empty_range_same_values():
-    a = sc.scalar(5., unit='m')
+    a = sc.scalar(5.0, unit='m')
     lims = fix_empty_range((a, a))
     assert sc.identical(lims[0], sc.scalar(2.5, unit='m'))
     assert sc.identical(lims[1], sc.scalar(7.5, unit='m'))
     lims = fix_empty_range((-a, -a))
     assert sc.identical(lims[0], sc.scalar(-7.5, unit='m'))
     assert sc.identical(lims[1], sc.scalar(-2.5, unit='m'))
 
 
 def test_fix_empty_range_zeros_values():
-    a = sc.scalar(0., unit='m')
+    a = sc.scalar(0.0, unit='m')
     lims = fix_empty_range((a, a))
     assert sc.identical(lims[0], sc.scalar(-0.5, unit='m'))
     assert sc.identical(lims[1], sc.scalar(0.5, unit='m'))
```

### Comparing `plopp-23.3.0/tests/core/utils_test.py` & `plopp-23.4.0/tests/core/utils_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,58 +3,66 @@
 
 import scipp as sc
 
 from plopp.core.utils import coord_as_bin_edges
 
 
 def test_coord_as_bin_edges_midpoints_input():
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'),
-                      coords={'x': sc.arange('x', 5., unit='m')})
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0, unit='K'), coords={'x': sc.arange('x', 5.0, unit='m')}
+    )
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, sc.linspace('x', -0.5, 4.5, num=6, unit='m'))
 
 
 def test_coord_as_bin_edges_edges_input():
-    x = sc.arange('x', 6., unit='m')
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'), coords={'x': x})
+    x = sc.arange('x', 6.0, unit='m')
+    da = sc.DataArray(data=sc.arange('x', 5.0, unit='K'), coords={'x': x})
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, x)
 
 
 def test_coord_as_bin_edges_string_midpoints_input():
     strings = ['a', 'b', 'c', 'd', 'e']
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'),
-                      coords={'x': sc.array(dims=['x'], values=strings, unit='s')})
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0, unit='K'),
+        coords={'x': sc.array(dims=['x'], values=strings, unit='s')},
+    )
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, sc.linspace('x', -0.5, 4.5, num=6, unit='s'))
 
 
 def test_coord_as_bin_edges_string_edges_input():
     strings = ['a', 'b', 'c', 'd', 'e', 'f']
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'),
-                      coords={'x': sc.array(dims=['x'], values=strings, unit='s')})
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0, unit='K'),
+        coords={'x': sc.array(dims=['x'], values=strings, unit='s')},
+    )
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, sc.arange('x', 6.0, unit='s'))
 
 
 def test_coord_as_bin_edges_int_midpoints_input():
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'),
-                      coords={'x': sc.arange('x', 5, unit='m')})
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0, unit='K'), coords={'x': sc.arange('x', 5, unit='m')}
+    )
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, sc.linspace('x', -0.5, 4.5, num=6, unit='m'))
 
 
 def test_coord_as_bin_edges_int_edges_input():
     x = sc.arange('x', 6, unit='m')
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'), coords={'x': x})
+    da = sc.DataArray(data=sc.arange('x', 5.0, unit='K'), coords={'x': x})
     result = coord_as_bin_edges(da, key='x')
     assert sc.identical(result, x)
 
 
 def test_coord_as_bin_edges_non_dimension_coord():
-    da = sc.DataArray(data=sc.arange('x', 5., unit='K'),
-                      coords={
-                          'x': sc.arange('x', 5., unit='m'),
-                          'y': sc.arange('x', 17., 22., unit='m')
-                      })
+    da = sc.DataArray(
+        data=sc.arange('x', 5.0, unit='K'),
+        coords={
+            'x': sc.arange('x', 5.0, unit='m'),
+            'y': sc.arange('x', 17.0, 22.0, unit='m'),
+        },
+    )
     result = coord_as_bin_edges(da, key='y', dim='x')
     assert sc.identical(result, sc.linspace('x', 16.5, 21.5, num=6, unit='m'))
```

### Comparing `plopp-23.3.0/tests/core/views.py` & `plopp-23.4.0/tests/core/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from plopp import View
 
 
 class SimpleView(View):
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.value = None
 
     def notify_view(self, message):
         self.value = message
 
 
 class DataView(View):
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.data = None
 
     def notify_view(self, message):
         node_id = message["node_id"]
         self.data = self.graph_nodes[node_id].request_data()
```

### Comparing `plopp-23.3.0/tests/functions/common_test.py` & `plopp-23.4.0/tests/functions/common_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,22 +24,25 @@
     assert out.coords['xx2'].max() == 7.5 * da.coords['xx'].max()
     assert out.coords['yy2'].max() == 3.3 * da.coords['yy'].max()
 
 
 def test_preprocess_warns_when_coordinate_is_not_sorted():
     da = data_array(ndim=1)
     unsorted = sc.concat([da['xx', 20:], da['xx', :20]], dim='xx')
-    with pytest.warns(UserWarning,
-                      match='The input contains a coordinate with unsorted values'):
+    with pytest.warns(
+        UserWarning, match='The input contains a coordinate with unsorted values'
+    ):
         preprocess(unsorted)
 
 
 def test_preprocess_no_warning_if_dtype_cannot_be_sorted():
     da = data_array(ndim=1)
-    da.coords['vecs'] = sc.vectors(dims=['xx'],
-                                   values=np.random.random((da.sizes['xx'], 3)))
+    da.coords['vecs'] = sc.vectors(
+        dims=['xx'], values=np.random.random((da.sizes['xx'], 3))
+    )
     out = preprocess(da)  # no warning should be emitted
     assert 'vecs' in out.coords
-    da.coords['strings'] = sc.array(dims=['xx'],
-                                    values=list('ba' * (da.sizes['xx'] // 2)))
+    da.coords['strings'] = sc.array(
+        dims=['xx'], values=list('ba' * (da.sizes['xx'] // 2))
+    )
     out = preprocess(da)  # no warning should be emitted
     assert 'strings' in out.coords
```

### Comparing `plopp-23.3.0/tests/functions/plot_test.py` & `plopp-23.4.0/tests/functions/plot_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 import scipp as sc
 
 import plopp as pp
 from plopp.data.testing import data_array, dataset
 
 
 def test_plot_ndarray():
-    pp.plot(np.arange(50.))
+    pp.plot(np.arange(50.0))
 
 
 def test_plot_list():
     pp.plot([1, 2, 3, 4, 5])
 
 
 def test_plot_variable():
-    pp.plot(sc.arange('x', 50.))
+    pp.plot(sc.arange('x', 50.0))
 
 
 def test_plot_data_array():
     pp.plot(data_array(ndim=1))
     da = data_array(ndim=2)
     pp.plot(da)
     pp.plot(da)
@@ -39,23 +39,23 @@
 
 def test_plot_dataset():
     ds = dataset(ndim=1)
     pp.plot(ds)
 
 
 def test_plot_dict_of_ndarrays():
-    pp.plot({'a': np.arange(50.), 'b': np.arange(60.)})
+    pp.plot({'a': np.arange(50.0), 'b': np.arange(60.0)})
 
 
 def test_plot_dict_of_lists():
     pp.plot({'a': [1, 2, 3, 4], 'b': [4, 5, 6, 7]})
 
 
 def test_plot_dict_of_variables():
-    pp.plot({'a': sc.arange('x', 50.), 'b': sc.arange('x', 60.)})
+    pp.plot({'a': sc.arange('x', 50.0), 'b': sc.arange('x', 60.0)})
 
 
 def test_plot_dict_of_data_arrays():
     ds = dataset(ndim=1)
     pp.plot({'a': ds['a'], 'b': ds['b']})
 
 
@@ -165,18 +165,16 @@
     assert p.canvas.ax.get_yscale() == 'log'
 
 
 def test_kwarg_crop_1d_min_max():
     da = data_array(ndim=1)
     p = pp.plot(
         da,
-        crop={'xx': {
-            'min': sc.scalar(20, unit='m'),
-            'max': sc.scalar(40, unit='m')
-        }})
+        crop={'xx': {'min': sc.scalar(20, unit='m'), 'max': sc.scalar(40, unit='m')}},
+    )
     assert np.array_equal(p.canvas.ax.get_xlim(), [20, 40])
 
 
 def test_kwarg_crop_1d_min_only():
     da = data_array(ndim=1)
     p = pp.plot(da, crop={'xx': {'min': sc.scalar(20, unit='m')}})
     assert p.canvas.ax.get_xlim()[0] == 20
@@ -194,24 +192,21 @@
     assert p.canvas.ax.get_xlim()[0] == 20
     p = pp.plot(da, crop={'xx': {'min': 20.5}})
     assert p.canvas.ax.get_xlim()[0] == 20.5
 
 
 def test_kwarg_crop_2d():
     da = data_array(ndim=2)
-    p = pp.plot(da,
-                crop={
-                    'xx': {
-                        'min': sc.scalar(20, unit='m')
-                    },
-                    'yy': {
-                        'min': sc.scalar(10, unit='m'),
-                        'max': sc.scalar(4000, unit='cm')
-                    }
-                })
+    p = pp.plot(
+        da,
+        crop={
+            'xx': {'min': sc.scalar(20, unit='m')},
+            'yy': {'min': sc.scalar(10, unit='m'), 'max': sc.scalar(4000, unit='cm')},
+        },
+    )
     assert p.canvas.ax.get_xlim()[0] == 20
     assert np.array_equal(p.canvas.ax.get_ylim(), [10, 40])
 
 
 def test_kwarg_for_two_lines():
     ds = dataset(ndim=1)
     p = pp.plot(ds, color='r')
@@ -291,10 +286,91 @@
     with pytest.raises(ValueError):
         fig.save(filename='plopp_fig2d.txt')
 
 
 def test_plot_raises_with_multiple_2d_inputs():
     a = data_array(ndim=2)
     b = 3.3 * a
-    with pytest.raises(ValueError,
-                       match='The plot function can only plot a single 2d data entry'):
+    with pytest.raises(
+        ValueError, match='The plot function can only plot a single 2d data entry'
+    ):
         pp.plot({'a': a, 'b': b})
+
+
+def test_plot_xarray_data_array_1d():
+    import xarray as xr
+
+    N = 50
+    data = np.random.random(N)
+    time = np.arange(float(N))
+    da = xr.DataArray(data, coords={'time': time}, dims=['time'])
+    p = pp.plot(da)
+    assert p._fig.dims['x'] == 'time'
+    assert p.canvas.xunit == 'dimensionless'
+    assert p.canvas.yunit == 'dimensionless'
+
+
+def test_plot_xarray_data_array_2d():
+    import xarray as xr
+
+    N = 50
+    M = 40
+    data = np.random.random([M, N])
+    time = np.arange(float(N))
+    space = np.arange(float(M))
+    da = xr.DataArray(
+        data, coords={'space': space, 'time': time}, dims=['space', 'time']
+    )
+    p = pp.plot(da)
+    assert p._fig.dims['x'] == 'time'
+    assert p._fig.dims['y'] == 'space'
+    assert p.canvas.xunit == 'dimensionless'
+    assert p.canvas.yunit == 'dimensionless'
+
+
+def test_plot_xarray_dataset():
+    import xarray as xr
+
+    N = 50
+    temp = 15 + 8 * np.random.random(N)
+    precip = 10 * np.random.random(N)
+    ds = xr.Dataset(
+        {
+            "temperature": (["time"], temp),
+            "precipitation": (["time"], precip),
+        },
+        coords={"time": np.arange(50)},
+    )
+    p = pp.plot(ds)
+    assert p._fig.dims['x'] == 'time'
+    assert p.canvas.xunit == 'dimensionless'
+    assert p.canvas.yunit == 'dimensionless'
+    assert len(p._fig.artists) == 2
+
+
+def test_plot_pandas_series():
+    import pandas as pd
+
+    s = pd.Series(np.arange(100.0), name='MyDataSeries')
+    p = pp.plot(s)
+    assert p._fig.dims['x'] == 'row'
+    assert p.canvas.xunit == 'dimensionless'
+    assert p.canvas.yunit == 'dimensionless'
+    assert list(p._fig.artists.values())[0].label == 'MyDataSeries'
+
+
+def test_plot_pandas_dataframe():
+    import pandas as pd
+
+    df = pd.DataFrame(
+        {
+            'A': np.arange(50.0),
+            'B': 1.5 * np.arange(50),
+            'C': np.random.random(50),
+            'D': np.random.normal(size=50),
+        }
+    )
+    p = pp.plot(df)
+    assert p._fig.dims['x'] == 'row'
+    assert p.canvas.xunit == 'dimensionless'
+    assert p.canvas.yunit == 'dimensionless'
+    assert len(p._fig.artists) == 4
```

### Comparing `plopp-23.3.0/tests/functions/scatter3d_test.py` & `plopp-23.4.0/tests/functions/scatter3d_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,34 @@
 
 
 def test_scatter3d_dimensions_are_flattened():
     nx = 12
     ny = 12
     x = sc.linspace(dim='x', start=-10.0, stop=10.0, num=nx, unit='m')
     y = sc.linspace(dim='y', start=-10.0, stop=10.0, num=ny, unit='m')
-    da = sc.DataArray(data=sc.array(dims=['x', 'y'], values=np.random.rand(nx, ny)),
-                      coords={'position': sc.geometry.position(x, y, 0.0 * sc.units.m)})
+    da = sc.DataArray(
+        data=sc.array(dims=['x', 'y'], values=np.random.rand(nx, ny)),
+        coords={'position': sc.geometry.position(x, y, 0.0 * sc.units.m)},
+    )
     p = pp.scatter3d(da, pos="position")
     assert list(p[0].artists.values())[0].data.ndim == 1
     nz = 12
     z = sc.linspace(dim='z', start=-10.0, stop=10.0, num=nz, unit='m')
-    da = sc.DataArray(data=sc.array(dims=['x', 'y', 'z'],
-                                    values=np.random.rand(nx, ny, nz)),
-                      coords={'position': sc.geometry.position(x, y, z)})
+    da = sc.DataArray(
+        data=sc.array(dims=['x', 'y', 'z'], values=np.random.rand(nx, ny, nz)),
+        coords={'position': sc.geometry.position(x, y, z)},
+    )
     p = pp.scatter3d(da, pos="position")
     assert list(p[0].artists.values())[0].data.ndim == 1
 
 
 def test_scatter3d_can_plot_scalar_data():
-    da = sc.DataArray(data=sc.scalar(1.2),
-                      coords={'position': sc.vector(value=[1, 2, 3])})
+    da = sc.DataArray(
+        data=sc.scalar(1.2), coords={'position': sc.vector(value=[1, 2, 3])}
+    )
     p = pp.scatter3d(da, pos='position')
     assert list(p.children[0].artists.values())[0].data.ndim == 1
 
 
 def test_raises_ValueError_when_given_binned_data():
     nx = 10
     da = sc.data.table_xyz(100).bin(x=nx)
@@ -64,7 +68,23 @@
         pp.scatter3d(da, pos='position')
 
 
 def test_raises_ValueError_when_given_ax_kwarg():
     da = scatter()
     with pytest.raises(ValueError, match='Keyword "ax" detected'):
         pp.scatter3d(da, x='x', y='y', z='z', ax='dummy')
+
+
+def test_scatter3d_from_xarray():
+    import xarray as xr
+
+    N = 200
+    data = np.random.random(N)
+    x = np.random.normal(size=N)
+    y = np.random.normal(size=N)
+    z = np.random.normal(size=N)
+    da = xr.DataArray(
+        data,
+        coords={'x': ('pixel', x), 'y': ('pixel', y), 'z': ('pixel', z)},
+        dims=['pixel'],
+    )
+    pp.scatter3d(da, x='x', y='y', z='z')
```

### Comparing `plopp-23.3.0/tests/functions/slicer_test.py` & `plopp-23.4.0/tests/functions/slicer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,24 @@
     sl = Slicer(ds, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), ds['a']['yy', 5])
     assert sc.identical(nodes[1].request_data(), ds['b']['yy', 5])
 
 
+def test_with_data_group():
+    da = data_array(ndim=2)
+    dg = sc.DataGroup(a=da, b=da * 2.5)
+    sl = Slicer(dg, keep=['xx'])
+    nodes = list(sl.figure.graph_nodes.values())
+    sl.slider.controls['yy']['slider'].value = 5
+    assert sc.identical(nodes[0].request_data(), dg['a']['yy', 5])
+    assert sc.identical(nodes[1].request_data(), dg['b']['yy', 5])
+
+
 def test_with_dict_of_data_arrays():
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     sl = Slicer({'a': a, 'b': b}, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), a['yy', 5])
@@ -80,10 +90,10 @@
     with pytest.raises(ValueError, match='Cannot plot binned data'):
         Slicer(da, keep=['x'])
 
 
 def test_raises_when_requested_keep_dims_do_not_exist():
     da = data_array(ndim=3)
     with pytest.raises(
-            ValueError,
-            match='Slicer plot: one or more of the requested dims to be kept'):
+        ValueError, match='Slicer plot: one or more of the requested dims to be kept'
+    ):
         Slicer(da, keep=['time'])
```

### Comparing `plopp-23.3.0/tests/functions/superplot_test.py` & `plopp-23.4.0/tests/functions/superplot_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/graphics/colormapper_test.py` & `plopp-23.4.0/tests/graphics/colormapper_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 from matplotlib.colors import LogNorm, Normalize
 
 from plopp.data.testing import data_array
 from plopp.graphics.colormapper import ColorMapper
 
 
 class DummyChild:
-
     def __init__(self, data):
         self._data = data
         self._colors = None
 
     def set_colors(self, colors):
         self._colors = colors
 
     @property
     def data(self):
         return self._data
 
 
 def test_creation():
-    mapper = ColorMapper(cmap='magma',
-                         mask_cmap='jet',
-                         norm='linear',
-                         vmin=sc.scalar(1, unit='K'),
-                         vmax=sc.scalar(10, unit='K'))
+    mapper = ColorMapper(
+        cmap='magma',
+        mask_cmap='jet',
+        norm='linear',
+        vmin=sc.scalar(1, unit='K'),
+        vmax=sc.scalar(10, unit='K'),
+    )
     assert mapper.cmap.name == 'magma'
     assert mapper.mask_cmap.name == 'jet'
     assert mapper.norm == 'linear'
     assert sc.identical(mapper.user_vmin, sc.scalar(1, unit='K'))
     assert sc.identical(mapper.user_vmax, sc.scalar(10, unit='K'))
 
 
@@ -86,27 +87,27 @@
 
 
 def test_vmin_vmax():
     da = data_array(ndim=2, unit='K')
     vmin = sc.scalar(-0.1, unit='K')
     vmax = sc.scalar(3.5, unit='K')
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
-    mapper.update(data=da * 100., key=None)
+    mapper.update(data=da * 100.0, key=None)
     assert sc.identical(mapper.user_vmin, vmin)
     assert sc.identical(mapper.user_vmax, vmax)
     assert mapper.vmin == vmin.value
     assert mapper.vmax == vmax.value
 
 
 def test_vmin_vmax_no_variable():
     da = data_array(ndim=2, unit='K')
     vmin = -0.1
     vmax = 3.5
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
-    mapper.update(data=da * 100., key=None)
+    mapper.update(data=da * 100.0, key=None)
     assert mapper.user_vmin == vmin
     assert mapper.user_vmax == vmax
     assert mapper.vmin == vmin
     assert mapper.vmax == vmax
 
 
 def test_toggle_norm():
@@ -140,15 +141,15 @@
     assert mapper.normalizer.vmax == (da.max() * const).value
 
 
 def test_rgba():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
     colors = mapper.rgba(da)
-    assert colors.shape == da.data.shape + (4, )
+    assert colors.shape == da.data.shape + (4,)
 
 
 def test_rgba_with_masks():
     da1 = data_array(ndim=2, unit='K')
     da2 = data_array(ndim=2, unit='K', masks=True)
     mapper = ColorMapper()
     assert not np.allclose(mapper.rgba(da1), mapper.rgba(da2))
@@ -175,14 +176,13 @@
 def test_colorbar_is_not_created_if_cbar_false():
     mapper = ColorMapper(cbar=False)
     assert mapper.colorbar is None
     assert mapper.cax is None
 
 
 def test_colorbar_cbar_false_overrides_cax():
-
     @dataclass
     class Canvas:
         cax: int
 
     mapper = ColorMapper(cbar=False, canvas=Canvas(cax=0))
     assert mapper.colorbar is None
```

### Comparing `plopp-23.3.0/tests/graphics/figimage_test.py` & `plopp-23.4.0/tests/graphics/figimage_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import pytest
 import scipp as sc
 
-from plopp import input_node
+from plopp import Node
 from plopp.data.testing import data_array
 from plopp.graphics.figimage import FigImage
 
 
 def test_empty():
     fig = FigImage()
     assert len(fig.artists) == 0
@@ -29,42 +29,42 @@
         fig.update(data_array(ndim=1), key='data1d')
     with pytest.raises(ValueError, match="FigImage can only be used to plot 2-D data."):
         fig.update(data_array(ndim=3), key='data3d')
 
 
 def test_create_with_node():
     da = data_array(ndim=2)
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert len(fig.artists) == 1
     assert sc.identical(list(fig.artists.values())[0]._data, da)
 
 
 def test_create_with_bin_edges():
     da = data_array(ndim=2, binedges=True)
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert len(fig.artists) == 1
     assert sc.identical(list(fig.artists.values())[0]._data, da)
 
 
 def test_create_with_only_one_bin_edge_coord():
     da = data_array(ndim=2, binedges=True)
     da.coords['xx'] = sc.midpoints(da.coords['xx'])
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert len(fig.artists) == 1
     assert sc.identical(list(fig.artists.values())[0]._data, da)
 
 
 def test_log_norm():
     fig = FigImage(norm='log')
     assert fig.colormapper.norm == 'log'
 
 
 def test_crop():
     da = data_array(ndim=2, binedges=True)
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert fig.canvas.xrange == (da.meta['xx'].min().value, da.meta['xx'].max().value)
     assert fig.canvas.yrange == (da.meta['yy'].min().value, da.meta['yy'].max().value)
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     ymin = sc.scalar(5.5, unit='m')
     ymax = sc.scalar(22.3, unit='m')
     fig.crop(xx={'min': xmin, 'max': xmax}, yy={'min': ymin, 'max': ymax})
@@ -74,88 +74,81 @@
 
 def test_crop_no_variable():
     da = data_array(ndim=2)
     xmin = 2.1
     xmax = 102.0
     ymin = 5.5
     ymax = 22.3
-    fig = FigImage(input_node(da),
-                   crop={
-                       'xx': {
-                           'min': xmin,
-                           'max': xmax
-                       },
-                       'yy': {
-                           'min': ymin,
-                           'max': ymax
-                       }
-                   })
+    fig = FigImage(
+        Node(da),
+        crop={'xx': {'min': xmin, 'max': xmax}, 'yy': {'min': ymin, 'max': ymax}},
+    )
     assert fig.canvas.xrange == (xmin, xmax)
     assert fig.canvas.yrange == (ymin, ymax)
 
 
 def test_raises_for_new_data_with_incompatible_dimension():
     a = data_array(ndim=2)
     b = a.rename(xx='zz')
     with pytest.raises(sc.DimensionError):
-        FigImage(input_node(a), input_node(b))
+        FigImage(Node(a), Node(b))
 
 
 def test_raises_for_new_data_with_incompatible_unit():
     a = data_array(ndim=2)
     b = a * a
     with pytest.raises(sc.UnitError):
-        FigImage(input_node(a), input_node(b))
+        FigImage(Node(a), Node(b))
 
 
 def test_raises_for_new_data_with_incompatible_coord_unit():
     a = data_array(ndim=2)
     b = a.copy()
     b.coords['xx'] = a.coords['xx'] * a.coords['xx']
     with pytest.raises(sc.UnitError):
-        FigImage(input_node(a), input_node(b))
+        FigImage(Node(a), Node(b))
 
 
 def test_converts_new_data_units():
     a = data_array(ndim=2, unit='m')
     b = data_array(ndim=2, unit='cm')
-    anode = input_node(a)
-    bnode = input_node(b)
+    anode = Node(a)
+    bnode = Node(b)
     fig = FigImage(anode, bnode)
     assert sc.identical(fig.artists[anode.id]._data, a)
     assert sc.identical(fig.artists[bnode.id]._data, b.to(unit='m'))
 
 
 def test_converts_new_data_coordinate_units():
     a = data_array(ndim=2)
     b = data_array(ndim=2)
     b.coords['xx'].unit = 'cm'
-    anode = input_node(a)
-    bnode = input_node(b)
+    anode = Node(a)
+    bnode = Node(b)
     fig = FigImage(anode, bnode)
     assert sc.identical(fig.artists[anode.id]._data, a)
     c = b.copy()
     c.coords['xx'] = c.coords['xx'].to(unit='m')
     assert sc.identical(fig.artists[bnode.id]._data, c)
 
 
 def test_colorbar_label_has_correct_unit():
     da = data_array(ndim=2, unit='K')
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert fig.canvas.cblabel == '[K]'
 
 
 def test_colorbar_label_has_correct_name():
     da = data_array(ndim=2, unit='K')
     name = 'My Experimental Data'
     da.name = name
-    fig = FigImage(input_node(da))
+    fig = FigImage(Node(da))
     assert fig.canvas.cblabel == name + ' [K]'
 
 
 def test_colorbar_label_has_no_name_with_multiple_artists():
     a = data_array(ndim=2, unit='K')
     b = 3.3 * a
     a.name = 'A data'
     b.name = 'B data'
-    fig = FigImage(input_node(a), input_node(b))
+    fig = FigImage(Node(a), Node(b))
     assert fig.canvas.cblabel == '[K]'
```

### Comparing `plopp-23.3.0/tests/graphics/figline_test.py` & `plopp-23.4.0/tests/graphics/figline_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
 
-from plopp import input_node
+from plopp import Node
 from plopp.data.testing import data_array
 from plopp.graphics.figline import FigLine
 
 
 def test_empty():
     fig = FigLine()
     assert len(fig.artists) == 0
@@ -30,35 +30,35 @@
         fig.update(data_array(ndim=2), key='data2d')
     with pytest.raises(ValueError, match="FigLine can only be used to plot 1-D data."):
         fig.update(data_array(ndim=3), key='data3d')
 
 
 def test_create_with_node():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     assert len(fig.artists) == 1
     line = list(fig.artists.values())[0]
     assert sc.identical(line._data, da)
     assert line._error is None
 
 
 def test_with_errorbars():
     da = data_array(ndim=1, variances=True)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     assert len(fig.artists) == 1
     line = list(fig.artists.values())[0]
     assert line._error is not None
-    fig = FigLine(input_node(da), errorbars=False)
+    fig = FigLine(Node(da), errorbars=False)
     line = list(fig.artists.values())[0]
     assert line._error is None
 
 
 def test_with_binedges():
     da = data_array(ndim=1, binedges=True)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     assert len(fig.artists) == 1
     line = list(fig.artists.values())[0]
     assert sc.identical(line._data, da)
     xdata = line._line.get_xdata()
     assert np.allclose(xdata, da.coords['xx'].values)
     assert len(xdata) == da.sizes['xx'] + 1
 
@@ -68,135 +68,141 @@
     assert fig.canvas.yscale == 'linear'
     fig = FigLine(norm='log')
     assert fig.canvas.yscale == 'log'
 
 
 def test_crop():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     assert fig.canvas.xmin < da.meta['xx'].min().value
     assert fig.canvas.xmax > da.meta['xx'].max().value
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     fig.crop(xx={'min': xmin, 'max': xmax})
     assert fig.canvas.xrange == (xmin.value, xmax.value)
     with pytest.raises(KeyError):
         fig.crop(yy={'min': xmin, 'max': xmax})
 
 
 def test_crop_no_variable():
     da = data_array(ndim=1)
     xmin = 2.1
     xmax = 33.4
-    fig = FigLine(input_node(da), crop={'xx': {'min': xmin, 'max': xmax}})
+    fig = FigLine(Node(da), crop={'xx': {'min': xmin, 'max': xmax}})
     assert fig.canvas.xrange == (xmin, xmax)
 
 
 def test_update_grows_limits():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
     fig.update(da * 2.5, key=key)
     new_lims = fig.canvas.yrange
     assert new_lims[0] < old_lims[0]
     assert new_lims[1] > old_lims[1]
 
 
 def test_update_does_not_shrink_limits():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da))
+    fig = FigLine(Node(da))
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
     fig.update(da * 0.5, key=key)
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0]
     assert new_lims[1] == old_lims[1]
 
 
 def test_vmin():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da), vmin=sc.scalar(-0.5, unit='m/s'))
+    fig = FigLine(Node(da), vmin=sc.scalar(-0.5, unit='m/s'))
     assert fig.canvas.ymin == -0.5
 
 
 def test_vmin_unit_mismatch_raises():
     da = data_array(ndim=1)
     with pytest.raises(sc.UnitError):
-        _ = FigLine(input_node(da), vmin=sc.scalar(-0.5, unit='m'))
+        _ = FigLine(Node(da), vmin=sc.scalar(-0.5, unit='m'))
 
 
 def test_vmax():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da), vmax=sc.scalar(0.68, unit='m/s'))
+    fig = FigLine(Node(da), vmax=sc.scalar(0.68, unit='m/s'))
     assert fig.canvas.ymax == 0.68
 
 
 def test_vmin_vmax():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da),
-                  vmin=sc.scalar(-0.5, unit='m/s'),
-                  vmax=sc.scalar(0.68, unit='m/s'))
+    fig = FigLine(
+        Node(da),
+        vmin=sc.scalar(-0.5, unit='m/s'),
+        vmax=sc.scalar(0.68, unit='m/s'),
+    )
     assert np.allclose(fig.canvas.yrange, [-0.5, 0.68])
 
 
 def test_vmin_vmax_no_variable():
     da = data_array(ndim=1)
-    fig = FigLine(input_node(da), vmin=-0.5, vmax=0.68)
+    fig = FigLine(Node(da), vmin=-0.5, vmax=0.68)
     assert np.allclose(fig.canvas.yrange, [-0.5, 0.68])
 
 
 def test_raises_for_new_data_with_incompatible_dimension():
     x = data_array(ndim=1)
     y = x.rename(xx='yy')
     with pytest.raises(sc.DimensionError):
-        FigLine(input_node(x), input_node(y))
+        FigLine(Node(x), Node(y))
 
 
 def test_raises_for_new_data_with_incompatible_unit():
     a = data_array(ndim=1)
     b = a * a
     with pytest.raises(sc.UnitError):
-        FigLine(input_node(a), input_node(b))
+        FigLine(Node(a), Node(b))
 
 
 def test_raises_for_new_data_with_incompatible_coord_unit():
     a = data_array(ndim=1)
     b = a.copy()
     b.coords['xx'] = a.coords['xx'] * a.coords['xx']
     with pytest.raises(sc.UnitError):
-        FigLine(input_node(a), input_node(b))
+        FigLine(Node(a), Node(b))
 
 
 def test_converts_new_data_units():
     a = data_array(ndim=1, unit='m')
     b = data_array(ndim=1, unit='cm')
-    anode = input_node(a)
-    bnode = input_node(b)
+    anode = Node(a)
+    bnode = Node(b)
     fig = FigLine(anode, bnode)
     assert sc.identical(fig.artists[anode.id]._data, a)
     assert sc.identical(fig.artists[bnode.id]._data, b.to(unit='m'))
 
 
 def test_converts_new_data_coordinate_units():
     a = data_array(ndim=1)
     b = data_array(ndim=1)
     b.coords['xx'].unit = 'cm'
-    anode = input_node(a)
-    bnode = input_node(b)
+    anode = Node(a)
+    bnode = Node(b)
     fig = FigLine(anode, bnode)
     assert sc.identical(fig.artists[anode.id]._data, a)
     c = b.copy()
     c.coords['xx'] = c.coords['xx'].to(unit='m')
     assert sc.identical(fig.artists[bnode.id]._data, c)
 
 
 def test_converts_new_data_units_integers():
-    a = sc.DataArray(data=sc.array(dims=['x'], values=[1, 2, 3, 4, 5], unit='m'),
-                     coords={'x': sc.arange('x', 5., unit='s')})
-    b = sc.DataArray(data=sc.array(dims=['x'], values=[10, 20, 30, 40, 50], unit='cm'),
-                     coords={'x': sc.arange('x', 5., unit='s')})
-    anode = input_node(a)
-    bnode = input_node(b)
+    a = sc.DataArray(
+        data=sc.array(dims=['x'], values=[1, 2, 3, 4, 5], unit='m'),
+        coords={'x': sc.arange('x', 5.0, unit='s')},
+    )
+    b = sc.DataArray(
+        data=sc.array(dims=['x'], values=[10, 20, 30, 40, 50], unit='cm'),
+        coords={'x': sc.arange('x', 5.0, unit='s')},
+    )
+    anode = Node(a)
+    bnode = Node(b)
     fig = FigLine(anode, bnode)
     assert sc.identical(fig.artists[anode.id]._data, a)
     assert sc.identical(fig.artists[bnode.id]._data, b.to(unit='m', dtype=float))
```

### Comparing `plopp-23.3.0/tests/widgets/box_test.py` & `plopp-23.4.0/tests/widgets/box_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/widgets/checkboxes_test.py` & `plopp-23.4.0/tests/widgets/checkboxes_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.3.0/tests/widgets/cut3d_test.py` & `plopp-23.4.0/tests/widgets/cut3d_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from plopp import input_node
+from plopp import Node
 from plopp.data.testing import scatter
 from plopp.graphics.figscatter3d import FigScatter3d
 from plopp.widgets import TriCutTool
 
 
 def test_show_hide_cuts():
     da = scatter()
-    fig = FigScatter3d(input_node(da), x='x', y='y', z='z')
+    fig = FigScatter3d(Node(da), x='x', y='y', z='z')
     tri = TriCutTool(fig)
     assert len(fig.artists) == 1
     tri.cut_x.button.value = True
     assert len(fig.artists) == 2
     tri.cut_y.button.value = True
     assert len(fig.artists) == 3
     tri.cut_z.button.value = True
@@ -24,29 +24,29 @@
     assert len(fig.artists) == 2
     tri.cut_z.button.value = False
     assert len(fig.artists) == 1
 
 
 def test_move_cut():
     da = scatter()
-    fig = FigScatter3d(input_node(da), x='x', y='y', z='z')
+    fig = FigScatter3d(Node(da), x='x', y='y', z='z')
     tri = TriCutTool(fig)
     tri.cut_x.button.value = True
     assert tri.cut_x.outline.position[0] == tri.cut_x.slider.value
     pts = list(fig.artists.values())[-1]
     npoints = pts.geometry.attributes['position'].array.shape[0]
     tri.cut_x.slider.value = -5.0
     assert tri.cut_x.outline.position[0] == tri.cut_x.slider.value
     new_pts = list(fig.artists.values())[-1]
     assert npoints != new_pts.geometry.attributes['position'].array.shape[0]
 
 
 def test_cut_thickness():
     da = scatter()
-    fig = FigScatter3d(input_node(da), x='x', y='y', z='z')
+    fig = FigScatter3d(Node(da), x='x', y='y', z='z')
     tri = TriCutTool(fig)
     tri.cut_x.button.value = True
     pts = list(fig.artists.values())[-1]
     npoints = pts.geometry.attributes['position'].array.shape[0]
     tri.cut_x.plus_minus.plus()
     new_pts = list(fig.artists.values())[-1]
     assert npoints < new_pts.geometry.attributes['position'].array.shape[0]
@@ -56,14 +56,14 @@
     tri.cut_x.plus_minus.minus()
     new_pts = list(fig.artists.values())[-1]
     assert npoints > new_pts.geometry.attributes['position'].array.shape[0]
 
 
 def test_empty_cut():
     da = scatter()
-    fig = FigScatter3d(input_node(da), x='x', y='y', z='z')
+    fig = FigScatter3d(Node(da), x='x', y='y', z='z')
     tri = TriCutTool(fig)
     assert len(fig.artists) == 1
     tri.cut_y.button.value = True
     assert len(fig.artists) == 2
     tri.cut_y.slider.value = 34.0  # This cut should contain no points
     assert len(fig.artists) == 1
```

### Comparing `plopp-23.3.0/tests/widgets/slice_test.py` & `plopp-23.4.0/tests/widgets/slice_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,43 +5,37 @@
 
 from plopp.data.testing import data_array
 from plopp.widgets import SliceWidget, slice_dims
 
 
 def test_slice_creation():
     da = data_array(ndim=3)
-    sizes = da.sizes.copy()
-    del sizes['zz']
-    sw = SliceWidget(sizes=sizes, coords=da.coords)
+    sw = SliceWidget(da, dims=['yy', 'xx'])
     assert sw._slider_dims == ['yy', 'xx']
     assert sw.controls['xx']['slider'].min == 0
     assert sw.controls['xx']['slider'].max == da.sizes['xx'] - 1
     assert sw.controls['xx']['slider'].description == 'xx'
     assert sw.controls['yy']['slider'].min == 0
     assert sw.controls['yy']['slider'].max == da.sizes['yy'] - 1
     assert sw.controls['yy']['slider'].description == 'yy'
 
 
 def test_slice_value_property():
     da = data_array(ndim=3)
-    sizes = da.sizes.copy()
-    del sizes['zz']
-    sw = SliceWidget(sizes=sizes, coords=da.coords)
+    sw = SliceWidget(da, dims=['yy', 'xx'])
     sw.controls['xx']['slider'].value = 10
     sw.controls['yy']['slider'].value = 15
     assert sw.value == {'xx': 10, 'yy': 15}
 
 
 def test_slice_label_updates():
     da = data_array(ndim=3)
     da.coords['xx'] *= 1.1
     da.coords['yy'] *= 3.3
-    sizes = da.sizes.copy()
-    del sizes['zz']
-    sw = SliceWidget(sizes=sizes, coords=da.coords)
+    sw = SliceWidget(da, dims=['yy', 'xx'])
     assert sw.controls['xx']['label'].value == '0.0 [m]'
     sw.controls['xx']['slider'].value = 10
     assert sw.controls['xx']['label'].value == '11.0 [m]'
     assert sw.controls['yy']['label'].value == '0.0 [m]'
     sw.controls['yy']['slider'].value = 15
     assert sw.controls['yy']['label'].value == '49.5 [m]'
```

### Comparing `plopp-23.3.0/tox.ini` & `plopp-23.4.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [tox]
-envlist = minimal,noplotly,py38
+envlist = minimal,noplotly,py39
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 commands = pytest
 
 [testenv:minimal]
 description = Test if plopp can plot when installed with only base dependencies
-basepython = python3.8
+basepython = python3.9
 deps = -r requirements/mini.txt
 commands = pytest tests/minimal_plot.py
 
 [testenv:noplotly]
 description = Test that plotly tests are skipped if plotly is not installed
-basepython = python3.8
+basepython = python3.9
 deps = -r requirements/noplotly.txt
 commands = pytest tests/backends/plotly
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = python3.8
+basepython = python3.9
 deps = {posargs:}
        -r requirements/docs.txt
 allowlist_externals=find
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
 
 [testenv:linkcheck]
 description = Run Sphinx linkcheck
 deps = -r requirements/docs.txt
 commands = python -m sphinx -j2 -v -b linkcheck -d {toxworkdir}/docs_doctrees docs html
 
 [testenv:static]
 description = Code formatting and static analysis
-basepython = python3.8
+basepython = python3.9
 skip_install = true
 deps = -r requirements/static.txt
 allowlist_externals = sh
 # The first run of pre-commit may reformat files. If this happens, it returns 1 but this
 # should not fail the job. So just run again if it fails. A second failure means that
 # either the different formatters can't agree on a format or that static analysis failed.
 commands = sh -c 'pre-commit run -a || (echo "" && pre-commit run -a)'
```

